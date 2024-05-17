# Comparing `tmp/owega-5.8.0.tar.gz` & `tmp/owega-5.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owega-5.8.0.tar", last modified: Fri May 17 21:54:38 2024, max compression
+gzip compressed data, was "owega-5.8.1.tar", last modified: Fri May 17 22:04:42 2024, max compression
```

## Comparing `owega-5.8.0.tar` & `owega-5.8.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 21:54:38.146937 owega-5.8.0/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6076 2024-05-17 21:44:57.000000 owega-5.8.0/LICENSE
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    16737 2024-05-17 21:54:38.146937 owega-5.8.0/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5183 2024-05-17 21:44:57.000000 owega-5.8.0/README.md
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 21:54:38.144938 owega-5.8.0/owega/
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 21:54:38.145938 owega-5.8.0/owega/OweHandlers/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      980 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_add_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1590 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_commands.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1185 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_context.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1601 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_del_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_dinput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3457 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_edit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1302 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_estimation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5059 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_finput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_frequency.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      521 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_genconf.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      523 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_history.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3246 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_image.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1118 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_load.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1698 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_model.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1791 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_presence.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      637 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_quit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1090 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_save.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      945 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_system.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1739 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_temperature.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1339 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_time.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1404 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_tokens.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1556 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_top_p.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1245 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_tts.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2470 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handlers.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 21:54:38.145938 owega-5.8.0/owega/OwegaFun/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OwegaFun/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OwegaFun/functions.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4342 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OwegaFun/longTermSouvenirs.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5816 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OwegaFun/utility.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 21:54:38.145938 owega-5.8.0/owega/OwegaSession/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OwegaSession/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3628 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OwegaSession/main_bottom_toolbar.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5592 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OwegaSession/promptsession.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      175 2024-05-17 21:44:57.000000 owega-5.8.0/owega/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-05-17 21:44:57.000000 owega-5.8.0/owega/__main__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10338 2024-05-17 21:44:57.000000 owega-5.8.0/owega/ask.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 21:54:38.146937 owega-5.8.0/owega/changelog/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-05-17 21:44:57.000000 owega-5.8.0/owega/changelog/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    25331 2024-05-17 21:44:57.000000 owega-5.8.0/owega/changelog/changelog.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1534 2024-05-17 21:44:57.000000 owega-5.8.0/owega/changelog/changelogEntry.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-05-17 21:44:57.000000 owega-5.8.0/owega/changelog/version.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 21:54:38.146937 owega-5.8.0/owega/config/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-05-17 21:44:57.000000 owega-5.8.0/owega/config/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2655 2024-05-17 21:44:57.000000 owega-5.8.0/owega/config/baseConf.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 21:54:38.146937 owega-5.8.0/owega/conversation/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-05-17 21:44:57.000000 owega-5.8.0/owega/conversation/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10105 2024-05-17 21:44:57.000000 owega-5.8.0/owega/conversation/conversation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1418 2024-05-17 21:44:57.000000 owega-5.8.0/owega/getLogger.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-05-17 21:44:57.000000 owega-5.8.0/owega/handlerBase.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6141 2024-05-17 21:44:57.000000 owega-5.8.0/owega/license.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    11780 2024-05-17 21:44:57.000000 owega-5.8.0/owega/owega.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     7504 2024-05-17 21:44:57.000000 owega-5.8.0/owega/utils.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 21:54:38.146937 owega-5.8.0/owega.egg-info/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    16737 2024-05-17 21:54:38.000000 owega-5.8.0/owega.egg-info/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1689 2024-05-17 21:54:38.000000 owega-5.8.0/owega.egg-info/SOURCES.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-05-17 21:54:38.000000 owega-5.8.0/owega.egg-info/dependency_links.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-05-17 21:54:38.000000 owega-5.8.0/owega.egg-info/entry_points.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      173 2024-05-17 21:54:38.000000 owega-5.8.0/owega.egg-info/requires.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-05-17 21:54:38.000000 owega-5.8.0/owega.egg-info/top_level.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-05-17 21:44:57.000000 owega-5.8.0/pyproject.toml
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-05-17 21:54:38.146937 owega-5.8.0/setup.cfg
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2093 2024-05-17 21:44:57.000000 owega-5.8.0/setup.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 22:04:42.119935 owega-5.8.1/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6076 2024-05-10 14:44:53.000000 owega-5.8.1/LICENSE
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    16793 2024-05-17 22:04:42.119935 owega-5.8.1/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5183 2024-05-14 00:10:08.000000 owega-5.8.1/README.md
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 22:04:42.117935 owega-5.8.1/owega/
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 22:04:42.118935 owega-5.8.1/owega/OweHandlers/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-27 12:05:16.000000 owega-5.8.1/owega/OweHandlers/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      980 2024-05-08 02:39:07.000000 owega-5.8.1/owega/OweHandlers/handle_add_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1590 2024-05-08 02:39:07.000000 owega-5.8.1/owega/OweHandlers/handle_commands.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1185 2024-05-08 02:39:07.000000 owega-5.8.1/owega/OweHandlers/handle_context.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1601 2024-05-08 02:39:07.000000 owega-5.8.1/owega/OweHandlers/handle_del_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 02:39:07.000000 owega-5.8.1/owega/OweHandlers/handle_dinput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3457 2024-05-08 02:39:07.000000 owega-5.8.1/owega/OweHandlers/handle_edit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1302 2024-05-17 21:35:33.000000 owega-5.8.1/owega/OweHandlers/handle_estimation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5059 2024-05-08 02:39:07.000000 owega-5.8.1/owega/OweHandlers/handle_finput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 02:39:07.000000 owega-5.8.1/owega/OweHandlers/handle_frequency.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      521 2024-05-08 02:39:07.000000 owega-5.8.1/owega/OweHandlers/handle_genconf.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      523 2024-05-08 02:39:07.000000 owega-5.8.1/owega/OweHandlers/handle_history.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3246 2024-05-13 23:20:56.000000 owega-5.8.1/owega/OweHandlers/handle_image.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1118 2024-05-08 02:39:08.000000 owega-5.8.1/owega/OweHandlers/handle_load.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1698 2024-05-08 02:39:08.000000 owega-5.8.1/owega/OweHandlers/handle_model.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1791 2024-05-08 02:39:08.000000 owega-5.8.1/owega/OweHandlers/handle_presence.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      637 2024-05-08 02:39:08.000000 owega-5.8.1/owega/OweHandlers/handle_quit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1090 2024-05-08 02:39:08.000000 owega-5.8.1/owega/OweHandlers/handle_save.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      945 2024-05-08 02:39:08.000000 owega-5.8.1/owega/OweHandlers/handle_system.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1739 2024-05-08 02:39:08.000000 owega-5.8.1/owega/OweHandlers/handle_temperature.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1339 2024-05-17 21:37:36.000000 owega-5.8.1/owega/OweHandlers/handle_time.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1404 2024-05-08 02:39:08.000000 owega-5.8.1/owega/OweHandlers/handle_tokens.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1556 2024-05-08 02:39:08.000000 owega-5.8.1/owega/OweHandlers/handle_top_p.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1245 2024-05-08 02:39:08.000000 owega-5.8.1/owega/OweHandlers/handle_tts.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2470 2024-05-17 21:32:24.000000 owega-5.8.1/owega/OweHandlers/handlers.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 22:04:42.118935 owega-5.8.1/owega/OwegaFun/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-04-27 12:05:16.000000 owega-5.8.1/owega/OwegaFun/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-04-17 02:21:38.000000 owega-5.8.1/owega/OwegaFun/functions.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4342 2024-04-27 12:05:16.000000 owega-5.8.1/owega/OwegaFun/longTermSouvenirs.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5816 2024-04-27 12:05:16.000000 owega-5.8.1/owega/OwegaFun/utility.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 22:04:42.118935 owega-5.8.1/owega/OwegaSession/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-17 02:21:38.000000 owega-5.8.1/owega/OwegaSession/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3628 2024-05-17 21:37:09.000000 owega-5.8.1/owega/OwegaSession/main_bottom_toolbar.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5592 2024-04-27 12:05:16.000000 owega-5.8.1/owega/OwegaSession/promptsession.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      175 2024-05-08 02:39:08.000000 owega-5.8.1/owega/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-17 02:21:38.000000 owega-5.8.1/owega/__main__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10338 2024-05-13 22:30:06.000000 owega-5.8.1/owega/ask.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 22:04:42.118935 owega-5.8.1/owega/changelog/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-04-27 12:05:16.000000 owega-5.8.1/owega/changelog/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    25476 2024-05-17 22:02:02.000000 owega-5.8.1/owega/changelog/changelog.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1534 2024-04-27 12:05:16.000000 owega-5.8.1/owega/changelog/changelogEntry.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-04-17 02:21:38.000000 owega-5.8.1/owega/changelog/version.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 22:04:42.118935 owega-5.8.1/owega/config/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-17 02:21:38.000000 owega-5.8.1/owega/config/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2655 2024-05-17 20:51:25.000000 owega-5.8.1/owega/config/baseConf.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 22:04:42.119935 owega-5.8.1/owega/conversation/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-17 02:21:38.000000 owega-5.8.1/owega/conversation/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10105 2024-05-13 22:26:17.000000 owega-5.8.1/owega/conversation/conversation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1418 2024-05-10 10:34:51.000000 owega-5.8.1/owega/getLogger.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-17 02:21:38.000000 owega-5.8.1/owega/handlerBase.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6141 2024-05-10 14:44:53.000000 owega-5.8.1/owega/license.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    11780 2024-05-17 21:28:43.000000 owega-5.8.1/owega/owega.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     7504 2024-05-13 23:20:56.000000 owega-5.8.1/owega/utils.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 22:04:42.119935 owega-5.8.1/owega.egg-info/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    16793 2024-05-17 22:04:42.000000 owega-5.8.1/owega.egg-info/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1689 2024-05-17 22:04:42.000000 owega-5.8.1/owega.egg-info/SOURCES.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-05-17 22:04:42.000000 owega-5.8.1/owega.egg-info/dependency_links.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-05-17 22:04:42.000000 owega-5.8.1/owega.egg-info/entry_points.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      173 2024-05-17 22:04:42.000000 owega-5.8.1/owega.egg-info/requires.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-05-17 22:04:42.000000 owega-5.8.1/owega.egg-info/top_level.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-17 02:21:38.000000 owega-5.8.1/pyproject.toml
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-05-17 22:04:42.119935 owega-5.8.1/setup.cfg
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2179 2024-05-17 22:00:42.000000 owega-5.8.1/setup.py
```

### Comparing `owega-5.8.0/LICENSE` & `owega-5.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/PKG-INFO` & `owega-5.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.8.0
+Version: 5.8.1
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: DGPL-1.0
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -142,15 +142,15 @@
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.8.0 CHANGELOG:
+OWEGA v5.8.1 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -381,9 +381,10 @@
        (all other models return a cost of 0)
 5.7.4: Added pretty print if the rich module is installed.
 5.7.5: Fixed the bottom toolbar being cut short when terminal
        doesn't have enough columns.
        (also, added gpt-4o and mixtral-8x22b to default list)
 
 5.8.0: Added time-aware mode...
