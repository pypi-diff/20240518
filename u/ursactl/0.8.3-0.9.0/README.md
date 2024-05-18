# Comparing `tmp/ursactl-0.8.3.tar.gz` & `tmp/ursactl-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jgsmith/Code/ursactl/dist/.tmp-vbb47dte/ursactl-0.8.3.tar", last modified: Mon Aug 21 19:50:43 2023, max compression
+gzip compressed data, was "/home/jgsmith/Code/UrsaFrontier/ursactl/dist/.tmp-zkts_ct3/ursactl-0.9.0.tar", last modified: Sat May 18 12:14:39 2024, max compression
```

## Comparing `ursactl-0.8.3.tar` & `ursactl-0.9.0.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-21 19:50:43.000000 ursactl-0.8.3/
--rw-r--r--   0 jgsmith    (501) staff       (20)       67 2023-01-01 19:09:45.000000 ursactl-0.8.3/CHANGELOG.md
--rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-01-01 19:09:45.000000 ursactl-0.8.3/LICENSE.md
--rw-r--r--   0 jgsmith    (501) staff       (20)      135 2023-01-01 19:09:45.000000 ursactl-0.8.3/MANIFEST.in
--rw-r--r--   0 jgsmith    (501) staff       (20)     2749 2023-08-21 19:50:43.000000 ursactl-0.8.3/PKG-INFO
--rw-r--r--   0 jgsmith    (501) staff       (20)     1675 2023-07-25 12:15:23.000000 ursactl-0.8.3/README.md
--rw-r--r--   0 jgsmith    (501) staff       (20)       81 2023-01-01 19:09:45.000000 ursactl-0.8.3/pyproject.toml
--rw-r--r--   0 jgsmith    (501) staff       (20)      168 2023-07-25 12:15:23.000000 ursactl-0.8.3/requirements-dev.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)      207 2023-07-16 14:14:44.000000 ursactl-0.8.3/requirements.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)     1287 2023-08-21 19:50:43.000000 ursactl-0.8.3/setup.cfg
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-21 19:50:43.000000 ursactl-0.8.3/tests/
--rw-r--r--   0 jgsmith    (501) staff       (20)      382 2023-01-31 15:40:54.000000 ursactl-0.8.3/tests/test_ursactl.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-21 19:50:43.000000 ursactl-0.8.3/ursactl/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.8.3/ursactl/__init__.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-21 19:50:43.000000 ursactl-0.8.3/ursactl/airflow_provider/
--rw-r--r--   0 jgsmith    (501) staff       (20)      434 2023-08-08 23:22:03.000000 ursactl-0.8.3/ursactl/airflow_provider/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     3787 2023-08-01 15:14:48.000000 ursactl-0.8.3/ursactl/airflow_provider/hooks.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-21 19:50:43.000000 ursactl-0.8.3/ursactl/controllers/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.8.3/ursactl/controllers/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1089 2023-08-21 12:03:35.000000 ursactl-0.8.3/ursactl/controllers/base.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     8678 2023-08-21 19:50:17.000000 ursactl-0.8.3/ursactl/controllers/create.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     3313 2023-06-04 21:29:27.000000 ursactl-0.8.3/ursactl/controllers/delete.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1150 2023-03-24 15:51:14.000000 ursactl-0.8.3/ursactl/controllers/get.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1218 2023-08-11 13:52:32.000000 ursactl-0.8.3/ursactl/controllers/init.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     8062 2023-08-21 19:50:17.000000 ursactl-0.8.3/ursactl/controllers/list.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      446 2023-02-16 21:42:16.000000 ursactl-0.8.3/ursactl/controllers/refresh.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2297 2023-07-25 12:15:23.000000 ursactl-0.8.3/ursactl/controllers/run.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1944 2023-05-04 12:27:25.000000 ursactl-0.8.3/ursactl/controllers/send.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      762 2023-07-16 14:14:44.000000 ursactl-0.8.3/ursactl/controllers/show.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      764 2023-04-18 14:46:09.000000 ursactl-0.8.3/ursactl/controllers/stop.py
--rw-r--r--   0 jgsmith    (501) staff       (20)    13704 2023-08-17 16:52:23.000000 ursactl-0.8.3/ursactl/controllers/sync.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     5853 2023-08-08 23:22:03.000000 ursactl-0.8.3/ursactl/controllers/update.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-21 19:50:43.000000 ursactl-0.8.3/ursactl/controllers/utils/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-06-04 21:29:27.000000 ursactl-0.8.3/ursactl/controllers/utils/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1299 2023-08-08 23:22:03.000000 ursactl-0.8.3/ursactl/controllers/utils/pages.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     5427 2023-08-08 23:22:03.000000 ursactl-0.8.3/ursactl/controllers/utils/transforms.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-21 19:50:43.000000 ursactl-0.8.3/ursactl/core/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.8.3/ursactl/core/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      640 2023-07-17 12:46:16.000000 ursactl-0.8.3/ursactl/core/_base.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1501 2023-07-17 12:46:16.000000 ursactl-0.8.3/ursactl/core/agent.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2345 2023-07-20 19:45:48.000000 ursactl-0.8.3/ursactl/core/dataset.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      389 2023-08-21 12:38:06.000000 ursactl-0.8.3/ursactl/core/exc.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2023 2023-07-20 15:12:38.000000 ursactl-0.8.3/ursactl/core/pipeline.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1793 2023-07-20 12:42:32.000000 ursactl-0.8.3/ursactl/core/pipeline_run.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1967 2023-07-20 12:42:32.000000 ursactl-0.8.3/ursactl/core/pipeline_sweep.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     4578 2023-07-25 12:15:23.000000 ursactl-0.8.3/ursactl/core/project.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1010 2023-07-20 12:42:32.000000 ursactl-0.8.3/ursactl/core/running_agent.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-21 19:50:43.000000 ursactl-0.8.3/ursactl/core/services/
--rw-r--r--   0 jgsmith    (501) staff       (20)      931 2023-08-08 23:22:03.000000 ursactl-0.8.3/ursactl/core/services/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1843 2023-08-08 23:22:03.000000 ursactl-0.8.3/ursactl/core/services/_base.py
--rw-r--r--   0 jgsmith    (501) staff       (20)    33834 2023-08-21 12:38:06.000000 ursactl-0.8.3/ursactl/core/services/ape_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)    13155 2023-08-21 12:38:06.000000 ursactl-0.8.3/ursactl/core/services/dss_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1892 2023-07-17 12:46:16.000000 ursactl-0.8.3/ursactl/core/services/iam_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     6905 2023-08-21 12:38:06.000000 ursactl-0.8.3/ursactl/core/services/page_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)    14109 2023-08-21 12:38:06.000000 ursactl-0.8.3/ursactl/core/services/planning_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2910 2023-05-04 12:27:25.000000 ursactl-0.8.3/ursactl/core/services/project_client.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-21 19:50:43.000000 ursactl-0.8.3/ursactl/core/utils/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-18 13:39:22.000000 ursactl-0.8.3/ursactl/core/utils/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1470 2023-04-18 14:46:09.000000 ursactl-0.8.3/ursactl/core/utils/magic.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      203 2023-08-21 19:50:17.000000 ursactl-0.8.3/ursactl/core/version.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-21 19:50:43.000000 ursactl-0.8.3/ursactl/ext/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.8.3/ursactl/ext/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     4544 2023-08-21 12:38:06.000000 ursactl-0.8.3/ursactl/main.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-21 19:50:43.000000 ursactl-0.8.3/ursactl/plugins/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.8.3/ursactl/plugins/__init__.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-21 19:50:43.000000 ursactl-0.8.3/ursactl/templates/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.8.3/ursactl/templates/__init__.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-08-21 19:50:43.000000 ursactl-0.8.3/ursactl.egg-info/
--rw-r--r--   0 jgsmith    (501) staff       (20)     2749 2023-08-21 19:50:43.000000 ursactl-0.8.3/ursactl.egg-info/PKG-INFO
--rw-r--r--   0 jgsmith    (501) staff       (20)     1675 2023-08-21 19:50:43.000000 ursactl-0.8.3/ursactl.egg-info/SOURCES.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-08-21 19:50:43.000000 ursactl-0.8.3/ursactl.egg-info/dependency_links.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)       46 2023-08-21 19:50:43.000000 ursactl-0.8.3/ursactl.egg-info/entry_points.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)      207 2023-08-21 19:50:43.000000 ursactl-0.8.3/ursactl.egg-info/requires.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)        8 2023-08-21 19:50:43.000000 ursactl-0.8.3/ursactl.egg-info/top_level.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-02-17 20:26:57.000000 ursactl-0.8.3/ursactl.egg-info/zip-safe
+drwxrwxr-x   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-18 12:14:39.000000 ursactl-0.9.0/
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)       67 2024-05-11 21:25:54.000000 ursactl-0.9.0/CHANGELOG.md
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)        1 2024-05-11 21:25:54.000000 ursactl-0.9.0/LICENSE.md
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)      135 2024-05-11 21:25:54.000000 ursactl-0.9.0/MANIFEST.in
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     2749 2024-05-18 12:14:39.000000 ursactl-0.9.0/PKG-INFO
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     1675 2024-05-11 21:25:54.000000 ursactl-0.9.0/README.md
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)       81 2024-05-11 21:25:54.000000 ursactl-0.9.0/pyproject.toml
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)      175 2024-05-17 19:47:14.000000 ursactl-0.9.0/requirements-dev.txt
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)      207 2024-05-16 15:04:33.000000 ursactl-0.9.0/requirements.txt
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     1287 2024-05-18 12:14:39.000000 ursactl-0.9.0/setup.cfg
+drwxrwxr-x   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-18 12:14:39.000000 ursactl-0.9.0/tests/
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)      382 2024-05-11 21:25:54.000000 ursactl-0.9.0/tests/test_ursactl.py
+drwxrwxr-x   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-18 12:14:39.000000 ursactl-0.9.0/ursactl/
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/__init__.py
+drwxrwxr-x   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-18 12:14:39.000000 ursactl-0.9.0/ursactl/airflow_provider/
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)      434 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/airflow_provider/__init__.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     3787 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/airflow_provider/hooks.py
+drwxrwxr-x   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-18 12:14:39.000000 ursactl-0.9.0/ursactl/controllers/
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/controllers/__init__.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     1089 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/controllers/base.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     9191 2024-05-17 19:47:14.000000 ursactl-0.9.0/ursactl/controllers/create.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     3913 2024-05-17 19:47:14.000000 ursactl-0.9.0/ursactl/controllers/delete.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     1150 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/controllers/get.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     1218 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/controllers/init.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     8715 2024-05-17 19:47:14.000000 ursactl-0.9.0/ursactl/controllers/list.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)      446 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/controllers/refresh.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     2297 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/controllers/run.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     3333 2024-05-17 19:47:14.000000 ursactl-0.9.0/ursactl/controllers/send.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)      762 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/controllers/show.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)      764 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/controllers/stop.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)    13704 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/controllers/sync.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     5853 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/controllers/update.py
+drwxrwxr-x   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-18 12:14:39.000000 ursactl-0.9.0/ursactl/controllers/utils/
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/controllers/utils/__init__.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     1299 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/controllers/utils/pages.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     5427 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/controllers/utils/transforms.py
+drwxrwxr-x   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-18 12:14:39.000000 ursactl-0.9.0/ursactl/core/
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/core/__init__.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)      640 2024-05-17 19:47:14.000000 ursactl-0.9.0/ursactl/core/_base.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     1564 2024-05-17 19:47:14.000000 ursactl-0.9.0/ursactl/core/agent.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     2148 2024-05-17 19:47:14.000000 ursactl-0.9.0/ursactl/core/agent_swarm.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     2345 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/core/dataset.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)      389 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/core/exc.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     2023 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/core/pipeline.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     1793 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/core/pipeline_run.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     1967 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/core/pipeline_sweep.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     6003 2024-05-17 19:47:14.000000 ursactl-0.9.0/ursactl/core/project.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     1010 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/core/running_agent.py
+drwxrwxr-x   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-18 12:14:39.000000 ursactl-0.9.0/ursactl/core/services/
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)      931 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/core/services/__init__.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     1843 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/core/services/_base.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)    33834 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/core/services/ape_client.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)    13155 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/core/services/dss_client.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     1892 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/core/services/iam_client.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     6905 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/core/services/page_client.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)    18765 2024-05-17 19:47:14.000000 ursactl-0.9.0/ursactl/core/services/planning_client.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     2910 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/core/services/project_client.py
+drwxrwxr-x   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-18 12:14:39.000000 ursactl-0.9.0/ursactl/core/utils/
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/core/utils/__init__.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     1470 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/core/utils/magic.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)      202 2024-05-17 19:47:14.000000 ursactl-0.9.0/ursactl/core/version.py
+drwxrwxr-x   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-18 12:14:39.000000 ursactl-0.9.0/ursactl/ext/
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/ext/__init__.py
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     5562 2024-05-17 19:47:14.000000 ursactl-0.9.0/ursactl/main.py
+drwxrwxr-x   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-18 12:14:39.000000 ursactl-0.9.0/ursactl/plugins/
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/plugins/__init__.py
+drwxrwxr-x   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-18 12:14:39.000000 ursactl-0.9.0/ursactl/templates/
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-11 21:25:54.000000 ursactl-0.9.0/ursactl/templates/__init__.py
+drwxrwxr-x   0 jgsmith   (1000) jgsmith   (1000)        0 2024-05-18 12:14:39.000000 ursactl-0.9.0/ursactl.egg-info/
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     2749 2024-05-18 12:14:39.000000 ursactl-0.9.0/ursactl.egg-info/PKG-INFO
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)     1703 2024-05-18 12:14:39.000000 ursactl-0.9.0/ursactl.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)        1 2024-05-18 12:14:39.000000 ursactl-0.9.0/ursactl.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)       46 2024-05-18 12:14:39.000000 ursactl-0.9.0/ursactl.egg-info/entry_points.txt
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)      207 2024-05-18 12:14:39.000000 ursactl-0.9.0/ursactl.egg-info/requires.txt
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)        8 2024-05-18 12:14:39.000000 ursactl-0.9.0/ursactl.egg-info/top_level.txt
+-rw-rw-r--   0 jgsmith   (1000) jgsmith   (1000)        1 2024-05-16 15:01:32.000000 ursactl-0.9.0/ursactl.egg-info/zip-safe
```

### Comparing `ursactl-0.8.3/PKG-INFO` & `ursactl-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ursactl
-Version: 0.8.3
+Version: 0.9.0
 Summary: command line tool and library for intercting with ursafrontier.cloud
 Home-page: https://ursafrontier.cloud/
 Author: Ursa Frontier LLC
 Author-email: contact@ursafrontier.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `ursactl-0.8.3/README.md` & `ursactl-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/setup.cfg` & `ursactl-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/airflow_provider/hooks.py` & `ursactl-0.9.0/ursactl/airflow_provider/hooks.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/controllers/base.py` & `ursactl-0.9.0/ursactl/controllers/base.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/controllers/create.py` & `ursactl-0.9.0/ursactl/controllers/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+import json
 import sys
 
-from cement import Controller, ex
-import json
 import yaml
+from cement import Controller, ex
+
+from ursactl.controllers.utils.pages import load_page
+from ursactl.controllers.utils.transforms import load_transform
 
 from ..core.services import client
 from ..core.utils.magic import magic
-from ursactl.controllers.utils.transforms import load_transform
-from ursactl.controllers.utils.pages import load_page
 
 
 def _yaml_load(fd):
     return list(yaml.load_all(fd, Loader=yaml.Loader))
 
 
 class Create(Controller):
@@ -56,14 +57,26 @@
                 'behaviors': content['behaviors'],
                 'project_uuid': project_uuid,
             }
 
             result = planning_client.create_agent(**args)
             self._print(result)
 
+    @ex(help='create agent swarm',
+        arguments=[
+            (['name'], {'help': 'agent swarm name', 'action': 'store', 'nargs': '?'}),
+            (['--project'], {'help': 'project identifier', 'dest': 'project', 'action': 'store'}),
+        ])
+    def agent_swarm(self):
+        project_uuid = self._project_scope
+        planning_client = client('planning', self.app)
+
+        result = planning_client.create_agent_swarm(name=self.app.pargs.name, project_uuid=project_uuid)
+        self._print(result)
+
     @ex(help='create transform',
         arguments=[
             (['file'], {'help': 'transform definition file', 'action': 'store'}),
             (['--project'], {'help': 'project identifier', 'dest': 'project', 'action': 'store'}),
         ])
     def transform(self):
         project_uuid = self._project_scope
```

