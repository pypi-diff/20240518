# Comparing `tmp/nexus3-cli-4.1.8.tar.gz` & `tmp/nexus3-cli-4.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus3-cli-4.1.8.tar", last modified: Fri Jun 10 06:15:29 2022, max compression
+gzip compressed data, was "nexus3-cli-4.1.9.tar", last modified: Wed Sep 13 21:05:32 2023, max compression
```

## Comparing `nexus3-cli-4.1.8.tar` & `nexus3-cli-4.1.9.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 06:15:29.107756 nexus3-cli-4.1.8/
--rw-rw-rw-   0 root         (0) root         (0)     1073 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      112 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6867 2022-06-10 06:15:29.107756 nexus3-cli-4.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6051 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)      549 2022-06-10 06:15:29.108756 nexus3-cli-4.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1858 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 06:15:29.078752 nexus3-cli-4.1.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 06:15:29.084753 nexus3-cli-4.1.8/src/nexus3_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6867 2022-06-10 06:15:29.000000 nexus3-cli-4.1.8/src/nexus3_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3153 2022-06-10 06:15:29.000000 nexus3-cli-4.1.8/src/nexus3_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-10 06:15:29.000000 nexus3-cli-4.1.8/src/nexus3_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2022-06-10 06:15:29.000000 nexus3-cli-4.1.8/src/nexus3_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      249 2022-06-10 06:15:29.000000 nexus3-cli-4.1.8/src/nexus3_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-06-10 06:15:29.000000 nexus3-cli-4.1.8/src/nexus3_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 06:15:29.086753 nexus3-cli-4.1.8/src/nexuscli/
--rw-rw-rw-   0 root         (0) root         (0)      341 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 06:15:29.088754 nexus3-cli-4.1.8/src/nexuscli/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3618 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/base_collection.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/base_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 06:15:29.089754 nexus3-cli-4.1.8/src/nexuscli/api/blobstore/
--rw-rw-rw-   0 root         (0) root         (0)      117 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/blobstore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2185 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/blobstore/collection.py
--rw-rw-rw-   0 root         (0) root         (0)     2844 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/blobstore/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 06:15:29.090754 nexus3-cli-4.1.8/src/nexuscli/api/cleanup_policy/
--rw-rw-rw-   0 root         (0) root         (0)      135 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/cleanup_policy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3606 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/cleanup_policy/collection.py
--rw-rw-rw-   0 root         (0) root         (0)     1393 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/cleanup_policy/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 06:15:29.091754 nexus3-cli-4.1.8/src/nexuscli/api/repository/
--rw-rw-rw-   0 root         (0) root         (0)      165 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 06:15:29.093754 nexus3-cli-4.1.8/src/nexuscli/api/repository/base_models/
--rw-rw-rw-   0 root         (0) root         (0)      315 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/base_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1662 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/base_models/base_repository.py
--rw-rw-rw-   0 root         (0) root         (0)      896 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/base_models/group_repository.py
--rw-rw-rw-   0 root         (0) root         (0)     1441 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/base_models/hosted_repository.py
--rw-rw-rw-   0 root         (0) root         (0)     3640 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/base_models/proxy_repository.py
--rw-rw-rw-   0 root         (0) root         (0)    16787 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/base_models/repository.py
--rw-rw-rw-   0 root         (0) root         (0)      709 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/base_models/util.py
--rwxrwxrwx   0 root         (0) root         (0)    10744 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/collection.py
--rwxrwxrwx   0 root         (0) root         (0)       96 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 06:15:29.097755 nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/
--rw-rw-rw-   0 root         (0) root         (0)      515 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1811 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/apt.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/bower.py
--rw-rw-rw-   0 root         (0) root         (0)     3381 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/docker.py
--rw-rw-rw-   0 root         (0) root         (0)     2879 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/maven.py
--rw-rw-rw-   0 root         (0) root         (0)     1689 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/npm.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/nuget.py
--rw-rw-rw-   0 root         (0) root         (0)     2003 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/pypi.py
--rw-rw-rw-   0 root         (0) root         (0)     1999 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/raw.py
--rw-rw-rw-   0 root         (0) root         (0)      658 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/rubygems.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/validations.py
--rw-rw-rw-   0 root         (0) root         (0)     2561 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/yum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 06:15:29.098755 nexus3-cli-4.1.8/src/nexuscli/api/script/
--rw-rw-rw-   0 root         (0) root         (0)       63 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/script/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 06:15:29.100755 nexus3-cli-4.1.8/src/nexuscli/api/script/groovy/
--rw-rw-rw-   0 root         (0) root         (0)     3676 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/script/groovy/nexus3-cli-cleanup-policy.groovy
--rw-rw-rw-   0 root         (0) root         (0)     3829 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/script/groovy/nexus3-cli-cleanup-policy_3.20.0.groovy
--rw-rw-rw-   0 root         (0) root         (0)     3680 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/script/groovy/nexus3-cli-cleanup-policy_3.27.0.groovy
--rw-rw-rw-   0 root         (0) root         (0)     2075 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/script/groovy/nexus3-cli-repository-create.groovy
--rw-rw-rw-   0 root         (0) root         (0)     2362 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/script/groovy/nexus3-cli-repository-create_3.21.0.groovy
--rw-rw-rw-   0 root         (0) root         (0)       84 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/script/groovy/nexus3-cli-repository-delete.groovy
--rw-rw-rw-   0 root         (0) root         (0)      483 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/script/groovy/nexus3-cli-repository-get.groovy
--rw-rw-rw-   0 root         (0) root         (0)     4060 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/script/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 06:15:29.101755 nexus3-cli-4.1.8/src/nexuscli/api/security/
--rw-rw-rw-   0 root         (0) root         (0)       41 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/security/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 06:15:29.102755 nexus3-cli-4.1.8/src/nexuscli/api/security/realms/
--rw-rw-rw-   0 root         (0) root         (0)      121 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/security/realms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2340 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/security/realms/collection.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/security/realms/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 06:15:29.103755 nexus3-cli-4.1.8/src/nexuscli/api/task/
--rw-rw-rw-   0 root         (0) root         (0)       97 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/task/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2045 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/task/collection.py
--rw-rw-rw-   0 root         (0) root         (0)       80 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/task/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3354 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/util.py
--rw-rw-rw-   0 root         (0) root         (0)      671 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/api/validations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-10 06:15:29.107756 nexus3-cli-4.1.8/src/nexuscli/cli/
--rw-rw-rw-   0 root         (0) root         (0)    20012 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1408 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/cli/blobstore_options.py
--rw-rw-rw-   0 root         (0) root         (0)      234 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/cli/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2847 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/cli/repository_options.py
--rw-rw-rw-   0 root         (0) root         (0)     3912 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/cli/root_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     2727 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/cli/subcommand_blobstore.py
--rw-rw-rw-   0 root         (0) root         (0)     1732 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/cli/subcommand_cleanup_policy.py
--rw-rw-rw-   0 root         (0) root         (0)      762 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/cli/subcommand_realm.py
--rw-rw-rw-   0 root         (0) root         (0)     1798 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/cli/subcommand_repository.py
--rw-rw-rw-   0 root         (0) root         (0)     1205 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/cli/subcommand_script.py
--rw-rw-rw-   0 root         (0) root         (0)      707 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/cli/subcommand_task.py
--rw-rw-rw-   0 root         (0) root         (0)     5025 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/cli/util.py
--rw-rw-rw-   0 root         (0) root         (0)     5291 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/exception.py
--rwxrwxrwx   0 root         (0) root         (0)     4278 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/nexus_client.py
--rw-rw-rw-   0 root         (0) root         (0)     5450 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/nexus_config.py
--rw-rw-rw-   0 root         (0) root         (0)     3919 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/nexus_http.py
--rw-rw-rw-   0 root         (0) root         (0)     9976 2022-06-10 06:15:25.000000 nexus3-cli-4.1.8/src/nexuscli/nexus_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 21:05:32.414549 nexus3-cli-4.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      112 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6867 2023-09-13 21:05:32.414549 nexus3-cli-4.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6051 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      549 2023-09-13 21:05:32.414549 nexus3-cli-4.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1835 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 21:05:32.393549 nexus3-cli-4.1.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 21:05:32.398549 nexus3-cli-4.1.9/src/nexus3_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6867 2023-09-13 21:05:32.000000 nexus3-cli-4.1.9/src/nexus3_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3153 2023-09-13 21:05:32.000000 nexus3-cli-4.1.9/src/nexus3_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-13 21:05:32.000000 nexus3-cli-4.1.9/src/nexus3_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-09-13 21:05:32.000000 nexus3-cli-4.1.9/src/nexus3_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      233 2023-09-13 21:05:32.000000 nexus3-cli-4.1.9/src/nexus3_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-09-13 21:05:32.000000 nexus3-cli-4.1.9/src/nexus3_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 21:05:32.399549 nexus3-cli-4.1.9/src/nexuscli/
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 21:05:32.400549 nexus3-cli-4.1.9/src/nexuscli/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-13 21:05:30.000000 nexus3-cli-4.1.9/src/nexuscli/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3618 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/base_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/base_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 21:05:32.401549 nexus3-cli-4.1.9/src/nexuscli/api/blobstore/
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/blobstore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2185 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/blobstore/collection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/blobstore/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 21:05:32.402549 nexus3-cli-4.1.9/src/nexuscli/api/cleanup_policy/
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/cleanup_policy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3606 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/cleanup_policy/collection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1393 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/cleanup_policy/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 21:05:32.403549 nexus3-cli-4.1.9/src/nexuscli/api/repository/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 21:05:32.405549 nexus3-cli-4.1.9/src/nexuscli/api/repository/base_models/
+-rw-rw-rw-   0 root         (0) root         (0)      315 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/base_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1662 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/base_models/base_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)      896 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/base_models/group_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     1441 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/base_models/hosted_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     3640 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/base_models/proxy_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)    16927 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/base_models/repository.py
+-rw-rw-rw-   0 root         (0) root         (0)      709 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/base_models/util.py
+-rwxrwxrwx   0 root         (0) root         (0)    10744 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/collection.py
+-rwxrwxrwx   0 root         (0) root         (0)       96 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 21:05:32.408549 nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/
+-rw-rw-rw-   0 root         (0) root         (0)      515 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/apt.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/bower.py
+-rw-rw-rw-   0 root         (0) root         (0)     3381 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/docker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2879 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/maven.py
+-rw-rw-rw-   0 root         (0) root         (0)     1689 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/npm.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/nuget.py
+-rw-rw-rw-   0 root         (0) root         (0)     2003 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/pypi.py
+-rw-rw-rw-   0 root         (0) root         (0)     1999 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/raw.py
+-rw-rw-rw-   0 root         (0) root         (0)      658 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/rubygems.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-13 21:05:30.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/validations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2561 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/yum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 21:05:32.408549 nexus3-cli-4.1.9/src/nexuscli/api/script/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/script/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 21:05:32.410549 nexus3-cli-4.1.9/src/nexuscli/api/script/groovy/
+-rw-rw-rw-   0 root         (0) root         (0)     3676 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/script/groovy/nexus3-cli-cleanup-policy.groovy
+-rw-rw-rw-   0 root         (0) root         (0)     3829 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/script/groovy/nexus3-cli-cleanup-policy_3.20.0.groovy
+-rw-rw-rw-   0 root         (0) root         (0)     3680 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/script/groovy/nexus3-cli-cleanup-policy_3.27.0.groovy
+-rw-rw-rw-   0 root         (0) root         (0)     2075 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/script/groovy/nexus3-cli-repository-create.groovy
+-rw-rw-rw-   0 root         (0) root         (0)     2362 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/script/groovy/nexus3-cli-repository-create_3.21.0.groovy
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/script/groovy/nexus3-cli-repository-delete.groovy
+-rw-rw-rw-   0 root         (0) root         (0)      483 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/script/groovy/nexus3-cli-repository-get.groovy
+-rw-rw-rw-   0 root         (0) root         (0)     4060 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/script/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 21:05:32.410549 nexus3-cli-4.1.9/src/nexuscli/api/security/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/security/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 21:05:32.410549 nexus3-cli-4.1.9/src/nexuscli/api/security/realms/
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/security/realms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2340 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/security/realms/collection.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/security/realms/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 21:05:32.411549 nexus3-cli-4.1.9/src/nexuscli/api/task/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/task/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/task/collection.py
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/task/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3354 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/util.py
+-rw-rw-rw-   0 root         (0) root         (0)      671 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/api/validations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 21:05:32.413549 nexus3-cli-4.1.9/src/nexuscli/cli/
+-rw-rw-rw-   0 root         (0) root         (0)    20012 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1408 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/cli/blobstore_options.py
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/cli/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2847 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/cli/repository_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     3912 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/cli/root_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     2727 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/cli/subcommand_blobstore.py
+-rw-rw-rw-   0 root         (0) root         (0)     1732 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/cli/subcommand_cleanup_policy.py
+-rw-rw-rw-   0 root         (0) root         (0)      762 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/cli/subcommand_realm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/cli/subcommand_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     1205 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/cli/subcommand_script.py
+-rw-rw-rw-   0 root         (0) root         (0)      707 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/cli/subcommand_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     5025 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/cli/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     5311 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/exception.py
+-rwxrwxrwx   0 root         (0) root         (0)     4278 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/nexus_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     5450 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/nexus_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3919 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/nexus_http.py
+-rw-rw-rw-   0 root         (0) root         (0)     9976 2023-09-13 21:05:29.000000 nexus3-cli-4.1.9/src/nexuscli/nexus_util.py
```

### Comparing `nexus3-cli-4.1.8/LICENSE` & `nexus3-cli-4.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/PKG-INFO` & `nexus3-cli-4.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus3-cli
-Version: 4.1.8
+Version: 4.1.9
 Summary: A python-based CLI for Sonatype Nexus OSS 3
 Home-page: https://gitlab.com/thiagocsf/nexus3-cli
 Author: Thiago Figueiró
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `nexus3-cli-4.1.8/README.md` & `nexus3-cli-4.1.9/README.md`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/setup.cfg` & `nexus3-cli-4.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/setup.py` & `nexus3-cli-4.1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # -*- coding: utf-8 -*-
 import io
 from setuptools import find_packages, setup
 
 package_name = 'nexus3-cli'
