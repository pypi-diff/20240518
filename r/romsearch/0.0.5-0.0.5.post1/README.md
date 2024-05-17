# Comparing `tmp/romsearch-0.0.5.tar.gz` & `tmp/romsearch-0.0.5.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "romsearch-0.0.5.tar", last modified: Fri May 17 22:56:01 2024, max compression
+gzip compressed data, was "romsearch-0.0.5.post1.tar", last modified: Fri May 17 23:04:40 2024, max compression
```

## Comparing `romsearch-0.0.5.tar` & `romsearch-0.0.5.post1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.878658 romsearch-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.858657 romsearch-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.862658 romsearch-0.0.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-17 22:55:57.000000 romsearch-0.0.5/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-17 22:55:57.000000 romsearch-0.0.5/.github/ISSUE_TEMPLATE/console_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-17 22:55:57.000000 romsearch-0.0.5/.github/ISSUE_TEMPLATE/feature_request.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.862658 romsearch-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-17 22:55:57.000000 romsearch-0.0.5/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-17 22:55:57.000000 romsearch-0.0.5/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-17 22:55:57.000000 romsearch-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-17 22:55:57.000000 romsearch-0.0.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-17 22:55:57.000000 romsearch-0.0.5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-17 22:55:57.000000 romsearch-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-17 22:55:57.000000 romsearch-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    43911 2024-05-17 22:56:01.878658 romsearch-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-17 22:55:57.000000 romsearch-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.866658 romsearch-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/1g1r.rst
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.866658 romsearch-0.0.5/docs/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/configs/clonelists.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/configs/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/configs/dats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/configs/defaults.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/configs/platforms.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/configs/regex.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/configs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/configuration.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.866658 romsearch-0.0.5/docs/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/gui/config_includes_excludes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/gui/config_main.rst
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/gui/config_modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/gui/config_platforms.rst
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/gui/config_regions_languages.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/gui/intro.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.866658 romsearch-0.0.5/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    24254 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/images/config_includes_excludes.png
--rw-r--r--   0 runner    (1001) docker     (127)    71922 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/images/config_main.png
--rw-r--r--   0 runner    (1001) docker     (127)    24790 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/images/config_modules.png
--rw-r--r--   0 runner    (1001) docker     (127)    39895 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/images/config_platforms.png
--rw-r--r--   0 runner    (1001) docker     (127)    73902 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/images/config_regions_languages.png
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/known_issues.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.870658 romsearch-0.0.5/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/modules/datparser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/modules/dupeparser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/modules/gamefinder.rst
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/modules/romchooser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/modules/romdownloader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/modules/rommover.rst
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/modules/romparser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/modules/romsearch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/reference_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-17 22:55:57.000000 romsearch-0.0.5/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-17 22:55:57.000000 romsearch-0.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.870658 romsearch-0.0.5/romsearch/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.870658 romsearch-0.0.5/romsearch/configs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.870658 romsearch-0.0.5/romsearch/configs/clonelists/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/clonelists/retool.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.870658 romsearch-0.0.5/romsearch/configs/dats/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/dats/no-intro.yml
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/dats/redump.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/defaults.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.874658 romsearch-0.0.5/romsearch/configs/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/platforms/Nintendo - GameCube.yml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/platforms/Nintendo - Nintendo Entertainment System.yml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/platforms/Nintendo - Super Nintendo Entertainment System.yml
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/platforms/Sony - PlayStation 2.yml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/platforms/Sony - PlayStation Portable.yml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/platforms/Sony - PlayStation.yml
--rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/regex.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/configs/sample_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.874658 romsearch-0.0.5/romsearch/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/dev/parsing_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.874658 romsearch-0.0.5/romsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/gui/gui_about.py
--rw-r--r--   0 runner    (1001) docker     (127)    27172 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/gui/gui_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/gui/gui_romsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/gui/gui_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/gui/layout_about.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/gui/layout_about.ui
--rw-r--r--   0 runner    (1001) docker     (127)    96327 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/gui/layout_romsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)    89017 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/gui/layout_romsearch.ui
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.878658 romsearch-0.0.5/romsearch/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/modules/datparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/modules/dupeparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/modules/gamefinder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16739 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/modules/romchooser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/modules/romdownloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/modules/rommover.py
--rw-r--r--   0 runner    (1001) docker     (127)    13987 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/modules/romparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    14022 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/modules/romsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.878658 romsearch-0.0.5/romsearch/util/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/util/discord.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/util/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/util/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch/util/regex_matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:56:01.878658 romsearch-0.0.5/romsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43911 2024-05-17 22:56:01.000000 romsearch-0.0.5/romsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-17 22:56:01.000000 romsearch-0.0.5/romsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:56:01.000000 romsearch-0.0.5/romsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-17 22:56:01.000000 romsearch-0.0.5/romsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 22:56:01.000000 romsearch-0.0.5/romsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-17 22:55:57.000000 romsearch-0.0.5/romsearch_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 22:56:01.878658 romsearch-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:04:40.021813 romsearch-0.0.5.post1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:04:40.001814 romsearch-0.0.5.post1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:04:40.005813 romsearch-0.0.5.post1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/.github/ISSUE_TEMPLATE/console_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/.github/ISSUE_TEMPLATE/feature_request.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:04:40.005813 romsearch-0.0.5.post1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    43912 2024-05-17 23:04:40.021813 romsearch-0.0.5.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:04:40.009813 romsearch-0.0.5.post1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/1g1r.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:04:40.009813 romsearch-0.0.5.post1/docs/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/configs/clonelists.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/configs/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/configs/dats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/configs/defaults.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/configs/platforms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/configs/regex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/configuration.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:04:40.009813 romsearch-0.0.5.post1/docs/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/gui/config_includes_excludes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/gui/config_main.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/gui/config_modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/gui/config_platforms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/gui/config_regions_languages.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/gui/intro.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:04:40.013813 romsearch-0.0.5.post1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    24254 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/images/config_includes_excludes.png
+-rw-r--r--   0 runner    (1001) docker     (127)    71922 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/images/config_main.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24790 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/images/config_modules.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39895 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/images/config_platforms.png
+-rw-r--r--   0 runner    (1001) docker     (127)    73902 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/images/config_regions_languages.png
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/known_issues.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:04:40.013813 romsearch-0.0.5.post1/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/modules/datparser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/modules/dupeparser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/modules/gamefinder.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/modules/romchooser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/modules/romdownloader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/modules/rommover.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/modules/romparser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/modules/romsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/reference_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:04:40.013813 romsearch-0.0.5.post1/romsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:04:40.013813 romsearch-0.0.5.post1/romsearch/configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:04:40.013813 romsearch-0.0.5.post1/romsearch/configs/clonelists/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/configs/clonelists/retool.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:04:40.013813 romsearch-0.0.5.post1/romsearch/configs/dats/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/configs/dats/no-intro.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/configs/dats/redump.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/configs/defaults.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:04:40.017814 romsearch-0.0.5.post1/romsearch/configs/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/configs/platforms/Nintendo - GameCube.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/configs/platforms/Nintendo - Nintendo Entertainment System.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/configs/platforms/Nintendo - Super Nintendo Entertainment System.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/configs/platforms/Sony - PlayStation 2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/configs/platforms/Sony - PlayStation Portable.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/configs/platforms/Sony - PlayStation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/configs/regex.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/configs/sample_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:04:40.017814 romsearch-0.0.5.post1/romsearch/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/dev/parsing_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:04:40.017814 romsearch-0.0.5.post1/romsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/gui/gui_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27172 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/gui/gui_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/gui/gui_romsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/gui/gui_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/gui/layout_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/gui/layout_about.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    96327 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/gui/layout_romsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89017 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/gui/layout_romsearch.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:04:40.017814 romsearch-0.0.5.post1/romsearch/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/modules/datparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/modules/dupeparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/modules/gamefinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16739 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/modules/romchooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/modules/romdownloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/modules/rommover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13987 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/modules/romparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14022 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/modules/romsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:04:40.021813 romsearch-0.0.5.post1/romsearch/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/util/discord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/util/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/util/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch/util/regex_matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:04:40.021813 romsearch-0.0.5.post1/romsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43912 2024-05-17 23:04:39.000000 romsearch-0.0.5.post1/romsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-17 23:04:40.000000 romsearch-0.0.5.post1/romsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 23:04:39.000000 romsearch-0.0.5.post1/romsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-17 23:04:39.000000 romsearch-0.0.5.post1/romsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 23:04:39.000000 romsearch-0.0.5.post1/romsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-17 23:04:36.000000 romsearch-0.0.5.post1/romsearch_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 23:04:40.021813 romsearch-0.0.5.post1/setup.cfg
```

### Comparing `romsearch-0.0.5/.github/ISSUE_TEMPLATE/bug_report.yml` & `romsearch-0.0.5.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/.github/ISSUE_TEMPLATE/feature_request.yml` & `romsearch-0.0.5.post1/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/.github/workflows/build.yaml` & `romsearch-0.0.5.post1/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/.github/workflows/publish.yaml` & `romsearch-0.0.5.post1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/.gitignore` & `romsearch-0.0.5.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/.readthedocs.yaml` & `romsearch-0.0.5.post1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/CHANGES.rst` & `romsearch-0.0.5.post1/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/LICENSE` & `romsearch-0.0.5.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/PKG-INFO` & `romsearch-0.0.5.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romsearch
-Version: 0.0.5
+Version: 0.0.5.post1
 Summary: One Stop ROM Shop
 Author: bbtufty
 Maintainer: bbtufty
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -707,15 +707,15 @@
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 
 # ROMSearch
 
 [![](https://img.shields.io/pypi/v/romsearch.svg?label=PyPI&style=flat-square)](https://pypi.org/pypi/romsearch/)
 [![](https://img.shields.io/pypi/pyversions/romsearch.svg?label=Python&color=yellow&style=flat-square)](https://pypi.org/pypi/romsearch/)
 [![Docs](https://readthedocs.org/projects/romsearch/badge/?version=latest&style=flat-square)](https://romsearch.readthedocs.io/en/latest/)
-[![Actions](https://img.shields.io/github/actions/workflow/status/bbtufty/romsearch/build_test.yaml?branch=main&style=flat-square)](https://github.com/bbtufty/romsearch/actions)
+[![Actions](https://img.shields.io/github/actions/workflow/status/bbtufty/romsearch/build.yaml?branch=main&style=flat-square)](https://github.com/bbtufty/romsearch/actions)
 [![License](https://img.shields.io/badge/license-GNUv3-blue.svg?label=License&style=flat-square)](LICENSE)
 
 ROMSearch is designed as a simple-to-inferface with tool that will allow you to pull ROM files from some remote (or
 local) location, figure out the best ROM, and move it cleanly to a folder that can imported into an emulator. ROMSearch
 is supposed to be a one-shot program to get you from files online to playing games (which is what we want, right?).
 
 ROMSearch also has a GUI! Currently only for Windows, but makes setting up configurations simple and clean.
```

### Comparing `romsearch-0.0.5/README.md` & `romsearch-0.0.5.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ROMSearch
 
 [![](https://img.shields.io/pypi/v/romsearch.svg?label=PyPI&style=flat-square)](https://pypi.org/pypi/romsearch/)
 [![](https://img.shields.io/pypi/pyversions/romsearch.svg?label=Python&color=yellow&style=flat-square)](https://pypi.org/pypi/romsearch/)
 [![Docs](https://readthedocs.org/projects/romsearch/badge/?version=latest&style=flat-square)](https://romsearch.readthedocs.io/en/latest/)
-[![Actions](https://img.shields.io/github/actions/workflow/status/bbtufty/romsearch/build_test.yaml?branch=main&style=flat-square)](https://github.com/bbtufty/romsearch/actions)
+[![Actions](https://img.shields.io/github/actions/workflow/status/bbtufty/romsearch/build.yaml?branch=main&style=flat-square)](https://github.com/bbtufty/romsearch/actions)
 [![License](https://img.shields.io/badge/license-GNUv3-blue.svg?label=License&style=flat-square)](LICENSE)
 
 ROMSearch is designed as a simple-to-inferface with tool that will allow you to pull ROM files from some remote (or
 local) location, figure out the best ROM, and move it cleanly to a folder that can imported into an emulator. ROMSearch
 is supposed to be a one-shot program to get you from files online to playing games (which is what we want, right?).
 
 ROMSearch also has a GUI! Currently only for Windows, but makes setting up configurations simple and clean.
```

### Comparing `romsearch-0.0.5/docs/1g1r.rst` & `romsearch-0.0.5.post1/docs/1g1r.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/docs/Makefile` & `romsearch-0.0.5.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/docs/conf.py` & `romsearch-0.0.5.post1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'romsearch'
 copyright = '2024, bbtufty'
 author = 'bbtufty'
-release = '0.0.5'
+release = '0.0.5.post1'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc',
               'sphinx.ext.coverage',
               'sphinx.ext.napoleon',
```

### Comparing `romsearch-0.0.5/docs/configs/config.rst` & `romsearch-0.0.5.post1/docs/configs/config.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/docs/configs/dats.rst` & `romsearch-0.0.5.post1/docs/configs/dats.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/docs/configs/platforms.rst` & `romsearch-0.0.5.post1/docs/configs/platforms.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/docs/configs/regex.rst` & `romsearch-0.0.5.post1/docs/configs/regex.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/docs/configuration.rst` & `romsearch-0.0.5.post1/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/docs/gui/intro.rst` & `romsearch-0.0.5.post1/docs/gui/intro.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/docs/images/config_includes_excludes.png` & `romsearch-0.0.5.post1/docs/images/config_includes_excludes.png`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/docs/images/config_main.png` & `romsearch-0.0.5.post1/docs/images/config_main.png`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/docs/images/config_modules.png` & `romsearch-0.0.5.post1/docs/images/config_modules.png`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/docs/images/config_platforms.png` & `romsearch-0.0.5.post1/docs/images/config_platforms.png`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/docs/images/config_regions_languages.png` & `romsearch-0.0.5.post1/docs/images/config_regions_languages.png`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/docs/index.rst` & `romsearch-0.0.5.post1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/docs/intro.rst` & `romsearch-0.0.5.post1/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/docs/known_issues.rst` & `romsearch-0.0.5.post1/docs/known_issues.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/docs/make.bat` & `romsearch-0.0.5.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/docs/modules/datparser.rst` & `romsearch-0.0.5.post1/docs/modules/datparser.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/docs/modules/dupeparser.rst` & `romsearch-0.0.5.post1/docs/modules/dupeparser.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/docs/modules/romdownloader.rst` & `romsearch-0.0.5.post1/docs/modules/romdownloader.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/docs/modules/romsearch.rst` & `romsearch-0.0.5.post1/docs/modules/romsearch.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/pyproject.toml` & `romsearch-0.0.5.post1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "romsearch"
-version = "0.0.5"
+version = "0.0.5.post1"
 description = "One Stop ROM Shop"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 
 authors = [
     {name = "bbtufty"},
```

### Comparing `romsearch-0.0.5/romsearch/__init__.py` & `romsearch-0.0.5.post1/romsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/configs/clonelists/retool.yml` & `romsearch-0.0.5.post1/romsearch/configs/clonelists/retool.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/configs/defaults.yml` & `romsearch-0.0.5.post1/romsearch/configs/defaults.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/configs/regex.yml` & `romsearch-0.0.5.post1/romsearch/configs/regex.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/configs/sample_config.yml` & `romsearch-0.0.5.post1/romsearch/configs/sample_config.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/dev/parsing_tools.py` & `romsearch-0.0.5.post1/romsearch/dev/parsing_tools.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/gui/gui_config.py` & `romsearch-0.0.5.post1/romsearch/gui/gui_config.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/gui/gui_romsearch.py` & `romsearch-0.0.5.post1/romsearch/gui/gui_romsearch.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/gui/gui_utils.py` & `romsearch-0.0.5.post1/romsearch/gui/gui_utils.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/gui/layout_about.py` & `romsearch-0.0.5.post1/romsearch/gui/layout_about.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/gui/layout_about.ui` & `romsearch-0.0.5.post1/romsearch/gui/layout_about.ui`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/gui/layout_romsearch.py` & `romsearch-0.0.5.post1/romsearch/gui/layout_romsearch.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/gui/layout_romsearch.ui` & `romsearch-0.0.5.post1/romsearch/gui/layout_romsearch.ui`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/modules/datparser.py` & `romsearch-0.0.5.post1/romsearch/modules/datparser.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/modules/dupeparser.py` & `romsearch-0.0.5.post1/romsearch/modules/dupeparser.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/modules/gamefinder.py` & `romsearch-0.0.5.post1/romsearch/modules/gamefinder.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/modules/romchooser.py` & `romsearch-0.0.5.post1/romsearch/modules/romchooser.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/modules/romdownloader.py` & `romsearch-0.0.5.post1/romsearch/modules/romdownloader.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/modules/rommover.py` & `romsearch-0.0.5.post1/romsearch/modules/rommover.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/modules/romparser.py` & `romsearch-0.0.5.post1/romsearch/modules/romparser.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/modules/romsearch.py` & `romsearch-0.0.5.post1/romsearch/modules/romsearch.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/util/__init__.py` & `romsearch-0.0.5.post1/romsearch/util/__init__.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/util/general.py` & `romsearch-0.0.5.post1/romsearch/util/general.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/util/io.py` & `romsearch-0.0.5.post1/romsearch/util/io.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/util/logger.py` & `romsearch-0.0.5.post1/romsearch/util/logger.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch/util/regex_matching.py` & `romsearch-0.0.5.post1/romsearch/util/regex_matching.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.5/romsearch.egg-info/PKG-INFO` & `romsearch-0.0.5.post1/romsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romsearch
-Version: 0.0.5
+Version: 0.0.5.post1
 Summary: One Stop ROM Shop
 Author: bbtufty
 Maintainer: bbtufty
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -707,15 +707,15 @@
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 
 # ROMSearch
 
 [![](https://img.shields.io/pypi/v/romsearch.svg?label=PyPI&style=flat-square)](https://pypi.org/pypi/romsearch/)
 [![](https://img.shields.io/pypi/pyversions/romsearch.svg?label=Python&color=yellow&style=flat-square)](https://pypi.org/pypi/romsearch/)
 [![Docs](https://readthedocs.org/projects/romsearch/badge/?version=latest&style=flat-square)](https://romsearch.readthedocs.io/en/latest/)
-[![Actions](https://img.shields.io/github/actions/workflow/status/bbtufty/romsearch/build_test.yaml?branch=main&style=flat-square)](https://github.com/bbtufty/romsearch/actions)
+[![Actions](https://img.shields.io/github/actions/workflow/status/bbtufty/romsearch/build.yaml?branch=main&style=flat-square)](https://github.com/bbtufty/romsearch/actions)
 [![License](https://img.shields.io/badge/license-GNUv3-blue.svg?label=License&style=flat-square)](LICENSE)
 
 ROMSearch is designed as a simple-to-inferface with tool that will allow you to pull ROM files from some remote (or
 local) location, figure out the best ROM, and move it cleanly to a folder that can imported into an emulator. ROMSearch
 is supposed to be a one-shot program to get you from files online to playing games (which is what we want, right?).
 
 ROMSearch also has a GUI! Currently only for Windows, but makes setting up configurations simple and clean.
```

### Comparing `romsearch-0.0.5/romsearch.egg-info/SOURCES.txt` & `romsearch-0.0.5.post1/romsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