### Comparing `ursactl-0.8.3/ursactl/controllers/delete.py` & `ursactl-0.9.0/ursactl/controllers/delete.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from cement import Controller, ex
 import json
+
 import yaml
+from cement import Controller, ex
 
 from ..core.services import client
 
 
 class Delete(Controller):
     """
     Provides the 'delete' verb.
@@ -22,14 +23,26 @@
             (['agent'], {'help': 'agent uuid or path', 'action': 'store'})
         ])
     def agent(self):
         planning_client = client('planning', self.app)
         result = planning_client.delete_agent(self.app.pargs.agent, project_uuid=self._project_scope)
         self._print(result)
 
+    @ex(help='delete an agent swarm',
+        arguments=[
+            (['--project'], {'help': 'project identifier', 'dest': 'project', 'action': 'store'}),
+            (['agent_swarm'], {'help': 'agent swarm uuid or name', 'action': 'store', 'nargs': '?'})
+        ])
+    def agent_swarm(self):
+        planning_client = client('planning', self.app)
+        result = planning_client.delete_agent_swarm(
+                                                    self.app.pargs.agent_swarm,
+                                                    project_uuid=self._project_scope)
+        self._print(result)
+
     @ex(help='delete a transform',
         arguments=[
             (['--project'], {'help': 'project identifier', 'dest': 'project', 'action': 'store'}),
             (['transform'], {'help': 'transform uuid or path', 'action': 'store'})
         ])
     def transform(self):
         ape_client = client('ape', self.app)
```

### Comparing `ursactl-0.8.3/ursactl/controllers/get.py` & `ursactl-0.9.0/ursactl/controllers/get.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/controllers/init.py` & `ursactl-0.9.0/ursactl/controllers/init.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/controllers/list.py` & `ursactl-0.9.0/ursactl/controllers/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from cement import Controller, ex
+from configparser import NoOptionError
 from json import dumps as json_dump
+
+from cement import Controller, ex
 from yaml import dump as yaml_dump
-from configparser import NoOptionError
 
-from ursactl.core.services import client
 from ursactl.core.exc import UrsaProjectNotDefined
+from ursactl.core.services import client
 
 
 class List(Controller):
     """
     Provides the `ursactl list ...` actions.
     """
 
@@ -33,14 +34,33 @@
                     [item['name']]
                 )
             data.sort()
             self.app.render(data, headers=['Name'])
         else:
             self._print(agents)
 
+    @ex(help='list agent swarms',
+        arguments=[
+            (['--project'], {'help': 'project identifier', 'dest': 'project', 'action': 'store'}),
+        ])
+    def agent_swarms(self):
+        planning_client = client('planning', self.app)
+
+        swarms = planning_client.list_agent_swarms(project_uuid=self._project_scope)
+        if self.app.pargs.output is None:
+            data = []
+            for item in swarms:
+                data.append(
+                    [item['name'], item['id']]
+                )
+            data.sort()
+            self.app.render(data, headers=['Name', 'ID'])
+        else:
+            self._print(swarms)
+
     @ex(help='list transforms',
         arguments=[
             (['--project'], {'help': 'project identifier', 'dest': 'project', 'action': 'store'}),
         ])
     def transforms(self):
         ape_client = client('ape', self.app)
```

### Comparing `ursactl-0.8.3/ursactl/controllers/run.py` & `ursactl-0.9.0/ursactl/controllers/run.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/controllers/show.py` & `ursactl-0.9.0/ursactl/controllers/show.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/controllers/stop.py` & `ursactl-0.9.0/ursactl/controllers/stop.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/controllers/sync.py` & `ursactl-0.9.0/ursactl/controllers/sync.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/controllers/update.py` & `ursactl-0.9.0/ursactl/controllers/update.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/controllers/utils/pages.py` & `ursactl-0.9.0/ursactl/controllers/utils/pages.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/controllers/utils/transforms.py` & `ursactl-0.9.0/ursactl/controllers/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/core/_base.py` & `ursactl-0.9.0/ursactl/core/_base.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-
-
 class Base:
     """
     Base class for OOP interface classes.
     """
+
     def __init__(self, uuid=None, client=None, app=None, project=None, **kwargs):
         self._client = client
         self._app = app
         self._uuid = uuid
         self.project = project
 
         if any(kwargs):
@@ -15,14 +14,15 @@
         else:
             self._cached_data = None
 
     @property
     def app(self):
         if self._app is None:
             from ursactl.main import UrsaCtl
+
             self._app = UrsaCtl()
             self._app.reload()
         return self._app
 
     @property
     def uuid(self):
         return self._uuid
```

### Comparing `ursactl-0.8.3/ursactl/core/agent.py` & `ursactl-0.9.0/ursactl/core/dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,88 @@
+"""
+Dataset object providing a OOP interface to datasets.
+"""
 from ursactl.core.services import client
 from ursactl.core._base import Base
-from .running_agent import RunningAgent
 
-import json
 
-
-class Agent(Base):
+class Dataset(Base):
     """
