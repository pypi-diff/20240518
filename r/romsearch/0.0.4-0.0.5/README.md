# Comparing `tmp/romsearch-0.0.4.tar.gz` & `tmp/romsearch-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "romsearch-0.0.4.tar", last modified: Thu May  9 11:41:16 2024, max compression
+gzip compressed data, was "romsearch-0.0.5.tar", last modified: Fri May 17 22:56:01 2024, max compression
```

## Comparing `romsearch-0.0.4.tar` & `romsearch-0.0.5.tar`

### file list

```diff
@@ -1,93 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.980947 romsearch-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.968947 romsearch-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.972947 romsearch-0.0.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-09 11:41:13.000000 romsearch-0.0.4/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-09 11:41:13.000000 romsearch-0.0.4/.github/ISSUE_TEMPLATE/console_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-09 11:41:13.000000 romsearch-0.0.4/.github/ISSUE_TEMPLATE/feature_request.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.972947 romsearch-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-09 11:41:13.000000 romsearch-0.0.4/.github/workflows/build_test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-09 11:41:13.000000 romsearch-0.0.4/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-09 11:41:13.000000 romsearch-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-09 11:41:13.000000 romsearch-0.0.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-09 11:41:13.000000 romsearch-0.0.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 11:41:13.000000 romsearch-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-09 11:41:13.000000 romsearch-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    43755 2024-05-09 11:41:16.980947 romsearch-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-09 11:41:13.000000 romsearch-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.972947 romsearch-0.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/1g1r.rst
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.972947 romsearch-0.0.4/docs/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/configs/clonelists.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/configs/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/configs/dats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/configs/defaults.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/configs/platforms.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/configs/regex.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/configs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/known_issues.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.976947 romsearch-0.0.4/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/modules/datparser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/modules/dupeparser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/modules/gamefinder.rst
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/modules/romchooser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/modules/romdownloader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/modules/rommover.rst
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/modules/romparser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/modules/romsearch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/reference_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-09 11:41:13.000000 romsearch-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.976947 romsearch-0.0.4/romsearch/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.976947 romsearch-0.0.4/romsearch/configs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.976947 romsearch-0.0.4/romsearch/configs/clonelists/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/clonelists/retool.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.976947 romsearch-0.0.4/romsearch/configs/dats/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/dats/no-intro.yml
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/dats/redump.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/defaults.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.976947 romsearch-0.0.4/romsearch/configs/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/platforms/Nintendo - GameCube.yml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/platforms/Nintendo - Nintendo Entertainment System.yml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/platforms/Nintendo - Super Nintendo Entertainment System.yml
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/platforms/Sony - PlayStation 2.yml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/platforms/Sony - PlayStation Portable.yml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/platforms/Sony - PlayStation.yml
--rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/regex.yml
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/sample_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.976947 romsearch-0.0.4/romsearch/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/dev/parsing_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.980947 romsearch-0.0.4/romsearch/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/modules/datparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/modules/dupeparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/modules/gamefinder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/modules/romchooser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/modules/romdownloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/modules/rommover.py
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/modules/romparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/modules/romsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.980947 romsearch-0.0.4/romsearch/util/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/util/discord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/util/general.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/util/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/util/regex_matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.980947 romsearch-0.0.4/romsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43755 2024-05-09 11:41:16.000000 romsearch-0.0.4/romsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-09 11:41:16.000000 romsearch-0.0.4/romsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:41:16.000000 romsearch-0.0.4/romsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-09 11:41:16.000000 romsearch-0.0.4/romsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 11:41:16.000000 romsearch-0.0.4/romsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 11:41:16.980947 romsearch-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.878658 romsearch-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.858657 romsearch-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.862658 romsearch-0.0.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-17 22:55:57.000000 romsearch-0.0.5/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-17 22:55:57.000000 romsearch-0.0.5/.github/ISSUE_TEMPLATE/console_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-17 22:55:57.000000 romsearch-0.0.5/.github/ISSUE_TEMPLATE/feature_request.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.862658 romsearch-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-17 22:55:57.000000 romsearch-0.0.5/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-17 22:55:57.000000 romsearch-0.0.5/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-17 22:55:57.000000 romsearch-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-17 22:55:57.000000 romsearch-0.0.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-17 22:55:57.000000 romsearch-0.0.5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-17 22:55:57.000000 romsearch-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-17 22:55:57.000000 romsearch-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    43911 2024-05-17 22:56:01.878658 romsearch-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-17 22:55:57.000000 romsearch-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.866658 romsearch-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/1g1r.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.866658 romsearch-0.0.5/docs/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/configs/clonelists.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/configs/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/configs/dats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/configs/defaults.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/configs/platforms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/configs/regex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/configuration.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.866658 romsearch-0.0.5/docs/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/gui/config_includes_excludes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/gui/config_main.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/gui/config_modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/gui/config_platforms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/gui/config_regions_languages.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/gui/intro.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.866658 romsearch-0.0.5/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    24254 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/images/config_includes_excludes.png
+-rw-r--r--   0 runner    (1001) docker     (127)    71922 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/images/config_main.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24790 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/images/config_modules.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39895 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/images/config_platforms.png
+-rw-r--r--   0 runner    (1001) docker     (127)    73902 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/images/config_regions_languages.png
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/known_issues.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.870658 romsearch-0.0.5/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/modules/datparser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/modules/dupeparser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/modules/gamefinder.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/modules/romchooser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/modules/romdownloader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/modules/rommover.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/modules/romparser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/modules/romsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/reference_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-17 22:55:57.000000 romsearch-0.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.870658 romsearch-0.0.5/romsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.870658 romsearch-0.0.5/romsearch/configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.870658 romsearch-0.0.5/romsearch/configs/clonelists/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/clonelists/retool.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.870658 romsearch-0.0.5/romsearch/configs/dats/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/dats/no-intro.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/dats/redump.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/defaults.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.874658 romsearch-0.0.5/romsearch/configs/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/platforms/Nintendo - GameCube.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/platforms/Nintendo - Nintendo Entertainment System.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/platforms/Nintendo - Super Nintendo Entertainment System.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/platforms/Sony - PlayStation 2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/platforms/Sony - PlayStation Portable.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/platforms/Sony - PlayStation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/regex.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/sample_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.874658 romsearch-0.0.5/romsearch/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/dev/parsing_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.874658 romsearch-0.0.5/romsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/gui/gui_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27172 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/gui/gui_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/gui/gui_romsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/gui/gui_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/gui/layout_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/gui/layout_about.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    96327 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/gui/layout_romsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89017 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/gui/layout_romsearch.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.878658 romsearch-0.0.5/romsearch/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/modules/datparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/modules/dupeparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/modules/gamefinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16739 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/modules/romchooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/modules/romdownloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/modules/rommover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13987 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/modules/romparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14022 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/modules/romsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.878658 romsearch-0.0.5/romsearch/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/util/discord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/util/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/util/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/util/regex_matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.878658 romsearch-0.0.5/romsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43911 2024-05-17 22:56:01.000000 romsearch-0.0.5/romsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-17 22:56:01.000000 romsearch-0.0.5/romsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:56:01.000000 romsearch-0.0.5/romsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-17 22:56:01.000000 romsearch-0.0.5/romsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 22:56:01.000000 romsearch-0.0.5/romsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 22:56:01.878658 romsearch-0.0.5/setup.cfg
```

### Comparing `romsearch-0.0.4/.github/ISSUE_TEMPLATE/bug_report.yml` & `romsearch-0.0.5/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files 13% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 body:
   - type: dropdown
     id: version
     attributes:
       label: Installation
       description: Are you using pip or GitHub? Which GitHub tag?
       options:
+        - Windows executable
         - pip
-        - GitHub - main branch
-        - GitHub - dev branch
+        - GitHub
     validations:
       required: true
   - type: textarea
     id: description
     attributes:
       label: Describe the Bug
       description: A clear and concise description of the bug.
```

### Comparing `romsearch-0.0.4/.github/ISSUE_TEMPLATE/feature_request.yml` & `romsearch-0.0.5/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.4/.gitignore` & `romsearch-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.4/.readthedocs.yaml` & `romsearch-0.0.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.4/LICENSE` & `romsearch-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.4/PKG-INFO` & `romsearch-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romsearch
-Version: 0.0.4
+Version: 0.0.5
 Summary: One Stop ROM Shop
 Author: bbtufty
 Maintainer: bbtufty
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -690,18 +690,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: colorlog
 Requires-Dist: discordwebhook
 Requires-Dist: numpy
 Requires-Dist: packaging
 Requires-Dist: pathvalidate
+Requires-Dist: PySide6
 Requires-Dist: pyyaml
 Requires-Dist: xmltodict
 Provides-Extra: docs
 Requires-Dist: sphinx-automodapi; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 
 # ROMSearch
