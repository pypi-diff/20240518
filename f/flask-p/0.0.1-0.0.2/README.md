# Comparing `tmp/flask-p-0.0.1.tar.gz` & `tmp/flask-p-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-p-0.0.1.tar", last modified: Wed May 15 16:28:15 2024, max compression
+gzip compressed data, was "flask-p-0.0.2.tar", last modified: Sat May 18 10:43:51 2024, max compression
```

## Comparing `flask-p-0.0.1.tar` & `flask-p-0.0.2.tar`

### file list

```diff
@@ -1,76 +1,83 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 16:28:15.170742 flask-p-0.0.1/
--rw-rw-rw-   0        0        0     1089 2024-04-21 03:38:34.000000 flask-p-0.0.1/LICENSE
--rw-rw-rw-   0        0        0    12839 2024-05-15 16:28:15.169705 flask-p-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    12120 2024-05-10 08:04:20.000000 flask-p-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 16:28:15.079950 flask-p-0.0.1/flask_p.egg-info/
--rw-rw-rw-   0        0        0    12839 2024-05-15 16:28:14.000000 flask-p-0.0.1/flask_p.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2132 2024-05-15 16:28:14.000000 flask-p-0.0.1/flask_p.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 16:28:14.000000 flask-p-0.0.1/flask_p.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-15 16:28:14.000000 flask-p-0.0.1/flask_p.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-15 16:28:14.000000 flask-p-0.0.1/flask_p.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-15 16:28:15.083059 flask-p-0.0.1/flask_projects/
--rw-rw-rw-   0        0        0        0 2024-05-15 16:08:10.000000 flask-p-0.0.1/flask_projects/__init__.py
--rw-rw-rw-   0        0        0      412 2024-05-15 16:16:33.000000 flask-p-0.0.1/flask_projects/convension.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:28:15.085147 flask-p-0.0.1/flask_projects/core/
--rw-rw-rw-   0        0        0        2 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:28:15.088294 flask-p-0.0.1/flask_projects/core/order/
--rw-rw-rw-   0        0        0        0 2024-05-03 07:56:02.000000 flask-p-0.0.1/flask_projects/core/order/__init__.py
--rw-rw-rw-   0        0        0     1863 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/core/order/executor.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:28:15.093975 flask-p-0.0.1/flask_projects/core/order/unity/
--rw-rw-rw-   0        0        0      143 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/core/order/unity/__init__.py
--rw-rw-rw-   0        0        0      328 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/core/order/unity/run.py
--rw-rw-rw-   0        0        0       99 2024-05-03 09:12:32.000000 flask-p-0.0.1/flask_projects/core/order/unity/shell.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:28:15.100652 flask-p-0.0.1/flask_projects/core/proj/
--rw-rw-rw-   0        0        0        0 2024-04-21 03:44:02.000000 flask-p-0.0.1/flask_projects/core/proj/__init__.py
--rw-rw-rw-   0        0        0     1987 2024-05-15 16:06:22.000000 flask-p-0.0.1/flask_projects/core/proj/abs.py
--rw-rw-rw-   0        0        0     4081 2024-05-15 16:16:33.000000 flask-p-0.0.1/flask_projects/core/proj/project.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:28:15.114349 flask-p-0.0.1/flask_projects/core/vars/
--rw-rw-rw-   0        0        0      400 2024-04-21 08:58:05.000000 flask-p-0.0.1/flask_projects/core/vars/__init__.py
--rw-rw-rw-   0        0        0     4017 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/core/vars/abs.py
--rw-rw-rw-   0        0        0     1888 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/core/vars/application.py
--rw-rw-rw-   0        0        0     5684 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/core/vars/extends.py
--rw-rw-rw-   0        0        0     1193 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/core/vars/http.py
--rw-rw-rw-   0        0        0      738 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/core/vars/info.py
--rw-rw-rw-   0        0        0      491 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/core/vars/others.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:28:15.115363 flask-p-0.0.1/flask_projects/default/
--rw-rw-rw-   0        0        0       66 2024-05-02 10:34:22.000000 flask-p-0.0.1/flask_projects/default/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:28:15.119552 flask-p-0.0.1/flask_projects/default/app/
--rw-rw-rw-   0        0        0        0 2024-05-05 08:02:20.000000 flask-p-0.0.1/flask_projects/default/app/__init__.py
--rw-rw-rw-   0        0        0      262 2024-05-15 16:06:22.000000 flask-p-0.0.1/flask_projects/default/app/factory.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:28:15.121662 flask-p-0.0.1/flask_projects/default/business/
--rw-rw-rw-   0        0        0     2779 2024-05-15 16:06:22.000000 flask-p-0.0.1/flask_projects/default/business/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:28:15.128097 flask-p-0.0.1/flask_projects/default/configuration/
--rw-rw-rw-   0        0        0       91 2024-05-05 12:55:37.000000 flask-p-0.0.1/flask_projects/default/configuration/NameFactory.py
--rw-rw-rw-   0        0        0      460 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/default/configuration/__init__.py
--rw-rw-rw-   0        0        0      651 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/default/configuration/convention.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:28:15.130179 flask-p-0.0.1/flask_projects/default/configuration/plan_1/
--rw-rw-rw-   0        0        0        0 2024-05-05 12:11:57.000000 flask-p-0.0.1/flask_projects/default/configuration/plan_1/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:28:15.135449 flask-p-0.0.1/flask_projects/default/configuration/plan_default/
--rw-rw-rw-   0        0        0        0 2024-05-05 12:11:16.000000 flask-p-0.0.1/flask_projects/default/configuration/plan_default/__init__.py
--rw-rw-rw-   0        0        0      576 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/default/configuration/plan_default/container.py
--rw-rw-rw-   0        0        0      485 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/default/configuration/plan_default/logic.py
--rw-rw-rw-   0        0        0     1337 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/default/configuration/plan_default/scanner.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:28:15.137513 flask-p-0.0.1/flask_projects/default/middle/
--rw-rw-rw-   0        0        0        0 2024-05-10 07:01:12.000000 flask-p-0.0.1/flask_projects/default/middle/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:28:15.139570 flask-p-0.0.1/flask_projects/default/resource/
--rw-rw-rw-   0        0        0     2148 2024-05-15 16:06:22.000000 flask-p-0.0.1/flask_projects/default/resource/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:28:15.145571 flask-p-0.0.1/flask_projects/default/router/
--rw-rw-rw-   0        0        0       91 2024-05-05 12:55:37.000000 flask-p-0.0.1/flask_projects/default/router/NameFactory.py
--rw-rw-rw-   0        0        0     1351 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/default/router/__init__.py
--rw-rw-rw-   0        0        0      998 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/default/router/convention.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:28:15.154184 flask-p-0.0.1/flask_projects/default/router/plan_0/
--rw-rw-rw-   0        0        0        0 2024-05-06 07:36:05.000000 flask-p-0.0.1/flask_projects/default/router/plan_0/__init__.py
--rw-rw-rw-   0        0        0      525 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/default/router/plan_0/container.py
--rw-rw-rw-   0        0        0      695 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/default/router/plan_0/logic.py
--rw-rw-rw-   0        0        0      447 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/default/router/plan_0/order.py
--rw-rw-rw-   0        0        0     1189 2024-05-15 16:13:03.000000 flask-p-0.0.1/flask_projects/default/router/plan_0/scanner.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:28:15.167367 flask-p-0.0.1/flask_projects/interface/
--rw-rw-rw-   0        0        0        0 2024-05-15 13:18:36.000000 flask-p-0.0.1/flask_projects/interface/__init__.py
--rw-rw-rw-   0        0        0      147 2024-05-15 12:31:52.000000 flask-p-0.0.1/flask_projects/interface/base.py
--rw-rw-rw-   0        0        0      461 2024-05-15 13:18:56.000000 flask-p-0.0.1/flask_projects/interface/container.py
--rw-rw-rw-   0        0        0      156 2024-05-05 08:12:43.000000 flask-p-0.0.1/flask_projects/interface/factory.py
--rw-rw-rw-   0        0        0      387 2024-05-15 13:18:56.000000 flask-p-0.0.1/flask_projects/interface/logic.py
--rw-rw-rw-   0        0        0      312 2024-05-15 13:18:56.000000 flask-p-0.0.1/flask_projects/interface/order.py
--rw-rw-rw-   0        0        0      317 2024-05-15 13:18:56.000000 flask-p-0.0.1/flask_projects/interface/scanner.py
--rw-rw-rw-   0        0        0       42 2024-05-15 16:28:15.171782 flask-p-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1016 2024-05-15 16:27:43.000000 flask-p-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:43:51.078693 flask-p-0.0.2/
+-rw-rw-rw-   0        0        0     1089 2024-04-21 03:38:34.000000 flask-p-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0    12839 2024-05-18 10:43:51.077685 flask-p-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    12120 2024-05-10 08:04:20.000000 flask-p-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 10:43:50.961379 flask-p-0.0.2/flask_p.egg-info/
+-rw-rw-rw-   0        0        0    12839 2024-05-18 10:43:50.000000 flask-p-0.0.2/flask_p.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2414 2024-05-18 10:43:50.000000 flask-p-0.0.2/flask_p.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 10:43:50.000000 flask-p-0.0.2/flask_p.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-18 10:43:50.000000 flask-p-0.0.2/flask_p.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-18 10:43:50.000000 flask-p-0.0.2/flask_p.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 10:43:50.965515 flask-p-0.0.2/flask_projects/
+-rw-rw-rw-   0        0        0        0 2024-05-15 16:08:10.000000 flask-p-0.0.2/flask_projects/__init__.py
+-rw-rw-rw-   0        0        0      412 2024-05-15 16:16:33.000000 flask-p-0.0.2/flask_projects/convension.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:43:50.967827 flask-p-0.0.2/flask_projects/core/
+-rw-rw-rw-   0        0        0        2 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:43:50.970889 flask-p-0.0.2/flask_projects/core/order/
+-rw-rw-rw-   0        0        0        0 2024-05-03 07:56:02.000000 flask-p-0.0.2/flask_projects/core/order/__init__.py
+-rw-rw-rw-   0        0        0     1863 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/core/order/executor.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:43:50.978685 flask-p-0.0.2/flask_projects/core/order/unity/
+-rw-rw-rw-   0        0        0      143 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/core/order/unity/__init__.py
+-rw-rw-rw-   0        0        0      328 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/core/order/unity/run.py
+-rw-rw-rw-   0        0        0       99 2024-05-03 09:12:32.000000 flask-p-0.0.2/flask_projects/core/order/unity/shell.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:43:50.985166 flask-p-0.0.2/flask_projects/core/proj/
+-rw-rw-rw-   0        0        0        0 2024-04-21 03:44:02.000000 flask-p-0.0.2/flask_projects/core/proj/__init__.py
+-rw-rw-rw-   0        0        0     1987 2024-05-15 16:06:22.000000 flask-p-0.0.2/flask_projects/core/proj/abs.py
+-rw-rw-rw-   0        0        0     4319 2024-05-16 12:16:38.000000 flask-p-0.0.2/flask_projects/core/proj/project.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:43:51.002025 flask-p-0.0.2/flask_projects/core/vars/
+-rw-rw-rw-   0        0        0      400 2024-04-21 08:58:05.000000 flask-p-0.0.2/flask_projects/core/vars/__init__.py
+-rw-rw-rw-   0        0        0     4017 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/core/vars/abs.py
+-rw-rw-rw-   0        0        0     1888 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/core/vars/application.py
+-rw-rw-rw-   0        0        0     5684 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/core/vars/extends.py
+-rw-rw-rw-   0        0        0     1193 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/core/vars/http.py
+-rw-rw-rw-   0        0        0      738 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/core/vars/info.py
+-rw-rw-rw-   0        0        0      491 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/core/vars/others.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:43:51.004173 flask-p-0.0.2/flask_projects/default/
+-rw-rw-rw-   0        0        0       66 2024-05-02 10:34:22.000000 flask-p-0.0.2/flask_projects/default/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:43:51.008412 flask-p-0.0.2/flask_projects/default/app/
+-rw-rw-rw-   0        0        0        0 2024-05-05 08:02:20.000000 flask-p-0.0.2/flask_projects/default/app/__init__.py
+-rw-rw-rw-   0        0        0      262 2024-05-15 16:06:22.000000 flask-p-0.0.2/flask_projects/default/app/factory.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:43:51.009408 flask-p-0.0.2/flask_projects/default/business/
+-rw-rw-rw-   0        0        0     2779 2024-05-15 16:06:22.000000 flask-p-0.0.2/flask_projects/default/business/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:43:51.016130 flask-p-0.0.2/flask_projects/default/configuration/
+-rw-rw-rw-   0        0        0       91 2024-05-05 12:55:37.000000 flask-p-0.0.2/flask_projects/default/configuration/NameFactory.py
+-rw-rw-rw-   0        0        0      460 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/default/configuration/__init__.py
+-rw-rw-rw-   0        0        0      651 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/default/configuration/convention.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:43:51.018146 flask-p-0.0.2/flask_projects/default/configuration/plan_1/
+-rw-rw-rw-   0        0        0        0 2024-05-05 12:11:57.000000 flask-p-0.0.2/flask_projects/default/configuration/plan_1/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:43:51.026147 flask-p-0.0.2/flask_projects/default/configuration/plan_default/
+-rw-rw-rw-   0        0        0        0 2024-05-05 12:11:16.000000 flask-p-0.0.2/flask_projects/default/configuration/plan_default/__init__.py
+-rw-rw-rw-   0        0        0      576 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/default/configuration/plan_default/container.py
+-rw-rw-rw-   0        0        0      485 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/default/configuration/plan_default/logic.py
+-rw-rw-rw-   0        0        0     1337 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/default/configuration/plan_default/scanner.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:43:51.032854 flask-p-0.0.2/flask_projects/default/middle/
+-rw-rw-rw-   0        0        0       91 2024-05-05 12:55:37.000000 flask-p-0.0.2/flask_projects/default/middle/NameFactory.py
+-rw-rw-rw-   0        0        0      303 2024-05-16 12:16:38.000000 flask-p-0.0.2/flask_projects/default/middle/__init__.py
+-rw-rw-rw-   0        0        0     1177 2024-05-18 10:32:47.000000 flask-p-0.0.2/flask_projects/default/middle/convention.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:43:51.039119 flask-p-0.0.2/flask_projects/default/middle/plan_0/
+-rw-rw-rw-   0        0        0        0 2024-05-16 10:21:04.000000 flask-p-0.0.2/flask_projects/default/middle/plan_0/__init__.py
+-rw-rw-rw-   0        0        0      564 2024-05-17 16:37:28.000000 flask-p-0.0.2/flask_projects/default/middle/plan_0/container.py
+-rw-rw-rw-   0        0        0     3546 2024-05-17 16:38:28.000000 flask-p-0.0.2/flask_projects/default/middle/plan_0/logic.py
+-rw-rw-rw-   0        0        0     2292 2024-05-17 16:33:05.000000 flask-p-0.0.2/flask_projects/default/middle/plan_0/scanner.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:43:51.041545 flask-p-0.0.2/flask_projects/default/resource/
+-rw-rw-rw-   0        0        0     2148 2024-05-15 16:06:22.000000 flask-p-0.0.2/flask_projects/default/resource/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:43:51.049584 flask-p-0.0.2/flask_projects/default/router/
+-rw-rw-rw-   0        0        0       91 2024-05-05 12:55:37.000000 flask-p-0.0.2/flask_projects/default/router/NameFactory.py
+-rw-rw-rw-   0        0        0     1351 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/default/router/__init__.py
+-rw-rw-rw-   0        0        0      998 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/default/router/convention.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:43:51.059944 flask-p-0.0.2/flask_projects/default/router/plan_0/
+-rw-rw-rw-   0        0        0        0 2024-05-06 07:36:05.000000 flask-p-0.0.2/flask_projects/default/router/plan_0/__init__.py
+-rw-rw-rw-   0        0        0      525 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/default/router/plan_0/container.py
+-rw-rw-rw-   0        0        0      695 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/default/router/plan_0/logic.py
+-rw-rw-rw-   0        0        0      447 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/default/router/plan_0/order.py
+-rw-rw-rw-   0        0        0     1189 2024-05-15 16:13:03.000000 flask-p-0.0.2/flask_projects/default/router/plan_0/scanner.py
+drwxrwxrwx   0        0        0        0 2024-05-18 10:43:51.074645 flask-p-0.0.2/flask_projects/interface/
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:18:36.000000 flask-p-0.0.2/flask_projects/interface/__init__.py
+-rw-rw-rw-   0        0        0      147 2024-05-15 12:31:52.000000 flask-p-0.0.2/flask_projects/interface/base.py
+-rw-rw-rw-   0        0        0      461 2024-05-15 13:18:56.000000 flask-p-0.0.2/flask_projects/interface/container.py
+-rw-rw-rw-   0        0        0      156 2024-05-05 08:12:43.000000 flask-p-0.0.2/flask_projects/interface/factory.py
+-rw-rw-rw-   0        0        0      387 2024-05-15 13:18:56.000000 flask-p-0.0.2/flask_projects/interface/logic.py
+-rw-rw-rw-   0        0        0      312 2024-05-15 13:18:56.000000 flask-p-0.0.2/flask_projects/interface/order.py
+-rw-rw-rw-   0        0        0      317 2024-05-15 13:18:56.000000 flask-p-0.0.2/flask_projects/interface/scanner.py
+-rw-rw-rw-   0        0        0       42 2024-05-18 10:43:51.079814 flask-p-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1016 2024-05-18 10:43:36.000000 flask-p-0.0.2/setup.py
```

### Comparing `flask-p-0.0.1/LICENSE` & `flask-p-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-p-0.0.1/PKG-INFO` & `flask-p-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-p
-Version: 0.0.1
+Version: 0.0.2
 Summary: flask projects系列快速开发手脚架核心
 Home-page: https://github.com/ababbabbb/flask_project_core
 Author: bichuantao
 Author-email: 17826066203@163.com
 License: MIT
 Keywords: python,flask,projects,Rapid development
 Requires-Python: >=3.6
