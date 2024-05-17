# Comparing `tmp/romsearch-0.0.3.tar.gz` & `tmp/romsearch-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "romsearch-0.0.3.tar", last modified: Wed May  8 11:56:07 2024, max compression
+gzip compressed data, was "romsearch-0.0.4.tar", last modified: Thu May  9 11:41:16 2024, max compression
```

## Comparing `romsearch-0.0.3.tar` & `romsearch-0.0.4.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.896916 romsearch-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.880916 romsearch-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.884916 romsearch-0.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-08 11:56:03.000000 romsearch-0.0.3/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-08 11:56:03.000000 romsearch-0.0.3/.github/ISSUE_TEMPLATE/console_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-08 11:56:03.000000 romsearch-0.0.3/.github/ISSUE_TEMPLATE/feature_request.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.884916 romsearch-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-08 11:56:03.000000 romsearch-0.0.3/.github/workflows/build_test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-08 11:56:03.000000 romsearch-0.0.3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-08 11:56:03.000000 romsearch-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-08 11:56:03.000000 romsearch-0.0.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-08 11:56:03.000000 romsearch-0.0.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 11:56:03.000000 romsearch-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 11:56:03.000000 romsearch-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    43725 2024-05-08 11:56:07.896916 romsearch-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-08 11:56:03.000000 romsearch-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.888916 romsearch-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/1g1r.rst
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.888916 romsearch-0.0.3/docs/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/configs/clonelists.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/configs/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/configs/dats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/configs/defaults.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/configs/platforms.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/configs/regex.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/configs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/known_issues.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.888916 romsearch-0.0.3/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/modules/datparser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/modules/dupeparser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/modules/gamefinder.rst
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/modules/romchooser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/modules/romdownloader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/modules/rommover.rst
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/modules/romparser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/modules/romsearch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/reference_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-08 11:56:03.000000 romsearch-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.888916 romsearch-0.0.3/romsearch/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.892916 romsearch-0.0.3/romsearch/configs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.892916 romsearch-0.0.3/romsearch/configs/clonelists/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/clonelists/retool.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.892916 romsearch-0.0.3/romsearch/configs/dats/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/dats/no-intro.yml
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/dats/redump.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/defaults.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.892916 romsearch-0.0.3/romsearch/configs/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/platforms/Nintendo - GameCube.yml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/platforms/Nintendo - Nintendo Entertainment System.yml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/platforms/Nintendo - Super Nintendo Entertainment System.yml
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/platforms/Sony - PlayStation 2.yml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/platforms/Sony - PlayStation.yml
--rw-r--r--   0 runner    (1001) docker     (127)    12437 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/regex.yml
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/sample_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.892916 romsearch-0.0.3/romsearch/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/dev/parsing_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.896916 romsearch-0.0.3/romsearch/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/modules/datparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/modules/dupeparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/modules/gamefinder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15816 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/modules/romchooser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/modules/romdownloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/modules/rommover.py
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/modules/romparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/modules/romsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.896916 romsearch-0.0.3/romsearch/util/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/util/discord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/util/general.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/util/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/util/regex_matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.896916 romsearch-0.0.3/romsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43725 2024-05-08 11:56:07.000000 romsearch-0.0.3/romsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-08 11:56:07.000000 romsearch-0.0.3/romsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 11:56:07.000000 romsearch-0.0.3/romsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-08 11:56:07.000000 romsearch-0.0.3/romsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 11:56:07.000000 romsearch-0.0.3/romsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 11:56:07.896916 romsearch-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.980947 romsearch-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.968947 romsearch-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.972947 romsearch-0.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-09 11:41:13.000000 romsearch-0.0.4/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-09 11:41:13.000000 romsearch-0.0.4/.github/ISSUE_TEMPLATE/console_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-09 11:41:13.000000 romsearch-0.0.4/.github/ISSUE_TEMPLATE/feature_request.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.972947 romsearch-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-09 11:41:13.000000 romsearch-0.0.4/.github/workflows/build_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-09 11:41:13.000000 romsearch-0.0.4/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-09 11:41:13.000000 romsearch-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-09 11:41:13.000000 romsearch-0.0.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-09 11:41:13.000000 romsearch-0.0.4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 11:41:13.000000 romsearch-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-09 11:41:13.000000 romsearch-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    43755 2024-05-09 11:41:16.980947 romsearch-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-09 11:41:13.000000 romsearch-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.972947 romsearch-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/1g1r.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.972947 romsearch-0.0.4/docs/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/configs/clonelists.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/configs/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/configs/dats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/configs/defaults.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/configs/platforms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/configs/regex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/known_issues.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.976947 romsearch-0.0.4/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/modules/datparser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/modules/dupeparser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/modules/gamefinder.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/modules/romchooser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/modules/romdownloader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/modules/rommover.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/modules/romparser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/modules/romsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/reference_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-09 11:41:13.000000 romsearch-0.0.4/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-09 11:41:13.000000 romsearch-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.976947 romsearch-0.0.4/romsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.976947 romsearch-0.0.4/romsearch/configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.976947 romsearch-0.0.4/romsearch/configs/clonelists/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/clonelists/retool.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.976947 romsearch-0.0.4/romsearch/configs/dats/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/dats/no-intro.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/dats/redump.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/defaults.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.976947 romsearch-0.0.4/romsearch/configs/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/platforms/Nintendo - GameCube.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/platforms/Nintendo - Nintendo Entertainment System.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/platforms/Nintendo - Super Nintendo Entertainment System.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/platforms/Sony - PlayStation 2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/platforms/Sony - PlayStation Portable.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/platforms/Sony - PlayStation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/regex.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/configs/sample_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.976947 romsearch-0.0.4/romsearch/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/dev/parsing_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.980947 romsearch-0.0.4/romsearch/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/modules/datparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/modules/dupeparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/modules/gamefinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/modules/romchooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/modules/romdownloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/modules/rommover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/modules/romparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/modules/romsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.980947 romsearch-0.0.4/romsearch/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/util/discord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/util/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/util/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-09 11:41:13.000000 romsearch-0.0.4/romsearch/util/regex_matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:41:16.980947 romsearch-0.0.4/romsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43755 2024-05-09 11:41:16.000000 romsearch-0.0.4/romsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-09 11:41:16.000000 romsearch-0.0.4/romsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:41:16.000000 romsearch-0.0.4/romsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-09 11:41:16.000000 romsearch-0.0.4/romsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 11:41:16.000000 romsearch-0.0.4/romsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 11:41:16.980947 romsearch-0.0.4/setup.cfg
```

### Comparing `romsearch-0.0.3/.github/ISSUE_TEMPLATE/bug_report.yml` & `romsearch-0.0.4/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/.github/ISSUE_TEMPLATE/feature_request.yml` & `romsearch-0.0.4/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/.github/workflows/build_test.yaml` & `romsearch-0.0.4/.github/workflows/build_test.yaml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/.github/workflows/publish.yaml` & `romsearch-0.0.4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/.gitignore` & `romsearch-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/.readthedocs.yaml` & `romsearch-0.0.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/CHANGES.rst` & `romsearch-0.0.4/CHANGES.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+0.0.4 (2024-05-09)
+==================
+
+Features
+--------
+
+- Added Sony - PlayStation Portable
+
+Fixes
+-----
+
+ROMChooser
+~~~~~~~~~~
+
+- Added regex terms for PSP
+- Fixed a bug with version scoring
+
+Util
+~~~~
+
+- Added feature to flag up tags but not remove them from the short name (e.g. "Demo" should be included in the name,
+  but should be used to flag up demo ROMs)
+
 0.0.3 (2024-05-08)
 ==================
 
 Features
 --------
 
 - Added Sony - PlayStation 2