-package_version = '4.1.8'
+package_version = '4.1.9'
 
 requires = [
     'click>=8.0.1,<9',
     'click_aliases>=1.0.1,<2',
-    'clint>=0.5.1,<1',
     'inflect>=5.3.0,<6',
     'requests[security]>=2.14.2,<3',
     'semver>=2.10.1,<3',
     'texttable>=1.6.2,<2',
     'twine>=3.4.1,<4'
 ]
```

### Comparing `nexus3-cli-4.1.8/src/nexus3_cli.egg-info/PKG-INFO` & `nexus3-cli-4.1.9/src/nexus3_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus3-cli
-Version: 4.1.8
+Version: 4.1.9
 Summary: A python-based CLI for Sonatype Nexus OSS 3
 Home-page: https://gitlab.com/thiagocsf/nexus3-cli
 Author: Thiago Figueiró
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `nexus3-cli-4.1.8/src/nexus3_cli.egg-info/SOURCES.txt` & `nexus3-cli-4.1.9/src/nexus3_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/base_collection.py` & `nexus3-cli-4.1.9/src/nexuscli/api/base_collection.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/base_model.py` & `nexus3-cli-4.1.9/src/nexuscli/api/base_model.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/blobstore/collection.py` & `nexus3-cli-4.1.9/src/nexuscli/api/blobstore/collection.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/blobstore/model.py` & `nexus3-cli-4.1.9/src/nexuscli/api/blobstore/model.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/cleanup_policy/collection.py` & `nexus3-cli-4.1.9/src/nexuscli/api/cleanup_policy/collection.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/cleanup_policy/model.py` & `nexus3-cli-4.1.9/src/nexuscli/api/cleanup_policy/model.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/repository/base_models/base_repository.py` & `nexus3-cli-4.1.9/src/nexuscli/api/repository/base_models/base_repository.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/repository/base_models/group_repository.py` & `nexus3-cli-4.1.9/src/nexuscli/api/repository/base_models/group_repository.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/repository/base_models/hosted_repository.py` & `nexus3-cli-4.1.9/src/nexuscli/api/repository/base_models/hosted_repository.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/repository/base_models/proxy_repository.py` & `nexus3-cli-4.1.9/src/nexuscli/api/repository/base_models/proxy_repository.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/repository/base_models/repository.py` & `nexus3-cli-4.1.9/src/nexuscli/api/repository/base_models/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import os
 import pathlib
 import warnings
 from typing import Dict, Iterator, Optional
 
 import semver
-from clint.textui import progress  # TODO: move to CLI
+from click import progressbar
 
 from nexuscli.api.repository.base_models import base_repository, util
 from nexuscli import exception, nexus_util
 
 # https://issues.sonatype.org/browse/NEXUS-19525
 # https://github.com/thiagofigueiro/nexus3-cli/issues/77
 CLEANUP_SET_MIN_VERSION = semver.VersionInfo(3, 19, 0)
@@ -244,29 +244,28 @@
         :return: number of deleted files. Negative number for errors.
         :rtype: int
         """
 
         delete_count = 0
         death_row = self.list_raw(repository_path)
 
-        death_row = progress.bar([a for a in death_row], label='Deleting')
-
-        for artefact in death_row:
-            id_ = artefact['id']
-            artefact_path = artefact['path']
-
-            response = self._client.delete(f'assets/{id_}')
-            LOG.info('Deleted: %s (%s)', artefact_path, id_)
-            delete_count += 1
-            if response.status_code == 404:
-                LOG.warning('File disappeared while deleting')
-                LOG.debug(response.reason)
-            elif response.status_code != 204:
-                LOG.error(response.reason)
-                return -1
+        with progressbar([a for a in death_row], label='Deleting') as death_row:
+            for artefact in death_row:
+                id_ = artefact['id']
+                artefact_path = artefact['path']
+
+                response = self._client.delete(f'assets/{id_}')
+                LOG.info('Deleted: %s (%s)', artefact_path, id_)
+                delete_count += 1
+                if response.status_code == 404:
+                    LOG.warning('File disappeared while deleting')
+                    LOG.debug(response.reason)
+                elif response.status_code != 204:
+                    LOG.error(response.reason)
+                    return -1
 
         return delete_count
 
     @staticmethod
     def _should_skip_download(download_url, download_path, artefact, nocache):
         """False when nocache is set or local file is out-of-date"""
         if nocache:
@@ -336,35 +335,35 @@
         download_count = 0
         if source.endswith(nexus_util.REMOTE_PATH_SEPARATOR) and \
                 not (destination.endswith('.') or destination.endswith('..')):
             destination += os.sep
 
         artefacts = self.list_raw(source)
 
-        artefacts = progress.bar(
-                [a for a in artefacts], label='Downloading')
-
-        for artefact in artefacts:
-            download_url = artefact['downloadUrl']
-            artefact_path = artefact['path']
-            LOG.debug('Downloading [%s] to [%s] from [%s], flatten=%s',
-                      artefact_path, destination, download_url, flatten)
-            download_path = nexus_util.remote_path_to_local(artefact_path, destination, flatten)
-
-            if self._should_skip_download(
-                    download_url, download_path, artefact, nocache):
-                download_count += 1
-                continue
-
-            try:
-                self.download_file(download_url, download_path)
-                download_count += 1
-            except exception.DownloadError:
-                LOG.warning('Error downloading %s', download_url)
-                continue
+        with progressbar([a for a in artefacts], label='Downloading') as artefacts:
+            for artefact in artefacts:
+                download_url = artefact['downloadUrl']
+                artefact_path = artefact['path']
+                LOG.debug('Downloading [%s] to [%s] from [%s], flatten=%s',
+                          artefact_path, destination, download_url, flatten)
+                download_path = nexus_util.remote_path_to_local(
+                    artefact_path, destination, flatten
+                )
+
+                if self._should_skip_download(
+                        download_url, download_path, artefact, nocache):
+                    download_count += 1
+                    continue
+
+                try:
+                    self.download_file(download_url, download_path)
+                    download_count += 1
+                except exception.DownloadError:
+                    LOG.warning('Error downloading %s', download_url)
+                    continue
 
         return download_count
 
     def upload(self, source, destination, recurse=True, flatten=False):
         """
         Upload artefacts. The source must be either a local file name or
         directory. The flatten and recurse options are honoured for
@@ -419,21 +418,20 @@
             on the destination.
         :return: number of files uploaded
         :rtype: int
         """
         destination = pathlib.Path(destination)
         file_set = util.get_files(source, recurse)
         expected_upload_count = len(file_set)
-        file_set = progress.bar(file_set, expected_size=expected_upload_count)
-
         upload_count = 0
-        for source_file in file_set:
-            dst_path = self._upload_dst_path(source, source_file, destination, flatten)
-            LOG.debug('Uploading [%s] to [%s] in repository=%s, flatten=%s',
-                      source_file, dst_path, self.name, flatten)
-            self.upload_file(source_file, dst_path)
-            upload_count += 1
+        with progressbar(file_set, length=expected_upload_count) as file_set:
+            for source_file in file_set:
+                dst_path = self._upload_dst_path(source, source_file, destination, flatten)
+                LOG.debug('Uploading [%s] to [%s] in repository=%s, flatten=%s',
+                          source_file, dst_path, self.name, flatten)
+                self.upload_file(source_file, dst_path)
+                upload_count += 1
 
         if expected_upload_count != upload_count:
             warnings.warn(f'expected {expected_upload_count} to upload but got {upload_count}')
 
         return upload_count
```

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/repository/base_models/util.py` & `nexus3-cli-4.1.9/src/nexuscli/api/repository/base_models/util.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/repository/collection.py` & `nexus3-cli-4.1.9/src/nexuscli/api/repository/collection.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/__init__.py` & `nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/__init__.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/apt.py` & `nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/apt.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/bower.py` & `nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/bower.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/docker.py` & `nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/docker.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/maven.py` & `nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/maven.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/npm.py` & `nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/npm.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/nuget.py` & `nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/nuget.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/pypi.py` & `nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/pypi.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/raw.py` & `nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/raw.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/rubygems.py` & `nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/rubygems.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/repository/recipes/yum.py` & `nexus3-cli-4.1.9/src/nexuscli/api/repository/recipes/yum.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/script/groovy/nexus3-cli-cleanup-policy.groovy` & `nexus3-cli-4.1.9/src/nexuscli/api/script/groovy/nexus3-cli-cleanup-policy.groovy`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/script/groovy/nexus3-cli-cleanup-policy_3.20.0.groovy` & `nexus3-cli-4.1.9/src/nexuscli/api/script/groovy/nexus3-cli-cleanup-policy_3.20.0.groovy`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/script/groovy/nexus3-cli-cleanup-policy_3.27.0.groovy` & `nexus3-cli-4.1.9/src/nexuscli/api/script/groovy/nexus3-cli-cleanup-policy_3.27.0.groovy`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/script/groovy/nexus3-cli-repository-create.groovy` & `nexus3-cli-4.1.9/src/nexuscli/api/script/groovy/nexus3-cli-repository-create.groovy`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/script/groovy/nexus3-cli-repository-create_3.21.0.groovy` & `nexus3-cli-4.1.9/src/nexuscli/api/script/groovy/nexus3-cli-repository-create_3.21.0.groovy`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/script/model.py` & `nexus3-cli-4.1.9/src/nexuscli/api/script/model.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/security/realms/collection.py` & `nexus3-cli-4.1.9/src/nexuscli/api/security/realms/collection.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/task/collection.py` & `nexus3-cli-4.1.9/src/nexuscli/api/task/collection.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/util.py` & `nexus3-cli-4.1.9/src/nexuscli/api/util.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/api/validations.py` & `nexus3-cli-4.1.9/src/nexuscli/api/validations.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/cli/__init__.py` & `nexus3-cli-4.1.9/src/nexuscli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/cli/blobstore_options.py` & `nexus3-cli-4.1.9/src/nexuscli/cli/blobstore_options.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/cli/repository_options.py` & `nexus3-cli-4.1.9/src/nexuscli/cli/repository_options.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/cli/root_commands.py` & `nexus3-cli-4.1.9/src/nexuscli/cli/root_commands.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/cli/subcommand_blobstore.py` & `nexus3-cli-4.1.9/src/nexuscli/cli/subcommand_blobstore.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/cli/subcommand_cleanup_policy.py` & `nexus3-cli-4.1.9/src/nexuscli/cli/subcommand_cleanup_policy.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/cli/subcommand_realm.py` & `nexus3-cli-4.1.9/src/nexuscli/cli/subcommand_realm.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/cli/subcommand_repository.py` & `nexus3-cli-4.1.9/src/nexuscli/cli/subcommand_repository.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/cli/subcommand_script.py` & `nexus3-cli-4.1.9/src/nexuscli/cli/subcommand_script.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/cli/subcommand_task.py` & `nexus3-cli-4.1.9/src/nexuscli/cli/subcommand_task.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/cli/util.py` & `nexus3-cli-4.1.9/src/nexuscli/cli/util.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/exception.py` & `nexus3-cli-4.1.9/src/nexuscli/exception.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,17 +66,17 @@
     except (TypeError, json.JSONDecodeError):
         return
 
     if not isinstance(nexus_response, dict):
         return
 
     try:
-        result = nexus_response['result']
+        result = nexus_response['message']
     except KeyError:
-        raise TypeError('Unrecognised Nexus error response') from None
+        raise TypeError(f'Unrecognised Nexus error response: {nexus_response}') from None
 
     _lookup_and_raise(result)
 
 
 class NexusClientBaseError(ClickException):
     exit_code = CliReturnCode.UNKNOWN_ERROR.value
```

### Comparing `nexus3-cli-4.1.8/src/nexuscli/nexus_client.py` & `nexus3-cli-4.1.9/src/nexuscli/nexus_client.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/nexus_config.py` & `nexus3-cli-4.1.9/src/nexuscli/nexus_config.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/nexus_http.py` & `nexus3-cli-4.1.9/src/nexuscli/nexus_http.py`

 * *Files identical despite different names*

### Comparing `nexus3-cli-4.1.8/src/nexuscli/nexus_util.py` & `nexus3-cli-4.1.9/src/nexuscli/nexus_util.py`

 * *Files identical despite different names*