```

### Comparing `flask-p-0.0.1/README.md` & `flask-p-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `flask-p-0.0.1/flask_p.egg-info/PKG-INFO` & `flask-p-0.0.2/flask_p.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-p
-Version: 0.0.1
+Version: 0.0.2
 Summary: flask projects系列快速开发手脚架核心
 Home-page: https://github.com/ababbabbb/flask_project_core
 Author: bichuantao
 Author-email: 17826066203@163.com
 License: MIT
 Keywords: python,flask,projects,Rapid development
 Requires-Python: >=3.6
```

### Comparing `flask-p-0.0.1/flask_p.egg-info/SOURCES.txt` & `flask-p-0.0.2/flask_p.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,21 @@
 flask_projects/default/configuration/__init__.py
 flask_projects/default/configuration/convention.py
 flask_projects/default/configuration/plan_1/__init__.py
 flask_projects/default/configuration/plan_default/__init__.py
 flask_projects/default/configuration/plan_default/container.py
 flask_projects/default/configuration/plan_default/logic.py
 flask_projects/default/configuration/plan_default/scanner.py
+flask_projects/default/middle/NameFactory.py
 flask_projects/default/middle/__init__.py
+flask_projects/default/middle/convention.py
+flask_projects/default/middle/plan_0/__init__.py
+flask_projects/default/middle/plan_0/container.py
+flask_projects/default/middle/plan_0/logic.py
+flask_projects/default/middle/plan_0/scanner.py
 flask_projects/default/resource/__init__.py
 flask_projects/default/router/NameFactory.py
 flask_projects/default/router/__init__.py
 flask_projects/default/router/convention.py
 flask_projects/default/router/plan_0/__init__.py
 flask_projects/default/router/plan_0/container.py
 flask_projects/default/router/plan_0/logic.py
