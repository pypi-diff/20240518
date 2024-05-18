# Comparing `tmp/arikaim-0.5.8.tar.gz` & `tmp/arikaim-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arikaim-0.5.8.tar", last modified: Sun May 12 10:45:23 2024, max compression
+gzip compressed data, was "arikaim-0.5.9.tar", last modified: Tue May 14 09:46:57 2024, max compression
```

## Comparing `arikaim-0.5.8.tar` & `arikaim-0.5.9.tar`

### file list

```diff
@@ -1,62 +1,61 @@
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:45:23.011574 arikaim-0.5.8/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      872 2024-05-12 10:45:23.011574 arikaim-0.5.8/PKG-INFO
--rwxr-xr-x   0 theuser   (1000) theuser   (1000)      315 2024-05-12 08:20:51.000000 arikaim-0.5.8/README.md
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:45:23.007574 arikaim-0.5.8/arikaim/
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:45:23.007574 arikaim-0.5.8/arikaim/core/
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:45:23.007574 arikaim-0.5.8/arikaim/core/access/
--rw-r--r--   0 theuser   (1000) theuser   (1000)     2661 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/access/access.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)       88 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/access/auth_error.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:45:23.011574 arikaim-0.5.8/arikaim/core/access/middleware/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      745 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/access/middleware/multiple.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:45:23.011574 arikaim-0.5.8/arikaim/core/access/providers/
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1644 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/access/providers/php_session.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      590 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/access/providers/token.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:45:23.011574 arikaim-0.5.8/arikaim/core/admin/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      907 2024-02-23 19:30:58.000000 arikaim-0.5.8/arikaim/core/admin/admin.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:45:23.011574 arikaim-0.5.8/arikaim/core/admin/controllers/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      416 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/admin/controllers/info.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      421 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/admin/controllers/service.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1206 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/admin/controllers/service_route.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1036 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/admin/controllers/service_routes.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      299 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/admin/controllers/services_list.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1023 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/api_descriptor.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     5280 2024-05-12 10:42:36.000000 arikaim-0.5.8/arikaim/core/app.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:45:23.011574 arikaim-0.5.8/arikaim/core/collection/
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1670 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/collection/property.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:45:23.011574 arikaim-0.5.8/arikaim/core/console/
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1291 2024-05-12 10:31:18.000000 arikaim-0.5.8/arikaim/core/console/app.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      662 2024-05-12 10:32:04.000000 arikaim-0.5.8/arikaim/core/console/config.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      774 2024-05-12 10:32:24.000000 arikaim-0.5.8/arikaim/core/console/install.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      257 2024-05-12 10:33:05.000000 arikaim-0.5.8/arikaim/core/console/packages.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:45:23.011574 arikaim-0.5.8/arikaim/core/console/templates/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      386 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/console/templates/config_file.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1041 2024-05-12 07:52:57.000000 arikaim-0.5.8/arikaim/core/container.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     2725 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/controller.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:45:23.011574 arikaim-0.5.8/arikaim/core/db/
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1077 2024-02-23 19:35:44.000000 arikaim-0.5.8/arikaim/core/db/db.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:45:23.011574 arikaim-0.5.8/arikaim/core/db/models/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      465 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/db/models/access_tokens.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      916 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/db/models/jobs.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      496 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/db/models/permission_relations.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      454 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/db/models/permissions.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      509 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/db/models/users.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      649 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/errors.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      239 2024-05-11 11:03:31.000000 arikaim-0.5.8/arikaim/core/logger.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      927 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/packages.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1453 2024-05-11 11:13:22.000000 arikaim-0.5.8/arikaim/core/path.py
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:45:23.011574 arikaim-0.5.8/arikaim/core/queue/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      282 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/queue/job.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1980 2024-02-21 20:29:02.000000 arikaim-0.5.8/arikaim/core/queue/queue.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)      443 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/response.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1455 2024-05-12 10:45:05.000000 arikaim-0.5.8/arikaim/core/server.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1702 2024-02-21 16:41:47.000000 arikaim-0.5.8/arikaim/core/service.py
--rw-r--r--   0 theuser   (1000) theuser   (1000)     2466 2024-05-12 07:12:38.000000 arikaim-0.5.8/arikaim/core/utils.py
--rwxr-xr-x   0 theuser   (1000) theuser   (1000)      109 2024-05-11 11:14:09.000000 arikaim-0.5.8/arikaim-server
-drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-12 10:45:23.011574 arikaim-0.5.8/arikaim.egg-info/
--rw-r--r--   0 theuser   (1000) theuser   (1000)      872 2024-05-12 10:45:22.000000 arikaim-0.5.8/arikaim.egg-info/PKG-INFO
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1392 2024-05-12 10:45:23.000000 arikaim-0.5.8/arikaim.egg-info/SOURCES.txt
--rw-r--r--   0 theuser   (1000) theuser   (1000)        1 2024-05-12 10:45:22.000000 arikaim-0.5.8/arikaim.egg-info/dependency_links.txt
--rw-r--r--   0 theuser   (1000) theuser   (1000)      112 2024-05-12 10:45:22.000000 arikaim-0.5.8/arikaim.egg-info/requires.txt
--rw-r--r--   0 theuser   (1000) theuser   (1000)        8 2024-05-12 10:45:22.000000 arikaim-0.5.8/arikaim.egg-info/top_level.txt
--rw-r--r--   0 theuser   (1000) theuser   (1000)       38 2024-05-12 10:45:23.011574 arikaim-0.5.8/setup.cfg
--rw-r--r--   0 theuser   (1000) theuser   (1000)     1832 2024-05-12 10:44:51.000000 arikaim-0.5.8/setup.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-14 09:46:57.414443 arikaim-0.5.9/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      872 2024-05-14 09:46:57.414443 arikaim-0.5.9/PKG-INFO
+-rwxr-xr-x   0 theuser   (1000) theuser   (1000)      315 2024-05-12 08:20:51.000000 arikaim-0.5.9/README.md
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-14 09:46:57.406443 arikaim-0.5.9/arikaim/
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-14 09:46:57.410443 arikaim-0.5.9/arikaim/core/
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-14 09:46:57.410443 arikaim-0.5.9/arikaim/core/access/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     2661 2024-02-21 16:41:47.000000 arikaim-0.5.9/arikaim/core/access/access.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)       88 2024-02-21 16:41:47.000000 arikaim-0.5.9/arikaim/core/access/auth_error.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-14 09:46:57.410443 arikaim-0.5.9/arikaim/core/access/middleware/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      745 2024-02-21 16:41:47.000000 arikaim-0.5.9/arikaim/core/access/middleware/multiple.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-14 09:46:57.410443 arikaim-0.5.9/arikaim/core/access/providers/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1850 2024-05-14 06:21:21.000000 arikaim-0.5.9/arikaim/core/access/providers/php_session.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      590 2024-02-21 16:41:47.000000 arikaim-0.5.9/arikaim/core/access/providers/token.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-14 09:46:57.410443 arikaim-0.5.9/arikaim/core/admin/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      660 2024-05-14 07:00:18.000000 arikaim-0.5.9/arikaim/core/admin/admin.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-14 09:46:57.410443 arikaim-0.5.9/arikaim/core/admin/controllers/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      500 2024-05-14 06:58:24.000000 arikaim-0.5.9/arikaim/core/admin/controllers/service.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1181 2024-05-14 06:58:39.000000 arikaim-0.5.9/arikaim/core/admin/controllers/service_route.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1118 2024-05-14 06:47:42.000000 arikaim-0.5.9/arikaim/core/admin/controllers/service_routes.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      293 2024-05-14 06:28:22.000000 arikaim-0.5.9/arikaim/core/admin/controllers/services_list.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1023 2024-02-21 16:41:47.000000 arikaim-0.5.9/arikaim/core/api_descriptor.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     5283 2024-05-14 06:18:10.000000 arikaim-0.5.9/arikaim/core/app.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-14 09:46:57.414443 arikaim-0.5.9/arikaim/core/collection/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1792 2024-05-14 07:33:49.000000 arikaim-0.5.9/arikaim/core/collection/property.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-14 09:46:57.414443 arikaim-0.5.9/arikaim/core/console/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1291 2024-05-12 10:31:18.000000 arikaim-0.5.9/arikaim/core/console/app.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      662 2024-05-12 10:32:04.000000 arikaim-0.5.9/arikaim/core/console/config.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      774 2024-05-12 10:32:24.000000 arikaim-0.5.9/arikaim/core/console/install.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      257 2024-05-12 10:33:05.000000 arikaim-0.5.9/arikaim/core/console/packages.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-14 09:46:57.414443 arikaim-0.5.9/arikaim/core/console/templates/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      386 2024-02-21 16:41:47.000000 arikaim-0.5.9/arikaim/core/console/templates/config_file.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1041 2024-05-12 07:52:57.000000 arikaim-0.5.9/arikaim/core/container.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     2725 2024-05-14 07:16:13.000000 arikaim-0.5.9/arikaim/core/controller.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-14 09:46:57.414443 arikaim-0.5.9/arikaim/core/db/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1077 2024-02-23 19:35:44.000000 arikaim-0.5.9/arikaim/core/db/db.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-14 09:46:57.414443 arikaim-0.5.9/arikaim/core/db/models/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      465 2024-02-21 16:41:47.000000 arikaim-0.5.9/arikaim/core/db/models/access_tokens.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      916 2024-02-21 16:41:47.000000 arikaim-0.5.9/arikaim/core/db/models/jobs.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      496 2024-02-21 16:41:47.000000 arikaim-0.5.9/arikaim/core/db/models/permission_relations.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      454 2024-02-21 16:41:47.000000 arikaim-0.5.9/arikaim/core/db/models/permissions.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      509 2024-02-21 16:41:47.000000 arikaim-0.5.9/arikaim/core/db/models/users.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      649 2024-02-21 16:41:47.000000 arikaim-0.5.9/arikaim/core/errors.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      239 2024-05-11 11:03:31.000000 arikaim-0.5.9/arikaim/core/logger.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      927 2024-02-21 16:41:47.000000 arikaim-0.5.9/arikaim/core/packages.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1453 2024-05-11 11:13:22.000000 arikaim-0.5.9/arikaim/core/path.py
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-14 09:46:57.414443 arikaim-0.5.9/arikaim/core/queue/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      282 2024-02-21 16:41:47.000000 arikaim-0.5.9/arikaim/core/queue/job.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1980 2024-02-21 20:29:02.000000 arikaim-0.5.9/arikaim/core/queue/queue.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      443 2024-02-21 16:41:47.000000 arikaim-0.5.9/arikaim/core/response.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1455 2024-05-14 09:46:07.000000 arikaim-0.5.9/arikaim/core/server.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1702 2024-02-21 16:41:47.000000 arikaim-0.5.9/arikaim/core/service.py
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     2466 2024-05-12 07:12:38.000000 arikaim-0.5.9/arikaim/core/utils.py
+-rwxr-xr-x   0 theuser   (1000) theuser   (1000)      109 2024-05-11 11:14:09.000000 arikaim-0.5.9/arikaim-server
+drwxr-xr-x   0 theuser   (1000) theuser   (1000)        0 2024-05-14 09:46:57.414443 arikaim-0.5.9/arikaim.egg-info/
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      872 2024-05-14 09:46:57.000000 arikaim-0.5.9/arikaim.egg-info/PKG-INFO
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1353 2024-05-14 09:46:57.000000 arikaim-0.5.9/arikaim.egg-info/SOURCES.txt
+-rw-r--r--   0 theuser   (1000) theuser   (1000)        1 2024-05-14 09:46:57.000000 arikaim-0.5.9/arikaim.egg-info/dependency_links.txt
+-rw-r--r--   0 theuser   (1000) theuser   (1000)      112 2024-05-14 09:46:57.000000 arikaim-0.5.9/arikaim.egg-info/requires.txt
+-rw-r--r--   0 theuser   (1000) theuser   (1000)        8 2024-05-14 09:46:57.000000 arikaim-0.5.9/arikaim.egg-info/top_level.txt
+-rw-r--r--   0 theuser   (1000) theuser   (1000)       38 2024-05-14 09:46:57.414443 arikaim-0.5.9/setup.cfg
+-rw-r--r--   0 theuser   (1000) theuser   (1000)     1832 2024-05-14 09:46:32.000000 arikaim-0.5.9/setup.py
```

### Comparing `arikaim-0.5.8/PKG-INFO` & `arikaim-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arikaim
-Version: 0.5.8
+Version: 0.5.9
 Summary: Arikaim services server
 Home-page: https://github.com/arikaim/arikaim-services-server.git
 Download-URL: 
 Author: Intersoft Ltd
 Author-email: info@arikaim.com
 License: MIT License
 Keywords: arikaim
