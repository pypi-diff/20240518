# Comparing `tmp/vertagus-0.1.0b3.tar.gz` & `tmp/vertagus-0.1.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertagus-0.1.0b3.tar", last modified: Thu May  9 15:10:54 2024, max compression
+gzip compressed data, was "vertagus-0.1.0b4.tar", last modified: Fri May 17 22:17:01 2024, max compression
```

## Comparing `vertagus-0.1.0b3.tar` & `vertagus-0.1.0b4.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:54.422621 vertagus-0.1.0b3/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1054 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-09 15:10:54.422621 vertagus-0.1.0b3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     3791 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1100 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 15:10:54.422621 vertagus-0.1.0b3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:54.410621 vertagus-0.1.0b3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:54.414621 vertagus-0.1.0b3/src/vertagus/
--rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:54.414621 vertagus-0.1.0b3/src/vertagus/aliases/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/aliases/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1151 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/aliases/library.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      747 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/aliases/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:54.414621 vertagus-0.1.0b3/src/vertagus/cli/
--rwxr-xr-x   0 runner    (1001) docker     (127)       21 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:54.418621 vertagus-0.1.0b3/src/vertagus/cli/commands/
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/cli/commands/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1188 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/cli/commands/create_tag.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1069 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/cli/commands/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:54.418621 vertagus-0.1.0b3/src/vertagus/configuration/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/configuration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      682 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/configuration/load.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4500 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/configuration/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:54.418621 vertagus-0.1.0b3/src/vertagus/core/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/core/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      512 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/core/manifest_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      770 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/core/package_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5961 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/core/project.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      665 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/core/rule_bases.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      648 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/core/scm_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1586 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/core/stage.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/core/tag_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2981 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:54.418621 vertagus-0.1.0b3/src/vertagus/providers/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:54.418621 vertagus-0.1.0b3/src/vertagus/providers/manifest/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/providers/manifest/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      552 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/providers/manifest/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:54.418621 vertagus-0.1.0b3/src/vertagus/providers/manifest/setuptools_/
--rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/providers/manifest/setuptools_/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      830 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/providers/manifest/setuptools_/pyproject_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:54.418621 vertagus-0.1.0b3/src/vertagus/providers/scm/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/providers/scm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:54.418621 vertagus-0.1.0b3/src/vertagus/providers/scm/git_/
--rwxr-xr-x   0 runner    (1001) docker     (127)       27 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/providers/scm/git_/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4296 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/providers/scm/git_/git_scm.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      405 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/providers/scm/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:54.422621 vertagus-0.1.0b3/src/vertagus/rules/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:54.422621 vertagus-0.1.0b3/src/vertagus/rules/comparison/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/rules/comparison/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      908 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/rules/comparison/library.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      732 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/rules/comparison/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:54.422621 vertagus-0.1.0b3/src/vertagus/rules/single_version/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/rules/single_version/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1564 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/rules/single_version/library.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      729 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/rules/single_version/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:54.422621 vertagus-0.1.0b3/src/vertagus/utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      588 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/utils/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/utils/factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      533 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/src/vertagus/utils/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:54.422621 vertagus-0.1.0b3/src/vertagus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-09 15:10:54.000000 vertagus-0.1.0b3/src/vertagus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-09 15:10:54.000000 vertagus-0.1.0b3/src/vertagus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 15:10:54.000000 vertagus-0.1.0b3/src/vertagus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-09 15:10:54.000000 vertagus-0.1.0b3/src/vertagus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-09 15:10:54.000000 vertagus-0.1.0b3/src/vertagus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 15:10:54.000000 vertagus-0.1.0b3/src/vertagus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:10:54.422621 vertagus-0.1.0b3/test/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2734 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/test/test_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1733 2024-05-09 15:10:50.000000 vertagus-0.1.0b3/test/test_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:17:01.026732 vertagus-0.1.0b4/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1054 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-17 22:17:01.026732 vertagus-0.1.0b4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3791 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1100 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 22:17:01.026732 vertagus-0.1.0b4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:17:01.014732 vertagus-0.1.0b4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:17:01.018732 vertagus-0.1.0b4/src/vertagus/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:17:01.018732 vertagus-0.1.0b4/src/vertagus/aliases/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/aliases/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1151 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/aliases/library.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      747 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/aliases/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:17:01.018732 vertagus-0.1.0b4/src/vertagus/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       21 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:17:01.018732 vertagus-0.1.0b4/src/vertagus/cli/commands/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/cli/commands/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1188 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/cli/commands/create_tag.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1069 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/cli/commands/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:17:01.018732 vertagus-0.1.0b4/src/vertagus/configuration/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/configuration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      682 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/configuration/load.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4485 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/configuration/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:17:01.022732 vertagus-0.1.0b4/src/vertagus/core/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/core/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      512 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/core/manifest_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      770 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/core/package_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5961 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/core/project.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      665 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/core/rule_bases.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      648 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/core/scm_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1586 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/core/stage.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/core/tag_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2981 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:17:01.022732 vertagus-0.1.0b4/src/vertagus/providers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:17:01.022732 vertagus-0.1.0b4/src/vertagus/providers/manifest/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/providers/manifest/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      552 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/providers/manifest/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:17:01.022732 vertagus-0.1.0b4/src/vertagus/providers/manifest/setuptools_/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/providers/manifest/setuptools_/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      830 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/providers/manifest/setuptools_/pyproject_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:17:01.022732 vertagus-0.1.0b4/src/vertagus/providers/scm/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/providers/scm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:17:01.022732 vertagus-0.1.0b4/src/vertagus/providers/scm/git_/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       27 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/providers/scm/git_/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4343 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/providers/scm/git_/git_scm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      405 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/providers/scm/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:17:01.022732 vertagus-0.1.0b4/src/vertagus/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:17:01.022732 vertagus-0.1.0b4/src/vertagus/rules/comparison/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/rules/comparison/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      908 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/rules/comparison/library.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      732 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/rules/comparison/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:17:01.022732 vertagus-0.1.0b4/src/vertagus/rules/single_version/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/rules/single_version/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1564 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/rules/single_version/library.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      729 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/rules/single_version/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:17:01.022732 vertagus-0.1.0b4/src/vertagus/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      588 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/utils/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/utils/factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      533 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/src/vertagus/utils/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:17:01.026732 vertagus-0.1.0b4/src/vertagus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-17 22:17:01.000000 vertagus-0.1.0b4/src/vertagus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-17 22:17:01.000000 vertagus-0.1.0b4/src/vertagus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:17:01.000000 vertagus-0.1.0b4/src/vertagus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-17 22:17:01.000000 vertagus-0.1.0b4/src/vertagus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-17 22:17:01.000000 vertagus-0.1.0b4/src/vertagus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 22:17:01.000000 vertagus-0.1.0b4/src/vertagus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:17:01.026732 vertagus-0.1.0b4/test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3650 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/test/test_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1733 2024-05-17 22:16:50.000000 vertagus-0.1.0b4/test/test_operations.py
```

### Comparing `vertagus-0.1.0b3/LICENSE` & `vertagus-0.1.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/PKG-INFO` & `vertagus-0.1.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertagus
-Version: 0.1.0b3
+Version: 0.1.0b4
 Summary: A tool to assist the maintenance of package versioning with scm tags
 Author-email: John Raines <johndanielraines@gmail.com>
 License: Copyright (c) 2024 John Raines
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `vertagus-0.1.0b3/README.md` & `vertagus-0.1.0b4/README.md`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/pyproject.toml` & `vertagus-0.1.0b4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vertagus"
-version = "0.1.0b3"
+version = "0.1.0b4"
 description = "A tool to assist the maintenance of package versioning with scm tags"
 readme = "README.md"
 authors = [
     {"name" = "John Raines", "email" = "johndanielraines@gmail.com"}
 ]
 dependencies = [
     "click",
```

### Comparing `vertagus-0.1.0b3/src/vertagus/aliases/library.py` & `vertagus-0.1.0b4/src/vertagus/aliases/library.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus/aliases/loader.py` & `vertagus-0.1.0b4/src/vertagus/aliases/loader.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus/cli/commands/create_tag.py` & `vertagus-0.1.0b4/src/vertagus/cli/commands/create_tag.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus/cli/commands/validate.py` & `vertagus-0.1.0b4/src/vertagus/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus/configuration/load.py` & `vertagus-0.1.0b4/src/vertagus/configuration/load.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus/configuration/types.py` & `vertagus-0.1.0b4/src/vertagus/configuration/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         )
 
 
 class ScmData:
     
     def __init__(self, type: str, root: str = None, **kwargs):
         self.scm_type = type