```

### Comparing `flask-p-0.0.1/flask_projects/core/order/executor.py` & `flask-p-0.0.2/flask_projects/core/order/executor.py`

 * *Files identical despite different names*

### Comparing `flask-p-0.0.1/flask_projects/core/proj/abs.py` & `flask-p-0.0.2/flask_projects/core/proj/abs.py`

 * *Files identical despite different names*

### Comparing `flask-p-0.0.1/flask_projects/core/proj/project.py` & `flask-p-0.0.2/flask_projects/core/proj/project.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from flask_projects.default.app.factory import default_factory
 from flask_projects.default.business import DefaultBusinessScanner, DefaultBusinessContainer, DefaultBusinessLogic
 from flask_projects.default.configuration import DefaultConfigurationScanner, DefaultConfigurationContainer, \
     DefaultConfigurationLogic
 from flask_projects.default.resource import DefaultResourceScanner, DefaultResourceContainer, DefaultResourceLogic
 from flask_projects.default.router import DefaultRouterScanner, DefaultRouterContainer, DefaultRouterLogic, \
     DefaultRouterOrder
+from flask_projects.default.middle import DefaultMiddleScanner, DefaultMiddleContainer, DefaultMiddleLogic
 from flask_projects.interface.factory import AppFactoryAbs
 
 
 class Project(ProjectAbs):
 
     def __init__(self):
         # 初始化，生成必要的容器/对象作为属性
