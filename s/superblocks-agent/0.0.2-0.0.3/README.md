# Comparing `tmp/superblocks-agent-0.0.2.tar.gz` & `tmp/superblocks-agent-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superblocks-agent-0.0.2.tar", last modified: Fri May 10 20:20:38 2024, max compression
+gzip compressed data, was "superblocks-agent-0.0.3.tar", last modified: Sat May 18 01:47:57 2024, max compression
```

## Comparing `superblocks-agent-0.0.2.tar` & `superblocks-agent-0.0.3.tar`

### file list

```diff
@@ -1,54 +1,66 @@
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-10 20:20:38.144200 superblocks-agent-0.0.2/
--rw-r--r--   0 joeygreco   (501) staff       (20)     1068 2024-05-06 19:43:05.000000 superblocks-agent-0.0.2/LICENSE
--rw-r--r--   0 joeygreco   (501) staff       (20)       24 2024-05-06 21:08:25.000000 superblocks-agent-0.0.2/MANIFEST.in
--rw-r--r--   0 joeygreco   (501) staff       (20)      746 2024-05-10 20:20:38.144008 superblocks-agent-0.0.2/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)      368 2024-05-06 21:13:04.000000 superblocks-agent-0.0.2/README.md
--rw-r--r--   0 joeygreco   (501) staff       (20)      258 2024-05-07 19:24:36.000000 superblocks-agent-0.0.2/pyproject.toml
--rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-09 20:55:53.000000 superblocks-agent-0.0.2/requirements.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-10 20:20:38.144277 superblocks-agent-0.0.2/setup.cfg
--rw-r--r--   0 joeygreco   (501) staff       (20)     1025 2024-05-10 20:19:54.000000 superblocks-agent-0.0.2/setup.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-10 20:20:38.136408 superblocks-agent-0.0.2/superblocks_agent/
--rw-r--r--   0 joeygreco   (501) staff       (20)       42 2024-05-06 20:42:01.000000 superblocks-agent-0.0.2/superblocks_agent/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       94 2024-05-10 20:20:10.000000 superblocks-agent-0.0.2/superblocks_agent/_version.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-10 20:20:38.137449 superblocks-agent-0.0.2/superblocks_agent/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-10 19:43:32.000000 superblocks-agent-0.0.2/superblocks_agent/v1/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-10 20:20:38.138272 superblocks-agent-0.0.2/superblocks_agent/v1/enumeration/
--rw-r--r--   0 joeygreco   (501) staff       (20)      363 2024-05-06 21:26:57.000000 superblocks-agent-0.0.2/superblocks_agent/v1/enumeration/BaseEnum.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1048 2024-05-10 19:44:12.000000 superblocks-agent-0.0.2/superblocks_agent/v1/enumeration/ViewMode.py
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-06 21:20:48.000000 superblocks-agent-0.0.2/superblocks_agent/v1/enumeration/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-10 20:20:38.140032 superblocks-agent-0.0.2/superblocks_agent/v1/model/
--rw-r--r--   0 joeygreco   (501) staff       (20)      181 2024-05-09 20:14:49.000000 superblocks-agent-0.0.2/superblocks_agent/v1/model/Agent.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      732 2024-05-09 15:54:46.000000 superblocks-agent-0.0.2/superblocks_agent/v1/model/ApiConfig.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      134 2024-05-06 21:26:19.000000 superblocks-agent-0.0.2/superblocks_agent/v1/model/Auth.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      258 2024-05-09 20:38:06.000000 superblocks-agent-0.0.2/superblocks_agent/v1/model/ClientConfig.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      953 2024-05-09 13:21:56.000000 superblocks-agent-0.0.2/superblocks_agent/v1/model/MockApiFilters.py
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-06 21:16:59.000000 superblocks-agent-0.0.2/superblocks_agent/v1/model/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-10 20:20:38.140828 superblocks-agent-0.0.2/superblocks_agent/v1/model/abstract/
--rw-r--r--   0 joeygreco   (501) staff       (20)      264 2024-05-10 16:46:50.000000 superblocks-agent-0.0.2/superblocks_agent/v1/model/abstract/BaseMock.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       54 2024-05-07 13:47:08.000000 superblocks-agent-0.0.2/superblocks_agent/v1/model/abstract/MockFilters.py
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-07 13:24:31.000000 superblocks-agent-0.0.2/superblocks_agent/v1/model/abstract/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-10 20:20:38.141785 superblocks-agent-0.0.2/superblocks_agent/v1/things/
--rw-r--r--   0 joeygreco   (501) staff       (20)     6114 2024-05-10 18:37:25.000000 superblocks-agent-0.0.2/superblocks_agent/v1/things/Api.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2595 2024-05-10 18:36:27.000000 superblocks-agent-0.0.2/superblocks_agent/v1/things/ApiMock.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2030 2024-05-10 16:52:30.000000 superblocks-agent-0.0.2/superblocks_agent/v1/things/Client.py
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-06 21:14:28.000000 superblocks-agent-0.0.2/superblocks_agent/v1/things/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1595 2024-05-09 20:07:50.000000 superblocks-agent-0.0.2/superblocks_agent/v1/things/jg.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-10 20:20:38.142570 superblocks-agent-0.0.2/superblocks_agent/v1/type_/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-10 16:44:38.000000 superblocks-agent-0.0.2/superblocks_agent/v1/type_/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      290 2024-05-10 16:53:54.000000 superblocks-agent-0.0.2/superblocks_agent/v1/type_/client.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      295 2024-05-10 19:44:37.000000 superblocks-agent-0.0.2/superblocks_agent/v1/type_/mock.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-10 20:20:38.143020 superblocks-agent-0.0.2/superblocks_agent/v1/util/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-08 13:45:31.000000 superblocks-agent-0.0.2/superblocks_agent/v1/util/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2025 2024-05-10 16:09:39.000000 superblocks-agent-0.0.2/superblocks_agent/v1/util/convert.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-10 20:20:38.137280 superblocks-agent-0.0.2/superblocks_agent.egg-info/
--rw-r--r--   0 joeygreco   (501) staff       (20)      746 2024-05-10 20:20:38.000000 superblocks-agent-0.0.2/superblocks_agent.egg-info/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)     1358 2024-05-10 20:20:38.000000 superblocks-agent-0.0.2/superblocks_agent.egg-info/SOURCES.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-10 20:20:38.000000 superblocks-agent-0.0.2/superblocks_agent.egg-info/dependency_links.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)       39 2024-05-10 20:20:38.000000 superblocks-agent-0.0.2/superblocks_agent.egg-info/requires.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)       28 2024-05-10 20:20:38.000000 superblocks-agent-0.0.2/superblocks_agent.egg-info/top_level.txt
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-10 20:20:38.134168 superblocks-agent-0.0.2/test_unit/
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-10 20:20:38.143384 superblocks-agent-0.0.2/test_unit/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-10 19:45:19.000000 superblocks-agent-0.0.2/test_unit/v1/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-10 20:20:38.143713 superblocks-agent-0.0.2/test_unit/v1/test_things/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-07 18:29:28.000000 superblocks-agent-0.0.2/test_unit/v1/test_things/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     7729 2024-05-10 19:42:56.000000 superblocks-agent-0.0.2/test_unit/v1/test_things/test_Api.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:47:57.358150 superblocks-agent-0.0.3/
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1068 2024-05-06 19:43:05.000000 superblocks-agent-0.0.3/LICENSE
+-rw-r--r--   0 joeygreco   (501) staff       (20)       25 2024-05-15 16:03:40.000000 superblocks-agent-0.0.3/MANIFEST.in
+-rw-r--r--   0 joeygreco   (501) staff       (20)      746 2024-05-18 01:47:57.357934 superblocks-agent-0.0.3/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)      368 2024-05-06 21:13:04.000000 superblocks-agent-0.0.3/README.md
+-rw-r--r--   0 joeygreco   (501) staff       (20)      298 2024-05-15 14:39:28.000000 superblocks-agent-0.0.3/pyproject.toml
+-rw-r--r--   0 joeygreco   (501) staff       (20)       65 2024-05-16 21:07:17.000000 superblocks-agent-0.0.3/requirements.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-18 01:47:57.358241 superblocks-agent-0.0.3/setup.cfg
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1025 2024-05-10 20:19:54.000000 superblocks-agent-0.0.3/setup.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:47:57.347873 superblocks-agent-0.0.3/superblocks_agent/
+-rw-r--r--   0 joeygreco   (501) staff       (20)       42 2024-05-06 20:42:01.000000 superblocks-agent-0.0.3/superblocks_agent/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       94 2024-05-18 01:47:48.000000 superblocks-agent-0.0.3/superblocks_agent/_version.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:47:57.349388 superblocks-agent-0.0.3/superblocks_agent/enumeration/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      363 2024-05-17 13:31:35.000000 superblocks-agent-0.0.3/superblocks_agent/enumeration/BaseEnum.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1057 2024-05-17 13:33:54.000000 superblocks-agent-0.0.3/superblocks_agent/enumeration/ViewMode.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.3/superblocks_agent/enumeration/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:47:57.352363 superblocks-agent-0.0.3/superblocks_agent/model/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      181 2024-05-17 13:31:35.000000 superblocks-agent-0.0.3/superblocks_agent/model/Agent.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      734 2024-05-17 13:36:17.000000 superblocks-agent-0.0.3/superblocks_agent/model/ApiConfig.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      250 2024-05-17 13:37:34.000000 superblocks-agent-0.0.3/superblocks_agent/model/ApiResult.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      124 2024-05-17 13:31:35.000000 superblocks-agent-0.0.3/superblocks_agent/model/Auth.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      284 2024-05-17 13:35:23.000000 superblocks-agent-0.0.3/superblocks_agent/model/ClientConfig.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      404 2024-05-17 13:31:35.000000 superblocks-agent-0.0.3/superblocks_agent/model/ExecutionError.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1890 2024-05-17 13:38:39.000000 superblocks-agent-0.0.3/superblocks_agent/model/ExecutionResult.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1000 2024-05-17 13:38:39.000000 superblocks-agent-0.0.3/superblocks_agent/model/MockApiFilters.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      270 2024-05-17 13:37:49.000000 superblocks-agent-0.0.3/superblocks_agent/model/StepResult.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.3/superblocks_agent/model/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:47:57.353084 superblocks-agent-0.0.3/superblocks_agent/model/abstract/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      475 2024-05-17 13:36:41.000000 superblocks-agent-0.0.3/superblocks_agent/model/abstract/BaseMock.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       54 2024-05-17 13:31:35.000000 superblocks-agent-0.0.3/superblocks_agent/model/abstract/MockFilters.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.3/superblocks_agent/model/abstract/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:47:57.354186 superblocks-agent-0.0.3/superblocks_agent/things/
+-rw-r--r--   0 joeygreco   (501) staff       (20)     6605 2024-05-17 13:38:39.000000 superblocks-agent-0.0.3/superblocks_agent/things/Api.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2449 2024-05-17 13:38:39.000000 superblocks-agent-0.0.3/superblocks_agent/things/ApiMock.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2068 2024-05-17 13:38:39.000000 superblocks-agent-0.0.3/superblocks_agent/things/Client.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.3/superblocks_agent/things/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:47:57.354699 superblocks-agent-0.0.3/superblocks_agent/type_/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.3/superblocks_agent/type_/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      290 2024-05-17 13:31:35.000000 superblocks-agent-0.0.3/superblocks_agent/type_/client.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      264 2024-05-17 13:40:43.000000 superblocks-agent-0.0.3/superblocks_agent/type_/mock.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:47:57.355367 superblocks-agent-0.0.3/superblocks_agent/util/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.3/superblocks_agent/util/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2905 2024-05-17 13:31:35.000000 superblocks-agent-0.0.3/superblocks_agent/util/convert.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       71 2024-05-17 13:31:35.000000 superblocks-agent-0.0.3/superblocks_agent/util/generate.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:47:57.348817 superblocks-agent-0.0.3/superblocks_agent.egg-info/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      746 2024-05-18 01:47:57.000000 superblocks-agent-0.0.3/superblocks_agent.egg-info/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1740 2024-05-18 01:47:57.000000 superblocks-agent-0.0.3/superblocks_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-18 01:47:57.000000 superblocks-agent-0.0.3/superblocks_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       65 2024-05-18 01:47:57.000000 superblocks-agent-0.0.3/superblocks_agent.egg-info/requires.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       28 2024-05-18 01:47:57.000000 superblocks-agent-0.0.3/superblocks_agent.egg-info/top_level.txt
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:47:57.345784 superblocks-agent-0.0.3/test_unit/
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:47:57.355705 superblocks-agent-0.0.3/test_unit/test_enumeration/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.3/test_unit/test_enumeration/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1400 2024-05-17 13:33:54.000000 superblocks-agent-0.0.3/test_unit/test_enumeration/test_ViewMode.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:47:57.356242 superblocks-agent-0.0.3/test_unit/test_model/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.3/test_unit/test_model/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2596 2024-05-17 13:33:54.000000 superblocks-agent-0.0.3/test_unit/test_model/test_ExecutionResult.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      743 2024-05-17 13:33:54.000000 superblocks-agent-0.0.3/test_unit/test_model/test_MockApiFilters.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:47:57.356786 superblocks-agent-0.0.3/test_unit/test_things/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.3/test_unit/test_things/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     8120 2024-05-17 13:33:54.000000 superblocks-agent-0.0.3/test_unit/test_things/test_Api.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4135 2024-05-17 13:33:54.000000 superblocks-agent-0.0.3/test_unit/test_things/test_ApiMock.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-18 01:47:57.357581 superblocks-agent-0.0.3/test_unit/test_util/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.3/test_unit/test_util/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3911 2024-05-17 13:33:54.000000 superblocks-agent-0.0.3/test_unit/test_util/test_convert.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      479 2024-05-17 13:33:54.000000 superblocks-agent-0.0.3/test_unit/test_util/test_generate.py
```

### Comparing `superblocks-agent-0.0.2/LICENSE` & `superblocks-agent-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.2/PKG-INFO` & `superblocks-agent-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblocks-agent
-Version: 0.0.2
+Version: 0.0.3
 Summary: The Official Python SDK for Superblocks
 Home-page: https://github.com/superblocksteam/orchestrator/tree/main/clients/python
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: superblocks api sdk
 Requires-Python: >=3.10