-        self.root = root or os.getcwd()
+        self.root = root
         self.kwargs = kwargs
 
     def config(self):
         return dict(
             root=self.root,
             **self.kwargs
         )
```

### Comparing `vertagus-0.1.0b3/src/vertagus/core/manifest_base.py` & `vertagus-0.1.0b4/src/vertagus/core/manifest_base.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus/core/package_base.py` & `vertagus-0.1.0b4/src/vertagus/core/package_base.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus/core/project.py` & `vertagus-0.1.0b4/src/vertagus/core/project.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus/core/rule_bases.py` & `vertagus-0.1.0b4/src/vertagus/core/rule_bases.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus/core/scm_base.py` & `vertagus-0.1.0b4/src/vertagus/core/scm_base.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus/core/stage.py` & `vertagus-0.1.0b4/src/vertagus/core/stage.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus/factory.py` & `vertagus-0.1.0b4/src/vertagus/factory.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus/operations.py` & `vertagus-0.1.0b4/src/vertagus/operations.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus/providers/manifest/registry.py` & `vertagus-0.1.0b4/src/vertagus/providers/manifest/registry.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus/providers/manifest/setuptools_/pyproject_manifest.py` & `vertagus-0.1.0b4/src/vertagus/providers/manifest/setuptools_/pyproject_manifest.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus/providers/scm/git_/git_scm.py` & `vertagus-0.1.0b4/src/vertagus/providers/scm/git_/git_scm.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 class GitScm(ScmBase):
 
     scm_type = "git"
     _default_user_data = {
         "name": "vertagus",
-        "email": "vertagus@example.com"
+        "email": "vertagus@none"
     }
     _default_remote_name = "origin"
 
     def __init__(self,
                  root: str = None,
                  tag_prefix: str = None,
                  user_data: dict = None,
@@ -109,15 +109,16 @@
         valid_versions = []
         for version in versions:
             try:
                 parse_version(version)
                 valid_versions.append(version)
             except InvalidVersion:
                 logger.warning(f"Invalid version found: {version}")
-
+        if not valid_versions:
+            return None
         return max(valid_versions, key=lambda v: parse_version(v))
     
     def _initialize_repo(self):
         repo = git.Repo(self.root)
         logger.info(
             f"Initializing git repository at {self.root} "
             f"with user data {self.user_data}."
```

### Comparing `vertagus-0.1.0b3/src/vertagus/rules/comparison/library.py` & `vertagus-0.1.0b4/src/vertagus/rules/comparison/library.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus/rules/comparison/loader.py` & `vertagus-0.1.0b4/src/vertagus/rules/comparison/loader.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus/rules/single_version/library.py` & `vertagus-0.1.0b4/src/vertagus/rules/single_version/library.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus/rules/single_version/loader.py` & `vertagus-0.1.0b4/src/vertagus/rules/single_version/loader.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus/utils/config.py` & `vertagus-0.1.0b4/src/vertagus/utils/config.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus/utils/regex.py` & `vertagus-0.1.0b4/src/vertagus/utils/regex.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/src/vertagus.egg-info/PKG-INFO` & `vertagus-0.1.0b4/src/vertagus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertagus
-Version: 0.1.0b3
+Version: 0.1.0b4
 Summary: A tool to assist the maintenance of package versioning with scm tags
 Author-email: John Raines <johndanielraines@gmail.com>
 License: Copyright (c) 2024 John Raines
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `vertagus-0.1.0b3/src/vertagus.egg-info/SOURCES.txt` & `vertagus-0.1.0b4/src/vertagus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b3/test/test_factory.py` & `vertagus-0.1.0b4/test/test_factory.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from unittest.mock import MagicMock
 import pytest
+import os
 from vertagus import factory
 from vertagus.core.rule_bases import SingleVersionRule
 from vertagus.configuration import types as t
+from vertagus.core.scm_base import ScmBase
 
 
 class DummyManifest:
     def __init__(self, **kwargs):
         pass
 
 
@@ -50,22 +52,52 @@
         assert isinstance(item, SingleVersionRule)
 
 
 @pytest.fixture
 def mock_scm_data():
     return t.ScmData(root="root", type="dummy_type", **{"key": "value"})
 
-
-def test_create_scm(mock_scm_data, monkeypatch):
-    mock = MagicMock()
-    monkeypatch.setattr(factory, "get_scm_cls", MagicMock(return_value=mock))
-    result = factory.create_scm(mock_scm_data)
+@pytest.fixture
+def mock_scm_cls():
+    class MockScm(ScmBase):
+        def __init__(self,
+                    root: str = None,
+                    tag_prefix: str = None,
+                    user_data: dict = None,
+                    remote_name: str = None,
+                    **kwargs
+                    ):
+            self.root = root or os.getcwd()
+            self.tag_prefix = tag_prefix
+            self.user_data = user_data 
+            self.remote_name = remote_name
+
+        def create_tag(self, tag, ref: str=None):
+            pass
+        
+        def delete_tag(self, tag_name: str):
+            pass
+        
+        def list_tags(self, prefix: str=None):
+            return ["tag1", "tag2", "tag3"]
+
+        def get_highest_version(self, prefix: str=None):
+            pass
+
+        def migrate_alias(self, alias: str, ref: str = None):
+            pass
+
+    return MockScm
+
+def test_create_scm(mock_scm_data, mock_scm_cls, monkeypatch):
+    monkeypatch.setattr(factory, "get_scm_cls", MagicMock(return_value=mock_scm_cls))
+    scm = factory.create_scm(mock_scm_data)
     factory.get_scm_cls.assert_called_with("dummy_type")
-    mock.assert_called_with(root="root", key="value")
-    assert result == mock.return_value
+    assert scm.root == "root"
+    assert scm.tag_prefix is None
 
 
 @pytest.fixture
 def project_data():
     return t.ProjectData(
         manifests=[t.ManifestData(name="test_manifest", type="dummy_type", path="test_path", loc=["1", "2"])],
         rules=t.RulesData(current=["rule1", "rule2"], increment=["rule3"]),
```

### Comparing `vertagus-0.1.0b3/test/test_operations.py` & `vertagus-0.1.0b4/test/test_operations.py`

 * *Files identical despite different names*