```

### Comparing `romsearch-0.0.3/LICENSE` & `romsearch-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/PKG-INFO` & `romsearch-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romsearch
-Version: 0.0.3
+Version: 0.0.4
 Summary: One Stop ROM Shop
 Author: bbtufty
 Maintainer: bbtufty
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -730,10 +730,11 @@
 works for the following consoles:
 
 * Nintendo - GameCube
 * Nintendo - Nintendo Entertainment System
 * Nintendo - Super Nintendo Entertainment System
 * Sony - PlayStation
 * Sony - PlayStation 2
+* Sony - PlayStation Portable
 
 but be aware there may be quirks that will only become apparent over time. We encourage users to open
 [issues](https://github.com/bbtufty/romsearch/issues) as and where they find them.
```

### Comparing `romsearch-0.0.3/README.md` & `romsearch-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,10 +24,11 @@
 works for the following consoles:
 
 * Nintendo - GameCube
 * Nintendo - Nintendo Entertainment System
 * Nintendo - Super Nintendo Entertainment System
 * Sony - PlayStation
 * Sony - PlayStation 2
+* Sony - PlayStation Portable
 
 but be aware there may be quirks that will only become apparent over time. We encourage users to open
 [issues](https://github.com/bbtufty/romsearch/issues) as and where they find them.
```

### Comparing `romsearch-0.0.3/docs/1g1r.rst` & `romsearch-0.0.4/docs/1g1r.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/docs/Makefile` & `romsearch-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/docs/conf.py` & `romsearch-0.0.4/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'romsearch'
 copyright = '2024, bbtufty'
 author = 'bbtufty'
-release = '0.0.3'
+release = '0.0.4'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc',
               'sphinx.ext.coverage',
               'sphinx.ext.napoleon',
```

### Comparing `romsearch-0.0.3/docs/configs/config.rst` & `romsearch-0.0.4/docs/configs/config.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/docs/configs/dats.rst` & `romsearch-0.0.4/docs/configs/dats.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/docs/configs/platforms.rst` & `romsearch-0.0.4/docs/configs/platforms.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/docs/configs/regex.rst` & `romsearch-0.0.4/docs/configs/regex.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/docs/configuration.rst` & `romsearch-0.0.4/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/docs/index.rst` & `romsearch-0.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/docs/intro.rst` & `romsearch-0.0.4/docs/intro.rst`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 has the capability for:
 
 * Nintendo - GameCube
 * Nintendo - Nintendo Entertainment System
 * Nintendo - Super Nintendo Entertainment System
 * Sony - PlayStation
 * Sony - PlayStation 2
+* Sony - PlayStation Portable
 
 but be aware there may be quirks that will only become apparent over time. We encourage users to open
 `issues <https://github.com/bbtufty/romsearch/issues>`_ as and where they find them. Known issues can be found at
 :doc:`known issues <known_issues>`.
 
 ROMSearch is also built in such a way that other platforms/filters can be added in a simple way using config files
 rather than manually adding to the base code. For more details of how these work, see the various
```

### Comparing `romsearch-0.0.3/docs/make.bat` & `romsearch-0.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/docs/modules/datparser.rst` & `romsearch-0.0.4/docs/modules/datparser.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/docs/modules/dupeparser.rst` & `romsearch-0.0.4/docs/modules/dupeparser.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/docs/modules/romdownloader.rst` & `romsearch-0.0.4/docs/modules/romdownloader.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/pyproject.toml` & `romsearch-0.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "romsearch"
-version = "0.0.3"
+version = "0.0.4"
 description = "One Stop ROM Shop"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 
 authors = [
     {name = "bbtufty"},
```

### Comparing `romsearch-0.0.3/romsearch/__init__.py` & `romsearch-0.0.4/romsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/romsearch/configs/defaults.yml` & `romsearch-0.0.4/romsearch/configs/defaults.yml`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 platforms:
   - "Nintendo - GameCube"
   - "Nintendo - Nintendo Entertainment System"
   - "Nintendo - Super Nintendo Entertainment System"
   - "Sony - PlayStation"
   - "Sony - PlayStation 2"
+  - "Sony - PlayStation Portable"
 
 video_types:
   - "NTSC"
   - "PAL"
   - "PAL 60Hz"
   - "MPAL"
   - "SECAM"
```

### Comparing `romsearch-0.0.3/romsearch/configs/regex.yml` & `romsearch-0.0.4/romsearch/configs/regex.yml`

 * *Files 10% similar despite different names*

```diff
@@ -20,78 +20,91 @@
   group: "alternate"
 
 # APPLICATIONS
 
 bracket_program:
   pattern: "\\((?:Test )?Program\\)"
   group: "applications"
+  include_in_short_name: true
 
 non_bracket_program:
   pattern: "(Check|Sample) Program"
   search_tags: false
   group: "applications"
+  include_in_short_name: true
 
 # BAD DUMP
 
 bad_dump:
   pattern: "\\[b\\]"
   search_tags: false
   group: "bad_dumps"
 
 # CONSOLE
 
 bios:
   pattern: "\\[BIOS\\]\\s?"
   search_tags: false
   group: "console"
+  include_in_short_name: true
 
 enhancement_chip:
   pattern: "\\(Enhancement Chip\\)"
   group: "console"
+  include_in_short_name: true
 
 # DEMOS
 barai:
   pattern: "\\(@barai\\)"
   group: "demos"
+  include_in_short_name: true
 
 demo:
   pattern: "\\((?:\\w[-.]?\\s*)*Demo(?:(?:,?\\s|-)[\\w0-9\\.]*)*\\)"
   group: "demos"
+  include_in_short_name: true
 
 kiosk:
   pattern: "\\((?:\\w-?\\s*)*?Kiosk,?(?:\\s\\w*?)*\\)|Kiosk Demo Disc|(PSP System|PS2) Kiosk"
   group: "demos"
   search_tags: false
+  include_in_short_name: true
 
 preview:
   pattern: "\\(Preview\\)"
   group: "demos"
+  include_in_short_name: true
 
 sample:
   pattern: "\\(Sample(?:\\s[0-9]*|\\s\\d{4}-\\d{2}-\\d{2})?\\)"
   group: "demos"
+  include_in_short_name: true
 
 taikenban_brackets:
   pattern: "\\((.*?)Taikenban(.*?)\\)"
   search_tags: false
   group: "demos"
+  include_in_short_name: true
 
 taikenban:
   pattern: "Taikenban"
   search_tags: false
   group: "demos"
+  include_in_short_name: true
 
 trial:
   pattern: "\\(Trial (Disc|Edition|Version|ver\\.)\\)"
   group: "demos"
+  include_in_short_name: true
 
 trial_non_bracket:
   pattern: "Trial (Disc|Edition|Version|ver\\.)"
   search_tags: false
   group: "demos"
+  include_in_short_name: true
 
 # PRE-PRODUCTION
 alpha:
   pattern: "\\((?:\\w*?\\s)*Alpha(?:\\s\\d+)?\\)"
   group: "preproduction"
 
 beta:
@@ -115,14 +128,15 @@
   group: "preproduction"
 
 # PROMOTIONAL
 promo:
   pattern: "EPK|Press Kit|\\(Promo\\)"
   group: "promotional"
   search_tags: false
+  include_in_short_name: true
 
 # VERSIONS AND REVISIONS
 version_no:
   pattern: "\\(v[\\.0-9].*?\\)"
   type: "str"
   group: "version"
 
@@ -143,14 +157,15 @@
 aftermarket:
   pattern: "\\(Aftermarket\\)"
   group: "unlicensed"
 
 homebrew:
   pattern: "\\(Homebrew\\)"
   group: "unlicensed"
+  include_in_short_name: true
 
 pirate:
   pattern: "\\(Pirate\\)"
   group: "pirate"
 
 unl:
   pattern: "\\(Unl\\)"
@@ -187,14 +202,18 @@
 e_reader_edition:
   pattern: "\\(e-Reader Edition\\)"
 
 gentei:
   pattern: "\\((?:(?!\\(|Gentei.*?)[\\s\\S])*Gentei.*?\\)"
   group: "improved_version"
 
+gps_receiver_doukonban:
+  pattern: "\\(GPS Receiver Doukonban\\)"
+  group: "improved_version"
+
 ideatek:
   pattern: "\\(Idea-Tek\\)"
   group: "improved_version"
 
 infinity_plus:
   pattern: "\\(Infinity Plus\\)"
   group: "improved_version"
@@ -203,14 +222,18 @@
   pattern: "\\(Later\\)"
   group: "improved_version"
 
 mega_soft:
   pattern: "\\(Mega Soft\\)"
   group: "improved_version"
 
+microphone_doukoban:
+  pattern: "\\(Microphone Doukonban\\)"
+  group: "improved_version"
+
 nina_03:
   pattern: "\\(NINA-03\\)"
   group: "improved_version"
 
 nina_06:
   pattern: "\\(NINA-06\\)"
   group: "improved_version"
@@ -265,14 +288,18 @@
 
 # BUDGET EDITIONS
 
 artdink:
   pattern: "\\(Artdink Best Choice\\)"
   group: "budget_edition"
 
+best_collection:
+  pattern: "\\(Best Collection\\)"
+  group: "budget_edition"
+
 best_of_the_best:
   pattern: "\\(Best of the Best\\)"
   group: "budget_edition"
 
 best_hit_selection:
   pattern: "\\(Best Hit Selection\\)"
   group: "budget_edition"
@@ -289,14 +316,18 @@
   pattern: "\\(Cyclone's Best\\)"
   group: "budget_edition"
 
 digicube:
   pattern: "\\(DigiCube Best Selection\\)"
   group: "budget_edition"
 
+ea_best_hits:
+  pattern: "\\(EA Best Hits\\)"
+  group: "budget_edition"
+
 fukyuuban:
   pattern: "\\(Fukyuuban\\)"
   group: "budget_edition"
 
 fukyuuban_1500:
   pattern: "\\(Fukyuuban 1500\\)"
   group: "budget_edition"
@@ -332,14 +363,18 @@
   pattern: "\\(PlayStation the Best for Family\\)"
   group: "budget_edition"
 
 playstation_2_the_best:
   pattern: "\\(PlayStation 2 the Best\\)"
   group: "budget_edition"
 
+psp_the_best:
+  pattern: "\\(PSP The Best\\)"
+  group: "budget_edition"
+
 rockstar_classics:
   pattern: "\\(Rockstar Classics\\)"
   group: "budget_edition"
 
 spike_library:
   pattern: "\\(Spike Library\\)"
   group: "budget_edition"
@@ -626,7 +661,13 @@
 
 pal:
   pattern: "([?:-][\\s])?[(]?PAL(?: [a-zA-Z]+| 50[Hh]z)?(?:\\)?| (?=\\())"
   flags: "NOFLAG"
 
 43_406_pcb:
   pattern: "\\(43-406 PCB\\)"
+
+fw:
+  pattern: "\\(FW[0-9].*?\\)"
+
+u_numbers:
+  pattern: "\\(U[CLT][EJUS][BST]-\\d{5}\\)"
```

### Comparing `romsearch-0.0.3/romsearch/configs/sample_config.yml` & `romsearch-0.0.4/romsearch/configs/sample_config.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/romsearch/dev/parsing_tools.py` & `romsearch-0.0.4/romsearch/dev/parsing_tools.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/romsearch/modules/datparser.py` & `romsearch-0.0.4/romsearch/modules/datparser.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/romsearch/modules/dupeparser.py` & `romsearch-0.0.4/romsearch/modules/dupeparser.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/romsearch/modules/gamefinder.py` & `romsearch-0.0.4/romsearch/modules/gamefinder.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/romsearch/modules/romchooser.py` & `romsearch-0.0.4/romsearch/modules/romchooser.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,19 +242,20 @@
         if rom_dict[f][key] == "":
             rom_dict[f][key] = "v0"
 
     versions = np.array([version.parse(rom_dict[f][key]) for f in files])
     versions_clean = [key for key, value in Counter(versions).most_common()]
     version_vals = sorted(range(len(versions_clean)), key=versions.__getitem__)
 
+    versions_sorted = versions[version_vals]
+
     file_scores_version = np.zeros(len(files))
-    for v_idx, v in enumerate(versions_clean):
-        for f_idx, f in enumerate(files):
-            if version.parse(rom_dict[f][key]) == v:
-                file_scores_version[f_idx] += version_vals[v_idx]
+    for i, v in enumerate(versions_sorted):
+        v_idx = np.where(versions == v)[0]
+        file_scores_version[v_idx] += i
 
     return file_scores_version
 
 
 def filter_by_list(rom_dict,
                    key,
                    key_prefs,
```

### Comparing `romsearch-0.0.3/romsearch/modules/romdownloader.py` & `romsearch-0.0.4/romsearch/modules/romdownloader.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/romsearch/modules/rommover.py` & `romsearch-0.0.4/romsearch/modules/rommover.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/romsearch/modules/romparser.py` & `romsearch-0.0.4/romsearch/modules/romparser.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/romsearch/modules/romsearch.py` & `romsearch-0.0.4/romsearch/modules/romsearch.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/romsearch/util/__init__.py` & `romsearch-0.0.4/romsearch/util/__init__.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/romsearch/util/general.py` & `romsearch-0.0.4/romsearch/util/general.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/romsearch/util/io.py` & `romsearch-0.0.4/romsearch/util/io.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/romsearch/util/logger.py` & `romsearch-0.0.4/romsearch/util/logger.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.3/romsearch/util/regex_matching.py` & `romsearch-0.0.4/romsearch/util/regex_matching.py`

 * *Files 11% similar despite different names*

```diff
@@ -65,14 +65,20 @@
         default_config = load_yml(default_file)
 
     if regex_config is None:
         regex_file = os.path.join(mod_dir, "configs", "regex.yml")
         regex_config = load_yml(regex_file)
 
     for regex_key in regex_config:
+
+        # If we have patterns that we do want to keep in the long name, then skip
+        include_in_short_title = regex_config[regex_key].get("include_in_short_name", False)
+        if include_in_short_title:
+            continue
+
         regex_type = regex_config[regex_key].get("type", "bool")
         regex_flags = regex_config[regex_key].get("flags", "I")
 
         pattern = regex_config[regex_key]["pattern"]
 
         if regex_type == "list":
```

### Comparing `romsearch-0.0.3/romsearch.egg-info/PKG-INFO` & `romsearch-0.0.4/romsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romsearch
-Version: 0.0.3
+Version: 0.0.4
 Summary: One Stop ROM Shop
 Author: bbtufty
 Maintainer: bbtufty
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -730,10 +730,11 @@
 works for the following consoles:
 
 * Nintendo - GameCube
 * Nintendo - Nintendo Entertainment System
 * Nintendo - Super Nintendo Entertainment System
 * Sony - PlayStation
 * Sony - PlayStation 2
+* Sony - PlayStation Portable
 
 but be aware there may be quirks that will only become apparent over time. We encourage users to open
 [issues](https://github.com/bbtufty/romsearch/issues) as and where they find them.
```

### Comparing `romsearch-0.0.3/romsearch.egg-info/SOURCES.txt` & `romsearch-0.0.4/romsearch.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 romsearch/configs/clonelists/retool.yml
 romsearch/configs/dats/no-intro.yml
 romsearch/configs/dats/redump.yml
 romsearch/configs/platforms/Nintendo - GameCube.yml
 romsearch/configs/platforms/Nintendo - Nintendo Entertainment System.yml
 romsearch/configs/platforms/Nintendo - Super Nintendo Entertainment System.yml
 romsearch/configs/platforms/Sony - PlayStation 2.yml
+romsearch/configs/platforms/Sony - PlayStation Portable.yml
 romsearch/configs/platforms/Sony - PlayStation.yml
 romsearch/dev/__init__.py
 romsearch/dev/parsing_tools.py
 romsearch/modules/__init__.py
 romsearch/modules/datparser.py
 romsearch/modules/dupeparser.py
 romsearch/modules/gamefinder.py
```