```

### Comparing `superblocks-agent-0.0.2/setup.py` & `superblocks-agent-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.2/superblocks_agent/v1/enumeration/ViewMode.py` & `superblocks-agent-0.0.3/superblocks_agent/enumeration/ViewMode.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
-from gen.api.v1.service_pb2 import ViewMode as ViewModeProto
+from superblocks_types.api.v1.service_pb2 import ViewMode as ViewModeProto
 
-from superblocks_agent.v1.enumeration.BaseEnum import BaseEnum
+from superblocks_agent.enumeration.BaseEnum import BaseEnum
 
 
 class ViewMode(BaseEnum):
     DEPLOYED = "deployed"
     EDITOR = "editor"
     PREVIEW = "preview"
 
@@ -23,11 +23,11 @@
         raise ValueError(f"'{s}' is not a valid {cls.__name__}")
 
     def to_proto_view_mode(self) -> ViewModeProto:
         match self:
             case ViewMode.DEPLOYED:
                 return ViewModeProto.VIEW_MODE_DEPLOYED
             case ViewMode.EDITOR:
-                return ViewModeProto.VIEW_MODE_EDITOR
+                return ViewModeProto.VIEW_MODE_EDIT
             case ViewMode.PREVIEW:
                 return ViewModeProto.VIEW_MODE_PREVIEW
         return ViewModeProto.VIEW_MODE_UNSPECIFIED