-    Provides access to an agent definition.
+    Provides access to a dataset.
     """
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._content = None
+
     @property
     def client(self):
         if self._client is None:
-            self._client = client('planning', self.app)
+            self._client = client('dss', self.app)
         return self._client
 
+    def commit(self):
+        if self.uuid is None:
+            # create rather than update
+            # don't support uploading data (yet)
+            result = self.client.create_dataset(
+                project_uuid=self.project.uuid,
+                name=self.name,
+                description=self.description
+            )
+            if result['accepted']:
+                self._uuid = result['uuid']
+                return True
+            return False
+        return False
+
+    @property
+    def path(self):
+        return self._data['path']
+
+    @property
+    def description(self):
+        return self._data['description']
+
+    @property
+    def content_type(self):
+        return self._data['contentType']
+
     @property
-    def name(self):
-        return self._data['name']
+    def size(self):
+        return self._data['size']
 
     @property
-    def packages(self):
-        return self._data['packages']
+    def url(self):
+        return self._data['url']
 
     @property
-    def behaviors(self):
-        return self._data['behaviors']
+    def content(self):
+        if self._content is None and self.url is not None:
+            self._content = self.client.download_dataset_content(self.url)
+        return self._content
 
-    def run(self, state=None, predicates=None):
-        result = self.client.run_agent(
-            self.uuid,
-            initial_state=json.dumps(state),
-            initial_predicates=json.dumps(predicates),
-            project_uuid=self.project.uuid
-        )
+    @property
+    def created_at(self):
+        return self._data['createdAt']
 
-        if result['errors']:
-            return None
-        running_agent_id = result['result']['id']
-        return RunningAgent(uuid=running_agent_id, app=self.app, client=self.client, project=self.project)
+    @property
+    def updated_at(self):
+        return self._data['updatedAt']
 
     @property
     def _data(self):
         if self._cached_data is None:
             if self.uuid is None:
                 self._cached_data = {
-                    'name': None,
-                    'packages': None,
-                    'behaviors': None,
-                    'project_uuid': None
+                    'path': None,
+                    'description': None,
+                    'contentType': None,
+                    'size': None,
+                    'url': None,
+                    'createdAt': None,
+                    'updatedAt': None
                 }
             else:
-                self._cached_data = self.client.get_agent(self.uuid)
+                self._cached_data = self.client.get_dataset_details(self.uuid)
+                self._cached_data['url'] = self.client.get_dataset_url(self.project.uuid, self.uuid)
+
         return self._cached_data
```

### Comparing `ursactl-0.8.3/ursactl/core/dataset.py` & `ursactl-0.9.0/ursactl/core/pipeline.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,73 @@
-"""
-Dataset object providing a OOP interface to datasets.
-"""
 from ursactl.core.services import client
 from ursactl.core._base import Base
+from .pipeline_run import PipelineRun
+from .pipeline_sweep import PipelineSweep
 
 
-class Dataset(Base):
+class Pipeline(Base):
     """
