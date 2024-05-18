# Comparing `tmp/abcli-8.172.1.tar.gz` & `tmp/abcli-8.175.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abcli-8.172.1.tar", last modified: Sat May 18 01:32:25 2024, max compression
+gzip compressed data, was "abcli-8.175.1.tar", last modified: Sat May 18 01:41:44 2024, max compression
```

## Comparing `abcli-8.172.1.tar` & `abcli-8.175.1.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.158897 abcli-8.172.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     1236 2024-05-18 01:32:25.157972 abcli-8.172.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     1034 2024-05-18 01:30:22.000000 abcli-8.172.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.075134 abcli-8.172.1/abcli/
--rw-r--r--   0 kamangir   (502) staff       (20)      290 2024-05-18 01:32:16.000000 abcli-8.172.1/abcli/__init__.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.083089 abcli-8.172.1/abcli/bash/
--rw-r--r--   0 kamangir   (502) staff       (20)        0 2022-08-19 04:11:13.000000 abcli-8.172.1/abcli/bash/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       96 2024-04-21 22:44:21.000000 abcli-8.172.1/abcli/bash/colors.py
--rw-r--r--   0 kamangir   (502) staff       (20)      598 2024-02-18 05:10:50.000000 abcli-8.172.1/abcli/bash/help.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2309 2024-04-21 22:45:41.000000 abcli-8.172.1/abcli/bash/list.py
--rw-r--r--   0 kamangir   (502) staff       (20)      777 2024-04-21 23:19:04.000000 abcli-8.172.1/abcli/bash/logging.py
--rw-r--r--   0 kamangir   (502) staff       (20)      784 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      537 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/elapsed_timer.py
--rw-r--r--   0 kamangir   (502) staff       (20)     5290 2024-04-27 21:10:00.000000 abcli-8.172.1/abcli/env.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.089977 abcli-8.172.1/abcli/file/
--rw-r--r--   0 kamangir   (502) staff       (20)      109 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/file/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      996 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/file/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      570 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/file/classes.py
--rw-r--r--   0 kamangir   (502) staff       (20)     9177 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/file/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)     6315 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/file/load.py
--rw-r--r--   0 kamangir   (502) staff       (20)     7303 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/file/save.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.094758 abcli-8.172.1/abcli/keywords/
--rw-r--r--   0 kamangir   (502) staff       (20)       84 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/keywords/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      897 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/keywords/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      236 2022-08-20 04:12:52.000000 abcli-8.172.1/abcli/keywords/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1407 2024-04-23 03:10:32.000000 abcli-8.172.1/abcli/keywords/keywords.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1353 2024-04-29 00:44:19.000000 abcli-8.172.1/abcli/logger.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.096489 abcli-8.172.1/abcli/modules/
--rw-r--r--   0 kamangir   (502) staff       (20)       23 2022-08-28 06:57:23.000000 abcli-8.172.1/abcli/modules/__init__.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.099309 abcli-8.172.1/abcli/modules/host/
--rw-r--r--   0 kamangir   (502) staff       (20)       90 2022-09-21 00:58:39.000000 abcli-8.172.1/abcli/modules/host/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2523 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/modules/host/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     5416 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/modules/host/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2025 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/modules/objects.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.103754 abcli-8.172.1/abcli/options/
--rw-r--r--   0 kamangir   (502) staff       (20)       53 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/options/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1751 2024-05-08 04:06:06.000000 abcli-8.172.1/abcli/options/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2826 2024-05-10 02:13:35.000000 abcli-8.172.1/abcli/options/classes.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.106193 abcli-8.172.1/abcli/path/
--rw-r--r--   0 kamangir   (502) staff       (20)       68 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/path/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       10 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/path/consts.py
--rw-r--r--   0 kamangir   (502) staff       (20)     5254 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/path/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.111814 abcli-8.172.1/abcli/plugins/
--rw-r--r--   0 kamangir   (502) staff       (20)       49 2022-08-20 04:12:52.000000 abcli-8.172.1/abcli/plugins/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      916 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/__main__.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.113961 abcli-8.172.1/abcli/plugins/cache/
--rw-r--r--   0 kamangir   (502) staff       (20)       55 2022-08-20 04:12:52.000000 abcli-8.172.1/abcli/plugins/cache/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1646 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/cache/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     4705 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/cache/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)      705 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.116431 abcli-8.172.1/abcli/plugins/git/
--rw-r--r--   0 kamangir   (502) staff       (20)       52 2024-04-21 00:01:01.000000 abcli-8.172.1/abcli/plugins/git/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      706 2024-04-21 23:37:21.000000 abcli-8.172.1/abcli/plugins/git/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1706 2024-05-17 02:03:11.000000 abcli-8.172.1/abcli/plugins/git/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.118799 abcli-8.172.1/abcli/plugins/gpu/
--rw-r--r--   0 kamangir   (502) staff       (20)       52 2022-08-20 04:12:52.000000 abcli-8.172.1/abcli/plugins/gpu/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      499 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/gpu/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      590 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/gpu/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.125908 abcli-8.172.1/abcli/plugins/graphics/
--rw-r--r--   0 kamangir   (502) staff       (20)      124 2022-09-25 02:29:01.000000 abcli-8.172.1/abcli/plugins/graphics/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1462 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/graphics/constants.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1740 2024-05-08 02:05:01.000000 abcli-8.172.1/abcli/plugins/graphics/gif.py
--rw-r--r--   0 kamangir   (502) staff       (20)      431 2022-08-14 18:15:57.000000 abcli-8.172.1/abcli/plugins/graphics/image.py
--rw-r--r--   0 kamangir   (502) staff       (20)     3591 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/graphics/signature.py
--rw-r--r--   0 kamangir   (502) staff       (20)     6641 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/graphics/text.py
--rw-r--r--   0 kamangir   (502) staff       (20)      953 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/markdown.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.128311 abcli-8.172.1/abcli/plugins/metadata/
--rw-r--r--   0 kamangir   (502) staff       (20)       58 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/metadata/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2109 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/metadata/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2231 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/metadata/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.130893 abcli-8.172.1/abcli/plugins/relations/
--rw-r--r--   0 kamangir   (502) staff       (20)       59 2022-08-20 04:12:52.000000 abcli-8.172.1/abcli/plugins/relations/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2102 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/relations/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     5157 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/relations/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)      680 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/seed.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.133770 abcli-8.172.1/abcli/plugins/storage/
--rw-r--r--   0 kamangir   (502) staff       (20)       83 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/storage/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2248 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/storage/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     8063 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/storage/classes.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.136344 abcli-8.172.1/abcli/plugins/tags/
--rw-r--r--   0 kamangir   (502) staff       (20)       55 2022-08-20 04:12:52.000000 abcli-8.172.1/abcli/plugins/tags/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2219 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/tags/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     5991 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/tags/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)      344 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/testing.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1313 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/plugins/video.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.140428 abcli-8.172.1/abcli/string/
--rw-r--r--   0 kamangir   (502) staff       (20)      244 2024-02-18 05:23:47.000000 abcli-8.172.1/abcli/string/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1138 2024-02-18 05:23:40.000000 abcli-8.172.1/abcli/string/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      216 2024-02-18 05:23:45.000000 abcli-8.172.1/abcli/string/constants.py
--rw-r--r--   0 kamangir   (502) staff       (20)    11283 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/string/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.142280 abcli-8.172.1/abcli/table/
--rw-r--r--   0 kamangir   (502) staff       (20)       45 2022-08-20 04:12:52.000000 abcli-8.172.1/abcli/table/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     4541 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/table/classes.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.155531 abcli-8.172.1/abcli/tests/
--rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/tests/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       69 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/tests/test_abcli.py
--rw-r--r--   0 kamangir   (502) staff       (20)      275 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/tests/test_env.py
--rw-r--r--   0 kamangir   (502) staff       (20)      410 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/tests/test_modules_objects.py
--rw-r--r--   0 kamangir   (502) staff       (20)     3194 2024-05-10 02:20:04.000000 abcli-8.172.1/abcli/tests/test_options.py
--rw-r--r--   0 kamangir   (502) staff       (20)      634 2024-05-08 02:13:37.000000 abcli-8.172.1/abcli/tests/test_plugins_graphics_gif_generate_animated_gif.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1037 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/tests/test_plugins_graphics_signature.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2831 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/tests/test_plugins_metadata.py
--rw-r--r--   0 kamangir   (502) staff       (20)      777 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/tests/test_plugins_testing.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2199 2024-04-21 00:00:57.000000 abcli-8.172.1/abcli/timer.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:32:25.157239 abcli-8.172.1/abcli.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     1236 2024-05-18 01:32:25.000000 abcli-8.172.1/abcli.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     2403 2024-05-18 01:32:25.000000 abcli-8.172.1/abcli.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-18 01:32:25.000000 abcli-8.172.1/abcli.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        6 2024-05-18 01:32:25.000000 abcli-8.172.1/abcli.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-18 01:32:25.159051 abcli-8.172.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)     1163 2024-05-18 01:31:55.000000 abcli-8.172.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:44.042930 abcli-8.175.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     1346 2024-05-18 01:41:44.041609 abcli-8.175.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     1034 2024-05-18 01:40:59.000000 abcli-8.175.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:43.950800 abcli-8.175.1/abcli/
+-rw-r--r--   0 kamangir   (502) staff       (20)      290 2024-05-18 01:41:13.000000 abcli-8.175.1/abcli/__init__.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:43.956521 abcli-8.175.1/abcli/bash/
+-rw-r--r--   0 kamangir   (502) staff       (20)        0 2022-08-19 04:11:13.000000 abcli-8.175.1/abcli/bash/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       96 2024-04-21 22:44:21.000000 abcli-8.175.1/abcli/bash/colors.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      598 2024-02-18 05:10:50.000000 abcli-8.175.1/abcli/bash/help.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2309 2024-04-21 22:45:41.000000 abcli-8.175.1/abcli/bash/list.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      777 2024-04-21 23:19:04.000000 abcli-8.175.1/abcli/bash/logging.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      784 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      537 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/elapsed_timer.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     5290 2024-04-27 21:10:00.000000 abcli-8.175.1/abcli/env.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:43.965343 abcli-8.175.1/abcli/file/
+-rw-r--r--   0 kamangir   (502) staff       (20)      109 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/file/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      996 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/file/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      570 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/file/classes.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     9177 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/file/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     6315 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/file/load.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     7303 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/file/save.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:43.969946 abcli-8.175.1/abcli/keywords/
+-rw-r--r--   0 kamangir   (502) staff       (20)       84 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/keywords/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      897 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/keywords/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      236 2022-08-20 04:12:52.000000 abcli-8.175.1/abcli/keywords/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1407 2024-04-23 03:10:32.000000 abcli-8.175.1/abcli/keywords/keywords.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1353 2024-04-29 00:44:19.000000 abcli-8.175.1/abcli/logger.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:43.971534 abcli-8.175.1/abcli/modules/
+-rw-r--r--   0 kamangir   (502) staff       (20)       23 2022-08-28 06:57:23.000000 abcli-8.175.1/abcli/modules/__init__.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:43.973985 abcli-8.175.1/abcli/modules/host/
+-rw-r--r--   0 kamangir   (502) staff       (20)       90 2022-09-21 00:58:39.000000 abcli-8.175.1/abcli/modules/host/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2523 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/modules/host/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     5416 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/modules/host/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2025 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/modules/objects.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:43.976574 abcli-8.175.1/abcli/options/
+-rw-r--r--   0 kamangir   (502) staff       (20)       53 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/options/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1751 2024-05-08 04:06:06.000000 abcli-8.175.1/abcli/options/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2826 2024-05-10 02:13:35.000000 abcli-8.175.1/abcli/options/classes.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:43.979027 abcli-8.175.1/abcli/path/
+-rw-r--r--   0 kamangir   (502) staff       (20)       68 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/path/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       10 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/path/consts.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     5254 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/path/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:43.985896 abcli-8.175.1/abcli/plugins/
+-rw-r--r--   0 kamangir   (502) staff       (20)       49 2022-08-20 04:12:52.000000 abcli-8.175.1/abcli/plugins/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      916 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/__main__.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:43.988427 abcli-8.175.1/abcli/plugins/cache/
+-rw-r--r--   0 kamangir   (502) staff       (20)       55 2022-08-20 04:12:52.000000 abcli-8.175.1/abcli/plugins/cache/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1646 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/cache/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     4705 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/cache/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      705 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:43.990677 abcli-8.175.1/abcli/plugins/git/
+-rw-r--r--   0 kamangir   (502) staff       (20)       52 2024-04-21 00:01:01.000000 abcli-8.175.1/abcli/plugins/git/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      706 2024-04-21 23:37:21.000000 abcli-8.175.1/abcli/plugins/git/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1706 2024-05-17 02:03:11.000000 abcli-8.175.1/abcli/plugins/git/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:43.993032 abcli-8.175.1/abcli/plugins/gpu/
+-rw-r--r--   0 kamangir   (502) staff       (20)       52 2022-08-20 04:12:52.000000 abcli-8.175.1/abcli/plugins/gpu/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      499 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/gpu/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      590 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/gpu/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:43.998296 abcli-8.175.1/abcli/plugins/graphics/
+-rw-r--r--   0 kamangir   (502) staff       (20)      124 2022-09-25 02:29:01.000000 abcli-8.175.1/abcli/plugins/graphics/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1462 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/graphics/constants.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1740 2024-05-08 02:05:01.000000 abcli-8.175.1/abcli/plugins/graphics/gif.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      431 2022-08-14 18:15:57.000000 abcli-8.175.1/abcli/plugins/graphics/image.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     3591 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/graphics/signature.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     6641 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/graphics/text.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      953 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/markdown.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:44.000934 abcli-8.175.1/abcli/plugins/metadata/
+-rw-r--r--   0 kamangir   (502) staff       (20)       58 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/metadata/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2109 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/metadata/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2231 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/metadata/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:44.003687 abcli-8.175.1/abcli/plugins/relations/
+-rw-r--r--   0 kamangir   (502) staff       (20)       59 2022-08-20 04:12:52.000000 abcli-8.175.1/abcli/plugins/relations/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2102 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/relations/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     5157 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/relations/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      680 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/seed.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:44.007470 abcli-8.175.1/abcli/plugins/storage/
+-rw-r--r--   0 kamangir   (502) staff       (20)       83 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/storage/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2248 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/storage/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     8063 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/storage/classes.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:44.010243 abcli-8.175.1/abcli/plugins/tags/
+-rw-r--r--   0 kamangir   (502) staff       (20)       55 2022-08-20 04:12:52.000000 abcli-8.175.1/abcli/plugins/tags/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2219 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/tags/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     5991 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/tags/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      344 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/testing.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1313 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/plugins/video.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:44.013735 abcli-8.175.1/abcli/string/
+-rw-r--r--   0 kamangir   (502) staff       (20)      244 2024-02-18 05:23:47.000000 abcli-8.175.1/abcli/string/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1138 2024-02-18 05:23:40.000000 abcli-8.175.1/abcli/string/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      216 2024-02-18 05:23:45.000000 abcli-8.175.1/abcli/string/constants.py
+-rw-r--r--   0 kamangir   (502) staff       (20)    11283 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/string/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:44.019292 abcli-8.175.1/abcli/table/
+-rw-r--r--   0 kamangir   (502) staff       (20)       45 2022-08-20 04:12:52.000000 abcli-8.175.1/abcli/table/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     4541 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/table/classes.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:44.039317 abcli-8.175.1/abcli/tests/
+-rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/tests/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       69 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/tests/test_abcli.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      275 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/tests/test_env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      410 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/tests/test_modules_objects.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     3194 2024-05-10 02:20:04.000000 abcli-8.175.1/abcli/tests/test_options.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      634 2024-05-08 02:13:37.000000 abcli-8.175.1/abcli/tests/test_plugins_graphics_gif_generate_animated_gif.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1037 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/tests/test_plugins_graphics_signature.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2831 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/tests/test_plugins_metadata.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      777 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/tests/test_plugins_testing.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2199 2024-04-21 00:00:57.000000 abcli-8.175.1/abcli/timer.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 01:41:44.040497 abcli-8.175.1/abcli.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     1346 2024-05-18 01:41:43.000000 abcli-8.175.1/abcli.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     2403 2024-05-18 01:41:43.000000 abcli-8.175.1/abcli.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-18 01:41:43.000000 abcli-8.175.1/abcli.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        6 2024-05-18 01:41:43.000000 abcli-8.175.1/abcli.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-18 01:41:44.043100 abcli-8.175.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)     1127 2024-05-18 01:40:51.000000 abcli-8.175.1/setup.py
```

### Comparing `abcli-8.172.1/PKG-INFO` & `abcli-8.175.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,10 @@
-Metadata-Version: 2.1
-Name: abcli
-Version: 8.172.1
-Summary: 🚀 a language to speak AI.
-Author: kamangir
-Description-Content-Type: text/markdown
-
 # awesome bash cli (abcli/abc)
 