@@ -36,14 +37,18 @@
             DefaultResourceContainer,
             DefaultResourceLogic
         ).setter_extend(
             DefaultBusinessScanner,
             DefaultBusinessContainer,
             DefaultBusinessLogic
         ).setter_extend(
+            DefaultMiddleScanner,
+            DefaultMiddleContainer,
+            DefaultMiddleLogic
+        ).setter_extend(
             DefaultConfigurationScanner,
             DefaultConfigurationContainer,
             DefaultConfigurationLogic
         ).setter_extend(
             DefaultRouterScanner,
             DefaultRouterContainer,
             DefaultRouterLogic,
```

### Comparing `flask-p-0.0.1/flask_projects/core/vars/abs.py` & `flask-p-0.0.2/flask_projects/core/vars/abs.py`

 * *Files identical despite different names*

### Comparing `flask-p-0.0.1/flask_projects/core/vars/application.py` & `flask-p-0.0.2/flask_projects/core/vars/application.py`

 * *Files identical despite different names*

### Comparing `flask-p-0.0.1/flask_projects/core/vars/extends.py` & `flask-p-0.0.2/flask_projects/core/vars/extends.py`

 * *Files identical despite different names*

### Comparing `flask-p-0.0.1/flask_projects/core/vars/http.py` & `flask-p-0.0.2/flask_projects/core/vars/http.py`

 * *Files identical despite different names*

### Comparing `flask-p-0.0.1/flask_projects/core/vars/info.py` & `flask-p-0.0.2/flask_projects/core/vars/info.py`

 * *Files identical despite different names*

### Comparing `flask-p-0.0.1/flask_projects/default/business/__init__.py` & `flask-p-0.0.2/flask_projects/default/business/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-p-0.0.1/flask_projects/default/configuration/convention.py` & `flask-p-0.0.2/flask_projects/default/configuration/convention.py`

 * *Files identical despite different names*

### Comparing `flask-p-0.0.1/flask_projects/default/configuration/plan_default/container.py` & `flask-p-0.0.2/flask_projects/default/configuration/plan_default/container.py`

 * *Files identical despite different names*

### Comparing `flask-p-0.0.1/flask_projects/default/configuration/plan_default/scanner.py` & `flask-p-0.0.2/flask_projects/default/configuration/plan_default/scanner.py`

 * *Files identical despite different names*

### Comparing `flask-p-0.0.1/flask_projects/default/resource/__init__.py` & `flask-p-0.0.2/flask_projects/default/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-p-0.0.1/flask_projects/default/router/__init__.py` & `flask-p-0.0.2/flask_projects/default/router/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-p-0.0.1/flask_projects/default/router/convention.py` & `flask-p-0.0.2/flask_projects/default/router/convention.py`

 * *Files identical despite different names*

### Comparing `flask-p-0.0.1/flask_projects/default/router/plan_0/container.py` & `flask-p-0.0.2/flask_projects/default/router/plan_0/container.py`

 * *Files identical despite different names*

### Comparing `flask-p-0.0.1/flask_projects/default/router/plan_0/logic.py` & `flask-p-0.0.2/flask_projects/default/router/plan_0/logic.py`

 * *Files identical despite different names*

### Comparing `flask-p-0.0.1/flask_projects/default/router/plan_0/scanner.py` & `flask-p-0.0.2/flask_projects/default/router/plan_0/scanner.py`

 * *Files identical despite different names*

### Comparing `flask-p-0.0.1/setup.py` & `flask-p-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # you need to change all these
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = "flask projects系列快速开发手脚架核心"
 
 setup(
     name="flask-p",
 
     author="bichuantao",
     author_email='17826066203@163.com',
```