-    Provides access to a dataset.
+    Provides access to a pipeline definition.
     """
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._content = None
-
     @property
     def client(self):
         if self._client is None:
-            self._client = client('dss', self.app)
+            self._client = client('ape', self.app)
         return self._client
 
-    def commit(self):
-        if self.uuid is None:
-            # create rather than update
-            # don't support uploading data (yet)
-            result = self.client.create_dataset(
-                project_uuid=self.project.uuid,
-                name=self.name,
-                description=self.description
-            )
-            if result['accepted']:
-                self._uuid = result['uuid']
-                return True
-            return False
-        return False
-
     @property
-    def path(self):
-        return self._data['path']
+    def name(self):
+        return self._data['name']
 
     @property
     def description(self):
         return self._data['description']
 
     @property
-    def content_type(self):
-        return self._data['contentType']
-
-    @property
-    def size(self):
-        return self._data['size']
-
-    @property
-    def url(self):
-        return self._data['url']
+    def pipeline_runs(self):
+        return []
 
     @property
-    def content(self):
-        if self._content is None and self.url is not None:
-            self._content = self.client.download_dataset_content(self.url)
-        return self._content
+    def pipeline_sweeps(self):
+        return []
 
-    @property
-    def created_at(self):
-        return self._data['createdAt']
-
-    @property
-    def updated_at(self):
-        return self._data['updatedAt']
+    def run(self, parameters=None):
+        """
+        Runs the pipeline, returning a PipelineRun object.
+        """
+        result = self.client.run_pipeline(
+            self.uuid,
+            parameters=parameters,
+            project_uuid=self.project.uuid)
+
+        return PipelineRun(pipeline=self, project=self.project, uuid=result['id'], app=self.app, client=self.client)
+
+    def sweep(self, parameters=None, sweep_parameters=None):
+        """
+        Sweeps the pipeline, returning a PipelineSweep object.
+        """
+        result = self.client.run_pipeline(
+            self.uuid,
+            parameters=parameters,
+            sweep_parameters=sweep_parameters,
+            project_uuid=self.project.uuid)
+
+        return PipelineSweep(
+            pipeline=self,
+            project=self.project,
+            uuid=result['result']['id'],
+            app=self.app,
+            client=self.client)
 
     @property
     def _data(self):
         if self._cached_data is None:
             if self.uuid is None:
                 self._cached_data = {
                     'path': None,
                     'description': None,
-                    'contentType': None,
-                    'size': None,
-                    'url': None,
-                    'createdAt': None,
-                    'updatedAt': None
+                    'seeders': [],
+                    'generators': []
                 }
             else:
-                self._cached_data = self.client.get_dataset_details(self.uuid)
-                self._cached_data['url'] = self.client.get_dataset_url(self.project.uuid, self.uuid)
-
+                self._cached_data = self.client.get_pipeline(uuid=self.uuid)
         return self._cached_data
```

### Comparing `ursactl-0.8.3/ursactl/core/pipeline_run.py` & `ursactl-0.9.0/ursactl/core/pipeline_run.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/core/pipeline_sweep.py` & `ursactl-0.9.0/ursactl/core/pipeline_sweep.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/core/project.py` & `ursactl-0.9.0/ursactl/core/project.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from ursactl.core.services import client
 from ursactl.core._base import Base
+from ursactl.core.services import client
 
 
 class Project(Base):
     """
     Provides access to a project and its related resources.
 
     When called without a project name,
@@ -11,76 +11,117 @@
 
     Parameters
     ----------
     uuid : string
         The project UUID (default: None)
 
     """
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if self._uuid is None:
-            self._uuid = self.app.config.get('ursactl', 'project')
+            self._uuid = self.app.config.get("ursactl", "project")
 
     @property
     def client(self):
         """
         The client used by the project object.
 
         :meta private:
         """
         if self._client is None:
-            self._client = client('usage', self.app)
+            self._client = client("usage", self.app)
         return self._client
 
     @property
     def name(self):
         """The project name."""
-        return self._data['name']
+        return self._data["name"]
 
     @property
     def description(self):
         """The project description."""
-        return self._data['description']
+        return self._data["description"]
 
     @property
     def is_archived(self):
         """Whether the project is archived."""
-        return self._data['isArchived']
+        return self._data["isArchived"]
 
     def Agent(self, *args, **kwargs):
         """
         Convenience method to create an agent object with the project scope.
 
         See :class:`ursactl.core.agent.Agent` for details.
         """
         from ursactl.core.agent import Agent as AgentClass
 
         return AgentClass(*args, project_uuid=self.uuid, **kwargs)
 
+    def AgentSwarm(self, *args, **kwargs):
+        """
+        Convenience method to create an agent swarm with the project scope.
+
+        See :class:`ursactl.core.agent_swarm.AgentSwarm` for details.
+        """
+        from ursactl.core.agent_swarm import AgentSwarm as AgentSwarmClass
+
+        if not args and not kwargs:
+            # create an anonymous agent swarm and return it
+            return AgentSwarmClass.create_anonymous(project=self, app=self.app)
+
+        return AgentSwarmClass(*args, project_uuid=self.uuid, **kwargs)
+
     def agents(self):
         """
         Returns a generator listing all agents belonging to the project.
         """
         from ursactl.core.agent import Agent
 
         if self.uuid is None:
             return []
-        planning_client = client('planning', self.app)
+        planning_client = client("planning", self.app)
         return (
             Agent(client=planning_client, app=self.app, project=self, **info)
             for info in planning_client.list_agents(project_scope=self.uuid)
         )
 
     def agent(self, name):
         """
         Returns an agent with the given name.
         """
-        planning_client = client('planning', self.app)
+        planning_client = client("planning", self.app)
         info = planning_client.get_agent(name, project_uuid=self.uuid)
-        return self.Agent(uuid=info['id'], project=self, client=planning_client, app=self.app, **info)
+        return self.Agent(
+            uuid=info["id"], project=self, client=planning_client, app=self.app, **info
+        )
+
+    def agent_swarms(self):
+        """
+        Returns a generator listing all agent swarms belonging to the project.
+        """
+        from ursactl.core.agent_swarm import AgentSwarm
+
+        if self.uuid is None:
+            return []
+        planning_client = client("planning", self.app)
+        return (
+            AgentSwarm(client=planning_client, app=self.app, project=self, **info)
+            for info in planning_client.list_agent_swarms(project_scope=self.uuid)
+        )
+
+    def agent_swarm(self, name):
+        """
+        Returns an agent swarm with the given name.
+        """
+        planning_client = client("planning", self.app)
+        info = planning_client.get_agent_swarm(name, project_uuid=self.uuid)
+        return self.AgentSwarm(
+            uuid=info["id"], project=self, client=planning_client, app=self.app, **info
+        )
 
     def Dataset(self, *args, **kwargs):
         """
         Convenience method to create a dataset object with the project scope.
 
         See :class:`ursactl.core.dataset.Dataset` for details.
         """
@@ -92,15 +133,15 @@
         """
         Returns a generator listing all datasets belonging to the project.
         """
         from ursactl.core.dataset import Dataset
 
         if self.uuid is None:
             return []
-        dss_client = client('dss', self.app)
+        dss_client = client("dss", self.app)
         return (
             Dataset(client=dss_client, app=self.app, project=self, **info)
             for info in dss_client.list_datasets(project_scope=self.uuid)
         )
 
     def Pipeline(self, *args, **kwargs):
         """