```

### Comparing `superblocks-agent-0.0.2/superblocks_agent/v1/model/ApiConfig.py` & `superblocks-agent-0.0.3/superblocks_agent/model/ApiConfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Optional
 
-from enumeration.ViewMode import ViewMode
+from superblocks_agent.enumeration.ViewMode import ViewMode
 
 
 @dataclass(kw_only=True, eq=False)
 class ApiConfig:
-    api_id: str
     # The application id used to provide a default scope.
     application_id: Optional[str] = None
     # The default branch to use.
     branch_name: Optional[str] = None
     # The id of the commit to use.
     commit_id: Optional[str] = None
     # The default profile to use. If not set, the default for view_mode will be used.
```

### Comparing `superblocks-agent-0.0.2/superblocks_agent/v1/model/MockApiFilters.py` & `superblocks-agent-0.0.3/superblocks_agent/model/MockApiFilters.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Optional
 
-from gen.api.v1.service_pb2 import Mock
-from model.abstract.MockFilters import MockFilters
-from util.convert import to_protobuf_value
+from superblocks_types.api.v1.service_pb2 import Mock
 
+from superblocks_agent.model.abstract.MockFilters import MockFilters
+from superblocks_agent.util.convert import to_protobuf_value
 
-@dataclass(kw_only=True, eq=False)
+
+@dataclass(kw_only=True)
 class MockApiFilters(MockFilters):
     # Filter on integrations with this type
     integration_type: Optional[str] = None
     # Filter on steps with this name
     # NOTE: steps are unique on name
     step_name: Optional[str] = None
     # Filter on these inputs
     inputs: Optional[dict] = None
 