```

### Comparing `arikaim-0.5.8/arikaim/core/access/access.py` & `arikaim-0.5.9/arikaim/core/access/access.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.8/arikaim/core/access/middleware/multiple.py` & `arikaim-0.5.9/arikaim/core/access/middleware/multiple.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.8/arikaim/core/access/providers/php_session.py` & `arikaim-0.5.9/arikaim/core/access/providers/php_session.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from os.path import exists
 import subprocess
 import json
-import arikaim.core.globals as globals
 
 from arikaim.core.db.models.users import Users
 from arikaim.core.db.models.access_tokens import AccessTokens
 from arikaim.core.utils import php_unserialize
 from arikaim.core.logger import logger
+from arikaim.core.path import Path 
 
 class PhpSessionAuthProvider:
     
     def __init__(self):
         self._php_session_path = None
         self.resolve_session_path()
 
@@ -31,25 +31,32 @@
     def read_php_session(self, session_id):
         file_name = self._php_session_path + '/sess_' + session_id
 
         if exists(file_name) == False:
             return {}
       
         logger.info('Read php session file: ' + file_name)
-
-        file = open(file_name,'r')
-        content = file.read()
-        file.close()
+        try:
+            file = open(file_name,'r')
+            content = file.read()
+            file.close()
+        except IOError:
+            return False
         
         return php_unserialize(content)
     
     def resolve_session_path(self):