-![image](https://github.com/kamangir/awesome-bash-cli/raw/current/assets/marquee.png)
+![image](./assets/marquee.png)
 
 `abcli` 🚀 is an implementation of [🔻 giza](https://github.com/kamangir/giza) and the library behind [these projects](https://github.com/kamangir/kamangir).
 
 To install `abcli` follow the instructions for:
 
 - [Amazon EC2 instances](https://github.com/kamangir/awesome-bash-cli/wiki/ec2)
 - [Amazon SageMaker](https://github.com/kamangir/blue-plugin/blob/main/SageMaker.md)
```

### Comparing `abcli-8.172.1/README.md` & `abcli-8.175.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,17 @@
+Metadata-Version: 2.1
+Name: abcli
+Version: 8.175.1
+Summary: 🚀 a language to speak AI.
+Author: kamangir
+Description-Content-Type: text/markdown
+
 # awesome bash cli (abcli/abc)
 
-![image](./assets/marquee.png)
+![image](https://github.com/kamangir/awesome-bash-cli/raw/current/assets/marquee.png)
 
 `abcli` 🚀 is an implementation of [🔻 giza](https://github.com/kamangir/giza) and the library behind [these projects](https://github.com/kamangir/kamangir).
 
 To install `abcli` follow the instructions for:
 
 - [Amazon EC2 instances](https://github.com/kamangir/awesome-bash-cli/wiki/ec2)
 - [Amazon SageMaker](https://github.com/kamangir/blue-plugin/blob/main/SageMaker.md)
@@ -14,13 +21,13 @@
 
 To see the list of `abcli` commands type in:
 
 ```
 abcli ?
 ```
 
-To configure `abcli` complete the [.env](./.env) file using this [sample](./sample.env).
+To configure `abcli` complete the [.env](https://github.com/kamangir/awesome-bash-cli/raw/current/.env) file using this [sample](https://github.com/kamangir/awesome-bash-cli/raw/current/sample.env).
 
 ## branches
 
 - [current](.) active branch.
 - [main](https://github.com/kamangir/awesome-bash-cli/tree/main) running on [a cluster of Raspberry pis](https://github.com/kamangir/blue-bracket), do not touch. ⚠️
```

### Comparing `abcli-8.172.1/abcli/bash/help.py` & `abcli-8.175.1/abcli/bash/help.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/bash/list.py` & `abcli-8.175.1/abcli/bash/list.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/bash/logging.py` & `abcli-8.175.1/abcli/bash/logging.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/config.env` & `abcli-8.175.1/abcli/config.env`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/elapsed_timer.py` & `abcli-8.175.1/abcli/elapsed_timer.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/env.py` & `abcli-8.175.1/abcli/env.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/file/__main__.py` & `abcli-8.175.1/abcli/file/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/file/classes.py` & `abcli-8.175.1/abcli/file/classes.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/file/functions.py` & `abcli-8.175.1/abcli/file/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/file/load.py` & `abcli-8.175.1/abcli/file/load.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/file/save.py` & `abcli-8.175.1/abcli/file/save.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/keywords/__main__.py` & `abcli-8.175.1/abcli/keywords/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/keywords/keywords.py` & `abcli-8.175.1/abcli/keywords/keywords.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/logger.py` & `abcli-8.175.1/abcli/logger.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/modules/host/__main__.py` & `abcli-8.175.1/abcli/modules/host/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/modules/host/functions.py` & `abcli-8.175.1/abcli/modules/host/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/modules/objects.py` & `abcli-8.175.1/abcli/modules/objects.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/options/__main__.py` & `abcli-8.175.1/abcli/options/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/options/classes.py` & `abcli-8.175.1/abcli/options/classes.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/path/functions.py` & `abcli-8.175.1/abcli/path/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/__main__.py` & `abcli-8.175.1/abcli/plugins/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/cache/__main__.py` & `abcli-8.175.1/abcli/plugins/cache/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/cache/functions.py` & `abcli-8.175.1/abcli/plugins/cache/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/functions.py` & `abcli-8.175.1/abcli/plugins/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/git/__main__.py` & `abcli-8.175.1/abcli/plugins/git/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/git/functions.py` & `abcli-8.175.1/abcli/plugins/git/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/gpu/functions.py` & `abcli-8.175.1/abcli/plugins/gpu/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/graphics/constants.py` & `abcli-8.175.1/abcli/plugins/graphics/constants.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/graphics/gif.py` & `abcli-8.175.1/abcli/plugins/graphics/gif.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/graphics/signature.py` & `abcli-8.175.1/abcli/plugins/graphics/signature.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/graphics/text.py` & `abcli-8.175.1/abcli/plugins/graphics/text.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/markdown.py` & `abcli-8.175.1/abcli/plugins/markdown.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/metadata/__main__.py` & `abcli-8.175.1/abcli/plugins/metadata/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/metadata/functions.py` & `abcli-8.175.1/abcli/plugins/metadata/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/relations/__main__.py` & `abcli-8.175.1/abcli/plugins/relations/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/relations/functions.py` & `abcli-8.175.1/abcli/plugins/relations/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/seed.py` & `abcli-8.175.1/abcli/plugins/seed.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/storage/__main__.py` & `abcli-8.175.1/abcli/plugins/storage/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/storage/classes.py` & `abcli-8.175.1/abcli/plugins/storage/classes.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/tags/__main__.py` & `abcli-8.175.1/abcli/plugins/tags/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/tags/functions.py` & `abcli-8.175.1/abcli/plugins/tags/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/plugins/video.py` & `abcli-8.175.1/abcli/plugins/video.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/string/__main__.py` & `abcli-8.175.1/abcli/string/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/string/functions.py` & `abcli-8.175.1/abcli/string/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/table/classes.py` & `abcli-8.175.1/abcli/table/classes.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/tests/test_options.py` & `abcli-8.175.1/abcli/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/tests/test_plugins_graphics_gif_generate_animated_gif.py` & `abcli-8.175.1/abcli/tests/test_plugins_graphics_gif_generate_animated_gif.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/tests/test_plugins_graphics_signature.py` & `abcli-8.175.1/abcli/tests/test_plugins_graphics_signature.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/tests/test_plugins_metadata.py` & `abcli-8.175.1/abcli/tests/test_plugins_metadata.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/tests/test_plugins_testing.py` & `abcli-8.175.1/abcli/tests/test_plugins_testing.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli/timer.py` & `abcli-8.175.1/abcli/timer.py`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/abcli.egg-info/PKG-INFO` & `abcli-8.175.1/abcli.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abcli
-Version: 8.172.1
+Version: 8.175.1
 Summary: 🚀 a language to speak AI.
 Author: kamangir
 Description-Content-Type: text/markdown
 
 # awesome bash cli (abcli/abc)
 
 ![image](https://github.com/kamangir/awesome-bash-cli/raw/current/assets/marquee.png)
@@ -21,13 +21,13 @@
 
 To see the list of `abcli` commands type in:
 
 ```
 abcli ?
 ```
 
-To configure `abcli` complete the [.env](./.env) file using this [sample](./sample.env).
+To configure `abcli` complete the [.env](https://github.com/kamangir/awesome-bash-cli/raw/current/.env) file using this [sample](https://github.com/kamangir/awesome-bash-cli/raw/current/sample.env).
 
 ## branches
 
 - [current](.) active branch.
 - [main](https://github.com/kamangir/awesome-bash-cli/tree/main) running on [a cluster of Raspberry pis](https://github.com/kamangir/blue-bracket), do not touch. ⚠️
```

### Comparing `abcli-8.172.1/abcli.egg-info/SOURCES.txt` & `abcli-8.175.1/abcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abcli-8.172.1/setup.py` & `abcli-8.175.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 import os
 
 from abcli import NAME, VERSION, DESCRIPTION
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as f:
     long_description = f.read().replace(
-        "./assets/marquee.png",
-        "https://github.com/kamangir/awesome-bash-cli/raw/current/assets/marquee.png",
+        "./",
+        "https://github.com/kamangir/awesome-bash-cli/raw/current/",
     )
 
 
 setup(
     name=NAME,
     author="kamangir",
     version=VERSION,
```