-    def to_params(self) -> Mock.Params:
+    def to_proto_params(self) -> Mock.Params:
         params = Mock.Params()
         if self.integration_type is not None:
             params.integration_type = self.integration_type
         if self.step_name is not None:
             params.step_name = self.step_name
         if self.inputs is not None:
             params.inputs.CopyFrom(to_protobuf_value(self.inputs))
```

### Comparing `superblocks-agent-0.0.2/superblocks_agent/v1/things/Api.py` & `superblocks-agent-0.0.3/superblocks_agent/things/Api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,72 @@
 from typing import Callable, Optional
 
-from gen.api.v1.service_pb2 import (
+from superblocks_types.api.v1.service_pb2 import (
     ExecuteRequest,
     Function,
     StreamResponse,
     TwoWayRequest,
     TwoWayResponse,
 )
-from gen.api.v1.service_pb2_grpc import ExecutorServiceStub
-from gen.common.v1.common_pb2 import Profile
-from gen.common.v1.errors_pb2 import Error
-from model.ApiConfig import ApiConfig
-from things.ApiMock import ApiMock
-from things.Client import Client
-from util.convert import from_protobuf_value, to_protobuf_value
+from superblocks_types.api.v1.service_pb2_grpc import ExecutorServiceStub
+from superblocks_types.common.v1.common_pb2 import Profile
+from superblocks_types.common.v1.errors_pb2 import Error
+
+from superblocks_agent.model.ApiConfig import ApiConfig
+from superblocks_agent.model.ExecutionResult import ExecutionResult
+from superblocks_agent.things.ApiMock import ApiMock
+from superblocks_agent.things.Client import Client
+from superblocks_agent.util.convert import from_protobuf_value, to_protobuf_value
+from superblocks_agent.util.generate import get_unique_id_for_object
 
 
 class Api:
-    def __init__(self, api_config: ApiConfig):
-        self.__api_config = api_config
+    def __init__(self, api_id: str, *, config: Optional[ApiConfig] = None):
+        self.__api_id = api_id
+        self.__config = config
         self.mock_func_lookup: dict[str, callable] = {}
 
     def hydrate_mock_func_lookup(self, mocks: list[ApiMock]) -> None:
         """
         This function is called before every API run.
         It hydrates a map that belongs to this API which allows the lookup of mock return functions.
         """
         for mock in mocks:
             if isinstance(mock.return_val_or_callable, Callable):
-                self.mock_func_lookup[mock.get_return_func_id()] = mock.return_val_or_callable
+                self.mock_func_lookup[
+                    get_unique_id_for_object(mock.return_val_or_callable)
+                ] = mock.return_val_or_callable
+            if mock.on_callable is not None:
+                self.mock_func_lookup[get_unique_id_for_object(mock.on_callable)] = mock.on_callable
 
     async def run(
         self,
         *,
         client: Client,
         inputs: Optional[dict] = None,
         mocks: Optional[list[ApiMock]] = None,
-    ) -> (
-        any
-    ):  # TODO: (joey) define a type for this response. I think we can return events and other useful stuff.
+    ) -> ExecutionResult:
         """
         Runs *this* api with the given inputs and mocks.
         """
         mocks = [] if mocks is None else mocks
         inputs = {} if inputs is None else inputs
 
         # hydrate mock lookup dict so we can reference it later
         self.hydrate_mock_func_lookup(mocks)
 