-        response = subprocess.Popen(
-            'php cli session:info --output json',
-            shell = True,
-            cwd = globals.ARIKAIM_PATH,
-            stdout = subprocess.PIPE          
-        )
-
-        json_text = response.stdout.read()
-        data = json.loads(json_text)
+        try:
+            response = subprocess.Popen(
+                'php cli session:info --output json',
+                shell = True,
+                cwd = Path.base(),
+                stdout = subprocess.PIPE          
+            )
+
+            json_text = response.stdout.read()
+            data = json.loads(json_text)
+        except BaseException:
+            self._php_session_path = None
+            return
+        
         self._php_session_path = data['save_path']
```

### Comparing `arikaim-0.5.8/arikaim/core/access/providers/token.py` & `arikaim-0.5.9/arikaim/core/access/providers/token.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.8/arikaim/core/admin/admin.py` & `arikaim-0.5.9/arikaim/core/admin/admin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,14 @@
-from arikaim.core.container import di
 from arikaim.core.service import Service
 from arikaim.core.admin.controllers.services_list import ServicesList
 from arikaim.core.admin.controllers.service import ServiceDescriptor
 from arikaim.core.admin.controllers.service_routes import ServiceRoutes
 from arikaim.core.admin.controllers.service_route import ServiceRoute