+5.8.1: Oops, I broke the build system again, my bad! :P
 
 ```
```

### Comparing `owega-5.8.0/README.md` & `owega-5.8.1/README.md`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_add_sysmem.py` & `owega-5.8.1/owega/OweHandlers/handle_add_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_commands.py` & `owega-5.8.1/owega/OweHandlers/handle_commands.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_context.py` & `owega-5.8.1/owega/OweHandlers/handle_context.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_del_sysmem.py` & `owega-5.8.1/owega/OweHandlers/handle_del_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_dinput.py` & `owega-5.8.1/owega/OweHandlers/handle_dinput.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_edit.py` & `owega-5.8.1/owega/OweHandlers/handle_edit.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_estimation.py` & `owega-5.8.1/owega/OweHandlers/handle_estimation.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_finput.py` & `owega-5.8.1/owega/OweHandlers/handle_finput.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_frequency.py` & `owega-5.8.1/owega/OweHandlers/handle_frequency.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_genconf.py` & `owega-5.8.1/owega/OweHandlers/handle_genconf.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_history.py` & `owega-5.8.1/owega/OweHandlers/handle_history.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_image.py` & `owega-5.8.1/owega/OweHandlers/handle_image.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_load.py` & `owega-5.8.1/owega/OweHandlers/handle_load.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_model.py` & `owega-5.8.1/owega/OweHandlers/handle_model.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_presence.py` & `owega-5.8.1/owega/OweHandlers/handle_presence.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_quit.py` & `owega-5.8.1/owega/OweHandlers/handle_quit.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_save.py` & `owega-5.8.1/owega/OweHandlers/handle_save.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_system.py` & `owega-5.8.1/owega/OweHandlers/handle_system.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_temperature.py` & `owega-5.8.1/owega/OweHandlers/handle_temperature.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_time.py` & `owega-5.8.1/owega/OweHandlers/handle_time.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_tokens.py` & `owega-5.8.1/owega/OweHandlers/handle_tokens.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_top_p.py` & `owega-5.8.1/owega/OweHandlers/handle_top_p.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handle_tts.py` & `owega-5.8.1/owega/OweHandlers/handle_tts.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OweHandlers/handlers.py` & `owega-5.8.1/owega/OweHandlers/handlers.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OwegaFun/__init__.py` & `owega-5.8.1/owega/OwegaFun/__init__.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OwegaFun/functions.py` & `owega-5.8.1/owega/OwegaFun/functions.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OwegaFun/longTermSouvenirs.py` & `owega-5.8.1/owega/OwegaFun/longTermSouvenirs.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OwegaFun/utility.py` & `owega-5.8.1/owega/OwegaFun/utility.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OwegaSession/main_bottom_toolbar.py` & `owega-5.8.1/owega/OwegaSession/main_bottom_toolbar.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/OwegaSession/promptsession.py` & `owega-5.8.1/owega/OwegaSession/promptsession.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/ask.py` & `owega-5.8.1/owega/ask.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/changelog/changelog.py` & `owega-5.8.1/owega/changelog/changelog.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,18 @@
         self.version = Version(0, 0, 0)
         self.initLogs()
         self.genLog()
 
     def initLogs(self):
         """Fill the changelog."""
         self.logs.append(
+            ChangelogEntry(5, 8, 1)
+            .addLine("Oops, I broke the build system again, my bad! :P")
+        )
+        self.logs.append(
             ChangelogEntry(5, 8, 0)
             .addLine("Added time-aware mode...")
         )
 
         self.logs.append(
             ChangelogEntry(5, 7, 5)
             .addLine("Fixed the bottom toolbar being cut short when terminal")
```

### Comparing `owega-5.8.0/owega/changelog/changelogEntry.py` & `owega-5.8.1/owega/changelog/changelogEntry.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/changelog/version.py` & `owega-5.8.1/owega/changelog/version.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/config/baseConf.py` & `owega-5.8.1/owega/config/baseConf.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/conversation/conversation.py` & `owega-5.8.1/owega/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/getLogger.py` & `owega-5.8.1/owega/getLogger.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/license.py` & `owega-5.8.1/owega/license.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/owega.py` & `owega-5.8.1/owega/owega.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega/utils.py` & `owega-5.8.1/owega/utils.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/owega.egg-info/PKG-INFO` & `owega-5.8.1/owega.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.8.0
+Version: 5.8.1
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: DGPL-1.0
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -142,15 +142,15 @@
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.8.0 CHANGELOG:
+OWEGA v5.8.1 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -381,9 +381,10 @@
        (all other models return a cost of 0)
 5.7.4: Added pretty print if the rich module is installed.
 5.7.5: Fixed the bottom toolbar being cut short when terminal
        doesn't have enough columns.
        (also, added gpt-4o and mixtral-8x22b to default list)
 
 5.8.0: Added time-aware mode...
+5.8.1: Oops, I broke the build system again, my bad! :P
 
 ```
```

### Comparing `owega-5.8.0/owega.egg-info/SOURCES.txt` & `owega-5.8.1/owega.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owega-5.8.0/setup.py` & `owega-5.8.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 # -*- coding: utf-8 -*-
 
 """Setup config for installing the package."""
 
 from setuptools import setup
 
 desc = open('README.md').read()
-desc += '\n\n'
-desc += "## CHANGELOG: "
-desc += '\n```\n'
-desc += open('CHANGELOG').read()
-desc += '\n```\n'
+try:
+    changelog = open('CHANGELOG').read()
+    desc += '\n\n'
+    desc += "## CHANGELOG: "
+    desc += '\n```\n'
+    desc += changelog
+    desc += '\n```\n'
+except FileNotFoundError:
+    pass
 
 requirements = [
     'openai>=1.1.1',
     'prompt_toolkit>=3.0',
     'requests>=2.0',
     'beautifulsoup4>=4.0',
     'lxml>=4.0',
```