@@ -712,14 +714,16 @@
 [![Actions](https://img.shields.io/github/actions/workflow/status/bbtufty/romsearch/build_test.yaml?branch=main&style=flat-square)](https://github.com/bbtufty/romsearch/actions)
 [![License](https://img.shields.io/badge/license-GNUv3-blue.svg?label=License&style=flat-square)](LICENSE)
 
 ROMSearch is designed as a simple-to-inferface with tool that will allow you to pull ROM files from some remote (or
 local) location, figure out the best ROM, and move it cleanly to a folder that can imported into an emulator. ROMSearch
 is supposed to be a one-shot program to get you from files online to playing games (which is what we want, right?).
 
+ROMSearch also has a GUI! Currently only for Windows, but makes setting up configurations simple and clean.
+
 ROMSearch offers the ability to:
 
 * Sync from remote folder using rclone
 * Parse DAT files as well as filenames for ROM information
 * Remove dupes from ROM lists using DAT files as well as the excellent ``retool`` clonelists
 * Moving files to a structured location, including potentially additional files that may be needed
 * Discord integration so users can see the results of runs in a simple, clean way
```

### Comparing `romsearch-0.0.4/README.md` & `romsearch-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 [![Actions](https://img.shields.io/github/actions/workflow/status/bbtufty/romsearch/build_test.yaml?branch=main&style=flat-square)](https://github.com/bbtufty/romsearch/actions)
 [![License](https://img.shields.io/badge/license-GNUv3-blue.svg?label=License&style=flat-square)](LICENSE)
 
 ROMSearch is designed as a simple-to-inferface with tool that will allow you to pull ROM files from some remote (or
 local) location, figure out the best ROM, and move it cleanly to a folder that can imported into an emulator. ROMSearch
 is supposed to be a one-shot program to get you from files online to playing games (which is what we want, right?).
 
+ROMSearch also has a GUI! Currently only for Windows, but makes setting up configurations simple and clean.
+
 ROMSearch offers the ability to:
 
 * Sync from remote folder using rclone
 * Parse DAT files as well as filenames for ROM information
 * Remove dupes from ROM lists using DAT files as well as the excellent ``retool`` clonelists
 * Moving files to a structured location, including potentially additional files that may be needed
 * Discord integration so users can see the results of runs in a simple, clean way
```

### Comparing `romsearch-0.0.4/docs/1g1r.rst` & `romsearch-0.0.5/docs/1g1r.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.4/docs/Makefile` & `romsearch-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.4/docs/conf.py` & `romsearch-0.0.5/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'romsearch'
 copyright = '2024, bbtufty'
 author = 'bbtufty'
-release = '0.0.4'
+release = '0.0.5'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc',
               'sphinx.ext.coverage',
               'sphinx.ext.napoleon',
```

### Comparing `romsearch-0.0.4/docs/configs/config.rst` & `romsearch-0.0.5/docs/configs/config.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,82 @@
 ######
 config
 ######
 
 The ``config.yml`` file defines how ROMSearch will do the run. As such, it has quite a number of options.
 
+As a note on includes, this will match something from the start of the string. So "Game Title VII" would include
+"Game Title VII", "Game Title VIII", but not "Game Title Anthology - Game Title VII", for example.
+
 Syntax: ::
 
-    raw_dir: [raw_dir]                # Raw directory to download ROM files using ROMDownloader
-    rom_dir: [rom_dir]                # Final output directory for ROMs. Will automatically subdivide by platform
-    dat_dir: [dat_dir]                # Directory to place raw .dat files
-    parsed_dat_dir: [parsed_dat_dir]  # Directory to place parsed .dat files, as well as clonelists
-    dupe_dir: [dupe_dir]              # Directory to place dupe files
-
-    run_romdownloader: true           # OPTIONAL. Whether to run ROMDownloader. Defaults to true
-    run_datparser: true               # OPTIONAL. Whether to run DATParser. Defaults to true
-    run_dupeparser: true              # OPTIONAL. Whether to run DupeParsed. Defaults to true
-    run_romchooser: true              # OPTIONAL. Whether to run ROMChooser. Defaults to true
-    run_rommover: true                # OPTIONAL. Whether to run ROMMover. Defaults to true
+    dirs:
+      raw_dir: [raw_dir]                # Raw directory to download ROM files using ROMDownloader
+      rom_dir: [rom_dir]                # Final output directory for ROMs. Will automatically subdivide by platform
+      dat_dir: [dat_dir]                # Directory to place raw .dat files
+      parsed_dat_dir: [parsed_dat_dir]  # Directory to place parsed .dat files, as well as clonelists
+      dupe_dir: [dupe_dir]              # Directory to place dupe files
+      log_dir: [log_dir]                # Directory to place logs
+      cache_dir: [cache_dir]            # Directory to place cache files
 
-    platforms:                        # List of platforms to download ROMs for
+    platforms:                          # List of platforms to download ROMs for
       - [platform]
 
-    region_preferences:               # List of regions, in preference order
+    region_preferences:                 # List of regions, in preference order
       - [most_preferred_region]
       - [next_preferred_region]
 
-    language_preferences:             # List of languages, in preference order
+    language_preferences:               # List of languages, in preference order
       - [most_preferred_language]
       - [next_preferred_language]
 
-    include_games:                    # OPTIONAL. Use this to trim down the number of ROMs downloaded
+    include_games:                      # OPTIONAL. Use this to trim down the number of ROMs downloaded
       [platform]:
         - [game]
 
-    romsearch:                        # ROMSearch specific options
-      dry_run: false                  # OPTIONAL. Set to true to not make any changes to filesystem. Defaults to false
-
-    romdownloader:                    # ROMDownloader specific options
-      dry_run: false                  # OPTIONAL. Set to true to not make any changes to filesystem. Defaults to false
-      remote_name: 'rclone_remote'    # Rclone remote name
-      sync_all: false                 # OPTIONAL. If true, will download everything that rclone finds. Set to false to
-                                      #           use the include_games above
-
-    dupeparser:                       # DupeParser specific options
-      use_dat: true                   # OPTIONAL. Whether to use .dat files or not. Defaults to true
-      use_retool: true                # OPTIONAL. Whether to use retool clonelists or not. Defaults to true
-
-    gamefinder:                       # GameFinder specific options
-      filter_dupes: true              # OPTIONAL. Whether to filter dupes or not. Defaults to true
-
-    romparser:                        # ROMParser specific options
-      use_dat: true                   # OPTIONAL. Whether to parse properties from .dat files. Defaults to true
-      use_filename: true              # OPTIONAL. Whether to parse properties from filename. Defaults to true
-
-    romchooser:                       # ROMChooser specific options
-      dry_run: false                  # OPTIONAL. Set to true to not make any changes to filesystem. Defaults to false
-      use_best_version: true          # OPTIONAL. Whether to choose only what ROMChooser decides is the best version.
-                                                  Defaults to true
-      allow_multiple_regions: false   # OPTIONAL. If true, will allow files from multiple regions, else will choose the
-                                                  highest region in the list. Defaults to false
-      filter_regions: true            # OPTIONAL. Whether to filter by region or not. Defaults to true
-      filter_languages: true          # OPTIONAL. Whether to filter by language or not. Defaults to true
-      bool_filters: "all_but_games"   # OPTIONAL. Can filter out non-games by various dat categories. If you want to
-                                                  include e.g. just games and applications, set to
-                                                  ['games', 'applications']. Defaults to 'all_but_games', which will
-                                                  remove everything except games
+    romsearch:                          # ROMSearch specific options
+      method: 'filter_then_download'    # OPTIONAL. Method to use, option are 'filter_then_download', or
+                                        #           'download_then_filter'. Defaults to 'filter_then_download'
+      run_romdownloader: true           # OPTIONAL. Whether to run ROMDownloader. Defaults to true
+      run_datparser: true               # OPTIONAL. Whether to run DATParser. Defaults to true
+      run_dupeparser: true              # OPTIONAL. Whether to run DupeParsed. Defaults to true
+      run_romchooser: true              # OPTIONAL. Whether to run ROMChooser. Defaults to true
+      run_rommover: true                # OPTIONAL. Whether to run ROMMover. Defaults to true
+      dry_run: false                    # OPTIONAL. Set to true to not make any changes to filesystem. Defaults to false
+
+    romdownloader:                      # ROMDownloader specific options
+      dry_run: false                    # OPTIONAL. Set to true to not make any changes to filesystem. Defaults to false
+      remote_name: 'rclone_remote'      # Rclone remote name
+      sync_all: false                   # OPTIONAL. If true, will download everything that rclone finds. Set to false to
+                                        #           use the include_games above
+
+    dupeparser:                         # DupeParser specific options
+      use_dat: true                     # OPTIONAL. Whether to use .dat files or not. Defaults to true
+      use_retool: true                  # OPTIONAL. Whether to use retool clonelists or not. Defaults to true
+
+    gamefinder:                         # GameFinder specific options
+      filter_dupes: true                # OPTIONAL. Whether to filter dupes or not. Defaults to true
+
+    romparser:                          # ROMParser specific options
+      use_dat: true                     # OPTIONAL. Whether to parse properties from .dat files. Defaults to true
+      use_filename: true                # OPTIONAL. Whether to parse properties from filename. Defaults to true
+
+    romchooser:                         # ROMChooser specific options
+      dry_run: false                    # OPTIONAL. Set to true to not make any changes to filesystem. Defaults to false
+      use_best_version: true            # OPTIONAL. Whether to choose only what ROMChooser decides is the best version.
+                                        #           Defaults to true
+      allow_multiple_regions: false     # OPTIONAL. If true, will allow files from multiple regions, else will choose the
+                                        #           highest region in the list. Defaults to false
+      filter_regions: true              # OPTIONAL. Whether to filter by region or not. Defaults to true
+      filter_languages: true            # OPTIONAL. Whether to filter by language or not. Defaults to true
+      bool_filters: "all_but_games"     # OPTIONAL. Can filter out non-games by various dat categories. If you want to
+                                        #           include e.g. just games and applications, set to
+                                        #           ['games', 'applications']. Defaults to 'all_but_games', which will
+                                        #           remove everything except games
 
-    discord:                          # OPTIONAL. If defined, supply a webhook URL so that ROMSearch can post Discord
-      webhook_url: [webhook_url]      #           notifications
+    discord:                            # OPTIONAL. If defined, supply a webhook URL so that ROMSearch can post Discord
+      webhook_url: [webhook_url]        #           notifications
 
 Sample
 ======
 
 .. literalinclude:: ../../romsearch/configs/sample_config.yml
```

### Comparing `romsearch-0.0.4/docs/configs/dats.rst` & `romsearch-0.0.5/docs/configs/dats.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.4/docs/configs/platforms.rst` & `romsearch-0.0.5/docs/configs/platforms.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.4/docs/configs/regex.rst` & `romsearch-0.0.5/docs/configs/regex.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.4/docs/configuration.rst` & `romsearch-0.0.5/docs/configuration.rst`

 * *Files 15% similar despite different names*

```diff
@@ -20,22 +20,26 @@
 
 The config file is an easy way to let ROMSearch know where to look for various files. It also includes a
 number of switches that may be useful in different use cases.
 
 **ROMSearch works in such a way that by default it will grab what it thinks is the best ROM file. You can disable
 many of the ways it decides this if you want to grab multiple files**
 
-As a minimal example, if we wanted to grab the entire US Catalog of PlayStation games and post what you've added to a
-Discord channel, the config file would look something like this: ::
+We generally recommend setting this up through the GUI. For details on how to do that, see the
+:doc:`GUI pages <gui/intro>`.
 
-    raw_dir: 'F:\Emulation\raw'
-    rom_dir: 'F:\Emulation\ROMs'
-    dat_dir: 'F:\Emulation\data\dats'
-    parsed_dat_dir: 'F:\Emulation\data\dats_parsed'
-    dupe_dir: 'F:\Emulation\data\dupes'
+If you want to manually edit these files, here is an example. If we wanted to grab the entire US Catalog of PlayStation
+games and post what you've added to a Discord channel, the config file would look something like this: ::
+
+    dirs:
+      raw_dir: 'F:\Emulation\raw'
+      rom_dir: 'F:\Emulation\ROMs'
+      dat_dir: 'F:\Emulation\data\dats'
+      parsed_dat_dir: 'F:\Emulation\data\dats_parsed'
+      dupe_dir: 'F:\Emulation\data\dupes'
 
     platforms:
       - Sony - PlayStation
 
     region_preferences:
       - USA
```

### Comparing `romsearch-0.0.4/docs/index.rst` & `romsearch-0.0.5/docs/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 .. toctree::
    :titlesonly:
    :maxdepth: 2
    :caption: Documentation
 
    installation
+   gui/intro
    configuration
    1g1r
    modules
    configs
    utils
    known_issues
    changelog
```

### Comparing `romsearch-0.0.4/docs/intro.rst` & `romsearch-0.0.5/docs/intro.rst`

 * *Files 15% similar despite different names*

```diff
@@ -21,15 +21,21 @@
 * Sync from remote folder using rclone
 * Parse DAT files as well as filenames for ROM information
 * Remove dupes from ROM lists using DAT files as well as the excellent ``retool`` clonelists
 * Moving files to a structured location, including potentially additional files that may be needed
 * Discord integration so users can see the results of runs in a simple, clean way
 
 To get started, see the :doc:`installation <installation>` and :doc:`configuration <configuration>` pages. For the
-philosophy behind how ROMSearch chooses a ROM, see :doc:`1G1R <1g1r>`.
+philosophy behind how ROMSearch chooses a ROM, see :doc:`1G1R <1g1r>`. Romsearch has a UI option which we recommend
+for most users. For this, see :doc:`the GUI pages <gui/intro>`.
+
+ROMSearch offers two modes: the default is "filter, then download" which will use the .dat file to find the best ROMs
+and only download those. For data hoarders, we also offer a "download, then filter" option, which will download
+everything and then filter from the downloaded files. For more details, see the
+:doc:`ROMSearch module docs <modules/romsearch>`.
 
 Currently, ROMSearch is in early development, and so many features may be added over time. At the moment, ROMSearch
 has the capability for:
 
 * Nintendo - GameCube
 * Nintendo - Nintendo Entertainment System
 * Nintendo - Super Nintendo Entertainment System
```

### Comparing `romsearch-0.0.4/docs/make.bat` & `romsearch-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.4/docs/modules/datparser.rst` & `romsearch-0.0.5/docs/modules/datparser.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.4/docs/modules/dupeparser.rst` & `romsearch-0.0.5/docs/modules/dupeparser.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.4/docs/modules/romdownloader.rst` & `romsearch-0.0.5/docs/modules/romdownloader.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.4/pyproject.toml` & `romsearch-0.0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "romsearch"
-version = "0.0.4"
+version = "0.0.5"
 description = "One Stop ROM Shop"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 
 authors = [
     {name = "bbtufty"},
@@ -29,18 +29,20 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
 ]
 
 dependencies = [
+    "colorlog",
     "discordwebhook",
     "numpy",
     "packaging",
     "pathvalidate",
+    "PySide6",
     "pyyaml",
     "xmltodict",
 ]
 
 [project.optional-dependencies]
 docs = [
     "sphinx-automodapi",
```

### Comparing `romsearch-0.0.4/romsearch/__init__.py` & `romsearch-0.0.5/romsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.4/romsearch/configs/clonelists/retool.yml` & `romsearch-0.0.5/romsearch/configs/clonelists/retool.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.4/romsearch/configs/defaults.yml` & `romsearch-0.0.5/romsearch/configs/defaults.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.4/romsearch/configs/regex.yml` & `romsearch-0.0.5/romsearch/configs/regex.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.4/romsearch/configs/sample_config.yml` & `romsearch-0.0.5/romsearch/configs/sample_config.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-raw_dir: 'F:\Emulation\raw'
-rom_dir: 'F:\Emulation\ROMs'
-dat_dir: 'F:\Emulation\data\dats'
-parsed_dat_dir: 'F:\Emulation\data\dats_parsed'
-dupe_dir: 'F:\Emulation\data\dupes'
-
-run_romdownloader: true
-run_datparser: true
-run_dupeparser: true
-run_romchooser: true
-run_rommover: false
+dirs:
+  raw_dir: 'F:\Emulation\raw'
+  rom_dir: 'F:\Emulation\ROMs'
+  dat_dir: 'F:\Emulation\data\dats'
+  parsed_dat_dir: 'F:\Emulation\data\dats_parsed'
+  dupe_dir: 'F:\Emulation\data\dupes'
+  log_dir: 'F:\Emulation\data\logs'
+  cache_dir: 'F:\Emulation\data\cache'
 
 platforms:
   - Nintendo - Super Nintendo Entertainment System
 
 region_preferences:
   - USA
 
@@ -20,14 +17,20 @@
   - English
 
 include_games:
   SNES:
     - "Chrono Trigger"
 
 romsearch:
+  method: "filter_then_download"
+  run_romdownloader: true
+  run_datparser: true
+  run_dupeparser: true
+  run_romchooser: true
+  run_rommover: false
   dry_run: false
 
 romdownloader:
   dry_run: false
   remote_name: 'rclone_remote'
   sync_all: false
```

### Comparing `romsearch-0.0.4/romsearch/dev/parsing_tools.py` & `romsearch-0.0.5/romsearch/dev/parsing_tools.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.4/romsearch/modules/dupeparser.py` & `romsearch-0.0.5/romsearch/modules/dupeparser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 
 import numpy as np
 import requests
 
 import romsearch
 from ..util import (setup_logger,
-                    create_bar,
                     load_yml,
                     get_parent_name,
                     get_short_name,
                     load_json,
                     save_json,
                     )
 
@@ -18,89 +17,108 @@
     "cloneofid",
 ]
 
 
 class DupeParser:
 
     def __init__(self,
-                 config_file,
-                 platform,
+                 platform=None,
+                 config_file=None,
+                 config=None,
+                 default_config=None,
+                 regex_config=None,
+                 logger=None,
                  ):
         """Tool for figuring out a list of dupes
 
+        Args:
+            platform (str, optional): Platform name. Defaults to None, which will throw a ValueError.
+            config_file (str, optional): Path to config file. Defaults to None
+            config (dict, optional): Configuration dictionary. Defaults to None
+            default_config (dict, optional): Default configuration dictionary. Defaults to None
+            regex_config (dict, optional): Configuration dictionary for regex search. Defaults to None
+            logger (logging.Logger, optional): Logger instance. Defaults to None
+
         TODO:
             - At some point, we might want to consider adding in the retool supersets
         """
 
-        logger_add_dir = str(os.path.join(platform))
+        if platform is None:
+            raise ValueError("platform must be specified")
+        self.platform = platform
 
-        self.logger = setup_logger(log_level="info",
-                                   script_name=f"DupeParser",
-                                   additional_dir=logger_add_dir,
-                                   )
+        if config_file is None and config is None:
+            raise ValueError("config_file or config must be specified")
 
-        config = load_yml(config_file)
+        if config is None:
+            config = load_yml(config_file)
+        self.config = config
+
+        if logger is None:
+            log_dir = self.config.get("dirs", {}).get("log_dir", os.path.join(os.getcwd(), "logs"))
+            logger = setup_logger(log_level="info",
+                                  script_name=f"DupeParser",
+                                  log_dir=log_dir,
+                                  additional_dir=platform,
+                                  )
+        self.logger = logger
 
-        self.use_dat = config.get("dupeparser", {}).get("use_dat", True)
-        self.use_retool = config.get("dupeparser", {}).get('use_retool', True)
+        self.use_dat = self.config.get("dupeparser", {}).get("use_dat", True)
+        self.use_retool = self.config.get("dupeparser", {}).get('use_retool', True)
 
-        self.parsed_dat_dir = config.get("parsed_dat_dir", None)
+        self.parsed_dat_dir = self.config.get("dirs", {}).get("parsed_dat_dir", None)
         if self.use_dat and self.parsed_dat_dir is None:
             raise ValueError("Must specify parsed_dat_dir if using dat files")
 
-        self.dupe_dir = config.get("dupe_dir", None)
+        self.dupe_dir = self.config.get("dirs", {}).get("dupe_dir", None)
         if self.dupe_dir is None:
             raise ValueError("dupe_dir should be specified in config file")
 
-        self.platform = platform
-
         # Pull in platform config that we need
         mod_dir = os.path.dirname(romsearch.__file__)
         retool_config_file = os.path.join(mod_dir, "configs", "clonelists", f"retool.yml")
         retool_config = load_yml(retool_config_file)
 
         self.retool_url = retool_config.get("url", None)
         self.retool_platform_file = retool_config.get(platform, None)
 
-        default_file = os.path.join(mod_dir, "configs", "defaults.yml")
-        self.default_config = load_yml(default_file)
-
-        regex_file = os.path.join(mod_dir, "configs", "regex.yml")
-        self.regex_config = load_yml(regex_file)
+        if default_config is None:
+            default_file = os.path.join(mod_dir, "configs", "defaults.yml")
+            default_config = load_yml(default_file)
+        self.default_config = default_config
+
+        if regex_config is None:
+            regex_file = os.path.join(mod_dir, "configs", "regex.yml")
+            regex_config = load_yml(regex_file)
+        self.regex_config = regex_config
 
     def run(self):
         """Run the dupe parser"""
 
         if (self.retool_platform_file is None or self.retool_url is None) and self.use_retool:
             self.logger.warning("retool config for the platform needs to be present if using retool")
             return False
 
-        self.logger.info(create_bar(f"START DupeParser"))
-
         dupe_dict = self.get_dupe_dict()
 
         # Save out the dupe dict
         out_file = os.path.join(self.dupe_dir, f"{self.platform} (dupes).json")
         save_json(dupe_dict, out_file)
 
-        self.logger.info(create_bar(f"FINISH DupeParser"))
-
         return True
 
     def get_dupe_dict(self):
         """Loop through potentially both the dat files and the retool config file to get out dupes"""
 
         dupe_dict = {}
 
         # Prefer retool dupes first
         if self.use_retool:
-            self.logger.info("Gettings dupes from retool file")
             dupe_dict = self.get_retool_dupes(dupe_dict)
         if self.use_dat:
-            self.logger.info("Gettings dupes from dat file")
             dupe_dict = self.get_dat_dupes(dupe_dict)
 
         dupe_dict = dict(sorted(dupe_dict.items()))
 
         return dupe_dict
 
     def get_dat_dupes(self, dupe_dict=None):
@@ -184,19 +202,14 @@
             group_titles = [get_short_name(f["searchTerm"],
                                            default_config=self.default_config,
                                            regex_config=self.regex_config,
                                            )
                             for f in retool_dupe["titles"]]
             priorities = [f.get("priority", 1) for f in retool_dupe["titles"]]
 
-            # Parse down to the game name here
-            # if "(" in group:
-            #     group_parsed = get_game_name(group)
-            # else:
-            #     group_parsed = copy.deepcopy(group)
             group_parsed = get_short_name(group,
                                           default_config=self.default_config,
                                           regex_config=self.regex_config,
                                           )
 
             found_parent_name = get_parent_name(game_name=group_parsed,
                                                 dupe_dict=dupe_dict,
```

### Comparing `romsearch-0.0.4/romsearch/modules/gamefinder.py` & `romsearch-0.0.5/romsearch/modules/gamefinder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import copy
 import os
 import re
 
 import numpy as np
 
 import romsearch
-from ..util import setup_logger, load_yml, get_parent_name, get_short_name, create_bar, load_json
+from ..util import (setup_logger,
+                    load_yml,
+                    get_parent_name,
+                    get_short_name,
+                    load_json
+                    )
 
 
 def get_all_games(files,
                   default_config=None,
                   regex_config=None,
                   ):
     """Get all unique game names from a list of game files."""
@@ -40,92 +45,98 @@
     # Otherwise, just return 1
     return 1
 
 
 class GameFinder:
 
     def __init__(self,
-                 config_file,
                  platform,
+                 config_file=None,
+                 config=None,
+                 default_config=None,
+                 regex_config=None,
+                 logger=None,
                  ):
         """Tool to find games within a list of files
 
         Will parse through files to get a unique list of games, then pull
         out potential aliases and optionally remove things from user excluded list
+        
+        Args:
+            platform (str): Platform name
+            config_file (str, optional): Path to config file. Defaults to None.
+            config (dict, optional): Configuration dictionary. Defaults to None.
+            default_config (dict, optional): Default configuration dictionary. Defaults to None.
+            regex_config (dict, optional): Dictionary of regex config. Defaults to None.
+            logger (logging.Logger, optional): Logger instance. Defaults to None.
         """
 
-        self.logger = setup_logger(log_level="info",
-                                   script_name=f"GameFinder",
-                                   additional_dir=platform,
-                                   )
-
         if platform is None:
             raise ValueError("platform must be specified")
         self.platform = platform
 
-        config = load_yml(config_file)
+        if config_file is None and config is None:
+            raise ValueError("config_file or config must be specified")
+
+        if config is None:
+            config = load_yml(config_file)
+        self.config = config
+
+        if logger is None:
+            log_dir = self.config.get("dirs", {}).get("log_dir", os.path.join(os.getcwd(), "logs"))
+            logger = setup_logger(log_level="info",
+                                  script_name=f"GameFinder",
+                                  log_dir=log_dir,
+                                  additional_dir=platform,
+                                  )
+        self.logger = logger
 
         # Pull in specifics to include/exclude
-        self.include_games = config.get("include_games", None)
-        self.exclude_games = config.get("exclude_games", None)
+        self.include_games = self.config.get("include_games", None)
+        self.exclude_games = self.config.get("exclude_games", None)
 
         # Pull in defaults for finding short game names
         mod_dir = os.path.dirname(romsearch.__file__)
-        default_file = os.path.join(mod_dir, "configs", "defaults.yml")
-        self.default_config = load_yml(default_file)
 
-        regex_file = os.path.join(mod_dir, "configs", "regex.yml")
-        self.regex_config = load_yml(regex_file)
+        if default_config is None:
+            default_file = os.path.join(mod_dir, "configs", "defaults.yml")
+            default_config = load_yml(default_file)
+        self.default_config = default_config
+
+        if regex_config is None:
+            regex_file = os.path.join(mod_dir, "configs", "regex.yml")
+            regex_config = load_yml(regex_file)
+        self.regex_config = regex_config
 
         # Info for dupes
-        self.dupe_dir = config.get("dupe_dir", None)
+        self.dupe_dir = config.get("dirs", {}).get("dupe_dir", None)
         self.filter_dupes = config.get("gamefinder", {}).get("filter_dupes", True)
 
     def run(self,
             files,
             ):
 
-        self.logger.info(create_bar(f"START GameFinder"))
-
         games_dict = self.get_game_dict(files)
         games_dict = dict(sorted(games_dict.items()))
 
-        self.logger.info(f"Found {len(games_dict)} games:")
+        self.logger.debug(f"Found {len(games_dict)} games:")
         for g in games_dict:
-            self.logger.info(f"{g}: {games_dict[g]}")
+            self.logger.debug(f"{g}: {games_dict[g]}")
 
         return games_dict
 
     def get_game_dict(self,
                       files,
                       ):
 
         games = get_all_games(files,
                               default_config=self.default_config,
                               regex_config=self.regex_config,
                               )
 
-        # Remove any excluded files
-        if self.exclude_games is not None:
-            games_to_remove = self.get_game_matches(games,
-                                                    self.exclude_games,
-                                                    )
-
-            if games_to_remove is not None:
-                for i in sorted(games_to_remove, reverse=True):
-                    games.pop(i)
-
-        # Include only included files
-        if self.include_games is not None:
-            games_to_include = self.get_game_matches(games,
-                                                     self.include_games,
-                                                     )
-            if games_to_include is not None:
-                games = np.asarray(games)[games_to_include]
-
         # We need to trim down dupes here. Otherwise, the
         #  dict is just the list we already have
         game_dict = None
         if self.filter_dupes:
             game_dict = self.get_filter_dupes(games)
 
         # If the dupe filtering has failed, then just assume everything is unique
@@ -133,46 +144,96 @@
 
             game_dict = {}
 
             for game in games:
                 game_dict[game] = {"priority": 1,
                                    }
 
+        # Remove any excluded files
+        if self.exclude_games is not None:
+            games_to_remove = self.get_game_matches(game_dict,
+                                                    self.exclude_games,
+                                                    )
+            if games_to_remove is not None:
+                for g in games_to_remove:
+                    del game_dict[g]
+
+        # Include only included files
+        if self.include_games is not None:
+
+            games_to_include = self.get_game_matches(game_dict,
+                                                     self.include_games,
+                                                     )
+            if games_to_include is not None:
+
+                filtered_game_dict = {}
+                for g in games_to_include:
+                    filtered_game_dict[g] = game_dict[g]
+
+                game_dict = copy.deepcopy(filtered_game_dict)
+
         return game_dict
 
-    def get_game_matches(self, files, games_to_match):
-        """Get files that match an input list (games_to_match)"""
+    def get_game_matches(self,
+                         game_dict,
+                         games_to_match,
+                         ):
+        """Get files that match an input dictionary (so as to properly handle dupes
+
+        Args:
+            - game_dict (dict): Dictionary of games to match against
+            - games_to_match (list): List of values to match against
+        """
         games_matched = []
 
         if isinstance(games_to_match, dict):
             games_to_match = games_to_match.get(self.platform, None)
         else:
             games_to_match = copy.deepcopy(games_to_match)
 
         if games_to_match is None:
             return None
 
         games_matched.extend(games_to_match)
 
-        idx = []
-        for i, f in enumerate(files):
+        game_dict_keys = []
+        for g in game_dict:
             found_f = False
-            # Search within each item since the matches might not be exact
+
             for game_matched in games_matched:
 
                 if found_f:
                     continue
 
-                re_find = re.findall(f"{game_matched}*", f)
+                # Look in the group name
+                re_find = re.findall(f"^({re.escape(game_matched)}).*", g)
 
                 if len(re_find) > 0:
-                    idx.append(i)
+                    game_dict_keys.append(g)
                     found_f = True
 
-        return idx
+                # If not found, look in the dupe names
+                if not found_f:
+                    for g_d in game_dict[g]:
+
+                        if found_f:
+                            continue
+
+                        re_find = re.findall(f"^({re.escape(game_matched)}).*", g_d)
+
+                        if len(re_find) > 0:
+                            game_dict_keys.append(g)
+                            found_f = True
+
+        game_dict_keys = np.unique(game_dict_keys)
+
+        if len(game_dict_keys) == 0:
+            game_dict_keys = None
+
+        return game_dict_keys
 
     def get_filter_dupes(self, games):
         """Parse down a list of files based on an input dupe list"""
 
         if self.dupe_dir is None:
             raise ValueError("dupe_dir must be specified if filtering dupes")
```

### Comparing `romsearch-0.0.4/romsearch/modules/romchooser.py` & `romsearch-0.0.5/romsearch/modules/romchooser.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 
 import numpy as np
 import packaging.version
 from packaging import version
 
 import romsearch
 from ..util import (setup_logger,
-                    create_bar,
                     load_yml,
                     )
 
-BOOL_FILTERS = [
+DAT_FILTERS = [
     "add-ons",
     "applications",
     "audio",
     "bad_dumps",
     "console",
     "bonus_discs",
     "coverdiscs",
@@ -150,14 +149,15 @@
                     keys_to_pop.append(f)
 
             for key in keys_to_pop:
                 rom_dict.pop(key)
 
     return rom_dict
 
+
 def remove_unwanted_roms(rom_dict, key_to_check, check_type="include"):
     """Remove unwanted ROMs from the dict
 
     If we have multiple versions lying around that may be preferred or demoted for some reason, parse them
     out here. Do this per region combo
     """
 
@@ -291,98 +291,117 @@
 
     return rom_dict
 
 
 class ROMChooser:
 
     def __init__(self,
-                 config_file,
                  platform,
-                 game
+                 game,
+                 config_file=None,
+                 config=None,
+                 default_config=None,
+                 regex_config=None,
+                 logger=None,
                  ):
         """ROM choose tool
 
         This works per-game, per-platform, so must be specified here
+
+        Args:
+            platform (str): Platform name
+            game (str): Game name
+            config_file (str, optional): Path to config file. Defaults to None.
+            config (dict, optional): Configuration dictionary. Defaults to None.
+            default_config (dict, optional): Default configuration dictionary. Defaults to None.
+            regex_config (dict, optional): Configuration dictionary. Defaults to None.
+            logger (logging.Logger, optional): Logger instance. Defaults to None.
         """
 
         if platform is None:
             raise ValueError("platform must be specified")
         self.platform = platform
 
-        logger_add_dir = str(os.path.join(platform, game))
-
-        self.logger = setup_logger(log_level="info",
-                                   script_name=f"ROMChooser",
-                                   additional_dir=logger_add_dir,
-                                   )
+        if config_file is None and config is None:
+            raise ValueError("config_file or config must be specified")
 
-        config = load_yml(config_file)
+        if config is None:
+            config = load_yml(config_file)
+        self.config = config
+
+        if logger is None:
+            log_dir = self.config.get("dirs", {}).get("log_dir", os.path.join(os.getcwd(), "logs"))
+            logger_add_dir = str(os.path.join(platform, game))
+            logger = setup_logger(log_level="info",
+                                  script_name=f"ROMChooser",
+                                  log_dir=log_dir,
+                                  additional_dir=logger_add_dir,
+                                  )
+        self.logger = logger
 
         mod_dir = os.path.dirname(romsearch.__file__)
 
-        default_config_file = os.path.join(mod_dir, "configs", "defaults.yml")
-        self.default_config = load_yml(default_config_file)
-
-        platform_config_file = os.path.join(mod_dir, "configs", "platforms", f"{platform}.yml")
-        self.platform_config = load_yml(platform_config_file)
+        if default_config is None:
+            default_file = os.path.join(mod_dir, "configs", "defaults.yml")
+            default_config = load_yml(default_file)
+        self.default_config = default_config
+
+        if regex_config is None:
+            regex_file = os.path.join(mod_dir, "configs", "regex.yml")
+            regex_config = load_yml(regex_file)
+        self.regex_config = regex_config
 
         # Region preference (usually set USA for retroachievements, can also be a list to fall back to)
-        region_preferences = config.get("region_preferences", self.default_config["default_region"])
+        region_preferences = self.config.get("region_preferences", self.default_config["default_region"])
         if isinstance(region_preferences, str):
             region_preferences = [region_preferences]
 
         for region_pref in region_preferences:
             if region_pref not in self.default_config["regions"]:
                 raise ValueError(f"Regions should be any of {self.default_config['regions']}, not {region_pref}")
 
         self.region_preferences = region_preferences
 
         # Language preference (usually set En, can also be a list to fall back to)
-        language_preferences = config.get("language_preferences", self.default_config["default_language"])
+        language_preferences = self.config.get("language_preferences", self.default_config["default_language"])
         if isinstance(language_preferences, str):
             language_preferences = [language_preferences]
 
         for language_pref in language_preferences:
             if language_pref not in self.default_config["languages"]:
                 raise ValueError(f"Regions should be any of {self.default_config['languages']}, not {language_pref}")
 
         self.language_preferences = language_preferences
 
         # Various filters. First are the boolean ones
-        bool_filters = config.get("romchooser", {}).get("bool_filters", "all_but_games")
-        if "all" in bool_filters:
-            all_bool_filters = copy.deepcopy(BOOL_FILTERS)
-            if "all_but" in bool_filters:
-                filter_to_remove = bool_filters.split("all_but_")[-1]
-                all_bool_filters.remove(filter_to_remove)
-            bool_filters = copy.deepcopy(all_bool_filters)
+        dat_filters = self.config.get("romchooser", {}).get("dat_filters", "all_but_games")
+        if "all" in dat_filters:
+            all_dat_filters = copy.deepcopy(DAT_FILTERS)
+            if "all_but" in dat_filters:
+                filter_to_remove = dat_filters.split("all_but_")[-1]
+                all_dat_filters.remove(filter_to_remove)
+            dat_filters = copy.deepcopy(all_dat_filters)
+
+        if isinstance(dat_filters, str):
+            dat_filters = [dat_filters]
+        self.dat_filters = dat_filters
+
+        self.filter_regions = self.config.get("romchooser", {}).get("filter_regions", True)
+        self.filter_languages = self.config.get("romchooser", {}).get("filter_languages", True)
+        self.allow_multiple_regions = self.config.get("romchooser", {}).get("allow_multiple_regions", False)
+        self.use_best_version = self.config.get("romchooser", {}).get("use_best_version", True)
 
-        if isinstance(bool_filters, str):
-            all_bool_filters = [bool_filters]
-        else:
-            all_bool_filters = bool_filters
-        self.bool_filters = all_bool_filters
-
-        self.filter_regions = config.get("romchooser", {}).get("filter_regions", True)
-        self.filter_languages = config.get("romchooser", {}).get("filter_languages", True)
-        self.allow_multiple_regions = config.get("romchooser", {}).get("allow_multiple_regions", False)
-        self.use_best_version = config.get("romchooser", {}).get("use_best_version", True)
-
-        self.dry_run = config.get("romchooser", {}).get("dry_run", False)
+        self.dry_run = self.config.get("romchooser", {}).get("dry_run", False)
 
     def run(self,
             rom_dict):
         """Run the ROM chooser"""
 
-        self.logger.info(create_bar(f"START ROMChooser"))
-
         rom_dict = self.run_chooser(rom_dict)
 
-        self.logger.info(create_bar(f"FINISH ROMChooser"))
-
         return rom_dict
 
     def run_chooser(self,
                     rom_dict):
         """Make a ROM choice based on various factors
 
         This chooser works in this order:
@@ -395,17 +414,17 @@
         - Get some "best version", via:
             - Revision number
             - Version number
             - Some kind of special name to indicate an improved version
         - Finally, if we only allow one region, parse down to a single region (first in the list)
         """
 
-        for f in self.bool_filters:
+        for f in self.dat_filters:
             self.logger.debug(f"Filtering {f}")
-            if f in BOOL_FILTERS:
+            if f in DAT_FILTERS:
                 rom_dict = remove_rom_dict_entries(rom_dict,
                                                    f,
                                                    remove_type="bool",
                                                    bool_remove=True,
                                                    )
             else:
                 raise ValueError(f"Unknown filter type {f}")
```

### Comparing `romsearch-0.0.4/romsearch/modules/romdownloader.py` & `romsearch-0.0.5/romsearch/modules/romdownloader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 import copy
 import glob
 import os
 import subprocess
 
 import romsearch
 from ..util import (setup_logger,
-                    create_bar,
                     load_yml,
                     get_file_pattern,
                     discord_push,
-split,
+                    split,
                     )
 
 
 def add_rclone_filter(pattern=None,
-                      # bracketed_pattern=None,
                       filter_type="include",
+                      include_wildcard=True,
                       ):
     if filter_type == "include":
         filter_str = "+"
     elif filter_type == "exclude":
         filter_str = "-"
     else:
         raise ValueError("filter_type should be one of include or exclude")
 
     # rclone wants double curly braces which we need to escape in python strings (yum)
     filter_pattern = ""
 
-    # # Add in non-bracketed stuff (i.e. game names) at the start
-    # if non_bracketed_pattern is not None:
-    #     filter_pattern += f"{{{{{non_bracketed_pattern}}}}}"
-    #
-    # filter_pattern += "*"
-
     if pattern is not None:
-        filter_pattern += f"{{{{{pattern}}}}}*"
+        filter_pattern += f"{{{{{pattern}}}}}"
+
+    if include_wildcard:
+        filter_pattern += "*"
 
     cmd = f' --filter "{filter_str} {filter_pattern}"'
 
     return cmd
 
+
 def get_tidy_files(glob_pattern):
     """Get a tidy list of files from a glob pattern.
 
     This just strips off the leading directories to just get a filename
 
     Args:
         glob_pattern (str): glob pattern to match
@@ -54,93 +51,133 @@
 
     return files
 
 
 class ROMDownloader:
 
     def __init__(self,
-                 config_file,
                  platform=None,
+                 config_file=None,
+                 config=None,
+                 platform_config=None,
+                 logger=None,
+                 override_includes=None,
+                 override_excludes=None,
+                 include_filter_wildcard=True,
                  ):
         """Downloader tool via rclone
 
         This works per-platform, so must be specified here
+
+        Args:
+            platform (str, optional): Platform name. Defaults to None, which will throw a ValueError
+            config (str, optional): Configuration file. Defaults to None
+            config (dict, optional): Configuration dictionary. Defaults to None
+            platform_config (dict, optional): Platform configuration dictionary. Defaults to None
+            logger (logging.Logger, optional): Logger instance. Defaults to None
+            override_includes (list, optional): If set, will override the config includes with custom
+                ones. Defaults to None.
+            override_excludes (list, optional): If set, will override the config excludes with custom
+                ones. Defaults to None.
+            include_filter_wildcard (bool, optional): If set, will include wildcards in rclone filters. Defaults to
+                True.
         """
 
         if platform is None:
             raise ValueError("platform must be specified")
         self.platform = platform
 
-        self.logger = setup_logger(log_level="info",
-                                   script_name=f"ROMDownloader",
-                                   additional_dir=platform,
-                                   )
+        if config_file is None and config is None:
+            raise ValueError("config_file or config must be specified")
 
-        config = load_yml(config_file)
+        if config is None:
+            config = load_yml(config_file)
+        self.config = config
+
+        if logger is None:
+            log_dir = self.config.get("dirs", {}).get("log_dir", os.path.join(os.getcwd(), "logs"))
+            logger = setup_logger(log_level="info",
+                                  script_name=f"ROMDownloader",
+                                  log_dir=log_dir,
+                                  additional_dir=platform,
+                                  )
+        self.logger = logger
 
-        out_dir = config.get("raw_dir", None)
+        out_dir = self.config.get("dirs", {}).get("raw_dir", None)
         if out_dir is None:
             raise ValueError("raw_dir needs to be defined in config")
         self.out_dir = os.path.join(out_dir, platform)
 
         # Get any specific includes/excludes
-        include_games = config.get("include_games", None)
+        include_games = self.config.get("include_games", None)
         if isinstance(include_games, dict):
             include_games = include_games.get(platform, None)
         else:
             include_games = copy.deepcopy(include_games)
+
+        if override_includes is not None:
+            include_games = copy.deepcopy(override_includes)
+
         self.include_games = include_games
 
-        exclude_games = config.get("exclude_games", None)
+        exclude_games = self.config.get("exclude_games", None)
         if isinstance(exclude_games, dict):
             exclude_games = exclude_games.get(platform, None)
         else:
             exclude_games = copy.deepcopy(exclude_games)
+
+        if override_excludes is not None:
+            exclude_games = copy.deepcopy(override_excludes)
+
         self.exclude_games = exclude_games
 
-        remote_name = config.get("romdownloader", {}).get("remote_name", None)
+        remote_name = self.config.get("romdownloader", {}).get("remote_name", None)
         if remote_name is None:
             raise ValueError("remote_name must be specified in config")
         self.remote_name = remote_name
 
-        sync_all = config.get("romdownloader", {}).get("sync_all", True)
+        sync_all = self.config.get("romdownloader", {}).get("sync_all", True)
+
+        # If we have includes or excludes, force sync all False
+        if self.include_games is not None or self.exclude_games is not None:
+            sync_all = False
+
         self.sync_all = sync_all
 
+        self.include_filter_wildcard = include_filter_wildcard
+
         # Read in the specific platform configuration
         mod_dir = os.path.dirname(romsearch.__file__)
 
-        platform_config_file = os.path.join(mod_dir, "configs", "platforms", f"{platform}.yml")
-        platform_config = load_yml(platform_config_file)
+        if platform_config is None:
+            platform_config_file = os.path.join(mod_dir, "configs", "platforms", f"{platform}.yml")
+            platform_config = load_yml(platform_config_file)
+        self.platform_config = platform_config
 
-        ftp_dir = platform_config.get("ftp_dir", None)
+        ftp_dir = self.platform_config.get("ftp_dir", None)
         if ftp_dir is None:
             raise ValueError(f"ftp_dir should be defined in the platform config file!")
         self.ftp_dir = ftp_dir
 
-        self.platform_config = platform_config
-
-        self.discord_url = config.get("discord", {}).get("webhook_url", None)
-        self.dry_run = config.get("romdownloader", {}).get("dry_run", False)
+        self.discord_url = self.config.get("discord", {}).get("webhook_url", None)
+        self.dry_run = self.config.get("romdownloader", {}).get("dry_run", False)
 
     def run(self,
             ):
         """Run Rclone sync tool"""
 
-        self.logger.info(create_bar(f"START ROMDownloader"))
-
         start_files = get_tidy_files(os.path.join(str(self.out_dir), "*"))
 
         self.rclone_sync(ftp_dir=self.ftp_dir,
                          out_dir=self.out_dir,
                          )
 
         end_files = get_tidy_files(os.path.join(str(self.out_dir), "*"))
 
         if self.discord_url is not None:
-
             name = f"ROMDownloader: {self.platform}"
             self.post_to_discord(start_files,
                                  end_files,
                                  name=name
                                  )
 
         # If there are potential additional files to download, do that here
@@ -162,16 +199,14 @@
                 if self.discord_url is not None:
                     name = f"ROMDownloader: {self.platform} ({add_dir})"
                     self.post_to_discord(start_files,
                                          end_files,
                                          name=name
                                          )
 
-        self.logger.info(create_bar(f"FINISH ROMDownloader"))
-
     def rclone_sync(self,
                     ftp_dir,
                     out_dir=None,
                     transfers=5,
                     ):
 
         if out_dir is None:
@@ -195,14 +230,15 @@
                 pattern = get_file_pattern(searches)
             else:
                 pattern = None
 
             if pattern:
                 cmd += add_rclone_filter(pattern=pattern,
                                          filter_type="exclude",
+                                         include_wildcard=self.include_wildcard,
                                          )
 
             # Now onto positive filters
             searches = []
 
             # Specific games
             if self.include_games is not None:
@@ -212,23 +248,27 @@
                 pattern = get_file_pattern(searches)
             else:
                 pattern = None
 
             if pattern:
                 cmd += add_rclone_filter(pattern=pattern,
                                          filter_type="include",
+                                         include_wildcard=self.include_filter_wildcard,
                                          )
 
                 cmd += ' --filter "- *"'
 
         if self.dry_run:
             self.logger.info(f"Dry run, would rclone_sync with:")
             self.logger.info(cmd)
         else:
-            # os.system(cmd)
+
+            if not os.path.exists(self.out_dir):
+                os.makedirs(self.out_dir)
+
             # Execute the command and capture the output
             with subprocess.Popen(cmd, text=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT) as process:
                 for line in process.stdout:
                     # Log each line of the output using the provided logger
                     self.logger.info(line[:-1])  # Exclude the newline character
 
         return True
@@ -249,14 +289,16 @@
         """
 
         items_added = list(set(end_files).difference(start_files))
         items_deleted = list(set(start_files).difference(end_files))
 
         if len(items_added) > 0:
 
+            items_added.sort()
+
             for items_split in split(items_added, chunk_size=max_per_message):
 
                 fields = []
 
                 field_dict = {"name": "Added",
                               "value": "\n".join(items_split)
                               }
@@ -266,14 +308,16 @@
                     discord_push(url=self.discord_url,
                                  name=name,
                                  fields=fields,
                                  )
 
         if len(items_deleted) > 0:
 
+            items_deleted.sort()
+
             for items_split in split(items_deleted, chunk_size=max_per_message):
 
                 fields = []
 
                 field_dict = {"name": "Deleted",
                               "value": "\n".join(items_split)
                               }
```

### Comparing `romsearch-0.0.4/romsearch/modules/rommover.py` & `romsearch-0.0.5/romsearch/modules/rommover.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,77 +1,101 @@
 import copy
 import os
 import shutil
 
 import romsearch
-from ..util import load_yml, setup_logger, create_bar, unzip_file, load_json, save_json
+from ..util import (load_yml,
+                    setup_logger,
+                    unzip_file,
+                    load_json,
+                    save_json
+                    )
 
 
 class ROMMover:
 
     def __init__(self,
-                 config_file,
                  platform,
-                 game
+                 game,
+                 config_file=None,
+                 config=None,
+                 platform_config=None,
+                 logger=None,
                  ):
         """ROM Moving and cache updating tool
 
         Because we do this per-platform, per-game, they need to be specified here
-        """
 
-        logger_add_dir = str(os.path.join(platform, game))
+        Args:
+            platform (str): Platform name
+            game (str): Game name
+            config_file (str, optional): path to config file. Defaults to None.
+            config (dict, optional): configuration dictionary. Defaults to None.
+            platform_config (dict, optional): platform configuration dictionary. Defaults to None.
+            logger (logging.Logger, optional): logger. Defaults to None.
+        """
 
-        self.logger = setup_logger(log_level="info",
-                                   script_name=f"ROMMover",
-                                   additional_dir=logger_add_dir,
-                                   )
+        if config_file is None and config is None:
+            raise ValueError("config_file or config must be specified")
 
-        config = load_yml(config_file)
+        if config is None:
+            config = load_yml(config_file)
+        self.config = config
+
+        if logger is None:
+            log_dir = self.config.get("dirs", {}).get("log_dir", os.path.join(os.getcwd(), "logs"))
+            logger_add_dir = str(os.path.join(platform, game))
+            logger = setup_logger(log_level="info",
+                                  script_name=f"ROMMover",
+                                  log_dir=log_dir,
+                                  additional_dir=logger_add_dir,
+                                  )
+        self.logger = logger
 
-        self.raw_dir = config.get("raw_dir", None)
+        self.raw_dir = self.config.get("dirs", {}).get("raw_dir", None)
         if self.raw_dir is None:
             raise ValueError("raw_dir needs to be defined in config")
 
-        self.rom_dir = config.get("rom_dir", None)
+        self.rom_dir = self.config.get("dirs", {}).get("rom_dir", None)
         if self.rom_dir is None:
             raise ValueError("rom_dir needs to be defined in config")
 
-        cache_file = config.get("rommover", {}).get("cache_file", None)
-        if cache_file is None:
-            cache_file = os.path.join(os.getcwd(), f"cache ({platform}).json")
+        cache_dir = self.config.get("dirs", {}).get("cache_dir", os.getcwd())
+        if not os.path.exists(cache_dir):
+            os.makedirs(cache_dir)
+
+        cache_file = os.path.join(cache_dir, f"cache ({platform}).json")
 
         if os.path.exists(cache_file):
             cache = load_json(cache_file)
         else:
             cache = {}
 
         self.platform = platform
         self.game = game
         self.cache_file = cache_file
         self.cache = cache
 
         # Pull in platform config that we need
         mod_dir = os.path.dirname(romsearch.__file__)
-        platform_config_file = os.path.join(mod_dir, "configs", "platforms", f"{platform}.yml")
-        platform_config = load_yml(platform_config_file)
 
+        if platform_config is None:
+            platform_config_file = os.path.join(mod_dir, "configs", "platforms", f"{platform}.yml")
+            platform_config = load_yml(platform_config_file)
         self.platform_config = platform_config
+
         self.unzip = self.platform_config.get("unzip", False)
 
     def run(self,
             rom_dict,
             ):
 
-        self.logger.info(create_bar(f"START ROMMover"))
-
         roms_moved = self.move_roms(rom_dict)
         self.save_cache()
 
-        self.logger.info(create_bar(f"FINISH ROMMover"))
-
         return roms_moved
 
     def move_roms(self, rom_dict):
         """Actually move the roms"""
 
         roms_moved = []
```

### Comparing `romsearch-0.0.4/romsearch/modules/romparser.py` & `romsearch-0.0.5/romsearch/modules/romparser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import copy
 import os
 import re
-import time
-from datetime import datetime
 
 import romsearch
 from ..util import (setup_logger,
-                    create_bar,
+                    get_file_time,
                     load_yml,
                     load_json,
-                    get_bracketed_file_pattern,
                     get_game_name,
                     )
 
 DICT_DEFAULT_VALS = {
     "bool": False,
     "str": "",
     "list": []
@@ -67,114 +64,124 @@
 
     else:
         pattern_val = None
 
     return pattern_val
 
 
-def get_file_time(f,
-                  datetime_format,
-                  ):
-    """Get created file time from the file itself"""
-
-    if os.path.exists(f):
-        ti_m = os.path.getmtime(f)
-        date_ti_m = datetime.strptime(time.ctime(ti_m), "%a %b %d %H:%M:%S %Y")
-    else:
-        date_ti_m = datetime(year=1900, month=1, day=1, hour=0, minute=0, second=0)
-    date_ti_m_str = date_ti_m.strftime(format=datetime_format)
-
-    return date_ti_m_str
-
-
 class ROMParser:
 
     def __init__(self,
-                 config_file,
                  platform,
                  game,
+                 config_file=None,
+                 config=None,
+                 platform_config=None,
+                 default_config=None,
+                 regex_config=None,
+                 logger=None,
                  ):
         """ROM parser tool
 
         This works per-game, per-platform, so must be specified here
 
+        Args:
+            platform (str): Platform name
+            game (str): Game name
+            config_file (str, optional): path to config file. Defaults to None.
+            config (dict, optional): configuration dictionary. Defaults to None.
+            platform_config (dict, optional): platform configuration dictionary. Defaults to None.
+            default_config (dict, optional): default configuration dictionary. Defaults to None.
+            regex_config (dict, optional): regex configuration dictionary. Defaults to None.
+            logger (logging.Logger, optional): logger instance. Defaults to None.
+
         TODO:
             - Default implied languages from regions
         """
 
         if platform is None:
             raise ValueError("platform must be specified")
         self.platform = platform
 
-        logger_add_dir = str(os.path.join(platform, game))
-
-        self.logger = setup_logger(log_level="info",
-                                   script_name=f"ROMParser",
-                                   additional_dir=logger_add_dir,
-                                   )
+        if config_file is None and config is None:
+            raise ValueError("config_file or config must be specified")
 
-        config = load_yml(config_file)
+        if config is None:
+            config = load_yml(config_file)
+        self.config = config
+
+        if logger is None:
+            log_dir = self.config.get("dirs", {}).get("log_dir", os.path.join(os.getcwd(), "logs"))
+            logger_add_dir = str(os.path.join(platform, game))
+            logger = setup_logger(log_level="info",
+                                  script_name=f"ROMParser",
+                                  log_dir=log_dir,
+                                  additional_dir=logger_add_dir,
+                                  )
+        self.logger = logger
 
         mod_dir = os.path.dirname(romsearch.__file__)
 
-        default_config_file = os.path.join(mod_dir, "configs", "defaults.yml")
-        self.default_config = load_yml(default_config_file)
-
-        regex_file = os.path.join(mod_dir, "configs", "regex.yml")
-        self.regex = load_yml(regex_file)
-
-        platform_config_file = os.path.join(mod_dir, "configs", "platforms", f"{platform}.yml")
-        self.platform_config = load_yml(platform_config_file)
+        if default_config is None:
+            default_file = os.path.join(mod_dir, "configs", "defaults.yml")
+            default_config = load_yml(default_file)
+        self.default_config = default_config
+
+        if regex_config is None:
+            regex_file = os.path.join(mod_dir, "configs", "regex.yml")
+            regex_config = load_yml(regex_file)
+        self.regex_config = regex_config
+
+        if platform_config is None:
+            platform_config_file = os.path.join(mod_dir, "configs", "platforms", f"{platform}.yml")
+            platform_config = load_yml(platform_config_file)
+        self.platform_config = platform_config
 
-        self.raw_dir = config.get("raw_dir", None)
+        self.raw_dir = self.config.get("dirs", {}).get("raw_dir", None)
         if not self.raw_dir:
             raise ValueError("raw_dir must be specified in config.yml")
 
-        self.use_dat = config.get("romparser", {}).get("use_dat", True)
-        self.use_retool = config.get("romparser", {}).get("use_retool", True)
-        self.use_filename = config.get("romparser", {}).get("use_filename", True)
-        self.dry_run = config.get("romparser", {}).get("dry_run", False)
+        self.use_dat = self.config.get("romparser", {}).get("use_dat", True)
+        self.use_retool = self.config.get("romparser", {}).get("use_retool", True)
+        self.use_filename = self.config.get("romparser", {}).get("use_filename", True)
+        self.dry_run = self.config.get("romparser", {}).get("dry_run", False)
 
         # If we're using the dat file, pull it out here
         self.dat = None
         if self.use_dat:
-            dat_dir = config.get("parsed_dat_dir", None)
+            dat_dir = self.config.get("dirs", {}).get("parsed_dat_dir", None)
             if dat_dir is None:
                 raise ValueError("parsed_dat_dir must be specified in config.yml")
             dat_file = os.path.join(dat_dir, f"{platform} (dat parsed).json")
             if os.path.exists(dat_file):
                 self.dat = load_json(dat_file)
 
         # If we're using the retool file, pull it out here
         self.retool = None
         if self.use_retool:
-            dat_dir = config.get("parsed_dat_dir", None)
+            dat_dir = self.config.get("dirs", {}).get("parsed_dat_dir", None)
             if dat_dir is None:
                 raise ValueError("parsed_dat_dir must be specified in config.yml")
             retool_file = os.path.join(dat_dir, f"{platform} (retool).json")
             if os.path.exists(retool_file):
                 self.retool = load_json(retool_file)
 
     def run(self,
             files,
             ):
         """Run the ROM parser"""
 
-        self.logger.info(create_bar(f"START ROMParser"))
-
         game_dict = {}
 
         for f in files:
             game_dict[f] = self.parse_file(f)
 
             # Include the priority
             game_dict[f]["priority"] = files[f]["priority"]
 
-        self.logger.info(create_bar(f"FINISH ROMParser"))
-
         return game_dict
 
     def parse_file(self,
                    f,
                    ):
         """Parse useful info out of a specific file"""
 
@@ -193,15 +200,15 @@
         # File modification time
         full_file_path = os.path.join(self.raw_dir, self.platform, f)
         file_time = get_file_time(full_file_path,
                                   datetime_format=self.default_config["datetime_format"],
                                   )
         file_dict["file_mod_time"] = file_time
 
-        self.logger.info(f"{f}: {file_dict}")
+        self.logger.debug(f"{f}: {file_dict}")
 
         return file_dict
 
     def parse_retool(self, f, file_dict=None):
         """Parse info out of the retool file"""
 
         if file_dict is None:
@@ -291,22 +298,22 @@
 
         if file_dict is None:
             file_dict = {}
 
         # Split file into tags
         tags = [f'({x}' for x in f.strip(".zip").split(' (')][1:]
 
-        for regex_key in self.regex:
+        for regex_key in self.regex_config:
 
-            regex_type = self.regex[regex_key].get("type", "bool")
-            search_tags = self.regex[regex_key].get("search_tags", True)
-            group = self.regex[regex_key].get("group", None)
-            regex_flags = self.regex[regex_key].get("flags", "I")
-            transform_pattern = self.regex[regex_key].get("transform_pattern", None)
-            transform_repl = self.regex[regex_key].get("transform_repl", None)
+            regex_type = self.regex_config[regex_key].get("type", "bool")
+            search_tags = self.regex_config[regex_key].get("search_tags", True)
+            group = self.regex_config[regex_key].get("group", None)
+            regex_flags = self.regex_config[regex_key].get("flags", "I")
+            transform_pattern = self.regex_config[regex_key].get("transform_pattern", None)
+            transform_repl = self.regex_config[regex_key].get("transform_repl", None)
 
             dict_default_val = DICT_DEFAULT_VALS.get(regex_type, None)
             if dict_default_val is None:
                 raise ValueError(f"regex_type should be one of {list(DICT_DEFAULT_VALS.keys())}")
 
             if regex_key not in file_dict:
                 file_dict[regex_key] = dict_default_val
@@ -314,15 +321,15 @@
             if regex_flags == "NOFLAG":
                 regex_flags = re.NOFLAG
             elif regex_flags == "I":
                 regex_flags = re.I
             else:
                 raise ValueError("regex_flags should be one of 'NOFLAG', 'I'")
 
-            pattern = self.regex[regex_key]["pattern"]
+            pattern = self.regex_config[regex_key]["pattern"]
 
             pattern_mappings = None
 
             if regex_type == "list":
 
                 if isinstance(self.default_config[regex_key], dict):
                     str_to_join = [self.default_config[regex_key][key] for key in self.default_config[regex_key]]
```

### Comparing `romsearch-0.0.4/romsearch/util/logger.py` & `romsearch-0.0.5/romsearch/util/logger.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 import logging
-import math
 import os
+import sys
 from logging.handlers import RotatingFileHandler
-from pathvalidate import sanitize_filename
 
-from .. import __version__
+import colorlog
+from pathvalidate import sanitize_filename
 
 
 def setup_logger(log_level,
                  script_name,
+                 log_dir,
                  additional_dir="",
                  max_logs=9,
                  ):
     """
     Set up the logger.
 
     Parameters:
         log_level (str): The log level to use
         script_name (str): The name of the script
+        log_dir (str): The directory to save logs to
         additional_dir (str): Any additional directories to keep log files tidy
         max_logs (int): Maximum number of log files to keep
 
     Returns:
         A logger object for logging messages.
     """
 
     # Sanitize the directories if we need to
     additional_dir = [sanitize_filename(f) for f in additional_dir.split(os.path.sep)]
 
     if os.environ.get('DOCKER_ENV'):
-        config_dir = os.getenv('CONFIG_DIR', '/config')
-        log_dir = os.path.join(config_dir, "logs", script_name, *additional_dir)
+        log_dir = os.path.join(log_dir, script_name, *additional_dir)
     else:
-        log_dir = os.path.join(os.getcwd(), "logs", script_name, *additional_dir)
+        log_dir = os.path.join(log_dir, script_name, *additional_dir)
 
     if log_level not in ['debug', 'info', 'critical']:
         log_level = 'info'
         print(f"Invalid log level '{log_level}', defaulting to 'info'")
 
     # Create the log directory if it doesn't exist
     if not os.path.exists(log_dir):
         os.makedirs(log_dir)
 
     # Define the log file path, and sanitize if needs be
-    log_file = f"{log_dir}/{script_name}.log"
+    log_file = os.path.join(log_dir, f"{script_name}.log")
 
     # Check if log file already exists
     if os.path.isfile(log_file):
         for i in range(max_logs - 1, 0, -1):
             old_log = f"{log_dir}/{script_name}.log.{i}"
             new_log = f"{log_dir}/{script_name}.log.{i + 1}"
             if os.path.exists(old_log):
                 if os.path.exists(new_log):
                     os.remove(new_log)
                 os.rename(old_log, new_log)
-        os.rename(log_file, f"{log_dir}/{script_name}.log.1")
+        os.rename(log_file, os.path.join(log_dir, f"{script_name}.log.1"))
 
     # Create a logger object with the script name
     logger = logging.getLogger(script_name)
     logger.propagate = False
 
     # Set the log level based on the provided parameter
     log_level = log_level.upper()
@@ -68,62 +69,36 @@
         logger.setLevel(logging.INFO)
     elif log_level == 'CRITICAL':
         logger.setLevel(logging.CRITICAL)
     else:
         logger.critical(f"Invalid log level '{log_level}', defaulting to 'INFO'")
         logger.setLevel(logging.INFO)
 
-    # Define the log message format
-    formatter = logging.Formatter(fmt='%(asctime)s %(levelname)s: %(message)s', datefmt='%m/%d/%y %I:%M %p')
+    # Define the log message format for the log files
+    logfile_formatter = logging.Formatter(fmt='%(asctime)s %(levelname)s: %(message)s', datefmt='%m/%d/%y %I:%M %p')
 
     # Create a RotatingFileHandler for log files
     handler = RotatingFileHandler(log_file, delay=True, mode="w", backupCount=max_logs)
-    handler.setFormatter(formatter)
+    handler.setFormatter(logfile_formatter)
 
     # Add the file handler to the logger
     logger.addHandler(handler)
 
     # Configure console logging with the specified log level
-    console_handler = logging.StreamHandler()
+    console_handler = colorlog.StreamHandler(sys.stdout)
     if log_level == 'DEBUG':
         console_handler.setLevel(logging.DEBUG)
     elif log_level == 'INFO':
         console_handler.setLevel(logging.INFO)
     elif log_level == 'CRITICAL':
         console_handler.setLevel(logging.CRITICAL)
 
     # Add the console handler to the logger
+    console_handler.setFormatter(colorlog.ColoredFormatter("%(log_color)s%(levelname)s: %(message)s"))
     logger.addHandler(console_handler)
 
     # Overwrite previous logger if exists
     logging.getLogger(script_name).handlers.clear()
     logging.getLogger(script_name).addHandler(handler)
     logging.getLogger(script_name).addHandler(console_handler)
 
-    # Insert version number at the head of every log file
-    name = script_name.replace("_", " ").upper()
-    logger.info(create_bar(f"{name} Version: {__version__}"))
-
     return logger
-
-
-def create_bar(middle_text):
-    """
-    Creates a separation bar with provided text in the center
-
-    Args:
-        middle_text (str): The text to place in the center of the separation bar
-
-    Returns:
-        str: The formatted separation bar
-    """
-    total_length = 80
-    if len(middle_text) == 1:
-        remaining_length = total_length - len(middle_text) - 2
-        left_side_length = 0
-        right_side_length = remaining_length
-        return f"\n{middle_text * left_side_length}{middle_text}{middle_text * right_side_length}\n"
-    else:
-        remaining_length = total_length - len(middle_text) - 4
-        left_side_length = math.floor(remaining_length / 2)
-        right_side_length = remaining_length - left_side_length
-        return f"\n{'*' * left_side_length} {middle_text} {'*' * right_side_length}\n"
```

### Comparing `romsearch-0.0.4/romsearch/util/regex_matching.py` & `romsearch-0.0.5/romsearch/util/regex_matching.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.4/romsearch.egg-info/PKG-INFO` & `romsearch-0.0.5/romsearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romsearch
-Version: 0.0.4
+Version: 0.0.5
 Summary: One Stop ROM Shop
 Author: bbtufty
 Maintainer: bbtufty
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -690,18 +690,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: colorlog
 Requires-Dist: discordwebhook
 Requires-Dist: numpy
 Requires-Dist: packaging
 Requires-Dist: pathvalidate
+Requires-Dist: PySide6
 Requires-Dist: pyyaml
 Requires-Dist: xmltodict
 Provides-Extra: docs
 Requires-Dist: sphinx-automodapi; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 
 # ROMSearch
@@ -712,14 +714,16 @@
 [![Actions](https://img.shields.io/github/actions/workflow/status/bbtufty/romsearch/build_test.yaml?branch=main&style=flat-square)](https://github.com/bbtufty/romsearch/actions)
 [![License](https://img.shields.io/badge/license-GNUv3-blue.svg?label=License&style=flat-square)](LICENSE)
 
 ROMSearch is designed as a simple-to-inferface with tool that will allow you to pull ROM files from some remote (or
 local) location, figure out the best ROM, and move it cleanly to a folder that can imported into an emulator. ROMSearch
 is supposed to be a one-shot program to get you from files online to playing games (which is what we want, right?).
 
+ROMSearch also has a GUI! Currently only for Windows, but makes setting up configurations simple and clean.
+
 ROMSearch offers the ability to:
 
 * Sync from remote folder using rclone
 * Parse DAT files as well as filenames for ROM information
 * Remove dupes from ROM lists using DAT files as well as the excellent ``retool`` clonelists
 * Moving files to a structured location, including potentially additional files that may be needed
 * Discord integration so users can see the results of runs in a simple, clean way
```

### Comparing `romsearch-0.0.4/romsearch.egg-info/SOURCES.txt` & `romsearch-0.0.5/romsearch.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 .gitignore
 .readthedocs.yaml
 CHANGES.rst
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+romsearch_gui.py
 .github/ISSUE_TEMPLATE/bug_report.yml
 .github/ISSUE_TEMPLATE/console_request.yml
 .github/ISSUE_TEMPLATE/feature_request.yml
-.github/workflows/build_test.yaml
+.github/workflows/build.yaml
 .github/workflows/publish.yaml
 docs/1g1r.rst
 docs/Makefile
 docs/changelog.rst
 docs/conf.py
 docs/configs.rst
 docs/configuration.rst
@@ -26,14 +27,25 @@
 docs/utils.rst
 docs/configs/clonelists.rst
 docs/configs/config.rst
 docs/configs/dats.rst
 docs/configs/defaults.rst
 docs/configs/platforms.rst
 docs/configs/regex.rst
+docs/gui/config_includes_excludes.rst
+docs/gui/config_main.rst
+docs/gui/config_modules.rst
+docs/gui/config_platforms.rst
+docs/gui/config_regions_languages.rst
+docs/gui/intro.rst
+docs/images/config_includes_excludes.png
+docs/images/config_main.png
+docs/images/config_modules.png
+docs/images/config_platforms.png
+docs/images/config_regions_languages.png
 docs/modules/datparser.rst
 docs/modules/dupeparser.rst
 docs/modules/gamefinder.rst
 docs/modules/romchooser.rst
 docs/modules/romdownloader.rst
 docs/modules/rommover.rst
 docs/modules/romparser.rst
@@ -54,14 +66,23 @@
 romsearch/configs/platforms/Nintendo - Nintendo Entertainment System.yml
 romsearch/configs/platforms/Nintendo - Super Nintendo Entertainment System.yml
 romsearch/configs/platforms/Sony - PlayStation 2.yml
 romsearch/configs/platforms/Sony - PlayStation Portable.yml
 romsearch/configs/platforms/Sony - PlayStation.yml
 romsearch/dev/__init__.py
 romsearch/dev/parsing_tools.py
+romsearch/gui/__init__.py
+romsearch/gui/gui_about.py
+romsearch/gui/gui_config.py
+romsearch/gui/gui_romsearch.py
+romsearch/gui/gui_utils.py
+romsearch/gui/layout_about.py
+romsearch/gui/layout_about.ui
+romsearch/gui/layout_romsearch.py
+romsearch/gui/layout_romsearch.ui
 romsearch/modules/__init__.py
 romsearch/modules/datparser.py
 romsearch/modules/dupeparser.py
 romsearch/modules/gamefinder.py
 romsearch/modules/romchooser.py
 romsearch/modules/romdownloader.py
 romsearch/modules/rommover.py
```