-from arikaim.core.admin.controllers.info import Info
 
 class AdminService(Service):
 
     def init_routes(self):
 
-        auth = di.get('access').middleware('multiple',['token','php_session'])
-        self.add_auth_middleware(auth)
-
-        self.add_route(["GET"],"/info",Info)
         self.add_route(["GET"],"/services",ServicesList)
-        self.add_route(["GET"],"/service/{name}",ServiceDescriptor)
+        self.add_route(["GET"],"/service/details/{name}",ServiceDescriptor)
         self.add_route(["GET"],"/service/routes/{name}",ServiceRoutes)
         self.add_route(["GET"],"/service/route/{name}/{path}",ServiceRoute)
```

### Comparing `arikaim-0.5.8/arikaim/core/admin/controllers/service_route.py` & `arikaim-0.5.9/arikaim/core/admin/controllers/service_route.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 from arikaim.core.container import di
 from arikaim.core.api_descriptor import *
 
 class ServiceRoute(Controller):
 
     @get
     async def get(self, request, data):  
-        app = di.get('app').app()
+        app = di.get('app')
         service = app.get_service(data['name'])
         path = data['path'].lstrip('/')
         result = {} 
+        
         for route in service.routes.routes:
-            if route.path.lstrip('/') == path:
+            service_path = service.mount + route.path
+            if service_path.lstrip('/') == path:
                 descriptor = get_descriptor(route.endpoint)
                 result = {
                     'title': descriptor.title,
                     'description': descriptor.description,
-                    'full_path': service.mount + route.path,     
-                    'path': route.path,
-                    'endpoint': route.name,
+                    'path': service_path,                         
+                    'name': route.name,
                     'methods': list(route.methods),
                     'params': descriptor.params,
                     'result': descriptor.result_fields          
                 }
                 break
 
         self.field('name',data['name'])