-        stream_responses = client.run(
+        stream_responses = await client.run(
             with_stub=ExecutorServiceStub,
             stub_func_name="TwoWayStream",
-            initial_messages=[self.build_execute_request(inputs=inputs, mocks=mocks)],
+            initial_requests=[
+                TwoWayRequest(execute=self.build_execute_request(inputs=inputs, mocks=mocks))
+            ],
             response_handler=self.get_handle_two_way_response_func(),
         )
-
-        # TODO: (joey) make this an actual type
-        return {"stream_responses": stream_responses}
+        return ExecutionResult.from_proto_stream_responses(stream_responses)
 
     def get_handle_two_way_response_func(self) -> callable:
         def handle_two_way_response(
             response: TwoWayResponse,
         ) -> tuple[Optional[TwoWayRequest], Optional[StreamResponse]]:
             """
             Function to handle each TwoWayResponse.
@@ -70,15 +76,14 @@
                 # RESPONSE TYPE: TwoWayResponse.Function.Request
                 # the orchestrator is asking us to run a local function to determine the step output
                 # 1. locate the function we should run
                 # 2. call the function with the parameters the orchestrator gave us
                 # 3. send the orchestrator a response with the output/error of the function call
                 case _ if response.HasField("function"):
                     # find function we want to execute
-
                     function_to_execute: Optional[callable] = self.mock_func_lookup.get(
                         response.function.name
                     )
 
                     if function_to_execute is None:
                         raise Exception(f"FOUND NO FUNCTION TO EXECUTE!")
                     # execute function with params and send response
@@ -131,19 +136,20 @@
         return execute_request
 
     def __to_proto_fetch(self) -> ExecuteRequest.Fetch:
         """
         Returns a hydrated Fetch object to be used in an ExecuteRequest.
         """
         fetch = ExecuteRequest.Fetch()
-        fetch.id = self.__api_config.api_id
-        if self.__api_config.profile_name is not None:
-            profile = Profile()
-            profile.name = self.__api_config.profile_name
-            fetch.profile.CopyFrom(profile)
-        if self.__api_config.view_mode is not None:
-            fetch.view_mode = self.__api_config.view_mode.to_proto_view_mode()
-        if self.__api_config.commit_id is not None:
-            fetch.commit_id = self.__api_config.commit_id
-        if self.__api_config.branch_name is not None:
-            fetch.branch_name = self.__api_config.branch_name
+        fetch.id = self.__api_id
+        if self.__config is not None:
+            if self.__config.profile_name is not None:
+                profile = Profile()
+                profile.name = self.__config.profile_name
+                fetch.profile.CopyFrom(profile)
+            if self.__config.view_mode is not None:
+                fetch.view_mode = self.__config.view_mode.to_proto_view_mode()
+            if self.__config.commit_id is not None:
+                fetch.commit_id = self.__config.commit_id
+            if self.__config.branch_name is not None:
+                fetch.branch_name = self.__config.branch_name
         return fetch
```

### Comparing `superblocks-agent-0.0.2/superblocks_agent/v1/things/ApiMock.py` & `superblocks-agent-0.0.3/superblocks_agent/things/ApiMock.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,59 @@
 from __future__ import annotations
 
 from typing import Optional
 
-from gen.api.v1.service_pb2 import Mock
-from model.abstract.BaseMock import BaseMock
-from model.MockApiFilters import MockApiFilters
-from type_.mock import FilteredDictCallable, WhenCallable
-from util.convert import to_protobuf_value
+from superblocks_types.api.v1.service_pb2 import Mock
+
+from superblocks_agent.model.abstract.BaseMock import BaseMock
+from superblocks_agent.model.MockApiFilters import MockApiFilters
+from superblocks_agent.type_.mock import FilteredDictCallable, WhenCallable
+from superblocks_agent.util.convert import Mock_, to_protobuf_value
+from superblocks_agent.util.generate import get_unique_id_for_object
 
 
 class ApiMock(BaseMock):
     def __init__(
         self,
         filters: Optional[MockApiFilters] = None,
         *,
         when: Optional[WhenCallable] = None,
+        # this can be set (more clearly) by calling .return_()
         return_val_or_callable: Optional[dict | FilteredDictCallable] = None,
     ):
-        # TODO: dunder these maybe
-        self.filters = filters
-        self.when = when
+        self.on_filters = filters
+        # these are public because they are accessed by Api.py
+        self.on_callable = when
         self.return_val_or_callable = return_val_or_callable
 
     def return_(self, value: dict | FilteredDictCallable) -> ApiMock:
         self.return_val_or_callable = value
         return self
 
-    def get_return_func_id(self) -> str:
-        """
-        This ID is used to retrieve a function to be called for this mock.
-        """
-        return str(id(self.return_val_or_callable))
-
     def to_proto_on(self) -> Optional[Mock.On]:
         mock_on = None
-        if self.filters is not None:
-            mock_on = Mock.On()
-            mock_on.static.CopyFrom(self.filters.to_params())
-            mock_on.dynamic = self.get_return_func_id()
+        if self.on_filters is not None:
+            mock_on = Mock.On() if mock_on is None else mock_on
+            mock_on.static.CopyFrom(self.on_filters.to_proto_params())
+        if self.on_callable is not None:
+            mock_on = Mock.On() if mock_on is None else mock_on
+            mock_on.dynamic = get_unique_id_for_object(self.on_callable)
         return mock_on
 
     def to_proto_return(self) -> Optional[Mock.Return]:
         mock_return = None
         if self.return_val_or_callable is not None:
             mock_return = Mock.Return()
             match self.return_val_or_callable:
                 case _ if isinstance(self.return_val_or_callable, dict):
                     mock_return.static.CopyFrom(to_protobuf_value(self.return_val_or_callable))
-                case _ if isinstance(self.return_val_or_callable, WhenCallable):
-                    mock_return.dynamic = self.get_return_func_id()
+                # should be type type_.mock.WhenCallable
+                case _ if callable(self.return_val_or_callable):
+                    mock_return.dynamic = get_unique_id_for_object(self.return_val_or_callable)
         return mock_return
 
     def to_proto_mock(self) -> Mock:
-        mock = Mock()
-        mock_on = self.to_proto_on()
-        if mock_on is not None:
-            mock.on.CopyFrom(mock_on)
-        mock_return = self.to_proto_return()
-        if mock_return is not None:
-            # NOTE: return is a reserved keyword, this workaround seems to do the trick
-            # source: https://stackoverflow.com/questions/30142750/reserved-keyword-is-used-in-protobuf-in-python
-            return_value = getattr(mock, "return")
-            return_value.CopyFrom(self.to_proto_return())
-        return mock
+        return Mock_(on=self.to_proto_on(), return_=self.to_proto_return())
 
 
 def on(filters: Optional[MockApiFilters] = None, *, when: Optional[WhenCallable] = None) -> ApiMock:
-    return ApiMock(filters, when)
+    return ApiMock(filters=filters, when=when)
```

### Comparing `superblocks-agent-0.0.2/superblocks_agent/v1/things/Client.py` & `superblocks-agent-0.0.3/superblocks_agent/things/Client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 from typing import Optional
 
 import grpc
-from gen.api.v1.service_pb2 import StreamResponse
-from model.ClientConfig import ClientConfig
-from type_.client import GenericMetadata, TwoWayStreamResponseHandler
+from superblocks_types.api.v1.service_pb2 import StreamResponse
+
+from superblocks_agent.model.ClientConfig import ClientConfig
+from superblocks_agent.type_.client import GenericMetadata, TwoWayStreamResponseHandler
 
 
 class Client:
     def __init__(self, client_config: ClientConfig):
         self.__client_config = client_config
 
-    def run(
+    async def run(
         self,
         *,
         with_stub: object,
         stub_func_name: str,
-        initial_messages: list[object],
+        initial_requests: list[object],
         response_handler: TwoWayStreamResponseHandler,
-    ) -> list[object]:
-        channel = grpc.insecure_channel(target=self.__client_config.agent.endpoint)
-        stub = with_stub(channel=channel)
+    ) -> list[StreamResponse]:
+        stub = with_stub(channel=grpc.insecure_channel(target=self.__client_config.agent.endpoint))
         stub_function = getattr(stub, stub_func_name)
 
         return self.__handle_two_way_stream(
             stub_function=stub_function,
-            messages=initial_messages,
+            requests=initial_requests,
             response_handler=response_handler,
         )
 
     def __handle_two_way_stream(
         self,
         *,
         stub_function: callable,
-        messages: list[object],
+        requests: list[object],
         response_handler: TwoWayStreamResponseHandler,
-        generic_metadatas: Optional[list[GenericMetadata]] = None,
+        stream_responses: Optional[list[GenericMetadata]] = None,
     ) -> list[StreamResponse]:
-        generic_metadatas = [] if generic_metadatas is None else generic_metadatas
+        stream_responses = [] if stream_responses is None else stream_responses
         try:
-            for response in stub_function(iter(messages)):
-                next_request, generic_metadata = response_handler(response)
-                if generic_metadata is not None:
-                    generic_metadatas.append(generic_metadata)
+            for response in stub_function(iter(requests)):
+                next_request, two_way_response = response_handler(response)
+                if two_way_response is not None:
+                    stream_responses.append(two_way_response.stream)
                 if next_request is not None:
                     # recursively call
                     self.__handle_two_way_stream(
                         stub_function=stub_function,
-                        messages=[next_request],
+                        requests=[next_request],
                         response_handler=response_handler,
-                        generic_metadatas=generic_metadatas,
+                        stream_responses=stream_responses,
                     )
         except Exception as e:
             print("Error processing responses:", e)
-        finally:
-            return generic_metadatas
+            raise e
+
+        return stream_responses
```

### Comparing `superblocks-agent-0.0.2/superblocks_agent.egg-info/PKG-INFO` & `superblocks-agent-0.0.3/superblocks_agent.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblocks-agent
-Version: 0.0.2
+Version: 0.0.3
 Summary: The Official Python SDK for Superblocks
 Home-page: https://github.com/superblocksteam/orchestrator/tree/main/clients/python
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: superblocks api sdk
 Requires-Python: >=3.10
```

### Comparing `superblocks-agent-0.0.2/superblocks_agent.egg-info/SOURCES.txt` & `superblocks-agent-0.0.3/superblocks_agent.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,33 +7,44 @@
 superblocks_agent/__init__.py
 superblocks_agent/_version.py
 superblocks_agent.egg-info/PKG-INFO
 superblocks_agent.egg-info/SOURCES.txt
 superblocks_agent.egg-info/dependency_links.txt
 superblocks_agent.egg-info/requires.txt
 superblocks_agent.egg-info/top_level.txt
-superblocks_agent/v1/__init__.py
-superblocks_agent/v1/enumeration/BaseEnum.py
-superblocks_agent/v1/enumeration/ViewMode.py
-superblocks_agent/v1/enumeration/__init__.py
-superblocks_agent/v1/model/Agent.py
-superblocks_agent/v1/model/ApiConfig.py
-superblocks_agent/v1/model/Auth.py
-superblocks_agent/v1/model/ClientConfig.py
-superblocks_agent/v1/model/MockApiFilters.py
-superblocks_agent/v1/model/__init__.py
-superblocks_agent/v1/model/abstract/BaseMock.py
-superblocks_agent/v1/model/abstract/MockFilters.py
-superblocks_agent/v1/model/abstract/__init__.py
-superblocks_agent/v1/things/Api.py
-superblocks_agent/v1/things/ApiMock.py
-superblocks_agent/v1/things/Client.py
-superblocks_agent/v1/things/__init__.py
-superblocks_agent/v1/things/jg.py
-superblocks_agent/v1/type_/__init__.py
-superblocks_agent/v1/type_/client.py
-superblocks_agent/v1/type_/mock.py
-superblocks_agent/v1/util/__init__.py
-superblocks_agent/v1/util/convert.py
-test_unit/v1/__init__.py
-test_unit/v1/test_things/__init__.py
-test_unit/v1/test_things/test_Api.py
+superblocks_agent/enumeration/BaseEnum.py
+superblocks_agent/enumeration/ViewMode.py
+superblocks_agent/enumeration/__init__.py
+superblocks_agent/model/Agent.py
+superblocks_agent/model/ApiConfig.py
+superblocks_agent/model/ApiResult.py
+superblocks_agent/model/Auth.py
+superblocks_agent/model/ClientConfig.py
+superblocks_agent/model/ExecutionError.py
+superblocks_agent/model/ExecutionResult.py
+superblocks_agent/model/MockApiFilters.py
+superblocks_agent/model/StepResult.py
+superblocks_agent/model/__init__.py
+superblocks_agent/model/abstract/BaseMock.py
+superblocks_agent/model/abstract/MockFilters.py
+superblocks_agent/model/abstract/__init__.py
+superblocks_agent/things/Api.py
+superblocks_agent/things/ApiMock.py
+superblocks_agent/things/Client.py
+superblocks_agent/things/__init__.py
+superblocks_agent/type_/__init__.py
+superblocks_agent/type_/client.py
+superblocks_agent/type_/mock.py
+superblocks_agent/util/__init__.py
+superblocks_agent/util/convert.py
+superblocks_agent/util/generate.py
+test_unit/test_enumeration/__init__.py
+test_unit/test_enumeration/test_ViewMode.py
+test_unit/test_model/__init__.py
+test_unit/test_model/test_ExecutionResult.py
+test_unit/test_model/test_MockApiFilters.py
+test_unit/test_things/__init__.py
+test_unit/test_things/test_Api.py
+test_unit/test_things/test_ApiMock.py
+test_unit/test_util/__init__.py
+test_unit/test_util/test_convert.py
+test_unit/test_util/test_generate.py
```

### Comparing `superblocks-agent-0.0.2/test_unit/v1/test_things/test_Api.py` & `superblocks-agent-0.0.3/test_unit/test_things/test_Api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 import unittest
 
-from superblocks_agent.v1.enumeration.ViewMode import ViewMode
-from superblocks_agent.v1.gen.api.v1.event_pb2 import Event
-from superblocks_agent.v1.gen.api.v1.service_pb2 import (
+from superblocks_types.api.v1.event_pb2 import Event
+from superblocks_types.api.v1.service_pb2 import (
     ExecuteRequest,
     Function,
     Mock,
     StreamResponse,
     TwoWayRequest,
     TwoWayResponse,
 )
-from superblocks_agent.v1.gen.common.v1.common_pb2 import Profile
-from superblocks_agent.v1.gen.common.v1.errors_pb2 import Error
-from superblocks_agent.v1.model.ApiConfig import ApiConfig
-from superblocks_agent.v1.model.MockApiFilters import MockApiFilters
-from superblocks_agent.v1.things.Api import Api
-from superblocks_agent.v1.things.ApiMock import ApiMock
-from superblocks_agent.v1.util.convert import to_protobuf_value
+from superblocks_types.common.v1.common_pb2 import Profile
+from superblocks_types.common.v1.errors_pb2 import Error
+
+from superblocks_agent.enumeration.ViewMode import ViewMode
+from superblocks_agent.model.ApiConfig import ApiConfig
+from superblocks_agent.model.MockApiFilters import MockApiFilters
+from superblocks_agent.things.Api import Api
+from superblocks_agent.things.ApiMock import ApiMock
+from superblocks_agent.util.convert import Mock_, to_protobuf_value
+from superblocks_agent.util.generate import get_unique_id_for_object
 
 
 class TestApi(unittest.TestCase):
     def test_build_execute_request(self):
         api = Api(
-            ApiConfig(
-                api_id="api_id",
+            "api_id",
+            config=ApiConfig(
                 application_id="app_id",
                 branch_name="branch_name",
                 commit_id="commit_id",
                 profile_name="profile_name",
                 page_id="page_id",
                 view_mode=ViewMode.DEPLOYED,
-            )
+            ),
         )
         api_mock = ApiMock(
             filters=MockApiFilters(
                 integration_type="integration_type", step_name="step_name", inputs={"foo": "bar"}
             ),
             when=lambda _: True,
             return_val_or_callable={"some": "return"},
@@ -47,94 +49,91 @@
                 "list_var": ["foo", 1, True, {}, []],
                 "dict_var": {"foo": "bar"},
                 "null_var": None,
             },
             mocks=[api_mock],
         )
 
-        expected_mock_return = Mock.Return(static=to_protobuf_value({"some": "return"}))
         expected = ExecuteRequest(
             inputs={
                 "str_var": to_protobuf_value("foo"),
                 "int_var": to_protobuf_value(1),
                 "bool_var": to_protobuf_value(True),
                 "list_var": to_protobuf_value(["foo", 1, True, {}, []]),
                 "dict_var": to_protobuf_value({"foo": "bar"}),
                 "null_var": to_protobuf_value(None),
             },
             options=ExecuteRequest.Options(
                 mocks=[
-                    Mock(
+                    Mock_(
                         on=Mock.On(
                             static=Mock.Params(
                                 integration_type="integration_type",
                                 step_name="step_name",
                                 inputs=to_protobuf_value({"foo": "bar"}),
                             ),
-                            dynamic=api_mock.get_return_func_id(),
-                        )
+                            dynamic=get_unique_id_for_object(api_mock.on_callable),
+                        ),
+                        return_=Mock.Return(static=to_protobuf_value({"some": "return"})),
                     )
                 ],
                 include_event_outputs=True,
             ),
             fetch=ExecuteRequest.Fetch(
                 id="api_id",
                 profile=Profile(name="profile_name"),
                 view_mode=ViewMode.DEPLOYED.to_proto_view_mode(),
                 commit_id="commit_id",
                 branch_name="branch_name",
             ),
         )
-        # i hate this but have not found a better way
-        return_value = getattr(expected.options.mocks[0], "return")
-        return_value.CopyFrom(expected_mock_return)
 
         self.assertEqual(expected, actual)
 
     def test_handle_two_way_response_invalid_type(self):
-        api = Api(ApiConfig(api_id="api_id"))
+        api = Api("api_id")
         func = api.get_handle_two_way_response_func()
 
         with self.assertRaises(Exception) as context:
             func(TwoWayResponse())
         self.assertEqual(
             "got unexpected type: <class 'api.v1.service_pb2.TwoWayResponse'>",
             str(context.exception),
         )
 
     def test_handle_two_way_response_stream_type(self):
-        api = Api(ApiConfig(api_id="api_id"))
+        api = Api("api_id")
         func = api.get_handle_two_way_response_func()
 
         stream_response = TwoWayResponse(
             stream=StreamResponse(
                 execution="execution",
                 event=Event(data=Event.Data(value=to_protobuf_value("some data"))),
             )
         )
         actual = func(stream_response)
         self.assertEqual(2, len(actual))
         self.assertIsNone(actual[0])
         self.assertEqual(stream_response, actual[1])
 
     def test_handle_two_way_response_function_type_function_call_succeeds(self):
-        api = Api(ApiConfig(api_id="api_id"))
+        api = Api("api_id")
         func = api.get_handle_two_way_response_func()
 
         # have to set up function map first
         def return_func(filters: MockApiFilters) -> dict:
             return {"given_params": filters}
 
         api_mock = ApiMock(return_val_or_callable=return_func)
 
         api.hydrate_mock_func_lookup([api_mock])
 
         function_response = TwoWayResponse(
             function=Function.Request(
-                name=api_mock.get_return_func_id(),
+                name=get_unique_id_for_object(api_mock.return_val_or_callable),
                 parameters=[to_protobuf_value({"foo": "bar"})],
                 id="some_id",
             )
         )
         actual = func(function_response)
         self.assertEqual(2, len(actual))
         self.assertIsNone(actual[1])
@@ -144,60 +143,79 @@
                     value=to_protobuf_value({"given_params": {"foo": "bar"}}), id="some_id"
                 )
             ),
             actual[0],
         )
 
     def test_handle_two_way_response_function_type_function_call_fails(self):
-        api = Api(ApiConfig(api_id="api_id"))
+        api = Api("api_id")
         func = api.get_handle_two_way_response_func()
 
         # have to set up function map first
         def return_func(_: MockApiFilters) -> dict:
-            raise Exception("called func error")
+            raise Exception("expected test error")
 
         api_mock = ApiMock(return_val_or_callable=return_func)
 
         api.hydrate_mock_func_lookup([api_mock])
 
         function_response = TwoWayResponse(
             function=Function.Request(
-                name=api_mock.get_return_func_id(),
+                name=get_unique_id_for_object(api_mock.return_val_or_callable),
                 parameters=[to_protobuf_value({"foo": "bar"})],
                 id="some_id",
             )
         )
         actual = func(function_response)
         self.assertEqual(2, len(actual))
         self.assertIsNone(actual[1])
         self.assertEqual(
             TwoWayRequest(
-                function=Function.Response(error=Error(message="called func error"), id="some_id")
+                function=Function.Response(error=Error(message="expected test error"), id="some_id")
             ),
             actual[0],
         )
 
     def test_hydrate_mock_func_lookup_no_mocks_given(self):
-        api = Api(ApiConfig(api_id="api_id"))
+        api = Api("api_id")
         api.hydrate_mock_func_lookup([])
         self.assertEqual({}, api.mock_func_lookup)
 
     def test_hydrate_mock_func_lookup_only_mocks_with_dict_value_given(self):
-        api = Api(ApiConfig(api_id="api_id"))
+        api = Api("api_id")
         mock_1 = ApiMock(return_val_or_callable={"foo": "bar"})
         api.hydrate_mock_func_lookup([mock_1])
         self.assertEqual({}, api.mock_func_lookup)
 
     def test_hydrate_mock_func_lookup_only_mocks_with_func_value_given(self):
-        api = Api(ApiConfig(api_id="api_id"))
+        api = Api("api_id")
         mock_1_func = lambda x: x
         mock_1 = ApiMock(return_val_or_callable=mock_1_func)
         api.hydrate_mock_func_lookup([mock_1])
-        self.assertEqual({mock_1.get_return_func_id(): mock_1_func}, api.mock_func_lookup)
+        self.assertEqual(
+            {get_unique_id_for_object(mock_1.return_val_or_callable): mock_1_func},
+            api.mock_func_lookup,
+        )
 
     def test_hydrate_mock_func_lookup_mocks_with_func_value_and_mocks_with_dict_value_given(self):
-        api = Api(ApiConfig(api_id="api_id"))
+        api = Api("api_id")
         mock_1_func = lambda x: x
         mock_1 = ApiMock(return_val_or_callable=mock_1_func)
         mock_2 = ApiMock(return_val_or_callable={"foo": "bar"})
         api.hydrate_mock_func_lookup([mock_1, mock_2])
-        self.assertEqual({mock_1.get_return_func_id(): mock_1_func}, api.mock_func_lookup)
+        self.assertEqual(
+            {get_unique_id_for_object(mock_1.return_val_or_callable): mock_1_func},
+            api.mock_func_lookup,
+        )
+
+    def test_handle_two_way_response__function_to_execute_not_found(self):
+        api = Api("api_id")
+
+        func = api.get_handle_two_way_response_func()
+
+        with self.assertRaises(Exception) as context:
+            func(
+                TwoWayResponse(
+                    function=Function.Request(id="some_id", name="im_not_found", parameters=[])
+                )
+            )
+        self.assertEqual("FOUND NO FUNCTION TO EXECUTE!", str(context.exception))
```