@@ -116,33 +157,33 @@
         """
         Returns a generator listing all pipelines belonging to the project.
         """
         from ursactl.core.pipeline import Pipeline
 
         if self.uuid is None:
             return []
-        ape_client = client('ape', self.app)
+        ape_client = client("ape", self.app)
         return (
             Pipeline(client=ape_client, app=self.app, project=self, **info)
             for info in ape_client.list_pipelines(project_scope=self.uuid)
         )
 
     def pipeline(self, path):
         """
         Returns a pipeline with the given path.
         """
-        ape_client = client('ape', self.app)
+        ape_client = client("ape", self.app)
         info = ape_client.get_pipeline(path=path, project_uuid=self.uuid)
-        return self.Pipeline(uuid=info['id'], client=ape_client, app=self.app, **info)
+        return self.Pipeline(uuid=info["id"], client=ape_client, app=self.app, **info)
 
     @property
     def _data(self):
         if self._cached_data is None:
             if self.uuid is None:
                 self._cached_data = {
-                    'name': None,
-                    'description': None,
-                    'isArchived': None
+                    "name": None,
+                    "description": None,
+                    "isArchived": None,
                 }
             else:
                 self._cached_data = self.client.get_project_details(self.uuid)
         return self._cached_data
```

### Comparing `ursactl-0.8.3/ursactl/core/running_agent.py` & `ursactl-0.9.0/ursactl/core/running_agent.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/core/services/__init__.py` & `ursactl-0.9.0/ursactl/core/services/__init__.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/core/services/_base.py` & `ursactl-0.9.0/ursactl/core/services/_base.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/core/services/ape_client.py` & `ursactl-0.9.0/ursactl/core/services/ape_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/core/services/dss_client.py` & `ursactl-0.9.0/ursactl/core/services/dss_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/core/services/iam_client.py` & `ursactl-0.9.0/ursactl/core/services/iam_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/core/services/page_client.py` & `ursactl-0.9.0/ursactl/core/services/page_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/core/services/planning_client.py` & `ursactl-0.9.0/ursactl/core/services/planning_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 Planning capabilities client.
 """
+
 import json
 
-from ._base import Base
 from ursactl.core.exc import UrsaBadProjectName
 
+from ._base import Base
+
 LIST_PACKAGES_QUERY = """\
 query list_packages($id: String!) {
     project(handleName: $id) {
         packages {
             id
             name
             isSynced
@@ -26,14 +28,25 @@
             name
             isSynced
         }
     }
 }
 """
 
+LIST_AGENT_SWARMS_QUERY = """\
+query list_packages($id: String!) {
+    project(handleName: $id) {
+        agent_swarms {
+            id
+            name
+        }
+    }
+}
+"""
+
 CREATE_PACKAGE_MUTATION = """\
 mutation create_package($input: CreatePackageInput!) {
     createPackage(input: $input) {
         errors {
             code
             message
             fields
@@ -210,14 +223,34 @@
     agent(id: $id) {
         id
         name
     }
 }
 """
 
+GET_AGENT_SWARM_BY_NAME = """\
+query get_agent_swarm($name: String!, $project_id: String!) {
+    project(handleName: $project_id) {
+        agentSwarms(limit: 1, filter: { name: { eq: $name } }) {
+            id
+            name
+        }
+    }
+}
+"""
+
+GET_AGENT_SWARM_BY_ID = """\
+query get_agent_swarm($id: ID!) {
+    agentSwarm(id: $id) {
+        id
+        name
+    }
+}
+"""
+
 RUN_AGENT_MUTATION = """\
 mutation run_agent($input: RunAgentInput!) {
     runAgent(input: $input) {
         errors {
             code
             message
             fields
@@ -240,14 +273,58 @@
         result {
             id
         }
     }
 }
 """
 
+CREATE_AGENT_SWARM_MUTATION = """\
+mutation create_agent_swarm($input: CreateAgentSwarmInput!) {
+    createAgentSwarm(input: $input) {
+        errors {
+            code
+            message
+            fields
+        }
+        result {
+            id
+        }
+    }
+}
+"""
+
+DELETE_AGENT_SWARM_MUTATION = """\
+mutation delete_agent_swarm($id: ID!) {
+    deleteAgentSwarm(id: $id) {
+        errors {
+            code
+            message
+            fields
+        }
+        result {
+            id
+            name
+        }
+    }
+}
+"""
+
+RUN_AGENTS_IN_SWARM_MUTATION = """\
+mutation run_agents_in_swarm($agentSwarmId: ID!, $agent: String!, $groups: [String], $params: [AgentState]) {
+    runAgentsInSwarm(agent: $agent, agentSwarmId: $agentSwarmId, groups: $groups, params: $params) {
+        errors {
+            code
+            message
+            fields
+        }
+        result
+    }
+}
+"""
+
 LIST_RUNNING_AGENTS_BY_PROJECT = """\
 query list_agents_by_project($id: String!) {
     project(handleName: $id) {
         agents {
             name
             runningAgents {
                 id
@@ -269,15 +346,15 @@
             status
         }
     }
 }
 """
 
 SEND_EVENT_TO_AGENT_MUTATION = """\
-mutation send_event($agentId: ID!, $domain:String!, $name:String!, $params:Json!) {
+mutation send_event($agentId: ID!, $domain: String!, $name: String!, $params: Json!) {
   sendEventToAgent(agentId:$agentId,domain:$domain,name:$name,params:$params) {
     errors {
         code
         message
         fields
     }
     result {
@@ -285,288 +362,375 @@
         name
         params
     }
   }
 }
 """
 
+SEND_EVENT_TO_AGENT_SWARM_MUTATION = """\
+        mutation send_event($agentSwarmId: ID!, $domain: String!, $name: String!, $params: Json!, $group: String) {
+  sendEventToAgentSwarm(agentSwarmId:$agentSwarmId,domain:$domain,name:$name,params:$params,group:$group) {
+    errors {
+        code
+        message
+        fields
+    }
+    result {
+        domain
+        name
+        params
+    }
+  }
+}
+"""
+
 
 class PlanningClient(Base):
     """-
     Client providing access to the planning capabilities.
     """
+
     def list_packages(self, project_uuid=None):
         """
         Return a list of available packages.
         """
 
-        query_response = self.raw_query(query=LIST_PACKAGES_QUERY, variables={
-            'id': project_uuid
-        })
-        if query_response['data']['project'] is None:
+        query_response = self.raw_query(
+            query=LIST_PACKAGES_QUERY, variables={"id": project_uuid}
+        )
+        if query_response["data"]["project"] is None:
             raise UrsaBadProjectName(project_uuid)
-        return query_response['data']['project']['packages']
+        return query_response["data"]["project"]["packages"]
 
     def list_agents(self, project_uuid=None):
         """
         Return a list of available agents.
         """
-        query_response = self.raw_query(query=LIST_AGENTS_QUERY, variables={
-            'id': project_uuid
-        })
-        if query_response['data']['project'] is None:
+        query_response = self.raw_query(
+            query=LIST_AGENTS_QUERY, variables={"id": project_uuid}
+        )
+        if query_response["data"]["project"] is None:
             raise UrsaBadProjectName(project_uuid)
-        return query_response['data']['project']['agents']
+        return query_response["data"]["project"]["agents"]
 
     def list_running_agents(self, agent_id=None, project_uuid=None):
         """
         Return a list of running agents.
         """
         if agent_id is not None:
             if self.is_uuid(agent_id):
-                variables = {'id': agent_id}
+                variables = {"id": agent_id}
             else:
                 agent = self.get_agent(agent_id, project_uuid)
                 if agent is None:
                     return []
-                variables = {'id': agent['id']}
-            query_response = self.raw_query(query=LIST_RUNNING_AGENTS_BY_AGENT, variables=variables)
-            agent_name = query_response['data']['agent']['name']
-            return [{'agent': agent_name, **info} for info in query_response['data']['agent']['runningAgents']]
+                variables = {"id": agent["id"]}
+            query_response = self.raw_query(
+                query=LIST_RUNNING_AGENTS_BY_AGENT, variables=variables
+            )
+            agent_name = query_response["data"]["agent"]["name"]
+            return [
+                {"agent": agent_name, **info}
+                for info in query_response["data"]["agent"]["runningAgents"]
+            ]
 
         elif project_uuid is not None:
-            query_response = self.raw_query(query=LIST_RUNNING_AGENTS_BY_PROJECT, variables={
-                'id': project_uuid
-            })
-            if query_response['data']['project'] is None:
+            query_response = self.raw_query(
+                query=LIST_RUNNING_AGENTS_BY_PROJECT, variables={"id": project_uuid}
+            )
+            if query_response["data"]["project"] is None:
                 raise UrsaBadProjectName(project_uuid)
             return [
-                {'agent': agent['name'], **info}
-                for agent in query_response['data']['project']['agents']
-                for info in agent['runningAgents']
+                {"agent": agent["name"], **info}
+                for agent in query_response["data"]["project"]["agents"]
+                for info in agent["runningAgents"]
             ]
 
+    def list_agent_swarms(self, project_uuid=None):
+        """
+        Return a list of available agents.
+        """
+        query_response = self.raw_query(
+            query=LIST_AGENT_SWARMS_QUERY, variables={"id": project_uuid}
+        )
+        if query_response["data"]["project"] is None:
+            raise UrsaBadProjectName(project_uuid)
+        return query_response["data"]["project"]["agent_swarms"]
+
     def create_package(self, project_uuid=None, content=None):
         """
         Create a new package.
         """
-        mutation_response = self.raw_query(query=CREATE_PACKAGE_MUTATION, variables={
-            'input': {
-                'source': content,
-                'project': project_uuid
-            }
-        })
-        return mutation_response['data']['createPackage']
+        mutation_response = self.raw_query(
+            query=CREATE_PACKAGE_MUTATION,
+            variables={"input": {"source": content, "project": project_uuid}},
+        )
+        return mutation_response["data"]["createPackage"]
 
     def sync_package(self, project_uuid=None, content=None):
         """
         Sync a new package.
         """
-        mutation_response = self.raw_query(query=SYNC_PACKAGE_MUTATION, variables={
-            'input': {
-                'source': content,
-                'project': project_uuid
-            }
-        })
-        return mutation_response['data']['syncPackage']
+        mutation_response = self.raw_query(
+            query=SYNC_PACKAGE_MUTATION,
+            variables={"input": {"source": content, "project": project_uuid}},
+        )
+        return mutation_response["data"]["syncPackage"]
 
     def update_package(self, project_uuid=None, content=None):
         """
         Update an existing package.
         """
-        mutation_response = self.raw_query(query=UPDATE_PACKAGE_MUTATION, variables={
-            'input': {
-                'source': content,
-                'project': project_uuid
-            }
-        })
-        return mutation_response['data']['updatePackage']
+        mutation_response = self.raw_query(
+            query=UPDATE_PACKAGE_MUTATION,
+            variables={"input": {"source": content, "project": project_uuid}},
+        )
+        return mutation_response["data"]["updatePackage"]
 
     def create_agent(self, project_uuid=None, name=None, packages=None, behaviors=None):
         """
         Create a new agent.
         """
-        mutation_response = self.raw_query(query=CREATE_AGENT_MUTATION, variables={
-            'input': {
-                'name': name,
-                'packages': packages,
-                'behaviors': behaviors,
-                'project': project_uuid
-            }
-        })
-        return mutation_response['data']['createAgent']
+        mutation_response = self.raw_query(
+            query=CREATE_AGENT_MUTATION,
+            variables={
+                "input": {
+                    "name": name,
+                    "packages": packages,
+                    "behaviors": behaviors,
+                    "project": project_uuid,
+                }
+            },
+        )
+        return mutation_response["data"]["createAgent"]
 
     def sync_agent(self, project_uuid=None, name=None, packages=None, behaviors=None):
         """
         Sync an agent.
         """
-        mutation_response = self.raw_query(query=SYNC_AGENT_MUTATION, variables={
-            'input': {
-                'name': name,
-                'packages': packages,
-                'behaviors': behaviors,
-                'project': project_uuid
-            }
-        })
-        return mutation_response['data']['syncAgent']
+        mutation_response = self.raw_query(
+            query=SYNC_AGENT_MUTATION,
+            variables={
+                "input": {
+                    "name": name,
+                    "packages": packages,
+                    "behaviors": behaviors,
+                    "project": project_uuid,
+                }
+            },
+        )
+        return mutation_response["data"]["syncAgent"]
+
+    def create_agent_swarm(self, project_uuid=None, name=None):
+        """
+        Create a new swarm.
+        """
+        mutation_response = self.raw_query(
+            query=CREATE_AGENT_SWARM_MUTATION,
+            variables={"input": {"name": name, "project": project_uuid}},
+        )
+        return mutation_response["data"]["createAgentSwarm"]
 
     def get_package(self, name=None, project_uuid=None):
         """
         Get the id and basic info about a package.
         """
         if self.is_uuid(name):
-            variables = {
-                'id': name
-            }
+            variables = {"id": name}
             query = GET_PACKAGE_BY_ID
         else:
-            variables = {
-                'name': name,
-                'project_id': project_uuid
-            }
+            variables = {"name": name, "project_id": project_uuid}
             query = GET_PACKAGE_BY_NAME
         result = self.raw_query(query=query, variables=variables)
         if query == GET_PACKAGE_BY_ID:
-            return result['data']['package']
-        else:
-            return result['data']['project']['packages'][0]
+            return result["data"]["package"]
+        return result["data"]["project"]["packages"][0]
 
     def get_agent(self, name=None, project_uuid=None):
         """
         Get the id and basic info about an agent.
         """
         if self.is_uuid(name):
-            variables = {
-                'id': name
-            }
+            variables = {"id": name}
             query = GET_AGENT_BY_ID
         else:
-            variables = {
-                'name': name,
-                'project_id': project_uuid
-            }
+            variables = {"name": name, "project_id": project_uuid}
             query = GET_AGENT_BY_NAME
         result = self.raw_query(query=query, variables=variables)
         if query == GET_AGENT_BY_ID:
-            return result['data']['agent']
+            return result["data"]["agent"]
+
+        return result["data"]["project"]["agents"][0]
+
+    def get_agent_swarm(self, name=None, project_uuid=None):
+        """
+        Get the id and basic info about an agent swarm.
+        """
+        if self.is_uuid(name):
+            variables = {"id": name}
+            query = GET_AGENT_SWARM_BY_ID
         else:
-            return result['data']['project']['agents'][0]
+            variables = {"name": name, "project_id": project_uuid}
+            query = GET_AGENT_SWARM_BY_NAME
+        result = self.raw_query(query=query, variables=variables)
+        if query == GET_AGENT_SWARM_BY_ID:
+            return result["data"]["agentSwarm"]
 
-    def delete_package(self, id, project_uuid=None):
+        return result["data"]["project"]["agentSwarms"][0]
+
+    def delete_package(self, package_id, project_uuid=None):
         """
         Deletes a package.
         """
-        if self.is_uuid(id):
-            variables = {
-                'id': id
-            }
+        if self.is_uuid(package_id):
+            variables = {"id": package_id}
         else:
-            package = self.get_package(name=id, project_uuid=project_uuid)
+            package = self.get_package(name=package_id, project_uuid=project_uuid)
             if package is None:
                 return {}
-            variables = {'id': package['id']}
+            variables = {"id": package["id"]}
 
         result = self.raw_query(query=DELETE_PACKAGE_MUTATION, variables=variables)
 
-        return result['data']['deletePackage']
+        return result["data"]["deletePackage"]
 
-    def delete_synced_package(self, id, project_uuid=None):
+    def delete_synced_package(self, package_id, project_uuid=None):
         """
         Deletes a synced package.
         """
-        if self.is_uuid(id):
-            variables = {
-                'id': id
-            }
+        if self.is_uuid(package_id):
+            variables = {"id": package_id}
         else:
-            package = self.get_package(name=id, project_uuid=project_uuid)
+            package = self.get_package(name=package_id, project_uuid=project_uuid)
             if package is None:
                 return {}
-            variables = {'id': package['id']}
+            variables = {"id": package["id"]}
 
-        result = self.raw_query(query=DELETE_SYNCED_PACKAGE_MUTATION, variables=variables)
+        result = self.raw_query(
+            query=DELETE_SYNCED_PACKAGE_MUTATION, variables=variables
+        )
 
-        return result['data']['deleteSyncedPackage']
+        return result["data"]["deleteSyncedPackage"]
 
-    def delete_agent(self, id, project_uuid=None):
+    def delete_agent(self, agent_id, project_uuid=None):
         """
         Deletes an agent.
         """
-        if self.is_uuid(id):
-            variables = {
-                'id': id
-            }
+        if self.is_uuid(agent_id):
+            variables = {"id": agent_id}
         else:
-            agent = self.get_agent(name=id, project_uuid=project_uuid)
+            agent = self.get_agent(name=agent_id, project_uuid=project_uuid)
             if agent is None:
                 return {}
-            variables = {'id': agent['id']}
+            variables = {"id": agent["id"]}
 
         result = self.raw_query(query=DELETE_AGENT_MUTATION, variables=variables)
 
-        return result['data']['deleteAgent']
+        return result["data"]["deleteAgent"]
 
-    def delete_synced_agent(self, id, project_uuid=None):
+    def delete_agent_swarm(self, agent_swarm_id, project_uuid=None):
+        """
+        Deletes an agent swarm.
+        """
+        if self.is_uuid(agent_swarm_id):
+            variables = {"id": agent_swarm_id}
+        else:
+            agent = self.get_agent_swarm(name=agent_swarm_id, project_uuid=project_uuid)
+            if agent is None:
+                return {}
+            variables = {"id": agent["id"]}
+
+        result = self.raw_query(query=DELETE_AGENT_SWARM_MUTATION, variables=variables)
+
+        return result["data"]["deleteAgentSwarm"]
+
+    def delete_synced_agent(self, agent_id, project_uuid=None):
         """
         Deletes a synced agent.
         """
-        if self.is_uuid(id):
-            variables = {
-                'id': id
-            }
+        if self.is_uuid(agent_id):
+            variables = {"id": agent_id}
         else:
-            agent = self.get_agent(name=id, project_uuid=project_uuid)
+            agent = self.get_agent(name=agent_id, project_uuid=project_uuid)
             if agent is None:
                 return {}
-            variables = {'id': agent['id']}
+            variables = {"id": agent["id"]}
 
         result = self.raw_query(query=DELETE_SYNCED_AGENT_MUTATION, variables=variables)
 
-        return result['data']['deleteSyncedAgent']
+        return result["data"]["deleteSyncedAgent"]
 
-    def run_agent(self, id, project_uuid=None, initial_predicates=None, initial_state=None):
+    def run_agent(
+        self, agent_id, project_uuid=None, initial_predicates=None, initial_state=None
+    ):
         """
         Runs an agent.
         """
-        variables = {'input': {'project': project_uuid}}
-        if self.is_uuid(id):
-            agent = self.get_agent(name=id, project_uuid=project_uuid)
+        variables = {"input": {"project": project_uuid}}
+        if self.is_uuid(agent_id):
+            agent = self.get_agent(name=agent_id, project_uuid=project_uuid)
             if agent is None:
                 return {}
-            variables['input']['agent'] = agent['name']
+            variables["input"]["agent"] = agent["name"]
         else:
-            agent = self.get_agent(name=id, project_uuid=project_uuid)
+            agent = self.get_agent(name=agent_id, project_uuid=project_uuid)
             if agent is None:
                 return {}
-            variables['input']['agent'] = id
+            variables["input"]["agent"] = agent_id
 
         if initial_state is not None:
-            variables['input']['initialState'] = initial_state
+            variables["input"]["initialState"] = initial_state
         if initial_predicates is not None:
-            variables['input']['initialPredicates'] = initial_predicates
+            variables["input"]["initialPredicates"] = initial_predicates
 
         result = self.raw_query(query=RUN_AGENT_MUTATION, variables=variables)
 
-        return result['data']['runAgent']
+        return result["data"]["runAgent"]
+
+    def run_agents_in_swarm(self, agent_swarm_id, agent_name, configs, groups=[]):
+        """
+        Runs agents in an agent swarm.
+        """
+        variables = {
+            "agent": agent_name,
+            "agentSwarmId": agent_swarm_id,
+            "params": configs,
+        }
+        if groups:
+            variables["groups"] = groups
+        result = self.raw_query(query=RUN_AGENTS_IN_SWARM_MUTATION, variables=variables)
+
+        return result["data"]["runAgentsInSwarm"]
 
     def send_event_to_agent(self, agent_instance_id, event):
         """
         Sends an event to an agent.
         """
-        variables = {'agentId': agent_instance_id, **event}
-        variables['params'] = json.dumps(variables['params'])
+        variables = {"agentId": agent_instance_id, **event}
+        variables["params"] = json.dumps(variables["params"])
 
         result = self.raw_query(query=SEND_EVENT_TO_AGENT_MUTATION, variables=variables)
 
-        return result['data']['sendEventToAgent']
+        return result["data"]["sendEventToAgent"]
 
-    def stop_agent(self, id):
+    def stop_agent(self, agent_id):
         """
         Stops an agent.
         """
-        variables = {
-            'id': id
-        }
+        variables = {"id": agent_id}
 
         result = self.raw_query(query=STOP_AGENT_MUTATION, variables=variables)
 
-        return result['data']['stopAgent']
+        return result["data"]["stopAgent"]
+
+    def send_event_to_agent_swarm(self, agent_swarm_id, event):
+        """
+        Sends an event to an agent swarm.
+        """
+        variables = {"agentSwarmId": agent_swarm_id, **event}
+        variables["params"] = json.dumps(variables["params"])
+
+        result = self.raw_query(
+            query=SEND_EVENT_TO_AGENT_SWARM_MUTATION, variables=variables
+        )
+
+        return result["data"]["sendEventToAgentSwarm"]
```

### Comparing `ursactl-0.8.3/ursactl/core/services/project_client.py` & `ursactl-0.9.0/ursactl/core/services/project_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/core/utils/magic.py` & `ursactl-0.9.0/ursactl/core/utils/magic.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.8.3/ursactl/main.py` & `ursactl-0.9.0/ursactl/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,112 +1,137 @@
+import configparser
 import os
+from pathlib import Path
 
 from cement import App, TestApp, init_defaults
 from cement.core.exc import CaughtSignal
 from cement.utils import fs
-from pathlib import Path
-from tinydb import TinyDB
 from requests.exceptions import ConnectionError
+from tinydb import TinyDB
 
 from .controllers.base import Base
 from .controllers.create import Create
 from .controllers.delete import Delete
 from .controllers.get import Get
 from .controllers.init import Init
 from .controllers.list import List
 from .controllers.refresh import Refresh
 from .controllers.run import Run
 from .controllers.send import Send
 from .controllers.show import Show
 from .controllers.stop import Stop
 from .controllers.sync import Sync
 from .controllers.update import Update
-from .core.exc import UrsaCtlError, UrsaBadProjectName
+from .core.exc import UrsaBadProjectName, UrsaCtlError
 
 # configuration defaults
-CONFIG = init_defaults('ursactl')
-CONFIG['ursactl']['cache_file'] = '~/.ursactl/.cache'
-CONFIG['ursactl']['platform'] = 'https://app.ursafrontier.cloud/'
+CONFIG = init_defaults("ursactl")
+CONFIG["ursactl"]["cache_file"] = "~/.ursactl/.cache"
+CONFIG["ursactl"]["platform"] = "https://app.ursafrontier.cloud/"
 
 
 def extend_cache(app):
-    app.log.info('extending with cache')
-    db_file = app.config.get('ursactl', 'cache_file')
+    app.log.info("extending with cache")
+    db_file = app.config.get("ursactl", "cache_file")
 
     # ensure that we expand the full path
     db_file = fs.abspath(db_file)
-    app.log.info('cache file is: %s' % db_file)
+    app.log.info("cache file is: %s" % db_file)
 
     # ensure our parent directory exists
     db_dir = os.path.dirname(db_file)
     if not os.path.exists(db_dir):
         os.makedirs(db_dir)
 
-    app.extend('db', TinyDB(db_file))
+    app.extend("db", TinyDB(db_file))
 
 
 def exploded_paths():
     """
     Returns a list of directories based on the current working directory.
     Doesn't go past the home directory, if under the home directory.
     """
     cwd = os.getcwd()
     parts = cwd.split(os.path.sep)
     paths = []
     homedir = str(Path.home())
 
     for i in range(len(parts)):
-        paths.append(os.path.sep.join(parts[:i+1]))
-        paths.append(os.path.sep.join(parts[:i+1]) + '/config')
-        paths.append(os.path.sep.join(parts[:i+1]) + '/.config')
-        paths.append(os.path.sep.join(parts[:i+1]) + '/.ursactl')
+        paths.append(os.path.sep.join(parts[: i + 1]))
+        paths.append(os.path.sep.join(parts[: i + 1]) + "/config")
+        paths.append(os.path.sep.join(parts[: i + 1]) + "/.config")
+        paths.append(os.path.sep.join(parts[: i + 1]) + "/.ursactl")
 
     if any((path.startswith(homedir) for path in paths)):
         paths = [path for path in paths if path.startswith(homedir)]
 
     return paths
 
 
+def find_config_files():
+    """
+    Returns a list of directories based on the current working directory.
+    Doesn't go past the home directory, if under the home directory.
+    """
+    cwd = os.getcwd()
+    parts = cwd.split(os.path.sep)
+    paths = []
+    homedir = str(Path.home())
+
+    for i in range(len(parts)):
+        paths.append(os.path.sep.join(parts[: i + 1]))
+        paths.append(os.path.sep.join(parts[: i + 1]) + "/config")
+        paths.append(os.path.sep.join(parts[: i + 1]) + "/.config")
+        paths.append(os.path.sep.join(parts[: i + 1]) + "/.ursactl")
+
+    if any((path.startswith(homedir) for path in paths)):
+        paths = [path for path in paths if path.startswith(homedir)]
+
+    files = [
+        file
+        for file in [os.path.sep.join([path, "ursactl.conf"]) for path in paths]
+        if os.path.isfile(file)
+    ]
+
+    return files
+
+
 class UrsaCtl(App):
     """Ursa Frontier Control primary application."""
 
     class Meta:
-        label = 'ursactl'
+        label = "ursactl"
 
         # configuration defaults
         config_defaults = CONFIG
 
         # call sys.exit() on close
         exit_on_close = True
 
         # load additional framework extensions
-        extensions = [
-            'configparser',
-            'colorlog',
-            'tabulate'
-        ]
+        extensions = ["configparser", "colorlog", "tabulate"]
 
-        hooks = [
-            ('post_setup', extend_cache)
-        ]
+        hooks = [("post_setup", extend_cache)]
 
         # configuration handler
-        config_handler = 'configparser'
+        config_handler = "configparser"
 
         # configuration file suffix
-        config_file_suffix = '.conf'
+        config_file_suffix = "ursactl.conf"
 
         # configuration directories
         config_dirs = exploded_paths()
 
+        # config_files = find_config_files()
+
         # set the log handler
-        log_handler = 'colorlog'
+        log_handler = "colorlog"
 
         # set the output handler
-        output_handler = 'tabulate'
+        output_handler = "tabulate"
 
         # register handlers
         handlers = [
             Base,
             Update,
             Sync,
             Stop,
@@ -114,63 +139,70 @@
             Send,
             Run,
             Refresh,
             List,
             Init,
             Get,
             Delete,
-            Create
+            Create,
         ]
 
 
 class UrsaCtlTest(TestApp, UrsaCtl):
     """A sub-class of UrsaCtl that is better suited for testing."""
 
     class Meta:
-        label = 'ursactl'
+        label = "ursactl"
 
     def rebuild_cache(self):
-        delattr(self, 'db')
+        delattr(self, "db")
         extend_cache(self)
 
 
-def main():
+def main():  # noqa: C901
     with UrsaCtl() as app:
         try:
             app.run()
 
         except AssertionError as e:
-            print('AssertionError > %s' % e.args[0])
+            print("AssertionError > %s" % e.args[0])
             app.exit_code = 1
 
             if app.debug is True:
                 import traceback
+
                 traceback.print_exc()
 
         except UrsaBadProjectName as e:
             print("The project '%s' is not a valid project name" % e.args[0])
             app.exit_code = 1
 
             if app.debug is True:
                 import traceback
+
                 traceback.print_exc()
 
         except UrsaCtlError as e:
-            print('UrsaCtlError > %s' % e.args[0])
+            print("UrsaCtlError > %s" % e.args[0])
             app.exit_code = 1
 
             if app.debug is True:
                 import traceback
+
                 traceback.print_exc()
 
         except CaughtSignal as e:
             # Default Cement signals are SIGINT and SIGTERM, exit 0 (non-error)
-            print('\n%s' % e)
+            print("\n%s" % e)
             app.exit_code = 0
 
+        except configparser.NoOptionError as e:
+            print("\n%s" % e)
+            app.exit_code = 1
+
         except ConnectionError:
-            print('Unable to connect to server')
+            print("Unable to connect to server")
             app.exit_code = 1
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `ursactl-0.8.3/ursactl.egg-info/PKG-INFO` & `ursactl-0.9.0/ursactl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ursactl
-Version: 0.8.3
+Version: 0.9.0
 Summary: command line tool and library for intercting with ursafrontier.cloud
 Home-page: https://ursafrontier.cloud/
 Author: Ursa Frontier LLC
 Author-email: contact@ursafrontier.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `ursactl-0.8.3/ursactl.egg-info/SOURCES.txt` & `ursactl-0.9.0/ursactl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 ursactl/controllers/update.py
 ursactl/controllers/utils/__init__.py
 ursactl/controllers/utils/pages.py
 ursactl/controllers/utils/transforms.py
 ursactl/core/__init__.py
 ursactl/core/_base.py
 ursactl/core/agent.py
+ursactl/core/agent_swarm.py
 ursactl/core/dataset.py
 ursactl/core/exc.py
 ursactl/core/pipeline.py
 ursactl/core/pipeline_run.py
 ursactl/core/pipeline_sweep.py
 ursactl/core/project.py
 ursactl/core/running_agent.py
```