-        self.field('path',data['path'])
-        self.field('server_url',app.server_url)
+        self.field('path',data['path'])       
         self.field('route',result)
         self.message('Service route')
```

### Comparing `arikaim-0.5.8/arikaim/core/api_descriptor.py` & `arikaim-0.5.9/arikaim/core/api_descriptor.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.8/arikaim/core/app.py` & `arikaim-0.5.9/arikaim/core/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
         di.get('db').close()
         logger.info('Db connection closed')
 
     def load_admin_routes(self):
         logger.info('Load admin routes')
 
-        admin = AdminService('admin')
+        admin = AdminService('admin','')
         admin.init_routes()
 
         self._routes.append(admin.routes)
 
     def boot_services(self, load_routes: bool = True, init_container: bool = True):
       
         for service_name in self._services:
```

### Comparing `arikaim-0.5.8/arikaim/core/collection/property.py` & `arikaim-0.5.9/arikaim/core/collection/property.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,31 +22,38 @@
         self._name = name
         self._title = ''
         self._description = ''
         self._type = 'text'
         self._readonly = False
         self._required = False
         self._value = None
-        
+        self._default = None
+
         if type(data) is dict:
             for key in data:
                 setattr(self,key,data[key])
 
+
     def to_json(self):
         return {
             'name': self._name,
             'description': self._description,
             'type': self._type,
             'readonly': self._readonly,
             'value': self._value,
+            'default': self._default,
             'required': self._required,
             'title': self._title
         }
        
-    def value(self, value: str):
+    def default(self, value):
+        self._default = value
+        return self
+    
+    def value(self, value):
         self._value = value
         return self
     
     def title(self, value: str):
         self._title = value
         return self
     
@@ -58,15 +65,15 @@
         return self
     
     def readonly(self, value: bool):
         self._readonly = value
         return self
     
     def type(self, type_name: str):
-        self._type = self.get_type_id(type_name)
+        self._type = type_name
         return self
     
     def get_type_id(self, type_name: str):
         try: 
             return self.TYPE_NAMES.index(type_name) 
         except ValueError: 
             return None
```

### Comparing `arikaim-0.5.8/arikaim/core/console/app.py` & `arikaim-0.5.9/arikaim/core/console/app.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.8/arikaim/core/console/config.py` & `arikaim-0.5.9/arikaim/core/console/config.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.8/arikaim/core/console/install.py` & `arikaim-0.5.9/arikaim/core/console/install.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.8/arikaim/core/container.py` & `arikaim-0.5.9/arikaim/core/container.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.8/arikaim/core/controller.py` & `arikaim-0.5.9/arikaim/core/controller.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.8/arikaim/core/db/db.py` & `arikaim-0.5.9/arikaim/core/db/db.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.8/arikaim/core/db/models/jobs.py` & `arikaim-0.5.9/arikaim/core/db/models/jobs.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.8/arikaim/core/errors.py` & `arikaim-0.5.9/arikaim/core/errors.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.8/arikaim/core/packages.py` & `arikaim-0.5.9/arikaim/core/packages.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.8/arikaim/core/path.py` & `arikaim-0.5.9/arikaim/core/path.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.8/arikaim/core/queue/queue.py` & `arikaim-0.5.9/arikaim/core/queue/queue.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.8/arikaim/core/server.py` & `arikaim-0.5.9/arikaim/core/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from arikaim.core.utils import *
 from arikaim.core.app import app
 
 class ArikaimServer:
     _instance = None
 
     def __init__(self,config):
-        self._version = '0.5.8'
+        self._version = '0.5.9'
         self._config = config
         
     def run(self, reload = False, path = None):
         if path is not None:          
             Path.base_path = path
             logger.info('Project path ' + Path.base())
```

### Comparing `arikaim-0.5.8/arikaim/core/service.py` & `arikaim-0.5.9/arikaim/core/service.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.8/arikaim/core/utils.py` & `arikaim-0.5.9/arikaim/core/utils.py`

 * *Files identical despite different names*

### Comparing `arikaim-0.5.8/arikaim.egg-info/PKG-INFO` & `arikaim-0.5.9/arikaim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arikaim
-Version: 0.5.8
+Version: 0.5.9
 Summary: Arikaim services server
 Home-page: https://github.com/arikaim/arikaim-services-server.git
 Download-URL: 
 Author: Intersoft Ltd
 Author-email: info@arikaim.com
 License: MIT License
 Keywords: arikaim
```

### Comparing `arikaim-0.5.8/arikaim.egg-info/SOURCES.txt` & `arikaim-0.5.9/arikaim.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 arikaim/core/utils.py
 arikaim/core/access/access.py
 arikaim/core/access/auth_error.py
 arikaim/core/access/middleware/multiple.py
 arikaim/core/access/providers/php_session.py
 arikaim/core/access/providers/token.py
 arikaim/core/admin/admin.py
-arikaim/core/admin/controllers/info.py
 arikaim/core/admin/controllers/service.py
 arikaim/core/admin/controllers/service_route.py
 arikaim/core/admin/controllers/service_routes.py
 arikaim/core/admin/controllers/services_list.py
 arikaim/core/collection/property.py
 arikaim/core/console/app.py
 arikaim/core/console/config.py
```

### Comparing `arikaim-0.5.8/setup.py` & `arikaim-0.5.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     'arikaim.core.console.templates',
     'arikaim.core.db',
     'arikaim.core.queue',
     'arikaim.core.db.models'
 ],
    
 # Project version number:
-version = '0.5.8',
+version = '0.5.9',
 
 # List a license for the project, eg. MIT License
 license = 'MIT License',
 
 # Short description of your library: 
 description = 'Arikaim services server',
```

