# Comparing `tmp/pyslth-0.3.3.tar.gz` & `tmp/pyslth-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.3.3.tar", last modified: Wed May 15 17:37:18 2024, max compression
+gzip compressed data, was "pyslth-0.3.4.tar", last modified: Sat May 18 10:13:00 2024, max compression
```

## Comparing `pyslth-0.3.3.tar` & `pyslth-0.3.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.808873 pyslth-0.3.3/
--rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.3.3/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-15 17:37:18.808606 pyslth-0.3.3/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.772220 pyslth-0.3.3/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-15 17:37:18.000000 pyslth-0.3.3/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1859 2024-05-15 17:37:18.000000 pyslth-0.3.3/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-15 17:37:18.000000 pyslth-0.3.3/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-15 17:37:18.000000 pyslth-0.3.3/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-15 17:37:18.000000 pyslth-0.3.3/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.3.3/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-15 17:37:18.808940 pyslth-0.3.3/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-15 17:37:05.000000 pyslth-0.3.3/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.778876 pyslth-0.3.3/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3779 2024-05-10 13:02:33.000000 pyslth-0.3.3/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     9637 2024-05-13 08:40:08.000000 pyslth-0.3.3/slth/components.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.779515 pyslth-0.3.3/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.3.3/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     5031 2024-05-13 19:37:29.000000 pyslth-0.3.3/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    24149 2024-05-12 23:58:33.000000 pyslth-0.3.3/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.3.3/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     3948 2024-05-05 11:08:21.000000 pyslth-0.3.3/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    26298 2024-05-14 12:48:00.000000 pyslth-0.3.3/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.779834 pyslth-0.3.3/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.3/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.780564 pyslth-0.3.3/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.3/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.3.3/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.3.3/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.783218 pyslth-0.3.3/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.3.3/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.3.3/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.3.3/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.3.3/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.3.3/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.3.3/slth/migrations/0006_user.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.3/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6546 2024-05-11 10:34:23.000000 pyslth-0.3.3/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.3.3/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.3.3/slth/oauth.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.3.3/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19846 2024-05-14 12:39:56.000000 pyslth-0.3.3/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.3.3/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.783760 pyslth-0.3.3/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.3.3/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.3.3/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    15898 2024-05-13 01:13:17.000000 pyslth-0.3.3/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.784086 pyslth-0.3.3/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.786029 pyslth-0.3.3/slth/static/css/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.3.3/slth/static/css/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.3.3/slth/static/css/fontawesome.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.790325 pyslth-0.3.3/slth/static/css/fonts/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.3.3/slth/static/css/fonts/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.3.3/slth/static/css/fonts/fa-solid-900.woff2
--rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.3.3/slth/static/css/fonts/rawline-400.woff
--rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.3.3/slth/static/css/fonts/rawline-500i.woff
--rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.3.3/slth/static/css/fonts/rawline-700.woff
--rw-r--r--   0 breno      (501) staff       (20)     1977 2024-05-12 18:54:58.000000 pyslth-0.3.3/slth/static/css/slth.css
--rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.3.3/slth/static/css/solid.min.css
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.3.3/slth/static/css/style.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.792484 pyslth-0.3.3/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.3.3/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.3.3/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.3.3/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.3.3/slth/static/images/user.svg
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.3.3/slth/static/index.html
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.804614 pyslth-0.3.3/slth/static/js/
--rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.3.3/slth/static/js/echarts.min.js
--rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-15 17:36:30.000000 pyslth-0.3.3/slth/static/js/index.min.js
--rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.3.3/slth/static/js/ios-splash.min.js
--rw-r--r--   0 breno      (501) staff       (20)   117723 2024-05-08 16:11:56.000000 pyslth-0.3.3/slth/static/js/peerjs.min.js
--rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.3.3/slth/static/js/qrcode.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.3.3/slth/static/js/react-trigger-change.js
--rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-15 17:36:30.000000 pyslth-0.3.3/slth/static/js/react.min.js
--rw-r--r--   0 breno      (501) staff       (20)   100211 2024-05-15 17:36:30.000000 pyslth-0.3.3/slth/static/js/slth.min.js
--rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.3.3/slth/static/js/vanilla-masker.js
--rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.3.3/slth/static/js/vanilla-masker.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.3.3/slth/statistics.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-15 17:37:18.806913 pyslth-0.3.3/slth/templates/
--rw-r--r--   0 breno      (501) staff       (20)     3146 2024-05-08 15:53:35.000000 pyslth-0.3.3/slth/templates/index.html
--rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.3.3/slth/templates/service-worker.js
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.3.3/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.3.3/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1000 2024-05-13 01:26:42.000000 pyslth-0.3.3/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     2572 2024-05-08 14:06:07.000000 pyslth-0.3.3/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.740301 pyslth-0.3.4/
+-rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.3.4/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-18 10:13:00.740156 pyslth-0.3.4/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.714243 pyslth-0.3.4/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-18 10:13:00.000000 pyslth-0.3.4/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1859 2024-05-18 10:13:00.000000 pyslth-0.3.4/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-18 10:13:00.000000 pyslth-0.3.4/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-18 10:13:00.000000 pyslth-0.3.4/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-18 10:13:00.000000 pyslth-0.3.4/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.3.4/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-18 10:13:00.740340 pyslth-0.3.4/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-18 10:12:36.000000 pyslth-0.3.4/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.719429 pyslth-0.3.4/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3779 2024-05-10 13:02:33.000000 pyslth-0.3.4/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     9685 2024-05-16 10:19:55.000000 pyslth-0.3.4/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.719881 pyslth-0.3.4/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.3.4/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     5031 2024-05-13 19:37:29.000000 pyslth-0.3.4/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    24698 2024-05-18 09:59:43.000000 pyslth-0.3.4/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.3.4/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     4451 2024-05-16 10:23:26.000000 pyslth-0.3.4/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    26476 2024-05-16 10:18:46.000000 pyslth-0.3.4/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.720100 pyslth-0.3.4/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.4/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.720526 pyslth-0.3.4/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.4/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.3.4/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.3.4/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.722861 pyslth-0.3.4/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.3.4/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.3.4/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.3.4/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.3.4/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.3.4/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.3.4/slth/migrations/0006_user.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.4/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6546 2024-05-11 10:34:23.000000 pyslth-0.3.4/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      565 2024-05-18 08:21:00.000000 pyslth-0.3.4/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.3.4/slth/oauth.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.3.4/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19965 2024-05-16 13:39:18.000000 pyslth-0.3.4/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.3.4/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.723199 pyslth-0.3.4/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.3.4/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.3.4/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    15898 2024-05-13 01:13:17.000000 pyslth-0.3.4/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.723451 pyslth-0.3.4/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.724840 pyslth-0.3.4/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.3.4/slth/static/css/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.3.4/slth/static/css/fontawesome.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.728153 pyslth-0.3.4/slth/static/css/fonts/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.3.4/slth/static/css/fonts/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.3.4/slth/static/css/fonts/fa-solid-900.woff2
+-rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.3.4/slth/static/css/fonts/rawline-400.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.3.4/slth/static/css/fonts/rawline-500i.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.3.4/slth/static/css/fonts/rawline-700.woff
+-rw-r--r--   0 breno      (501) staff       (20)     1977 2024-05-12 18:54:58.000000 pyslth-0.3.4/slth/static/css/slth.css
+-rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.3.4/slth/static/css/solid.min.css
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.3.4/slth/static/css/style.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.730120 pyslth-0.3.4/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.3.4/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.3.4/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.3.4/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.3.4/slth/static/images/user.svg
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.3.4/slth/static/index.html
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.739437 pyslth-0.3.4/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.3.4/slth/static/js/echarts.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-18 10:12:29.000000 pyslth-0.3.4/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.3.4/slth/static/js/ios-splash.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   117723 2024-05-08 16:11:56.000000 pyslth-0.3.4/slth/static/js/peerjs.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.3.4/slth/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.3.4/slth/static/js/react-trigger-change.js
+-rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-18 10:12:29.000000 pyslth-0.3.4/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   100846 2024-05-18 10:12:29.000000 pyslth-0.3.4/slth/static/js/slth.min.js
+-rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.3.4/slth/static/js/vanilla-masker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.3.4/slth/static/js/vanilla-masker.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6361 2024-05-16 13:05:44.000000 pyslth-0.3.4/slth/statistics.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.739884 pyslth-0.3.4/slth/templates/
+-rw-r--r--   0 breno      (501) staff       (20)     3146 2024-05-18 08:08:43.000000 pyslth-0.3.4/slth/templates/index.html
+-rw-r--r--   0 breno      (501) staff       (20)     1456 2024-05-18 10:06:11.000000 pyslth-0.3.4/slth/templates/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.3.4/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.3.4/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1000 2024-05-13 01:26:42.000000 pyslth-0.3.4/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2572 2024-05-08 14:06:07.000000 pyslth-0.3.4/slth/views.py
```

### Comparing `pyslth-0.3.3/PKG-INFO` & `pyslth-0.3.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.3.3
+Version: 0.3.4
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.3.3/pyslth.egg-info/PKG-INFO` & `pyslth-0.3.4/pyslth.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.3.3
+Version: 0.3.4
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.3.3/pyslth.egg-info/SOURCES.txt` & `pyslth-0.3.4/pyslth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/setup.py` & `pyslth-0.3.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.3.3',
+    version='0.3.4',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.3.3/slth/__init__.py` & `pyslth-0.3.4/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/components.py` & `pyslth-0.3.4/slth/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,19 +249,20 @@
         self["footer"] = footer
         self["oauth"] = oauth
         self["sponsors"] = sponsors
 
 
 class Response(dict):
 
-    def __init__(self, message=None, redirect=None, store=None):
+    def __init__(self, message=None, redirect=None, store=None, **kwargs):
         self["type"] = "response"
         self["message"] = message
-        self["redirect"] = redirect
+        self["redirect"] = redirect or '..'
         self["store"] = store or {}
+        self.update(**kwargs)
 
 
 class IconSet(dict):
     def __init__(self):
         self["type"] = "iconset"
```

### Comparing `pyslth-0.3.3/slth/db/models.py` & `pyslth-0.3.4/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/endpoints.py` & `pyslth-0.3.4/slth/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,23 +147,28 @@
         elif isinstance(data, Serializer):
             data = data.contextualize(self.request).settitle(title)
         elif isinstance(data, FormFactory):
             form = self.getform(data.settitle(title).form(self))
             if self.request.method == "POST" or self.request.GET.get("form") == title:
                 try:
                     self.cleaned_data = form.submit()
-                    return self.post()
+                    if form._message or form._redirect or form._dispose:
+                        return Response(form._message, form._redirect, dispose=form._dispose)
+                    else:
+                        return self.post()
                 except ValidationError as e:
                     raise JsonResponseException(
                         dict(type="error", text="\n".join(e.messages), errors={})
                     )
             else:
                 data = form
         elif isinstance(data, Form) or isinstance(data, ModelForm):
             data = data.settitle(title)
+        elif self.request.method == "POST" and not data:
+            return self.post()
         return data
 
     def serialize(self):
         return serialize(self.process())
 
     def to_response(self):
         return ApiResponse(self.serialize(), safe=False)
@@ -710,45 +715,46 @@
 
     class Meta:
         verbose_name = "Subscrever para Notificações"
 
     def post(self):
         data = json.loads(self.request.POST.get("subscription"))
         device = self.request.META.get("HTTP_USER_AGENT", "")
-        qs = PushSubscription.objects.filter(user=User.objects.first(), device=device)
-        (
+        qs = PushSubscription.objects.filter(user=self.request.user, device=device)
+        if qs.exists():
             qs.update(data=data)
-            if qs.exists()
-            else PushSubscription.objects.create(
-                user=User.objects.first(), data=data, device=device
-            )
-        )
+        else:
+            PushSubscription.objects.create(user=self.request.user, data=data, device=device)
         return Response()
 
     def check_permission(self):
         return True
 
 
 class PushSubscriptions(ListEndpoint[PushSubscription]):
     class Meta:
         verbose_name = "Notificações"
 
 
 class SendPushNotification(ChildInstanceEndpoint):
+    title = forms.CharField(label='Título')
     message = forms.CharField(label="Texto", widget=forms.Textarea())
+    url = forms.CharField(label='URL', required=False)
 
     class Meta:
         icon = "mail-bulk"
         verbose_name = "Enviar Notificação"
 
     def get(self):
-        return self.formfactory().fields("message")
+        return self.formfactory().fields("title", "message", "url").initial(
+            title='Mais uma notificação', message='Corpo da notificação', url='http://localhost:8000/app/dashboard/'
+        )
 
     def post(self):
-        send_push_web_notification(self.instance, self.cleaned_data["message"])
+        send_push_web_notification(self.instance, self.cleaned_data["title"], self.cleaned_data["message"], url=self.cleaned_data["url"])
         return Response(message="Notificação enviada com sucesso.")
 
 
 class EditProfile(Endpoint):
     password = forms.CharField(label="Senha", required=False)
     password2 = forms.CharField(label="Confirmação", required=False)
```

### Comparing `pyslth-0.3.3/slth/factory.py` & `pyslth-0.3.4/slth/factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,17 @@
         self._info = None
         self._actions = {}
         self._initial = {}
         self._choices = {}
         self._empty = False
         self._method = method
         self._hidden= []
+        self._redirect = None
+        self._message = None
+        self._dispose = False
 
     def _append_field(self, field_name):
         if ':' in field_name:
             field_name, action_name = field_name.split(':')
             self._actions[field_name] = action_name
         self._fieldlist.append(field_name)
         return field_name
@@ -75,14 +78,24 @@
     def settitle(self, title) -> 'FormFactory':
         self._title = title
         return self
     
     def hidden(self, *names):
         self._hidden.extend(names)
         return self
+    
+    def onsuccess(self, message=None, redirect=None, dispose=False):
+        if message:
+            self._message = message
+        if redirect:
+            self._redirect = redirect
+        if dispose:
+            self._dispose = dispose
+            self._redirect = '.'
+        return self
 
     def form(self, endpoint):
         from .forms import ModelForm, Form
         
         if isinstance(self._instance, Model):
             fieldlist = [field.name for field in type(self._instance)._meta.get_fields() if field.name in self._fieldlist]
             class Form(ModelForm):
@@ -92,14 +105,17 @@
                 
         form = Form(instance=self._instance, endpoint=endpoint, initial=self._initial)
         form._key = endpoint.get_api_name()
         form._title = self._title
         form._method = self._method
         form._info = self._info
         form._actions = self._actions
+        form._message = self._message
+        form._redirect = self._redirect
+        form._dispose = self._dispose
         for name in self._fieldlist:
             if name not in form.fields:
                 form.fields[name] = getattr(endpoint, name)
         for name, queryset in self._choices.items():
             form.fields[name].queryset = queryset
         form.fieldsets = self._fieldsets
         form.setvalue(**self._values)
```

### Comparing `pyslth-0.3.3/slth/forms.py` & `pyslth-0.3.4/slth/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -491,14 +491,17 @@
 
 class Form(DjangoForm, FormMixin):
 
     def __init__(self, *args, endpoint=None, **kwargs):
         self._display = []
         self._endpoint = endpoint
         self._info = None
+        self._message = None
+        self._redirect = None
+        self._dispose = False
         self._values = {}
         self._title = type(self).__name__
         self._actions = {}
         self._method = "POST"
         self._key = self._title.lower()
 
         self.fieldsets = {}
@@ -523,14 +526,17 @@
 
 class ModelForm(DjangoModelForm, FormMixin):
 
     def __init__(self, instance=None, endpoint=None, **kwargs):
         self._display = []
         self._endpoint = endpoint
         self._info = None
+        self._message = None
+        self._redirect = None
+        self._dispose = False
         self._values = {}
         self._title = type(self).__name__
         self._actions = {}
         self._method = "POST"
         self._key = self._title.lower()
 
         self.fieldsets = {}
```

### Comparing `pyslth-0.3.3/slth/management/commands/integration_test.py` & `pyslth-0.3.4/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/management/commands/sync.py` & `pyslth-0.3.4/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/migrations/0001_initial.py` & `pyslth-0.3.4/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.3.4/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.3.4/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/migrations/0006_user.py` & `pyslth-0.3.4/slth/migrations/0006_user.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/models.py` & `pyslth-0.3.4/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/oauth.py` & `pyslth-0.3.4/slth/oauth.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/permissions.py` & `pyslth-0.3.4/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/queryset.py` & `pyslth-0.3.4/slth/queryset.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 class QuerySet(models.QuerySet):
 
     def __init__(self, *args, **kwargs):
         self.metadata = {}
         self.request = None
         super().__init__(*args, **kwargs)
 
+    def total(self, x=None):
+        return self.values_list(x).order_by(x).distinct().count() if x else self.count()
+
     def counter(self, x=None, y=None, title=None, chart=None):
         return Statistics(self, title=title, chart=chart).count(x=x, y=y) if x else super().count()
 
     def sum(self, z, x=None, y=None, title=None, chart=None):
         return Statistics(self, title=title, chart=chart).sum(z, x=x, y=y) if x else super().aggregate(sum=Sum(z))['sum'] or 0
 
     def _clone(self):
```

### Comparing `pyslth-0.3.3/slth/roles.py` & `pyslth-0.3.4/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/selenium/__init__.py` & `pyslth-0.3.4/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/selenium/browser.py` & `pyslth-0.3.4/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/serializer.py` & `pyslth-0.3.4/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/css/.DS_Store` & `pyslth-0.3.4/slth/static/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/css/fontawesome.min.css` & `pyslth-0.3.4/slth/static/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/css/fonts/.DS_Store` & `pyslth-0.3.4/slth/static/css/fonts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/css/fonts/fa-solid-900.woff2` & `pyslth-0.3.4/slth/static/css/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/css/fonts/rawline-400.woff` & `pyslth-0.3.4/slth/static/css/fonts/rawline-400.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/css/fonts/rawline-500i.woff` & `pyslth-0.3.4/slth/static/css/fonts/rawline-500i.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/css/fonts/rawline-700.woff` & `pyslth-0.3.4/slth/static/css/fonts/rawline-700.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/css/slth.css` & `pyslth-0.3.4/slth/static/css/slth.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/css/solid.min.css` & `pyslth-0.3.4/slth/static/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/images/logo.png` & `pyslth-0.3.4/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/images/logo.svg` & `pyslth-0.3.4/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/images/user.png` & `pyslth-0.3.4/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/js/echarts.min.js` & `pyslth-0.3.4/slth/static/js/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/js/index.min.js` & `pyslth-0.3.4/slth/static/js/index.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/js/ios-splash.min.js` & `pyslth-0.3.4/slth/static/js/ios-splash.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/js/peerjs.min.js` & `pyslth-0.3.4/slth/static/js/peerjs.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/js/qrcode.min.js` & `pyslth-0.3.4/slth/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/js/react-trigger-change.js` & `pyslth-0.3.4/slth/static/js/react-trigger-change.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/js/react.min.js` & `pyslth-0.3.4/slth/static/js/react.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/js/slth.min.js` & `pyslth-0.3.4/slth/static/js/slth.min.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 import {
     j as t,
-    c as z,
-    r as I,
+    c as W,
+    r as B,
     R as Te
 } from "./react.min.js";
 const k = {
     colors: {
         primary: "var(--primary-color)",
         success: "var(--success-color)",
         warning: "var(--warning-color)",
@@ -19,44 +19,44 @@
         radius: "var(--border-radius)"
     },
     background: {
         info: "var(--info-background)"
     }
 };
 
-function De(e) {
+function Ie(e) {
     function n() {
         const a = {
             width: 30,
             height: 30,
             borderRadius: "50%",
             backgroundColor: e.data.value
         };
         return t.jsx("div", {
             style: a
         })
     }
     return n()
 }
 
-function Ie(e) {
+function De(e) {
     function n(r) {
-        navigator.clipboard.writeText(r), te('Icon "' + r + '" copied to clipboard!')
+        navigator.clipboard.writeText(r), G('Icon "' + r + '" copied to clipboard!')
     }
     const a = {
         display: "inline-block",
         width: 150,
         textAlign: "center",
         cursor: "pointer"
     };
     return t.jsx("div", {
         style: {
             marginTop: 30
         },
-        children: qe.map(r => t.jsxs("div", {
+        children: Ne.map(r => t.jsxs("div", {
             className: "icon-box",
             onClick: () => n(r),
             style: a,
             children: [t.jsx("i", {
                 className: "fa-solid fa-fw fa-" + r
             }), t.jsx("div", {
                 className: "icon-text",
@@ -105,17 +105,17 @@
             children: t.jsx(S, {
                 icon: e.icon
             })
         })
     }
     return n()
 }
-const qe = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "fill-drip", "arrows-to-circle", "circle-chevron-right", "at", "trash-can", "text-height", "user-xmark", "stethoscope", "message", "info", "down-left-and-up-right-to-center", "explosion", "file-text", "wave-square", "ring", "building-un", "dice-three", "calendar-days", "anchor-circle-check", "building-circle-arrow-right", "volleyball", "arrows-up-to-line", "sort-down", "minus-circle", "door-open", "sign-out-alt", "atom", "soap", "icons", "microphone-lines-slash", "bridge-circle-check", "pump-medical", "fingerprint", "hand-point-right", "search-location", "step-forward", "smile-beam", "flag-checkered", "football", "school-circle-exclamation", "crop", "angles-down", "users-rectangle", "people-roof", "people-line", "beer", "diagram-predecessor", "long-arrow-up", "fire-flame-simple", "person", "laptop", "file-csv", "menorah", "truck-plane", "record-vinyl", "grin-stars", "bong", "spaghetti-monster-flying", "arrow-down-up-across-line", "utensil-spoon", "jar-wheat", "mail-bulk", "file-circle-exclamation", "hospital-symbol", "pager", "contact-book", "strikethrough", "k", "landmark-flag", "pencil", "backward", "caret-right", "comments", "paste", "code-pull-request", "clipboard-list", "truck-ramp-box", "user-check", "vial-virus", "sheet-plastic", "blog", "user-ninja", "person-arrow-up-from-line", "torah", "quidditch", "toggle-off", "box-archive", "person-drowning", "sort-numeric-down-alt", "grin-tongue-squint", "spray-can", "truck-monster", "w", "globe-africa", "rainbow", "circle-notch", "tablet-screen-button", "paw", "cloud", "trowel-bricks", "flushed", "hospital-user", "tent-arrow-left-right", "legal", "binoculars", "microphone-slash", "box-tissue", "motorcycle", "concierge-bell", "pencil-ruler", "people-arrows", "mars-and-venus-burst", "square-caret-right", "scissors", "sun-plant-wilt", "toilets-portable", "hockey-puck", "table", "magnifying-glass-arrow-right", "tachograph-digital", "users-slash", "clover", "reply", "star-and-crescent", "house-fire", "square-minus", "helicopter", "compass", "square-caret-down", "file-circle-question", "laptop-code", "swatchbook", "prescription-bottle", "navicon", "people-group", "hourglass-end", "heart-crack", "square-up-right", "kiss-beam", "film", "ruler-horizontal", "people-robbery", "lightbulb", "caret-left", "exclamation-circle", "school-circle-xmark", "sign-out", "circle-chevron-down", "unlock-keyhole", "cloud-showers-heavy", "headphones-simple", "sitemap", "donate", "memory", "road-spikes", "fire-burner", "flag", "hanukiah", "feather", "volume-low", "comment-slash", "cloud-sun-rain", "compress", "wheat-awn", "ankh", "hands-holding-child", "asterisk", "square-check", "peseta-sign", "heading", "ghost", "list", "square-phone-flip", "cart-plus", "gamepad", "dot-circle", "face-dizzy", "egg", "house-medical-circle-xmark", "campground", "folder-plus", "soccer-ball", "paintbrush", "lock", "gas-pump", "hot-tub", "map-marked", "house-flood-water", "tree", "bridge-lock", "sack-dollar", "pen-to-square", "car-side", "share-nodes", "heart-circle-minus", "hourglass-half", "microscope", "sink", "shopping-bag", "sort-alpha-down-alt", "mitten", "person-rays", "users", "eye-slash", "flask-vial", "hand", "om", "worm", "house-circle-xmark", "plug", "chevron-up", "hand-spock", "stopwatch", "kiss", "bridge-circle-xmark", "grin-tongue", "chess-bishop", "grin-wink", "hard-of-hearing", "road-circle-check", "dice-five", "square-rss", "land-mine-on", "i-cursor", "stamp", "stairs", "i", "hryvnia", "pills", "grin-alt", "tooth", "v", "bangladeshi-taka-sign", "bicycle", "staff-snake", "head-side-cough-slash", "truck-medical", "wheat-awn-circle-exclamation", "snowman", "mortar-pestle", "road-barrier", "school", "igloo", "joint", "angle-right", "horse", "q", "g", "notes-medical", "thermometer-half", "dong-sign", "capsules", "poo-storm", "frown-open", "hand-point-up", "money-bill", "bookmark", "align-justify", "umbrella-beach", "helmet-un", "bullseye", "bacon", "hand-point-down", "arrow-up-from-bracket", "folder", "file-waveform", "radiation", "chart-simple", "mars-stroke", "vial", "tachometer-alt-average", "wand-magic-sparkles", "e", "pen-clip", "bridge-circle-exclamation", "user", "school-circle-check", "dumpster", "van-shuttle", "building-user", "square-caret-left", "highlighter", "key", "bullhorn", "globe", "synagogue", "person-half-dress", "road-bridge", "location-arrow", "c", "tablet-button", "building-lock", "pizza-slice", "money-bill-wave", "chart-area", "house-flag", "person-circle-minus", "cancel", "camera-rotate", "spray-can-sparkles", "star", "repeat", "cross", "box", "venus-mars", "mouse-pointer", "maximize", "charging-station", "triangle-circle-square", "shuffle", "running", "mobile-retro", "grip-lines-vertical", "spider", "hands-bound", "file-invoice-dollar", "plane-circle-exclamation", "x-ray", "spell-check", "slash", "mouse", "sign-in", "store-alt-slash", "server", "virus-covid-slash", "shop-lock", "hourglass-start", "blender-phone", "building-wheat", "person-breastfeeding", "sign-in-alt", "venus", "passport", "heartbeat", "people-carry", "temperature-high", "microchip", "crown", "weight-hanging", "xmarks-lines", "file-prescription", "weight", "user-group", "sort-alpha-up", "chess-knight", "laugh-squint", "wheelchair", "circle-arrow-up", "toggle-on", "walking", "l", "fire", "procedures", "space-shuttle", "laugh", "folder-open", "heart-circle-plus", "code-fork", "city", "microphone-lines", "pepper-hot", "unlock", "colon-sign", "headset", "store-slash", "road-circle-xmark", "user-minus", "mars-stroke-v", "glass-cheers", "clipboard", "house-circle-exclamation", "file-upload", "wifi", "bathtub", "underline", "user-pen", "signature", "stroopwafel", "bold", "anchor-lock", "building-ngo", "manat-sign", "not-equal", "border-top-left", "map-marked-alt", "jedi", "square-poll-vertical", "mug-hot", "car-battery", "gift", "dice-two", "chess-queen", "glasses", "chess-board", "building-circle-check", "person-chalkboard", "mars-stroke-right", "hand-rock", "square-caret-up", "cloud-showers-water", "chart-bar", "hands-wash", "less-than-equal", "train", "low-vision", "crow", "sailboat", "window-restore", "square-plus", "torii-gate", "frog", "bucket", "image", "microphone", "cow", "caret-up", "screwdriver", "folder-closed", "house-tsunami", "square-nfi", "arrow-up-from-ground-water", "martini-glass", "undo-alt", "table-columns", "lemon", "head-side-mask", "handshake", "gem", "dolly", "smoking", "minimize", "monument", "snowplow", "angles-right", "cannabis", "play-circle", "tablets", "ethernet", "euro", "chair", "circle-check", "stop-circle", "drafting-compass", "plate-wheat", "icicles", "person-shelter", "neuter", "id-badge", "marker", "laugh-beam", "helicopter-symbol", "universal-access", "circle-chevron-up", "lari-sign", "volcano", "person-walking-dashed-line-arrow-right", "sterling-sign", "viruses", "square-person-confined", "user-tie", "long-arrow-down", "tent-arrow-down-to-line", "certificate", "reply-all", "suitcase", "skating", "funnel-dollar", "camera-retro", "circle-arrow-down", "file-import", "square-arrow-up-right", "box-open", "scroll", "spa", "location-pin-lock", "pause", "hill-avalanche", "thermometer-empty", "bomb", "registered", "vcard", "scale-unbalanced-flip", "subscript", "directions", "burst", "laptop-house", "tired", "money-bills", "smog", "crutch", "cloud-upload", "palette", "arrows-turn-right", "vest", "ferry", "arrows-down-to-people", "sprout", "left-right", "boxes-packing", "circle-arrow-left", "group-arrows-rotate", "bowl-food", "candy-cane", "sort-amount-down", "thunderstorm", "text-slash", "smile-wink", "file-word", "file-powerpoint", "arrows-left-right", "house-lock", "cloud-download", "children", "chalkboard", "user-large-slash", "envelope-open", "handshake-simple-slash", "mattress-pillow", "guarani-sign", "sync", "fire-extinguisher", "cruzeiro-sign", "greater-than-equal", "shield-halved", "book-atlas", "virus", "envelope-circle-check", "layer-group", "arrows-to-dot", "archway", "heart-circle-check", "house-damage", "file-zipper", "square", "martini-glass-empty", "couch", "cedi-sign", "italic", "church", "comments-dollar", "democrat", "z", "skiing", "road-lock", "a", "temperature-down", "feather-pointed", "p", "snowflake", "newspaper", "rectangle-ad", "circle-arrow-right", "filter-circle-xmark", "locust", "unsorted", "list-ol", "person-dress-burst", "money-check-dollar", "vector-square", "bread-slice", "language", "kiss-wink-heart", "filter", "question", "file-signature", "up-down-left-right", "house-chimney-user", "hand-holding-heart", "puzzle-piece", "money-check", "star-half-stroke", "code", "whiskey-glass", "building-circle-exclamation", "magnifying-glass-chart", "external-link", "cubes-stacked", "won", "virus-covid", "austral-sign", "f", "leaf", "road", "taxi", "person-circle-plus", "pie-chart", "bolt-lightning", "sack-xmark", "file-excel", "file-contract", "fish-fins", "building-flag", "grin-beam", "object-ungroup", "poop", "map-marker", "kaaba", "toilet-paper", "helmet-safety", "eject", "circle-right", "plane-circle-check", "meh-rolling-eyes", "object-group", "line-chart", "mask-ventilator", "arrow-right", "signs-post", "cash-register", "person-circle-question", "h", "tarp", "tools", "arrows-to-eye", "plug-circle-bolt", "heart", "mars-and-venus", "house-user", "dumpster-fire", "house-crack", "martini-glass-citrus", "surprise", "bottle-water", "pause-circle", "toilet-paper-slash", "apple-whole", "kitchen-set", "r", "thermometer-quarter", "cube", "bitcoin-sign", "shield-dog", "solar-panel", "lock-open", "elevator", "money-bill-transfer", "money-bill-trend-up", "house-flood-water-circle-arrow-right", "square-poll-horizontal", "circle", "fast-backward", "recycle", "user-astronaut", "plane-slash", "trademark", "basketball", "satellite-dish", "circle-up", "mobile-screen-button", "volume-up", "users-rays", "wallet", "clipboard-check", "file-audio", "hamburger", "wrench", "bugs", "rupee", "file-image", "question-circle", "plane-departure", "handshake-slash", "book-bookmark", "code-branch", "hat-cowboy", "bridge", "phone-flip", "truck-front", "cat", "anchor-circle-exclamation", "truck-field", "route", "clipboard-question", "panorama", "comment-medical", "teeth-open", "file-circle-minus", "tags", "wine-glass", "fast", "meh-blank", "square-parking", "house-signal", "tasks-alt", "faucet-drip", "dolly-flatbed", "smoking-ban", "terminal", "mobile-button", "house-medical-flag", "shopping-basket", "tape", "bus-simple", "eye", "sad-cry", "audio-description", "person-military-to-person", "file-shield", "user-slash", "pen", "tower-observation", "file-code", "signal", "bus", "heart-circle-xmark", "house-chimney", "window-maximize", "frown", "prescription", "store-alt", "save", "vihara", "scale-unbalanced", "sort-up", "commenting", "plant-wilt", "diamond", "grin-squint", "hand-holding-usd", "bacterium", "hand-pointer", "drum-steelpan", "hand-scissors", "praying-hands", "redo", "biohazard", "location", "mars-double", "child-dress", "users-between-lines", "lungs-virus", "grin-tears", "phone", "calendar-xmark", "child-reaching", "head-side-virus", "user-gear", "sort-numeric-up", "door-closed", "shield-virus", "dice-six", "mosquito-net", "bridge-water", "person-booth", "text-width", "hat-wizard", "fancy", "person-digging", "trash", "tachometer-average", "book-medical", "poo", "quote-right", "tshirt", "cubes", "divide", "tenge", "headphones", "hands-holding", "hands-clapping", "republican", "arrow-left", "person-circle-xmark", "ruler", "align-left", "dice-d6", "restroom", "j", "users-viewfinder", "file-video", "up-right-from-square", "th", "file-pdf", "book-bible", "o", "suitcase-medical", "user-secret", "otter", "person-dress", "comment-dollar", "business-time", "th-large", "tanakh", "volume-control-phone", "hat-cowboy-side", "clipboard-user", "child", "lira-sign", "satellite", "plane-lock", "tag", "comment", "cake", "envelope", "angles-up", "paperclip", "arrow-right-to-city", "ribbon", "lungs", "sort-numeric-up-alt", "litecoin-sign", "border-none", "circle-nodes", "parachute-box", "indent", "truck-field-un", "hourglass", "mountain", "user-md", "info-circle", "cloud-meatball", "camera", "square-virus", "meteor", "car-on", "sleigh", "sort-numeric-down", "hand-holding-water", "water", "calendar-check", "braille", "prescription-bottle-medical", "landmark", "truck", "crosshairs", "person-cane", "tent", "vest-patches", "check-double", "sort-alpha-down", "money-bill-wheat", "cookie", "undo", "hdd", "grin-squint-tears", "dumbbell", "rectangle-list", "tarp-droplet", "house-medical-circle-check", "skiing-nordic", "calendar-plus", "plane-arrival", "circle-left", "train-subway", "chart-gantt", "inr", "crop-simple", "money-bill-alt", "long-arrow-alt-left", "dna", "virus-slash", "subtract", "chess", "long-arrow-left", "plug-circle-check", "street-view", "franc-sign", "volume-off", "hands-asl-interpreting", "gear", "tint-slash", "mosque", "mosquito", "star-of-david", "person-military-rifle", "shopping-cart", "vials", "plug-circle-plus", "place-of-worship", "grip-vertical", "level-up", "u", "square-root-variable", "clock", "step-backward", "pallet", "faucet", "baseball-bat-ball", "s", "timeline", "keyboard", "caret-down", "house-chimney-medical", "thermometer-three-quarters", "mobile-screen", "plane-up", "piggy-bank", "battery-half", "mountain-city", "coins", "khanda", "sliders", "folder-tree", "network-wired", "map-pin", "hamsa", "cent-sign", "flask", "person-pregnant", "wand-sparkles", "ellipsis-vertical", "ticket", "power-off", "right-long", "flag-usa", "laptop-file", "tty", "diagram-next", "person-rifle", "house-medical-circle-exclamation", "closed-captioning", "person-hiking", "venus-double", "images", "calculator", "people-pulling", "n", "tram", "cloud-rain", "building-circle-xmark", "ship", "arrows-down-to-line", "download", "grin", "delete-left", "eyedropper", "file-circle-check", "forward", "mobile", "meh", "align-center", "book-skull", "id-card", "outdent", "heart-circle-exclamation", "house", "calendar-week", "laptop-medical", "b", "file-medical", "dice-one", "kiwi-bird", "exchange", "rotate-right", "utensils", "sort-amount-up", "mill-sign", "bowl-rice", "skull", "tower-broadcast", "truck-pickup", "up-long", "stop", "code-merge", "upload", "hurricane", "mound", "toilet-portable", "compact-disc", "file-download", "caravan", "shield-cat", "zap", "glass-water", "oil-well", "vault", "mars", "toilet", "plane-circle-xmark", "yen", "ruble", "sun", "guitar", "laugh-wink", "horse-head", "bore-hole", "industry", "circle-down", "arrows-turn-to-dots", "florin-sign", "sort-amount-down-alt", "less-than", "angle-down", "car-tunnel", "head-side-cough", "grip-lines", "thumbs-down", "user-lock", "long-arrow-right", "anchor-circle-xmark", "ellipsis", "chess-pawn", "kit-medical", "person-through-window", "toolbox", "hands-holding-circle", "bug", "credit-card", "car", "hand-holding-hand", "book-reader", "mountain-sun", "arrows-left-right-to-line", "dice-d20", "truck-droplet", "file-circle-xmark", "temperature-up", "medal", "bed", "square-h", "podcast", "thermometer-full", "bell", "superscript", "plug-circle-xmark", "star-of-life", "phone-slash", "paint-roller", "handshake-angle", "map-marker-alt", "file", "greater-than", "swimmer", "arrow-down", "tint", "eraser", "globe-americas", "person-burst", "dove", "battery-empty", "socks", "inbox", "section", "tachometer-alt", "envelope-open-text", "hospital", "wine-bottle", "chess-rook", "stream", "dharmachakra", "hotdog", "person-walking-with-cane", "drum", "ice-cream", "heart-circle-bolt", "fax", "paragraph", "vote-yea", "star-half", "boxes", "link", "ear-listen", "tree-city", "play", "font", "rupiah-sign", "search", "table-tennis", "person-dots-from-line", "trash-restore-alt", "naira-sign", "cart-arrow-down", "walkie-talkie", "file-pen", "receipt", "square-pen", "suitcase-rolling", "person-circle-exclamation", "chevron-down", "battery", "skull-crossbones", "code-compare", "list-ul", "school-lock", "tower-cell", "long-arrow-alt-down", "ranking-star", "chess-king", "person-harassing", "brazilian-real-sign", "landmark-dome", "arrow-up", "tv", "shrimp", "tasks", "jug-detergent", "user-circle", "user-shield", "wind", "car-crash", "y", "snowboarding", "fast", "fish", "user-graduate", "circle-half-stroke", "clapperboard", "radiation-alt", "baseball", "jet-fighter-up", "project-diagram", "copy", "volume-xmark", "hand-sparkles", "grip", "share-square", "child-rifle", "gun", "square-phone", "plus", "expand", "computer", "xmark", "arrows", "chalkboard-user", "peso-sign", "building-shield", "baby", "users-line", "quote-left", "tractor", "trash-restore", "arrow-down-up-lock", "lines-leaning", "ruler-combined", "copyright", "equals", "blender", "teeth", "sheqel", "map", "rocket", "photo-video", "folder-minus", "store", "arrow-trend-up", "plug-circle-minus", "sign", "bezier-curve", "bell-slash", "tablet", "school-flag", "fill", "angle-up", "drumstick-bite", "holly-berry", "chevron-left", "bacteria", "hand-lizard", "notdef", "disease", "briefcase-medical", "genderless", "chevron-right", "retweet", "car-rear", "pump-soap", "video-slash", "battery-quarter", "radio", "carriage-baby", "traffic-light", "thermometer", "vr-cardboard", "hand-middle-finger", "percentage", "truck-moving", "glass-water-droplet", "display", "smile", "thumbtack", "trophy", "pray", "hammer", "hand-peace", "sync-alt", "spinner", "robot", "peace", "gears", "warehouse", "arrow-up-right-dots", "splotch", "grin-hearts", "dice-four", "sim-card", "transgender", "mercury", "level-down", "falling-burst", "award", "ticket-simple", "building", "angles-left", "qrcode", "history", "grin-beam-sweat", "file-export", "shield", "sort-amount-up-alt", "house-medical", "golf-ball", "circle-chevron-left", "house-chimney-window", "pen-nib", "tent-arrow-turn-left", "tents", "wand-magic", "dog", "carrot", "moon", "wine-glass-empty", "cheese", "yin-yang", "music", "code-commit", "temperature-low", "person-biking", "broom", "shield-heart", "gopuram", "globe-oceania", "xmark-square", "hashtag", "up-right-and-down-left-from-center", "oil-can", "t", "hippo", "chart-column", "infinity", "vial-circle-check", "person-arrow-down-to-line", "voicemail", "fan", "person-walking-luggage", "up-down", "cloud-moon-rain", "calendar", "trailer", "haykal", "sd-card", "dragon", "shoe-prints", "plus-circle", "grin-tongue-wink", "hand-holding", "plug-circle-exclamation", "unlink", "clone", "person-walking-arrow-loop-left", "sort-alpha-up-alt", "fire-flame-curved", "tornado", "file-circle-plus", "quran", "anchor", "border-all", "face-angry", "cookie-bite", "arrow-trend-down", "rss", "draw-polygon", "scale-balanced", "tachometer", "shower", "desktop", "m", "th-list", "sms", "book", "user-plus", "check", "battery-three-quarters", "house-circle-check", "angle-left", "diagram-successor", "truck-arrow-right", "arrows-split-up-and-left", "hand-fist", "cloud-moon", "briefcase", "falling", "portrait", "user-tag", "rug", "globe-europe", "luggage-cart", "window-close", "baht-sign", "book-open", "journal-whills", "handcuffs", "warning", "database", "share", "bottle-droplet", "face", "hill-rockslide", "right-left", "paper-plane", "road-circle-exclamation", "dungeon", "align-right", "money-bill-wave-alt", "life-ring", "signing", "calendar-day", "water-ladder", "arrows-v", "grimace", "wheelchair-move", "turn-down", "person-walking-arrow-right", "square-envelope", "dice", "bowling-ball", "brain", "bandage", "calendar-minus", "xmark-circle", "gifts", "hotel", "globe-asia", "id-card-clip", "search-plus", "thumbs-up", "user-clock", "hand-dots", "file-invoice", "window-minimize", "mug-saucer", "brush", "mask", "search-minus", "ruler-vertical", "user-large", "train-tram", "user-nurse", "syringe", "cloud-sun", "stopwatch-20", "square-full", "magnet", "jar", "sticky-note", "bug-slash", "arrow-up-from-water-pump", "bone", "user-injured", "sad-tear", "plane", "tent-arrows-down", "exclamation", "arrows-spin", "print", "turkish-lira", "usd", "x", "search-dollar", "users-gear", "person-military-pointing", "university", "umbrella", "trowel", "d", "stapler", "theater-masks", "kip-sign", "hand-point-left", "handshake-simple", "jet-fighter", "square-share-nodes", "barcode", "plus-minus", "video", "mortar-board", "hand-holding-medical", "person-circle-check", "turn-up"];
+const Ne = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "fill-drip", "arrows-to-circle", "circle-chevron-right", "at", "trash-can", "text-height", "user-xmark", "stethoscope", "message", "info", "down-left-and-up-right-to-center", "explosion", "file-text", "wave-square", "ring", "building-un", "dice-three", "calendar-days", "anchor-circle-check", "building-circle-arrow-right", "volleyball", "arrows-up-to-line", "sort-down", "minus-circle", "door-open", "sign-out-alt", "atom", "soap", "icons", "microphone-lines-slash", "bridge-circle-check", "pump-medical", "fingerprint", "hand-point-right", "search-location", "step-forward", "smile-beam", "flag-checkered", "football", "school-circle-exclamation", "crop", "angles-down", "users-rectangle", "people-roof", "people-line", "beer", "diagram-predecessor", "long-arrow-up", "fire-flame-simple", "person", "laptop", "file-csv", "menorah", "truck-plane", "record-vinyl", "grin-stars", "bong", "spaghetti-monster-flying", "arrow-down-up-across-line", "utensil-spoon", "jar-wheat", "mail-bulk", "file-circle-exclamation", "hospital-symbol", "pager", "contact-book", "strikethrough", "k", "landmark-flag", "pencil", "backward", "caret-right", "comments", "paste", "code-pull-request", "clipboard-list", "truck-ramp-box", "user-check", "vial-virus", "sheet-plastic", "blog", "user-ninja", "person-arrow-up-from-line", "torah", "quidditch", "toggle-off", "box-archive", "person-drowning", "sort-numeric-down-alt", "grin-tongue-squint", "spray-can", "truck-monster", "w", "globe-africa", "rainbow", "circle-notch", "tablet-screen-button", "paw", "cloud", "trowel-bricks", "flushed", "hospital-user", "tent-arrow-left-right", "legal", "binoculars", "microphone-slash", "box-tissue", "motorcycle", "concierge-bell", "pencil-ruler", "people-arrows", "mars-and-venus-burst", "square-caret-right", "scissors", "sun-plant-wilt", "toilets-portable", "hockey-puck", "table", "magnifying-glass-arrow-right", "tachograph-digital", "users-slash", "clover", "reply", "star-and-crescent", "house-fire", "square-minus", "helicopter", "compass", "square-caret-down", "file-circle-question", "laptop-code", "swatchbook", "prescription-bottle", "navicon", "people-group", "hourglass-end", "heart-crack", "square-up-right", "kiss-beam", "film", "ruler-horizontal", "people-robbery", "lightbulb", "caret-left", "exclamation-circle", "school-circle-xmark", "sign-out", "circle-chevron-down", "unlock-keyhole", "cloud-showers-heavy", "headphones-simple", "sitemap", "donate", "memory", "road-spikes", "fire-burner", "flag", "hanukiah", "feather", "volume-low", "comment-slash", "cloud-sun-rain", "compress", "wheat-awn", "ankh", "hands-holding-child", "asterisk", "square-check", "peseta-sign", "heading", "ghost", "list", "square-phone-flip", "cart-plus", "gamepad", "dot-circle", "face-dizzy", "egg", "house-medical-circle-xmark", "campground", "folder-plus", "soccer-ball", "paintbrush", "lock", "gas-pump", "hot-tub", "map-marked", "house-flood-water", "tree", "bridge-lock", "sack-dollar", "pen-to-square", "car-side", "share-nodes", "heart-circle-minus", "hourglass-half", "microscope", "sink", "shopping-bag", "sort-alpha-down-alt", "mitten", "person-rays", "users", "eye-slash", "flask-vial", "hand", "om", "worm", "house-circle-xmark", "plug", "chevron-up", "hand-spock", "stopwatch", "kiss", "bridge-circle-xmark", "grin-tongue", "chess-bishop", "grin-wink", "hard-of-hearing", "road-circle-check", "dice-five", "square-rss", "land-mine-on", "i-cursor", "stamp", "stairs", "i", "hryvnia", "pills", "grin-alt", "tooth", "v", "bangladeshi-taka-sign", "bicycle", "staff-snake", "head-side-cough-slash", "truck-medical", "wheat-awn-circle-exclamation", "snowman", "mortar-pestle", "road-barrier", "school", "igloo", "joint", "angle-right", "horse", "q", "g", "notes-medical", "thermometer-half", "dong-sign", "capsules", "poo-storm", "frown-open", "hand-point-up", "money-bill", "bookmark", "align-justify", "umbrella-beach", "helmet-un", "bullseye", "bacon", "hand-point-down", "arrow-up-from-bracket", "folder", "file-waveform", "radiation", "chart-simple", "mars-stroke", "vial", "tachometer-alt-average", "wand-magic-sparkles", "e", "pen-clip", "bridge-circle-exclamation", "user", "school-circle-check", "dumpster", "van-shuttle", "building-user", "square-caret-left", "highlighter", "key", "bullhorn", "globe", "synagogue", "person-half-dress", "road-bridge", "location-arrow", "c", "tablet-button", "building-lock", "pizza-slice", "money-bill-wave", "chart-area", "house-flag", "person-circle-minus", "cancel", "camera-rotate", "spray-can-sparkles", "star", "repeat", "cross", "box", "venus-mars", "mouse-pointer", "maximize", "charging-station", "triangle-circle-square", "shuffle", "running", "mobile-retro", "grip-lines-vertical", "spider", "hands-bound", "file-invoice-dollar", "plane-circle-exclamation", "x-ray", "spell-check", "slash", "mouse", "sign-in", "store-alt-slash", "server", "virus-covid-slash", "shop-lock", "hourglass-start", "blender-phone", "building-wheat", "person-breastfeeding", "sign-in-alt", "venus", "passport", "heartbeat", "people-carry", "temperature-high", "microchip", "crown", "weight-hanging", "xmarks-lines", "file-prescription", "weight", "user-group", "sort-alpha-up", "chess-knight", "laugh-squint", "wheelchair", "circle-arrow-up", "toggle-on", "walking", "l", "fire", "procedures", "space-shuttle", "laugh", "folder-open", "heart-circle-plus", "code-fork", "city", "microphone-lines", "pepper-hot", "unlock", "colon-sign", "headset", "store-slash", "road-circle-xmark", "user-minus", "mars-stroke-v", "glass-cheers", "clipboard", "house-circle-exclamation", "file-upload", "wifi", "bathtub", "underline", "user-pen", "signature", "stroopwafel", "bold", "anchor-lock", "building-ngo", "manat-sign", "not-equal", "border-top-left", "map-marked-alt", "jedi", "square-poll-vertical", "mug-hot", "car-battery", "gift", "dice-two", "chess-queen", "glasses", "chess-board", "building-circle-check", "person-chalkboard", "mars-stroke-right", "hand-rock", "square-caret-up", "cloud-showers-water", "chart-bar", "hands-wash", "less-than-equal", "train", "low-vision", "crow", "sailboat", "window-restore", "square-plus", "torii-gate", "frog", "bucket", "image", "microphone", "cow", "caret-up", "screwdriver", "folder-closed", "house-tsunami", "square-nfi", "arrow-up-from-ground-water", "martini-glass", "undo-alt", "table-columns", "lemon", "head-side-mask", "handshake", "gem", "dolly", "smoking", "minimize", "monument", "snowplow", "angles-right", "cannabis", "play-circle", "tablets", "ethernet", "euro", "chair", "circle-check", "stop-circle", "drafting-compass", "plate-wheat", "icicles", "person-shelter", "neuter", "id-badge", "marker", "laugh-beam", "helicopter-symbol", "universal-access", "circle-chevron-up", "lari-sign", "volcano", "person-walking-dashed-line-arrow-right", "sterling-sign", "viruses", "square-person-confined", "user-tie", "long-arrow-down", "tent-arrow-down-to-line", "certificate", "reply-all", "suitcase", "skating", "funnel-dollar", "camera-retro", "circle-arrow-down", "file-import", "square-arrow-up-right", "box-open", "scroll", "spa", "location-pin-lock", "pause", "hill-avalanche", "thermometer-empty", "bomb", "registered", "vcard", "scale-unbalanced-flip", "subscript", "directions", "burst", "laptop-house", "tired", "money-bills", "smog", "crutch", "cloud-upload", "palette", "arrows-turn-right", "vest", "ferry", "arrows-down-to-people", "sprout", "left-right", "boxes-packing", "circle-arrow-left", "group-arrows-rotate", "bowl-food", "candy-cane", "sort-amount-down", "thunderstorm", "text-slash", "smile-wink", "file-word", "file-powerpoint", "arrows-left-right", "house-lock", "cloud-download", "children", "chalkboard", "user-large-slash", "envelope-open", "handshake-simple-slash", "mattress-pillow", "guarani-sign", "sync", "fire-extinguisher", "cruzeiro-sign", "greater-than-equal", "shield-halved", "book-atlas", "virus", "envelope-circle-check", "layer-group", "arrows-to-dot", "archway", "heart-circle-check", "house-damage", "file-zipper", "square", "martini-glass-empty", "couch", "cedi-sign", "italic", "church", "comments-dollar", "democrat", "z", "skiing", "road-lock", "a", "temperature-down", "feather-pointed", "p", "snowflake", "newspaper", "rectangle-ad", "circle-arrow-right", "filter-circle-xmark", "locust", "unsorted", "list-ol", "person-dress-burst", "money-check-dollar", "vector-square", "bread-slice", "language", "kiss-wink-heart", "filter", "question", "file-signature", "up-down-left-right", "house-chimney-user", "hand-holding-heart", "puzzle-piece", "money-check", "star-half-stroke", "code", "whiskey-glass", "building-circle-exclamation", "magnifying-glass-chart", "external-link", "cubes-stacked", "won", "virus-covid", "austral-sign", "f", "leaf", "road", "taxi", "person-circle-plus", "pie-chart", "bolt-lightning", "sack-xmark", "file-excel", "file-contract", "fish-fins", "building-flag", "grin-beam", "object-ungroup", "poop", "map-marker", "kaaba", "toilet-paper", "helmet-safety", "eject", "circle-right", "plane-circle-check", "meh-rolling-eyes", "object-group", "line-chart", "mask-ventilator", "arrow-right", "signs-post", "cash-register", "person-circle-question", "h", "tarp", "tools", "arrows-to-eye", "plug-circle-bolt", "heart", "mars-and-venus", "house-user", "dumpster-fire", "house-crack", "martini-glass-citrus", "surprise", "bottle-water", "pause-circle", "toilet-paper-slash", "apple-whole", "kitchen-set", "r", "thermometer-quarter", "cube", "bitcoin-sign", "shield-dog", "solar-panel", "lock-open", "elevator", "money-bill-transfer", "money-bill-trend-up", "house-flood-water-circle-arrow-right", "square-poll-horizontal", "circle", "fast-backward", "recycle", "user-astronaut", "plane-slash", "trademark", "basketball", "satellite-dish", "circle-up", "mobile-screen-button", "volume-up", "users-rays", "wallet", "clipboard-check", "file-audio", "hamburger", "wrench", "bugs", "rupee", "file-image", "question-circle", "plane-departure", "handshake-slash", "book-bookmark", "code-branch", "hat-cowboy", "bridge", "phone-flip", "truck-front", "cat", "anchor-circle-exclamation", "truck-field", "route", "clipboard-question", "panorama", "comment-medical", "teeth-open", "file-circle-minus", "tags", "wine-glass", "fast", "meh-blank", "square-parking", "house-signal", "tasks-alt", "faucet-drip", "dolly-flatbed", "smoking-ban", "terminal", "mobile-button", "house-medical-flag", "shopping-basket", "tape", "bus-simple", "eye", "sad-cry", "audio-description", "person-military-to-person", "file-shield", "user-slash", "pen", "tower-observation", "file-code", "signal", "bus", "heart-circle-xmark", "house-chimney", "window-maximize", "frown", "prescription", "store-alt", "save", "vihara", "scale-unbalanced", "sort-up", "commenting", "plant-wilt", "diamond", "grin-squint", "hand-holding-usd", "bacterium", "hand-pointer", "drum-steelpan", "hand-scissors", "praying-hands", "redo", "biohazard", "location", "mars-double", "child-dress", "users-between-lines", "lungs-virus", "grin-tears", "phone", "calendar-xmark", "child-reaching", "head-side-virus", "user-gear", "sort-numeric-up", "door-closed", "shield-virus", "dice-six", "mosquito-net", "bridge-water", "person-booth", "text-width", "hat-wizard", "fancy", "person-digging", "trash", "tachometer-average", "book-medical", "poo", "quote-right", "tshirt", "cubes", "divide", "tenge", "headphones", "hands-holding", "hands-clapping", "republican", "arrow-left", "person-circle-xmark", "ruler", "align-left", "dice-d6", "restroom", "j", "users-viewfinder", "file-video", "up-right-from-square", "th", "file-pdf", "book-bible", "o", "suitcase-medical", "user-secret", "otter", "person-dress", "comment-dollar", "business-time", "th-large", "tanakh", "volume-control-phone", "hat-cowboy-side", "clipboard-user", "child", "lira-sign", "satellite", "plane-lock", "tag", "comment", "cake", "envelope", "angles-up", "paperclip", "arrow-right-to-city", "ribbon", "lungs", "sort-numeric-up-alt", "litecoin-sign", "border-none", "circle-nodes", "parachute-box", "indent", "truck-field-un", "hourglass", "mountain", "user-md", "info-circle", "cloud-meatball", "camera", "square-virus", "meteor", "car-on", "sleigh", "sort-numeric-down", "hand-holding-water", "water", "calendar-check", "braille", "prescription-bottle-medical", "landmark", "truck", "crosshairs", "person-cane", "tent", "vest-patches", "check-double", "sort-alpha-down", "money-bill-wheat", "cookie", "undo", "hdd", "grin-squint-tears", "dumbbell", "rectangle-list", "tarp-droplet", "house-medical-circle-check", "skiing-nordic", "calendar-plus", "plane-arrival", "circle-left", "train-subway", "chart-gantt", "inr", "crop-simple", "money-bill-alt", "long-arrow-alt-left", "dna", "virus-slash", "subtract", "chess", "long-arrow-left", "plug-circle-check", "street-view", "franc-sign", "volume-off", "hands-asl-interpreting", "gear", "tint-slash", "mosque", "mosquito", "star-of-david", "person-military-rifle", "shopping-cart", "vials", "plug-circle-plus", "place-of-worship", "grip-vertical", "level-up", "u", "square-root-variable", "clock", "step-backward", "pallet", "faucet", "baseball-bat-ball", "s", "timeline", "keyboard", "caret-down", "house-chimney-medical", "thermometer-three-quarters", "mobile-screen", "plane-up", "piggy-bank", "battery-half", "mountain-city", "coins", "khanda", "sliders", "folder-tree", "network-wired", "map-pin", "hamsa", "cent-sign", "flask", "person-pregnant", "wand-sparkles", "ellipsis-vertical", "ticket", "power-off", "right-long", "flag-usa", "laptop-file", "tty", "diagram-next", "person-rifle", "house-medical-circle-exclamation", "closed-captioning", "person-hiking", "venus-double", "images", "calculator", "people-pulling", "n", "tram", "cloud-rain", "building-circle-xmark", "ship", "arrows-down-to-line", "download", "grin", "delete-left", "eyedropper", "file-circle-check", "forward", "mobile", "meh", "align-center", "book-skull", "id-card", "outdent", "heart-circle-exclamation", "house", "calendar-week", "laptop-medical", "b", "file-medical", "dice-one", "kiwi-bird", "exchange", "rotate-right", "utensils", "sort-amount-up", "mill-sign", "bowl-rice", "skull", "tower-broadcast", "truck-pickup", "up-long", "stop", "code-merge", "upload", "hurricane", "mound", "toilet-portable", "compact-disc", "file-download", "caravan", "shield-cat", "zap", "glass-water", "oil-well", "vault", "mars", "toilet", "plane-circle-xmark", "yen", "ruble", "sun", "guitar", "laugh-wink", "horse-head", "bore-hole", "industry", "circle-down", "arrows-turn-to-dots", "florin-sign", "sort-amount-down-alt", "less-than", "angle-down", "car-tunnel", "head-side-cough", "grip-lines", "thumbs-down", "user-lock", "long-arrow-right", "anchor-circle-xmark", "ellipsis", "chess-pawn", "kit-medical", "person-through-window", "toolbox", "hands-holding-circle", "bug", "credit-card", "car", "hand-holding-hand", "book-reader", "mountain-sun", "arrows-left-right-to-line", "dice-d20", "truck-droplet", "file-circle-xmark", "temperature-up", "medal", "bed", "square-h", "podcast", "thermometer-full", "bell", "superscript", "plug-circle-xmark", "star-of-life", "phone-slash", "paint-roller", "handshake-angle", "map-marker-alt", "file", "greater-than", "swimmer", "arrow-down", "tint", "eraser", "globe-americas", "person-burst", "dove", "battery-empty", "socks", "inbox", "section", "tachometer-alt", "envelope-open-text", "hospital", "wine-bottle", "chess-rook", "stream", "dharmachakra", "hotdog", "person-walking-with-cane", "drum", "ice-cream", "heart-circle-bolt", "fax", "paragraph", "vote-yea", "star-half", "boxes", "link", "ear-listen", "tree-city", "play", "font", "rupiah-sign", "search", "table-tennis", "person-dots-from-line", "trash-restore-alt", "naira-sign", "cart-arrow-down", "walkie-talkie", "file-pen", "receipt", "square-pen", "suitcase-rolling", "person-circle-exclamation", "chevron-down", "battery", "skull-crossbones", "code-compare", "list-ul", "school-lock", "tower-cell", "long-arrow-alt-down", "ranking-star", "chess-king", "person-harassing", "brazilian-real-sign", "landmark-dome", "arrow-up", "tv", "shrimp", "tasks", "jug-detergent", "user-circle", "user-shield", "wind", "car-crash", "y", "snowboarding", "fast", "fish", "user-graduate", "circle-half-stroke", "clapperboard", "radiation-alt", "baseball", "jet-fighter-up", "project-diagram", "copy", "volume-xmark", "hand-sparkles", "grip", "share-square", "child-rifle", "gun", "square-phone", "plus", "expand", "computer", "xmark", "arrows", "chalkboard-user", "peso-sign", "building-shield", "baby", "users-line", "quote-left", "tractor", "trash-restore", "arrow-down-up-lock", "lines-leaning", "ruler-combined", "copyright", "equals", "blender", "teeth", "sheqel", "map", "rocket", "photo-video", "folder-minus", "store", "arrow-trend-up", "plug-circle-minus", "sign", "bezier-curve", "bell-slash", "tablet", "school-flag", "fill", "angle-up", "drumstick-bite", "holly-berry", "chevron-left", "bacteria", "hand-lizard", "notdef", "disease", "briefcase-medical", "genderless", "chevron-right", "retweet", "car-rear", "pump-soap", "video-slash", "battery-quarter", "radio", "carriage-baby", "traffic-light", "thermometer", "vr-cardboard", "hand-middle-finger", "percentage", "truck-moving", "glass-water-droplet", "display", "smile", "thumbtack", "trophy", "pray", "hammer", "hand-peace", "sync-alt", "spinner", "robot", "peace", "gears", "warehouse", "arrow-up-right-dots", "splotch", "grin-hearts", "dice-four", "sim-card", "transgender", "mercury", "level-down", "falling-burst", "award", "ticket-simple", "building", "angles-left", "qrcode", "history", "grin-beam-sweat", "file-export", "shield", "sort-amount-up-alt", "house-medical", "golf-ball", "circle-chevron-left", "house-chimney-window", "pen-nib", "tent-arrow-turn-left", "tents", "wand-magic", "dog", "carrot", "moon", "wine-glass-empty", "cheese", "yin-yang", "music", "code-commit", "temperature-low", "person-biking", "broom", "shield-heart", "gopuram", "globe-oceania", "xmark-square", "hashtag", "up-right-and-down-left-from-center", "oil-can", "t", "hippo", "chart-column", "infinity", "vial-circle-check", "person-arrow-down-to-line", "voicemail", "fan", "person-walking-luggage", "up-down", "cloud-moon-rain", "calendar", "trailer", "haykal", "sd-card", "dragon", "shoe-prints", "plus-circle", "grin-tongue-wink", "hand-holding", "plug-circle-exclamation", "unlink", "clone", "person-walking-arrow-loop-left", "sort-alpha-up-alt", "fire-flame-curved", "tornado", "file-circle-plus", "quran", "anchor", "border-all", "face-angry", "cookie-bite", "arrow-trend-down", "rss", "draw-polygon", "scale-balanced", "tachometer", "shower", "desktop", "m", "th-list", "sms", "book", "user-plus", "check", "battery-three-quarters", "house-circle-check", "angle-left", "diagram-successor", "truck-arrow-right", "arrows-split-up-and-left", "hand-fist", "cloud-moon", "briefcase", "falling", "portrait", "user-tag", "rug", "globe-europe", "luggage-cart", "window-close", "baht-sign", "book-open", "journal-whills", "handcuffs", "warning", "database", "share", "bottle-droplet", "face", "hill-rockslide", "right-left", "paper-plane", "road-circle-exclamation", "dungeon", "align-right", "money-bill-wave-alt", "life-ring", "signing", "calendar-day", "water-ladder", "arrows-v", "grimace", "wheelchair-move", "turn-down", "person-walking-arrow-right", "square-envelope", "dice", "bowling-ball", "brain", "bandage", "calendar-minus", "xmark-circle", "gifts", "hotel", "globe-asia", "id-card-clip", "search-plus", "thumbs-up", "user-clock", "hand-dots", "file-invoice", "window-minimize", "mug-saucer", "brush", "mask", "search-minus", "ruler-vertical", "user-large", "train-tram", "user-nurse", "syringe", "cloud-sun", "stopwatch-20", "square-full", "magnet", "jar", "sticky-note", "bug-slash", "arrow-up-from-water-pump", "bone", "user-injured", "sad-tear", "plane", "tent-arrows-down", "exclamation", "arrows-spin", "print", "turkish-lira", "usd", "x", "search-dollar", "users-gear", "person-military-pointing", "university", "umbrella", "trowel", "d", "stapler", "theater-masks", "kip-sign", "hand-point-left", "handshake-simple", "jet-fighter", "square-share-nodes", "barcode", "plus-minus", "video", "mortar-board", "hand-holding-medical", "person-circle-check", "turn-up"];
 
-function Le(e) {
+function qe(e) {
     function n() {
         const a = {
             position: "fixed",
             color: "white",
             backgroundColor: e.isError ? "#e52207" : k.colors.success,
             width: 300,
             top: 10,
@@ -131,17 +131,17 @@
                 }
             }), e.text]
         })
     }
     return n()
 }
 
-function te(e, n = !1) {
+function G(e, n = !1) {
     const a = document.createElement("div");
-    a.classList.add("message"), z.createRoot(document.body.appendChild(a)).render(t.jsx(Le, {
+    a.classList.add("message"), W.createRoot(document.body.appendChild(a)).render(t.jsx(qe, {
         text: e,
         isError: n
     })), setTimeout(function() {
         a.remove()
     }, 3e3)
 }
 
@@ -170,27 +170,30 @@
                 children: e.children
             })]
         })
     }
     return n()
 }
 
-function Ne(e) {
-    return we(e.data)
+function Le(e) {
+    const n = e.data;
+    n.store && Object.keys(n.store).map(function(a) {
+        n.store[a] ? localStorage.setItem(a, n.store[a]) : localStorage.removeItem(a, n.store[a])
+    }), n.redirect && n.redirect.length > 2 ? (n.message && localStorage.setItem("message", n.message), document.location.href = H(n.redirect)) : n.message && G(n.message)
 }
 
 function A(e) {
     return e.replace("/app/", "/api/")
 }
 
-function U(e) {
+function H(e) {
     return e.replace("/api/", "/app/")
 }
 
-function L(e, n, a, r) {
+function q(e, n, a, r) {
     const i = localStorage.getItem("token");
     var l = {
         Accept: "application/json"
     };
     i && (l.Authorization = "Token " + i);
     const d = A(n);
     var c = {
@@ -204,41 +207,35 @@
     fetch(d, c).then(function(o) {
         if (s = o, u = s.headers.get("Content-Type"), u == "application/json") return o.text();
         if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) return o.arrayBuffer();
         o.text()
     }).then(o => {
         if (u == "application/json") {
             var h = JSON.parse(o || "{}");
-            typeof h == "object" && h.type == "redirect" ? document.location.href = U(h.url) : a && a(h, s)
+            typeof h == "object" && h.type == "redirect" ? document.location.href = H(h.url) : a && a(h, s)
         } else if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) {
-            var f = window.URL.createObjectURL(new Blob([new Uint8Array(o)], {
+            var g = window.URL.createObjectURL(new Blob([new Uint8Array(o)], {
                     type: u
                 })),
                 w = document.createElement("a");
-            w.href = f, u.indexOf("excel") >= 0 ? w.download = "Download.xls" : u.indexOf("pdf") >= 0 ? w.download = "Download.pdf" : u.indexOf("zip") >= 0 ? w.download = "Download.zip" : u.indexOf("json") >= 0 ? w.download = "Download.json" : u.indexOf("csv") >= 0 ? w.download = "Download.csv" : u.indexOf("png") >= 0 && (w.download = "Download.png"), document.body.appendChild(w), w.click(), a && a({}, s)
+            w.href = g, u.indexOf("excel") >= 0 ? w.download = "Download.xls" : u.indexOf("pdf") >= 0 ? w.download = "Download.pdf" : u.indexOf("zip") >= 0 ? w.download = "Download.zip" : u.indexOf("json") >= 0 ? w.download = "Download.json" : u.indexOf("csv") >= 0 ? w.download = "Download.csv" : u.indexOf("png") >= 0 && (w.download = "Download.png"), document.body.appendChild(w), w.click(), a && a({}, s)
         } else a && a(o, s)
     })
 }
 
-function we(e) {
-    e.store && Object.keys(e.store).map(function(n) {
-        e.store[n] ? localStorage.setItem(n, e.store[n]) : localStorage.removeItem(n, e.store[n])
-    }), e.redirect ? (e.message && localStorage.setItem("message", e.message), document.location.href = U(e.redirect)) : e.message && te(e.message)
-}
-
-function F(e) {
+function z(e) {
     if (e === null || e === "") return "-";
     if (e === !0) return "Sim";
     if (e === !1) return "Não";
     if (typeof e == "number") {
         var n = e.toString().split(".");
         return n.length == 1 ? e.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ".") : (n[0] = n[0].toString().replace(/\B(?=(\d{3})+(?!\d))/g, "."), n[1] = n[1].substring(0, 2), n[1].length == 1 && (n[1] = n[1] + "0"), n[0] + "," + n[1])
     }
     if (typeof e == "string") {
-        if (e.length == 7 && e[0] == "#") return t.jsx(x, {
+        if (e.length == 7 && e[0] == "#") return t.jsx(y, {
             data: {
                 type: "color",
                 value: e
             }
         });
         if (e.length == 19 && e[13] == ":" && e[16] == ":") {
             var n = e.split(" "),
@@ -250,19 +247,19 @@
 `).map(function(i, l) {
             return t.jsx("div", {
                 children: i
             }, Math.random())
         });
         return e
     }
-    return typeof e == "object" && e.type ? t.jsx(x, {
+    return typeof e == "object" && e.type ? t.jsx(y, {
         data: e
     }) : typeof e == "object" && Array.isArray(e) ? e.length == 0 ? "-" : typeof e[0] == "object" && e[0].type != null ? t.jsx(t.Fragment, {
         children: e.map(function(i) {
-            return t.jsx(x, {
+            return t.jsx(y, {
                 data: i
             }, Math.random())
         })
     }) : t.jsx("ul", {
         style: {
             padding: 0,
             marginLeft: 17
@@ -272,42 +269,42 @@
                 children: i
             }, Math.random())
         })
     }) : typeof e == "object" && JSON.stringify(Object.keys(e)) == JSON.stringify(["id", "text"]) ? e.text : JSON.stringify(e)
 }
 
 function de() {
-    document.querySelector(".layer") == null && z.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Oe, {}))
+    document.querySelector(".layer") == null && W.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Oe, {}))
 }
 
 function pe(e, n) {
     le(), de(), window.reloader = n;
     for (var a = document.getElementsByTagName("dialog"), r = 0; r < a.length; r++) a[r].style.display = "none";
-    z.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(_e, {
+    W.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(_e, {
         url: A(e)
     }))
 }
 
 function Ae(e) {
-    le(), de(), z.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Fe, {
+    le(), de(), W.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Fe, {
         url: A(e)
     }))
 }
 
-function G(e) {
+function V(e) {
     e != null && showMessage(e);
     for (var n = document.getElementsByTagName("dialog"), a = 0; a < n.length; a++)
         if (a == n.length - 1) {
             var r = n[a];
             r.close(), r.classList.remove("opened"), r.remove(), a == 0 ? (document.querySelector(".layer").style.display = "none", window.reloader && window.reloader()) : n[a - 1].style.display = "block"
         }
 }
 
 function Re(e) {
-    le(), de(), z.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(ze, {
+    le(), de(), W.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(ze, {
         actions: e
     }))
 }
 
 function Oe(e) {
     const n = {
         backgroundColor: "black",
@@ -318,28 +315,28 @@
         top: 0,
         opacity: .7,
         display: "none"
     };
     return t.jsx("div", {
         className: "layer",
         onClick: function() {
-            G()
+            V()
         },
         style: n
     })
 }
 
 function _e(e) {
-    const [n, a] = I.useState(null), [r, i] = I.useState(0);
-    I.useEffect(() => {
+    const [n, a] = B.useState(null), [r, i] = B.useState(0);
+    B.useEffect(() => {
         l(A(e.url)), document.querySelector(".layer").style.display = "block"
     }, []);
 
     function l(s) {
-        L("GET", A(s), function(u) {
+        q("GET", A(s), function(u) {
             a(u), i(r + 1)
         })
     }
 
     function d() {
         const s = {
                 maxWidth: 800
@@ -351,17 +348,17 @@
             };
         if (n) return t.jsxs("div", {
             style: s,
             children: [t.jsx("div", {
                 style: u,
                 children: t.jsx(S, {
                     icon: "x",
-                    onClick: () => G()
+                    onClick: () => V()
                 })
-            }), t.jsx(x, {
+            }), t.jsx(y, {
                 data: n
             })]
         })
     }
     const c = {
         minWidth: window.innerWidth < 800 ? "calc(100% - 60px)" : 800,
         display: n ? "block" : "none",
@@ -373,15 +370,15 @@
         style: c,
         children: d()
     }, r)
 }
 
 function Fe(e) {
     var n = Math.random();
-    I.useEffect(() => {
+    B.useEffect(() => {
         document.querySelector(".layer").style.display = "block";
         var r = document.getElementById(n);
         r.style.top = document.documentElement.scrollTop + 100
     }, []);
 
     function a() {
         const r = {
@@ -399,15 +396,15 @@
         return t.jsxs("dialog", {
             style: r,
             id: n,
             children: [t.jsx("div", {
                 style: i,
                 children: t.jsx(S, {
                     icon: "x",
-                    onClick: () => G()
+                    onClick: () => V()
                 })
             }), t.jsx("iframe", {
                 src: A(e.url),
                 width: "100%",
                 height: 500,
                 style: {
                     border: 0
@@ -416,15 +413,15 @@
         })
     }
     return a()
 }
 
 function ze(e) {
     const n = Math.random();
-    I.useEffect(() => {
+    B.useEffect(() => {
         document.querySelector(".layer").style.display = "block"
     }, []);
 
     function a() {
         const l = {
             width: "100%",
             borderBottom: "solid 1px #DDDD",
@@ -461,26 +458,26 @@
     return t.jsx("dialog", {
         id: n,
         style: i,
         children: a()
     })
 }
 
-function M(e) {
+function E(e) {
     return e != null && (e = e.toString().replace("-", "").normalize("NFD").replace("_", "").toLowerCase()), e
 }
 
 function _(e) {
     const n = e.id || Math.random(),
-        [a, r] = I.useState(e.data.name);
+        [a, r] = B.useState(e.data.name);
 
     function i(c) {
         c.preventDefault();
         var s = e.data.url;
-        e.data.urlfunc && (s = e.data.urlfunc()), e.onClick ? (a && r("Aguarde...."), e.onClick(c)) : e.data.modal == !1 ? window.load(U(s)) : pe(s)
+        e.data.urlfunc && (s = e.data.urlfunc()), e.onClick ? (a && r("Aguarde...."), e.onClick(c)) : e.data.modal == !1 ? window.load(H(s)) : pe(s)
     }
 
     function l() {
         return e.strech ? e.data.name : e.data.icon ? e.compact || !e.data.name || window.innerWidth < 800 ? t.jsx(S, {
             icon: e.data.icon
         }) : t.jsxs(t.Fragment, {
             children: [t.jsx(S, {
@@ -500,25 +497,25 @@
             margin: 5,
             minWidth: 50
         };
         return e.primary && (c.backgroundColor = k.colors.primary, c.color = "white"), e.default && (c.border = "solid 1px " + k.colors.primary, c.color = k.colors.primary), e.style && Object.keys(e.style).map(function(s) {
             c[s] = e.style[s]
         }), t.jsx("a", {
             id: n,
-            href: U(e.data.url) || "#",
+            href: H(e.data.url) || "#",
             onClick: i,
             style: c,
-            "data-label": M(e.data.name),
+            "data-label": E(e.data.name),
             children: l()
         })
     }
     return d()
 }
 
-function K(e) {
+function Z(e) {
     function n(l) {
         var d = l.target.parentNode.querySelector(".dropdown");
         return d == null && (d = l.target.parentNode.parentNode.querySelector(".dropdown")), d == null && (d = l.target.parentNode.parentNode.parentNode.querySelector(".dropdown")), d
     }
 
     function a(l) {
         const d = n(l);
@@ -551,15 +548,15 @@
             };
         return t.jsxs(t.Fragment, {
             children: [t.jsx("div", {
                 onClick: a,
                 style: {
                     cursor: "pointer"
                 },
-                "data-label": M(e.dataLabel),
+                "data-label": E(e.dataLabel),
                 children: e.children
             }), e.actions && e.actions.length > 0 && t.jsx("ul", {
                 style: l,
                 onMouseLeave: r,
                 className: "dropdown",
                 children: e.actions.map(c => t.jsx("li", {
                     style: d,
@@ -582,26 +579,26 @@
     modal: a,
     imodal: r,
     children: i,
     onClick: l,
     dataLabel: d,
     style: c
 }) {
-    const s = n && n.indexOf("/media/") < 0 ? U(n) : n;
+    const s = n && n.indexOf("/media/") < 0 ? H(n) : n;
 
     function u(h) {
         s.indexOf("http") == 0 ? document.location.href = s : (h.preventDefault(), a ? pe(s) : r ? Ae(s) : window.load(s))
     }
 
     function o() {
         return t.jsx("a", {
             id: e,
             onClick: l || u,
             href: s || "#",
-            "data-label": M(d),
+            "data-label": E(d),
             style: c,
             children: i
         })
     }
     return o()
 }
 
@@ -616,25 +613,26 @@
         return t.jsx("div", {
             style: r,
             children: e.children
         }, Math.random())
     }
     return n()
 }
+const xe = {};
 
-function W(e) {
+function F(e) {
     let n = "",
         a = window.document.styleSheets[0];
     e.split("}").forEach(r => {
         let i = (r + "}").replace(/\r?\n|\r/g, "");
-        n = n === "" ? i : n + i, n.split("{").length === n.split("}").length && (a.insertRule(n, a.cssRules.length), n = "")
+        n = n === "" ? i : n + i, n.split("{").length === n.split("}").length && xe[n] == null && (a.insertRule(n, a.cssRules.length), n = "", xe[n] = !0)
     })
 }
 
-function V(e) {
+function $(e) {
     function n() {
         return e.data.url ? t.jsx(We, {
             data: e.data
         }) : t.jsx(je, {
             data: e.data
         })
     }
@@ -650,22 +648,22 @@
         })
     }
 
     function a() {
         return e.data.url && e.data.url.indexOf("only=") < 0 ? t.jsx(O, {
             href: e.data.url,
             children: t.jsxs(t.Fragment, {
-                children: [F(e.data.value), t.jsx(S, {
+                children: [z(e.data.value), t.jsx(S, {
                     icon: "external-link",
                     style: {
                         marginLeft: 10
                     }
                 })]
             })
-        }) : F(e.data.value)
+        }) : z(e.data.value)
     }
 
     function r() {
         const i = {
             minWidth: e.width + "%",
             marginTop: 5,
             marginBottom: 5
@@ -676,18 +674,18 @@
         })
     }
     return r()
 }
 
 function We(e) {
     const n = Math.random(),
-        [a, r] = I.useState(e.data);
+        [a, r] = B.useState(e.data);
 
     function i(d) {
-        L("GET", d, function(c) {
+        q("GET", d, function(c) {
             r(c)
         })
     }
 
     function l() {
         return window[n] = () => i(e.data.url), t.jsx("div", {
             className: e.data.url && "reloadable",
@@ -723,21 +721,21 @@
 
 function ce(e) {
     function n() {
         return e.data.map(function(a) {
             if (Array.isArray(a)) return t.jsx(P, {
                 width: 300,
                 alignItems: "start",
-                children: a.map(r => t.jsx(V, {
+                children: a.map(r => t.jsx($, {
                     data: r,
                     width: 100 / a.length
                 }, Math.random()))
             }, Math.random());
             if (a.label != "ID" && (e.exclude == null || a.label != e.exclude)) return t.jsx("div", {
-                children: t.jsx(V, {
+                children: t.jsx($, {
                     data: a,
                     width: 100
                 })
             }, Math.random())
         })
     }
     return n()
@@ -778,15 +776,15 @@
             children: [n(), a(), r()]
         })
     }
     return i()
 }
 
 function He(e) {
-    W(`
+    F(`
     .cards{
       padding: 10px;
       box-shadow: 0 1px 6px rgba( 0, 0, 0 , 0.16 );
       margin: 10px;
     }
     .cards h3{
       margin-top: 5px;
@@ -908,16 +906,16 @@
         })
     }
     return l()
 }
 
 function Ge(e) {
     const n = Math.random(),
-        [a, r] = I.useState(e.data);
-    W(`
+        [a, r] = B.useState(e.data);
+    F(`
     .object-fieldset{
       margin-top: 10px;
     }
   `);
 
     function i() {
         return t.jsx(ke, {
@@ -939,31 +937,31 @@
 
     function d() {
         return Array.isArray(a.data) ? a.data.length == 0 ? t.jsx("div", {
             children: "Nenhum registro encontrado."
         }) : a.data.map(function(u) {
             return Array.isArray(u) ? t.jsx(P, {
                 width: 300,
-                children: u.map(o => t.jsx(V, {
+                children: u.map(o => t.jsx($, {
                     data: o,
                     width: 100 / u.length
                 }, Math.random()))
             }, Math.random()) : t.jsx("div", {
-                children: t.jsx(V, {
+                children: t.jsx($, {
                     data: u,
                     width: 100
                 })
             }, Math.random())
-        }) : t.jsx(x, {
+        }) : t.jsx(y, {
             data: a.data
         })
     }
 
     function c(u) {
-        L("GET", u, function(o) {
+        q("GET", u, function(o) {
             r(o)
         })
     }
 
     function s() {
         return e.data.url ? (window[n] = () => c(e.data.url), t.jsxs("div", {
             className: e.data.url ? "reloadable object-fieldset" : "object-fieldset",
@@ -975,23 +973,23 @@
         })
     }
     return s()
 }
 
 function Ve(e) {
     const n = Math.random(),
-        [a, r] = I.useState(e.data.actions);
+        [a, r] = B.useState(e.data.actions);
 
     function i() {
         const c = e.data.url.indexOf("?") < 0 ? "?" : "&";
         return e.data.url + c + "only=actions"
     }
 
     function l() {
-        L("GET", i(), function(c) {
+        q("GET", i(), function(c) {
             r(c)
         })
     }
 
     function d() {
         return window[n] = () => l(), t.jsx("div", {
             className: "reloadable",
@@ -1005,54 +1003,54 @@
         })
     }
     return d()
 }
 
 function $e(e) {
     function n() {
-        return W(`
+        return F(`
       .object-title {
         display: flex;
         justify-content: space-between;
         align-items: baseline;
       }
       .object-title h1 {
           margin: 0;
           color: ${k.colors.primary};
       }
     `), t.jsxs("div", {
             className: "object-title",
             children: [e.data.title && t.jsx("h1", {
-                "data-label": M(e.data.title),
+                "data-label": E(e.data.title),
                 children: e.data.title
             }), t.jsx(Ve, {
                 data: e.data
             })]
         })
     }
     return n()
 }
 
 function ke(e) {
-    W(`
+    F(`
       .fieldset-title {
         display: flex;
         justify-content: space-between;
         align-items: baseline;
       }
       .fieldset-title h2 {
           margin: 0
       }
     `);
 
     function n() {
         return t.jsxs("div", {
             className: "fieldset-title",
             children: [e.data.title && t.jsx("h2", {
-                "data-label": M(e.data.title),
+                "data-label": E(e.data.title),
                 children: e.data.title
             }), e.data.actions && e.data.actions.length > 0 && t.jsx("div", {
                 children: e.data.actions.map(function(a) {
                     return t.jsx(_, {
                         data: a,
                         default: !0
                     }, Math.random())
@@ -1068,15 +1066,15 @@
         return t.jsx($e, {
             data: e.data
         })
     }
 
     function a() {
         return e.data.data.map(function(i, l) {
-            return t.jsx(x, {
+            return t.jsx(y, {
                 data: i
             }, Math.random())
         })
     }
 
     function r() {
         return t.jsxs("div", {
@@ -1097,15 +1095,15 @@
     function a() {
         const i = {
             backgroundColor: "white"
         };
         return e.data.data.map(function(l, d) {
             return t.jsx("div", {
                 style: i,
-                children: t.jsx(x, {
+                children: t.jsx(y, {
                     data: l
                 }, Math.random())
             })
         })
     }
 
     function r() {
@@ -1113,15 +1111,15 @@
             children: [n(), a()]
         })
     }
     return r()
 }
 
 function Qe(e) {
-    const [n, a] = I.useState(0);
+    const [n, a] = B.useState(0);
 
     function r() {
         return t.jsx("div", {
             style: {
                 display: "inline-block",
                 textAlign: "center",
                 width: "100%",
@@ -1138,30 +1136,30 @@
                         textDecoration: "none",
                         color: "#0c326f",
                         margin: 15
                     },
                     onClick: function(d) {
                         d.preventDefault(), a(l), e.loadContent(i.url)
                     },
-                    dataLabel: M(i.title),
+                    dataLabel: E(i.title),
                     children: i.title
                 }, Math.random())
             })
         })
     }
     return r()
 }
 
 function Xe(e) {
     var n = Math.random();
-    const [a, r] = I.useState(e.data.data[0]);
+    const [a, r] = B.useState(e.data.data[0]);
 
     function i() {
         return e.data.title != "Top" && t.jsx("h2", {
-            "data-label": M(e.data.title),
+            "data-label": E(e.data.title),
             children: e.data.title
         })
     }
 
     function l() {
         return t.jsx(Qe, {
             data: e.data.data,
@@ -1175,15 +1173,15 @@
         };
         o.title = null;
         const h = {
             padding: 0
         };
         return t.jsx("div", {
             style: h,
-            children: t.jsx(x, {
+            children: t.jsx(y, {
                 data: o
             }, Math.random())
         })
     }
 
     function c() {
         const o = {
@@ -1195,15 +1193,15 @@
         };
         return t.jsx("div", {
             style: o
         })
     }
 
     function s(o) {
-        L("GET", o, function(h) {
+        q("GET", o, function(h) {
             r(h)
         })
     }
 
     function u() {
         return window[n] = () => s(a.url), e.data.data.length > 0 && t.jsxs("div", {
             className: "reloadable",
@@ -1259,15 +1257,15 @@
             display: i || "block",
             width: "fit-content",
             textWrap: "nowrap"
         };
         return l ? (o.backgroundColor = k.colors.primary, o.color = "white") : (o.border = "solid 1px " + k.colors.primary, o.color = k.colors.primary), t.jsx("a", {
             id: e,
             style: o,
-            "data-label": M(r || a),
+            "data-label": E(r || a),
             onClick: h => {
                 h.preventDefault(), a && c && (h.target.dataset.spinning = a, h.target.querySelector("i.fa-spin").style.display = "inline-block", h.target.querySelector("i.fa-" + a).style.display = "none"), n(h)
             },
             children: s()
         })
     }
     return u()
@@ -1499,15 +1497,15 @@
                 textTransform: "uppercase",
                 height: 70,
                 color: k.colors.primary
             };
         return e.data.items.length ? t.jsxs("div", {
             style: a,
             children: [t.jsx("h2", {
-                "data-label": M(e.data.title),
+                "data-label": E(e.data.title),
                 style: {
                     color: k.colors.primary
                 },
                 children: e.data.title
             }), t.jsx("div", {
                 children: e.data.items.map(d => t.jsxs(O, {
                     href: d.url,
@@ -1576,15 +1574,15 @@
         })
     }
     return n()
 }
 
 function st(e) {
     const n = Math.random();
-    I.useEffect(() => {
+    B.useEffect(() => {
         new QRCode(document.getElementById(n), {
             text: e.data.text,
             width: 128,
             height: 128,
             colorDark: "#333333",
             colorLight: "#ffffff",
             correctLevel: QRCode.CorrectLevel.H
@@ -1619,22 +1617,22 @@
                 maxWidth: 200,
                 margin: "auto"
             };
         if (e.data) return t.jsxs("div", {
             className: "indicators",
             style: a,
             children: [t.jsx("h1", {
-                "data-label": M(e.data.title),
+                "data-label": E(e.data.title),
                 children: e.data.title
             }), t.jsx(P, {
                 width: 300,
                 children: e.data.items.map(l => t.jsxs("div", {
                     children: [t.jsx("div", {
                         style: r,
-                        children: F(l.value)
+                        children: z(l.value)
                     }), t.jsx("div", {
                         style: i,
                         children: l.name
                     })]
                 }, Math.random()))
             }, Math.random()), t.jsx("div", {
                 className: "actions",
@@ -1651,31 +1649,32 @@
 }
 
 function ut(e) {
     function n() {
         return t.jsx(P, {
             width: 400,
             children: e.data.items.map((a, r) => t.jsx("div", {
-                children: t.jsx(x, {
+                children: t.jsx(y, {
                     data: a
                 })
             }, Math.random()))
         })
     }
     return n()
 }
 
 function ht(e) {
     function n() {
         return t.jsxs("div", {
             children: [t.jsx("h2", {
+                align: "center",
                 children: e.data.title
             }), t.jsx("div", {
                 style: {
-                    fontSize: "12rem",
+                    fontSize: "8rem",
                     textAlign: "center",
                     color: "#5470c6"
                 },
                 children: e.data.value
             })]
         })
     }
@@ -1703,84 +1702,84 @@
         a = !1, document.getElementById("input" + n).value = JSON.stringify({
             select: d,
             deselect: c
         })
     }
 
     function h(v) {
-        e.data.readonly || e.data.single_selection && f().length > 0 && v.target.style.backgroundColor != i || a && v.target.style.backgroundColor != l && (v.target.style.backgroundColor == r ? (v.target.style.backgroundColor = i, console.log("MARCOU", v.target.dataset.day, v.target.dataset.time), d.push([v.target.dataset.day, v.target.dataset.time])) : (v.target.style.backgroundColor = r, console.log("DEMARCOU", v.target.dataset.day, v.target.dataset.time), c.push([v.target.dataset.day, v.target.dataset.time])))
+        e.data.readonly || e.data.single_selection && g().length > 0 && v.target.style.backgroundColor != i || a && v.target.style.backgroundColor != l && (v.target.style.backgroundColor == r ? (v.target.style.backgroundColor = i, console.log("MARCOU", v.target.dataset.day, v.target.dataset.time), d.push([v.target.dataset.day, v.target.dataset.time])) : (v.target.style.backgroundColor = r, console.log("DEMARCOU", v.target.dataset.day, v.target.dataset.time), c.push([v.target.dataset.day, v.target.dataset.time])))
     }
 
-    function f() {
+    function g() {
         const v = [];
-        return document.getElementById(n).querySelectorAll("td").forEach(function(B) {
-            B.style.backgroundColor == i && v.push(B.dataset.day, B.dataset.time)
+        return document.getElementById(n).querySelectorAll("td").forEach(function(D) {
+            D.style.backgroundColor == i && v.push(D.dataset.day, D.dataset.time)
         }), v
     }
 
     function w() {
         const v = {
                 overflowX: "auto"
             },
-            B = {
+            D = {
                 width: "100%",
                 borderSpacing: 0,
                 borderCollapse: "collapse",
                 marginTop: 15,
                 marginBottom: 15
             },
-            g = {
+            m = {
                 border: "solid 4px white"
             };
         return t.jsxs("div", {
             id: n,
             style: v,
             children: [t.jsx("input", {
                 id: "input" + n,
                 type: "hidden",
                 name: e.data.input_name
             }), t.jsxs("table", {
-                style: B,
+                style: D,
                 onMouseDown: u,
                 onMouseUp: o,
                 children: [t.jsx("thead", {
                     children: t.jsx("tr", {
                         children: e.data.matrix[0].map(function(j) {
                             return t.jsx("th", {
                                 className: "bold",
-                                style: g,
+                                style: m,
                                 children: j.text
                             }, Math.random())
                         })
                     })
                 }), t.jsx("tbody", {
-                    children: e.data.matrix.map(function(j, y) {
-                        if (y > 0) return t.jsx("tr", {
-                            children: j.map(function(D, b) {
+                    children: e.data.matrix.map(function(j, x) {
+                        if (x > 0) return t.jsx("tr", {
+                            children: j.map(function(I, b) {
                                 if (b == 0) return t.jsx("th", {
                                     className: "bold",
                                     align: "center",
-                                    style: g,
-                                    children: D.text
+                                    style: m,
+                                    children: I.text
                                 }, Math.random());
                                 {
                                     const C = {
-                                        backgroundColor: s(D),
+                                        backgroundColor: s(I),
                                         border: "solid 4px white"
                                     };
                                     return t.jsx("td", {
                                         align: "center",
                                         style: C,
                                         onMouseDown: h,
                                         onMouseLeave: h,
                                         onMouseUp: h,
                                         "data-day": e.data.matrix[0][b].text,
                                         "data-time": j[0].text,
-                                        children: D && D.text && t.jsx(mt, {
-                                            text: D.text,
+                                        children: I && I.text && t.jsx(mt, {
+                                            text: I.text,
                                             children: t.jsx(S, {
                                                 icon: "stethoscope",
                                                 style: {
                                                     color: "white",
                                                     cursor: "help"
                                                 }
                                             })
@@ -1795,15 +1794,15 @@
         })
     }
     return w()
 }
 
 function mt(e) {
     function n() {
-        return W(`
+        return F(`
       .tooltip {
         position: relative;
         display: inline-block;
       }
       .tooltip .tooltiptext {
         visibility: hidden;
         width: 220px;
@@ -1822,22 +1821,22 @@
       .tooltip:hover .tooltiptext {
         visibility: visible;
       }
     `), t.jsxs("div", {
             className: "tooltip",
             children: [e.children, t.jsx("div", {
                 className: "tooltiptext",
-                children: F(e.text)
+                children: z(e.text)
             })]
         })
     }
     return n()
 }
 const ft = ["text", "password", "email", "number", "date", "datetime-local", "file", "image", "range", "search", "tel", "time", "url", "week", "hidden", "color"],
-    $ = {
+    J = {
         padding: 15,
         border: "solid 1px #d9d9d9",
         borderRadius: 5,
         backgroundColor: "white"
     };
 
 function gt(e) {
@@ -1845,30 +1844,30 @@
     for (let [a, r] of Array.from(n.entries())) {
         const i = e[a];
         (r === "" || !(i.tagName == "SELECT" || i.tagName == null)) && n.delete(a)
     }
     return new URLSearchParams(n).toString()
 }
 
-function Y(e, n) {
+function Q(e, n) {
     const a = e.indexOf("?") < 0 ? "?" : "&",
         r = gt(n);
     return e = e + (r ? a + r : ""), e
 }
 
 function re(e) {
     if (e) {
         const a = [".png", ".jpeg", ".jpeg", ".gif"];
         for (var n = 0; n < a.length; n++)
             if (e.toLowerCase().indexOf(a[n]) > 0) return !0
     }
 }
 
-function J(e, n) {
-    L("GET", Y(n, e.closest("form")), Me)
+function Y(e, n) {
+    q("GET", Q(n, e.closest("form")), Ee)
 }
 
 function xt(e) {
     if (e) {
         var n = document.querySelector(".form-fieldset." + e);
         n && (n.style.display = "none");
         var a = document.querySelector(".form-group." + e);
@@ -1904,15 +1903,15 @@
                 if (r.options[i].value == n) {
                     r.selectedIndex = i;
                     break
                 }
     }
 }
 
-function Me(e) {
+function Ee(e) {
     if (e) {
         for (var n = 0; n < e.hide.length; n++) xt(e.hide[n]);
         for (var n = 0; n < e.show.length; n++) yt(e.show[n]);
         for (var n = 0; n < e.reload.length; n++) vt(e.reload[n]);
         for (var a in e.set) bt(a, e.set[a])
     }
 }
@@ -1984,25 +1983,25 @@
                 children: e.text
             })
         })
     }
     return n()
 }
 
-function Z(e) {
+function ee(e) {
     const n = e.data.name + Math.random();
 
     function a() {
         const c = {
             display: "flex",
             justifyContent: "space-between",
             alignItems: "baseline"
         };
         return e.data.action && (e.data.action.icon = null, e.data.action.modal = !0, e.data.action.urlfunc = function() {
-            return Y(e.data.action.url, document.getElementById(n).closest("form"))
+            return Q(e.data.action.url, document.getElementById(n).closest("form"))
         }), t.jsxs("div", {
             style: c,
             children: [t.jsxs("label", {
                 className: "bold",
                 children: [e.data.label, " ", e.data.required ? "*" : ""]
             }), e.data.action && t.jsx(_, {
                 data: e.data.action,
@@ -2010,29 +2009,29 @@
                     padding: 0
                 }
             })]
         })
     }
 
     function r() {
-        return e.data.type == "datetime" && (e.data.type = "datetime-local"), ft.indexOf(e.data.type) >= 0 ? t.jsx(xe, {
+        return e.data.type == "datetime" && (e.data.type = "datetime-local"), ft.indexOf(e.data.type) >= 0 ? t.jsx(ye, {
             data: e.data
-        }) : e.data.type == "choice" && Array.isArray(e.data.choices) ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(ye, {
+        }) : e.data.type == "choice" && Array.isArray(e.data.choices) ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(ve, {
             data: e.data
         }) : t.jsx(ie, {
             data: e.data
         }) : t.jsx(Ct, {
             data: e.data
-        }) : e.data.type == "choice" ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(ye, {
+        }) : e.data.type == "choice" ? e.data.pick ? Array.isArray(e.data.value) ? t.jsx(ve, {
             data: e.data
         }) : t.jsx(ie, {
             data: e.data
-        }) : t.jsx(Ee, {
+        }) : t.jsx(Me, {
             data: e.data
-        }) : e.data.type == "decimal" ? t.jsx(xe, {
+        }) : e.data.type == "decimal" ? t.jsx(ye, {
             data: e.data
         }) : e.data.type == "boolean" ? t.jsx(St, {
             data: e.data
         }) : e.data.type == "textarea" ? t.jsx(kt, {
             data: e.data
         }) : e.data.type == "scheduler" ? (e.data.scheduler.input_name = e.data.name, t.jsx(Ce, {
             data: e.data.scheduler
@@ -2067,23 +2066,23 @@
             style: c,
             children: [a(), r(), l(), i()]
         })
     }
     return d()
 }
 
-function xe(e) {
+function ye(e) {
     var n = "";
     const a = e.data.name + Math.random();
-    e.data.mask == "decimal" && (n = "decimal", e.data.value && (e.data.value = Math.round(parseFloat(e.data.value)).toFixed(2).replace(".", ","))), I.useEffect(() => {
+    e.data.mask == "decimal" && (n = "decimal", e.data.value && (e.data.value = Math.round(parseFloat(e.data.value)).toFixed(2).replace(".", ","))), B.useEffect(() => {
         function d(u, o, h) {
-            var f = h.target,
-                w = f.value.replace(/\D/g, ""),
-                v = f.value.length > o ? 1 : 0;
-            VMasker(f).unMask(), VMasker(f).maskPattern(u[v]), f.value = VMasker.toPattern(w, u[v])
+            var g = h.target,
+                w = g.value.replace(/\D/g, ""),
+                v = g.value.length > o ? 1 : 0;
+            VMasker(g).unMask(), VMasker(g).maskPattern(u[v]), g.value = VMasker.toPattern(w, u[v])
         }
         if (e.data.mask) {
             var c = document.getElementById(a);
             if (e.data.mask == "decimal") VMasker(c).maskMoney({
                 precision: 2,
                 separator: ",",
                 delimiter: "."
@@ -2092,43 +2091,43 @@
                 var s = e.data.mask.split("|");
                 VMasker(c).maskPattern(s[0]), c.addEventListener("input", d.bind(void 0, s, 14), !1)
             } else VMasker(c).maskPattern(e.data.mask)
         }
     }, []);
 
     function r(d) {
-        J(d.target, e.data.onchange)
+        Y(d.target, e.data.onchange)
     }
 
     function i(d) {
         if (e.data.type == "file" && d.target.files) {
             let s = d.target.files[0];
             var c = new FileReader;
             c.onload = function(u) {
                 if (re(s.name)) {
                     const w = "display" + a;
                     var o = document.createElement("img");
                     o.id = d.target.id + "img", o.style.width = "200px", o.style.display = "block", o.style.margin = "auto", o.style.marginTop = "20px", o.onload = function(v) {
-                        const B = e.data.width > e.data.height ? e.data.width / o.width : e.data.height / o.height;
-                        var g = document.createElement("canvas");
-                        const j = g.getContext("2d");
-                        g.height = g.width * (o.height / o.width);
-                        const y = document.createElement("canvas"),
-                            D = y.getContext("2d");
-                        y.width = o.width * B, y.height = o.height * B, D.drawImage(o, 0, 0, y.width, y.height), j.drawImage(y, 0, 0, y.width * B, y.height * B, 0, 0, g.width, g.height), y.toBlob(function(C) {
+                        const D = e.data.width > e.data.height ? e.data.width / o.width : e.data.height / o.height;
+                        var m = document.createElement("canvas");
+                        const j = m.getContext("2d");
+                        m.height = m.width * (o.height / o.width);
+                        const x = document.createElement("canvas"),
+                            I = x.getContext("2d");
+                        x.width = o.width * D, x.height = o.height * D, I.drawImage(o, 0, 0, x.width, x.height), j.drawImage(x, 0, 0, x.width * D, x.height * D, 0, 0, m.width, m.height), x.toBlob(function(C) {
                             const T = new DataTransfer;
                             T.items.add(new File([C], s.name)), d.target.files = T.files
                         });
                         var b = document.getElementById(w);
                         b == null ? (b = document.createElement("div"), b.id = w) : b.removeChild(b.childNodes[0]), b.appendChild(o), d.target.parentNode.appendChild(b)
                     }, o.src = u.target.result
                 }
                 const h = document.getElementById("fileinfo" + a);
-                var f = s.size / 1024;
-                f < 1024 ? f = parseInt(f) + " Kb" : f = (f / 1024).toFixed(2) + " Mb", h.innerHTML = s.name + " / " + f, e.data.max_size && s.size / 1024 / 1024 > e.data.max_size && alert("O limite de tamanho é " + e.data.max_size + "Mb. O arquivo informado possui " + f + ". Por favor, adicione um arquivo menor.")
+                var g = s.size / 1024;
+                g < 1024 ? g = parseInt(g) + " Kb" : g = (g / 1024).toFixed(2) + " Mb", h.innerHTML = s.name + " / " + g, e.data.max_size && s.size / 1024 / 1024 > e.data.max_size && alert("O limite de tamanho é " + e.data.max_size + "Mb. O arquivo informado possui " + g + ". Por favor, adicione um arquivo menor.")
             }, c.readAsDataURL(s)
         }
     }
 
     function l() {
         var d = e.data.type;
         if (d == "datetime" && (d = "datetime-regional"), d == "decimal" && (d = "text"), d == "file") {
@@ -2188,65 +2187,65 @@
                         })
                     })]
                 }), t.jsx("input", {
                     className: "form-control " + n,
                     type: d,
                     name: e.data.name,
                     id: a,
-                    "data-label": M(e.data.label),
+                    "data-label": E(e.data.label),
                     readOnly: e.data.read_only,
                     onBlur: e.data.onchange ? r : null,
                     onChange: i,
                     style: {
                         zIndex: "-1",
                         marginTop: -20
                     },
                     accept: c
                 })]
             })
         } else {
-            var s = $;
+            var s = J;
             return d == "color" && (s = {
-                ...$
+                ...J
             }, s.width = "100%", s.backgroundColor = "white", s.height = 47.5), t.jsx("input", {
                 className: "form-control " + n,
                 type: d,
                 name: e.data.name,
                 id: a,
                 defaultValue: e.data.value,
-                "data-label": M(e.data.label),
+                "data-label": E(e.data.label),
                 readOnly: e.data.read_only,
                 onBlur: e.data.onchange ? r : null,
                 onChange: i,
                 style: s
             })
         }
     }
     return l()
 }
 
-function Ee(e) {
+function Me(e) {
     var n = [];
     Array.isArray(e.data.value) ? e.data.value.forEach(function(b, C) {
         n.push({
             id: b.id,
             value: b.label
         })
     }) : e.data.value != null && n.push({
         id: e.data.value.id,
         value: e.data.value.label
     }), e.data.id == null && (e.data.id = Math.random()), e.data.id2 == null && (e.data.id2 = e.data.id + "__autocomplete");
     const a = e.data.id,
         r = e.data.id2,
         i = Array.isArray(e.data.value),
-        [l, d] = I.useState(!1),
-        [c, s] = I.useState(null);
+        [l, d] = B.useState(!1),
+        [c, s] = B.useState(null);
     var u = !1;
     let o;
-    I.useEffect(() => {
+    B.useEffect(() => {
         j(n, !0), document.getElementById(a).addEventListener("customchange", function(b) {
             j(b.detail.value), reactTriggerChange(document.getElementById(e.data.name))
         })
     }, []);
 
     function h() {
         const b = document.getElementById(a);
@@ -2255,58 +2254,58 @@
                     padding: 5,
                     display: "inline"
                 },
                 T = {
                     cursor: "pointer",
                     marginRight: 5
                 },
-                m = {
+                f = {
                     fontSize: "0.8rem"
                 };
             return t.jsxs("div", {
-                children: [b == null && n.map((p, E) => t.jsxs("div", {
+                children: [b == null && n.map((p, M) => t.jsxs("div", {
                     style: C,
                     children: [t.jsx("span", {
-                        onClick: () => y(E),
+                        onClick: () => x(M),
                         style: T,
                         children: t.jsx(S, {
                             icon: "trash-can",
-                            style: m
+                            style: f
                         })
                     }), p.value]
-                }, Math.random())), b != null && Array.from(b.options).map((p, E) => t.jsxs("div", {
+                }, Math.random())), b != null && Array.from(b.options).map((p, M) => t.jsxs("div", {
                     style: C,
                     children: [t.jsx("span", {
-                        onClick: () => y(E),
+                        onClick: () => x(M),
                         style: T,
                         children: t.jsx(S, {
                             icon: "trash-can",
-                            style: m
+                            style: f
                         })
                     }), p.innerHTML]
                 }, Math.random()))]
             })
         }
     }
 
-    function f() {
+    function g() {
         return t.jsx("select", {
             id: a,
             name: e.data.name,
             multiple: i,
             readOnly: !0,
             style: {
                 display: "contents"
             }
         })
     }
 
     function w() {
         const b = {
-                ...$,
+                ...J,
                 ...e.style || {}
             },
             C = {
                 padding: 0,
                 margin: 0,
                 border: "solid 1px #d9d9d9",
                 marginTop: -1,
@@ -2314,130 +2313,130 @@
                 maxHeight: 150,
                 overflowY: "auto",
                 zIndex: 99999
             };
         C.position = "absolute", C.backgroundColor = "white";
         const T = document.getElementById(r);
         if (e.data.icon && (b.paddingLeft = 30), T) {
-            let q = null,
-                Q = T,
+            let N = null,
+                X = T,
                 ae = null;
-            for (; !ae && (Q = Q.parentElement) instanceof HTMLElement;) Q.matches("dialog") && (ae = Q);
-            q = ae;
-            const X = T.getBoundingClientRect();
-            var m = X.top + X.height,
-                p = X.left;
-            if (q) {
-                const fe = q.getBoundingClientRect();
-                m = m - fe.top, p = p - fe.left
-            } else m += window.scrollY, p += window.scrollX;
-            C.width = X.width, C.top = m, C.left = p
+            for (; !ae && (X = X.parentElement) instanceof HTMLElement;) X.matches("dialog") && (ae = X);
+            N = ae;
+            const K = T.getBoundingClientRect();
+            var f = K.top + K.height,
+                p = K.left;
+            if (N) {
+                const fe = N.getBoundingClientRect();
+                f = f - fe.top, p = p - fe.left
+            } else f += window.scrollY, p += window.scrollX;
+            C.width = K.width, C.top = f, C.left = p
         }
-        const E = {
+        const M = {
                 cursor: "pointer",
                 padding: 10
             },
-            N = !i && n.length > 0 && n[0].value || "";
+            L = !i && n.length > 0 && n[0].value || "";
         return t.jsxs(t.Fragment, {
             children: [e.data.icon && t.jsx(S, {
                 icon: e.data.icon,
                 style: {
                     position: "absolute",
                     margin: 13,
                     color: "#d9d9d9"
                 }
             }), t.jsx("input", {
                 id: r,
                 name: e.data.name + "__autocomplete",
                 type: "text",
                 className: "form-control",
-                onFocus: q => {
-                    q.target.select(), g(q)
+                onFocus: N => {
+                    N.target.select(), m(N)
                 },
-                onChange: g,
+                onChange: m,
                 onMouseLeave: v,
                 onBlur: v,
-                defaultValue: N,
+                defaultValue: L,
                 style: b,
-                "data-label": M(e.data.label)
+                "data-label": E(e.data.label)
             }), c && l && t.jsxs("ul", {
                 style: C,
-                onMouseLeave: B,
-                onMouseEnter: function(q) {
+                onMouseLeave: D,
+                onMouseEnter: function(N) {
                     u = !0
                 },
                 children: [c.length == 0 && t.jsx("li", {
-                    style: E,
+                    style: M,
                     children: "Nenhuma opção encontrada."
-                }), c.map(q => t.jsx("li", {
+                }), c.map(N => t.jsx("li", {
                     onClick: () => {
-                        d(!1), e.onSelect ? e.onSelect(q) : j(q)
+                        d(!1), e.onSelect ? e.onSelect(N) : j(N)
                     },
-                    style: E,
+                    style: M,
                     className: "autocomplete-item",
-                    "data-label": M(q.value),
-                    children: q.value
+                    "data-label": E(N.value),
+                    children: N.value
                 }, Math.random()))]
             })]
         })
     }
 
     function v(b) {
         u = !1, setTimeout(function() {
-            u || B(b)
+            u || D(b)
         }, 250)
     }
 
-    function B(b) {
+    function D(b) {
         const C = document.getElementById(a);
         if (C) {
             const T = document.getElementById(r);
-            i || C.options.length > 0 && T.value != C.options[0].innerHTML && (C.innerHTML = "", T.value = "", d(!1), e.data.onchange && J(T, e.data.onchange)), b.target.tagName == "UL" ? d(!1) : u || d(!1)
+            i || C.options.length > 0 && T.value != C.options[0].innerHTML && (C.innerHTML = "", T.value = "", d(!1), e.data.onchange && Y(T, e.data.onchange)), b.target.tagName == "UL" ? d(!1) : u || d(!1)
         }
     }
 
-    function g(b) {
+    function m(b) {
         clearTimeout(o), o = setTimeout(function() {
             const C = b.target.closest("form"),
                 T = e.data.choices.indexOf("?") < 0 ? "?" : "&";
-            d(!0), L("GET", Y(e.data.choices + T + "term=" + b.target.value, C), function(p) {
+            d(!0), q("GET", Q(e.data.choices + T + "term=" + b.target.value, C), function(p) {
                 s(p)
             })
         }, 1e3)
     }
 
     function j(b, C = !1) {
         const T = document.getElementById(a),
-            m = document.getElementById(r);
-        T.innerHTML == null && (T.innerHTML = ""), Array.isArray(b) ? T.innerHTML = b.map(p => `<option selected value="${p.id}">${p.value}</option>`).join("") : i ? (T.innerHTML += `<option selected value="${b.id}">${b.value}</option>`, m.value = "") : (T.innerHTML = `<option selected value="${b.id}">${b.value}</option>`, m.value = b.value), e.data.onchange && !C && J(m, e.data.onchange)
+            f = document.getElementById(r);
+        T.innerHTML == null && (T.innerHTML = ""), Array.isArray(b) ? T.innerHTML = b.map(p => `<option selected value="${p.id}">${p.value}</option>`).join("") : i ? (T.innerHTML += `<option selected value="${b.id}">${b.value}</option>`, f.value = "") : (T.innerHTML = `<option selected value="${b.id}">${b.value}</option>`, f.value = b.value), e.data.onchange && !C && Y(f, e.data.onchange)
     }
 
-    function y(b) {
+    function x(b) {
         const C = document.getElementById(a);
         var T = Array.from(C.options);
-        C.innerHTML = T.slice(0, b).concat(T.slice(b + 1)).map(m => `<option selected value="${m.value}">${m.innerHTML}</option>`).join(""), s([])
+        C.innerHTML = T.slice(0, b).concat(T.slice(b + 1)).map(f => `<option selected value="${f.value}">${f.innerHTML}</option>`).join(""), s([])
     }
 
-    function D() {
+    function I() {
         return t.jsxs(t.Fragment, {
-            children: [h(), f(), w()]
+            children: [h(), g(), w()]
         })
     }
-    return D()
+    return I()
 }
 
 function kt(e) {
     function n() {
         var a = {
-            ...$
+            ...J
         };
         return a.height = 100, t.jsx("textarea", {
             id: e.data.name,
             name: e.data.name,
-            "data-label": M(e.data.label),
+            "data-label": E(e.data.label),
             style: a,
             defaultValue: e.data.value || "",
             className: "form-control"
         })
     }
     return n()
 }
@@ -2452,35 +2451,35 @@
         value: "Não"
     }], t.jsx(ie, {
         data: n
     })
 }
 
 function ie(e) {
-    const [n, a] = I.useState(e.data.choices);
+    const [n, a] = B.useState(e.data.choices);
     var r = Math.random(),
         i = e.data;
 
     function l(u) {
         return i.value != null ? i.value == u.id ? !0 : i.value.id == u.id : !1
     }
 
     function d(u) {
         var o = document.getElementById(u);
-        i.checked && (o.checked = !1), e.data.onchange && J(o, e.data.onchange)
+        i.checked && (o.checked = !1), e.data.onchange && Y(o, e.data.onchange)
     }
 
     function c(u) {
         var o = document.getElementById(u);
         i.checked = o.checked
     }
 
     function s() {
         return window["reload-" + i.name + "-field"] = function() {
-            L("GET", Y(e.data.pick, document.querySelector(".radio-group." + i.name).closest("form")), function(o) {
+            q("GET", Q(e.data.pick, document.querySelector(".radio-group." + i.name).closest("form")), function(o) {
                 a(o)
             })
         }, n.length > 0 ? t.jsx("div", {
             className: "radio-group " + i.name,
             children: n.map((u, o) => (u.id || u.id === !1) && t.jsxs("div", {
                 style: {
                     paddingTop: 10,
@@ -2490,15 +2489,15 @@
                 },
                 children: [t.jsx("input", {
                     id: i.name + r + o,
                     type: "radio",
                     name: i.name,
                     defaultValue: u.id,
                     defaultChecked: l(u),
-                    "data-label": M(u.value),
+                    "data-label": E(u.value),
                     onClick: function() {
                         d(i.name + r + o)
                     },
                     onMouseEnter: function() {
                         c(i.name + r + o)
                     }
                 }), t.jsx("label", {
@@ -2512,36 +2511,36 @@
                 children: "Nenhuma opção disponível para seleção."
             })
         })
     }
     return s()
 }
 
-function ye(e) {
-    const [n, a] = I.useState(e.data.choices);
+function ve(e) {
+    const [n, a] = B.useState(e.data.choices);
     var r = Math.random(),
         i = e.data;
 
     function l(s) {
         var u = !1;
         if (i.value)
             for (var o = 0; o < i.value.length; o++) {
                 var h = i.value[o];
                 (h == s.id || h.id == s.id) && (u = !0)
             }
         return u
     }
 
     function d(s) {
-        e.data.onchange && J(s.target, e.data.onchange)
+        e.data.onchange && Y(s.target, e.data.onchange)
     }
 
     function c() {
         return window["reload-" + i.name + "-field"] = function() {
-            L("GET", Y(e.data.pick, document.querySelector(".checkbox-group." + i.name).closest("form")), function(u) {
+            q("GET", Q(e.data.pick, document.querySelector(".checkbox-group." + i.name).closest("form")), function(u) {
                 a(u)
             })
         }, n.length > 0 ? t.jsx("div", {
             className: "checkbox-group " + i.name,
             children: n.map((s, u) => (s.id || s.id === !1) && t.jsxs("div", {
                 style: {
                     paddingTop: 10,
@@ -2552,15 +2551,15 @@
                 children: [t.jsx("input", {
                     id: i.name + r + u,
                     type: "checkbox",
                     name: i.name,
                     onClick: d,
                     defaultValue: s.id,
                     defaultChecked: l(s),
-                    "data-label": M(s.value)
+                    "data-label": E(s.value)
                 }), t.jsx("label", {
                     htmlFor: i.name + r + u,
                     children: s.value
                 })]
             }, r + u))
         }) : t.jsx("div", {
             className: "checkbox-group " + i.name,
@@ -2575,26 +2574,26 @@
 function Ct(e) {
     var n = e.data;
     return t.jsx(t.Fragment, {
         children: t.jsx("select", {
             className: "form-control",
             id: n.name,
             name: n.name,
-            "data-label": M(n.label),
+            "data-label": E(n.label),
             defaultValue: n.value,
-            style: $,
+            style: J,
             children: n.choices.map(a => t.jsx("option", {
                 value: a.id,
                 children: a.value
             }, Math.random()))
         })
     })
 }
 
-function Mt(e) {
+function Et(e) {
     const n = Math.random(),
         a = e.data.value[0],
         r = a.fields ? a.fields[0] : a.fieldsets[0].fields[0][0];
 
     function i() {
         return !e.data.required && t.jsx("div", {
             id: "info-" + n,
@@ -2619,16 +2618,16 @@
         })
     }
 
     function l(s) {
         const u = document.querySelector("input[name=" + r.name + "]"),
             o = document.getElementById("inline-form-" + n),
             h = document.getElementById("show-" + n),
-            f = document.getElementById("hide-" + n);
-        o.style.display = s ? "block" : "none", h.style.display = s ? "none" : "inline", f.style.display = s ? "inline" : "none", s ? u.value === "" ? u.value = 0 : u.value = -parseInt(u.value) : parseInt(u.value) == 0 ? u.value = "" : u.value = -parseInt(u.value)
+            g = document.getElementById("hide-" + n);
+        o.style.display = s ? "block" : "none", h.style.display = s ? "none" : "inline", g.style.display = s ? "inline" : "none", s ? u.value === "" ? u.value = 0 : u.value = -parseInt(u.value) : parseInt(u.value) == 0 ? u.value = "" : u.value = -parseInt(u.value)
     }
 
     function d() {
         const s = {
             display: r.value ? "block" : "none"
         };
         return e.data.required && (s.display = "block", r.value === "" && (r.value = 0)), t.jsx("div", {
@@ -2647,84 +2646,84 @@
         const s = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
                 style: s,
-                "data-label": M(e.data.label),
+                "data-label": E(e.data.label),
                 children: e.data.label
             }), i(), d()]
         })
     }
     return c()
 }
 
-function Et(e) {
+function Mt(e) {
     var n = 0;
     const a = Math.random();
     e.data.template == null && (e.data.template = e.data.value.pop());
 
     function r(o, h) {
-        const f = n;
+        const g = n;
         return n += 1, t.jsxs("div", {
             style: {
                 display: "block"
             },
-            id: "form-" + f + "-" + a,
+            id: "form-" + g + "-" + a,
             children: [t.jsx(ue, {
                 data: o
             }), t.jsxs("div", {
                 style: {
                     textAlign: "center",
                     marginTop: 10,
                     marginBottom: 10
                 },
                 children: [t.jsx(R, {
                     primary: !0,
                     icon: "plus",
                     onClick: () => l(),
-                    id: "extra-add-" + f + "-",
+                    id: "extra-add-" + g + "-",
                     display: h
                 }), t.jsx(R, {
                     primary: !0,
                     icon: "trash",
-                    onClick: () => d(f),
+                    onClick: () => d(g),
                     display: "inline"
                 })]
             })]
         }, Math.random())
     }
 
     function i() {
         const o = c(),
             h = o.length > 0 ? "none" : "inline";
         document.getElementById("add-" + a).style.display = h;
-        for (var f = 0; f < n; f++) {
-            var w = document.getElementById("extra-add-" + f + "-");
+        for (var g = 0; g < n; g++) {
+            var w = document.getElementById("extra-add-" + g + "-");
             w.style.display = "none"
         }
         if (o.length > 0) {
             var w = document.getElementById("extra-add-" + o[o.length - 1] + "-");
             w.style.display = "inline"
         }
     }
 
     function l() {
         i();
         var o = JSON.parse(JSON.stringify(e.data.template));
         o.fields ? (o.fields.map(function(h) {
             h.name = h.name.replace("__n__", "__" + n + "__")
         }), o.fields[0].value = 0) : o.fieldsets.map(function(h) {
-            h.fields.map(function(f) {
-                f.map(function(w) {
+            h.fields.map(function(g) {
+                g.map(function(w) {
                     w.name = w.name.replace("__n__", "__" + n + "__")
-                }), f[0].value = 0
+                }), g[0].value = 0
             })
-        }), z.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(o, "inline")), setTimeout(i, 100)
+        }), W.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(o, "inline")), setTimeout(i, 100)
     }
 
     function d(o) {
         const h = e.data.template,
             w = (h.fields ? h.fields[0] : h.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + o + "__"),
             v = document.querySelector("input[name=" + w + "]");
         parseInt(v.value) == 0 ? v.value = "" : v.value = -parseInt(v.value), document.getElementById("form-" + o + "-" + a).style.display = "none", i()
@@ -2757,54 +2756,54 @@
         const o = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
                 style: o,
-                "data-label": M(e.data.label),
+                "data-label": E(e.data.label),
                 children: e.data.label
             }), t.jsx("div", {
                 children: !1
             }), t.jsxs("div", {
                 id: a,
                 className: "fieldset-inline-forms",
-                children: [s(), e.data.value.map(function(h, f) {
-                    return r(h, f == e.data.value.length - 1 ? "inline" : "none")
+                children: [s(), e.data.value.map(function(h, g) {
+                    return r(h, g == e.data.value.length - 1 ? "inline" : "none")
                 })]
             })]
         })
     }
     return u()
 }
 
 function ue(e) {
-    I.useEffect(() => {
-        e.data.controls && Me(e.data.controls)
+    B.useEffect(() => {
+        e.data.controls && Ee(e.data.controls)
     }, []);
 
     function n(r) {
-        return r.type == "inline" ? r.max == r.min == 1 ? t.jsx(Mt, {
+        return r.type == "inline" ? r.max == r.min == 1 ? t.jsx(Et, {
             data: r
-        }, Math.random()) : t.jsx(Et, {
+        }, Math.random()) : t.jsx(Mt, {
             data: r
-        }, Math.random()) : t.jsx(Z, {
+        }, Math.random()) : t.jsx(ee, {
             data: r
         }, Math.random())
     }
 
     function a() {
         return e.data.fields ? t.jsx("div", {
             className: "form-fields",
             children: e.data.fields.map(r => n(r))
         }) : e.data.fieldsets.map(r => t.jsx("div", {
             className: "form-fieldset",
             children: r.type == "inline" ? n(r) : t.jsxs(t.Fragment, {
                 children: [t.jsx("h2", {
-                    "data-label": M(r.title),
+                    "data-label": E(r.title),
                     style: {
                         margin: 0
                     },
                     children: r.title
                 }), r.fields.map(i => t.jsx("div", {
                     children: i.map(l => t.jsx("div", {
                         className: "form-group " + l.name,
@@ -2841,15 +2840,15 @@
                 text: e.data.info
             }
         })
     }
 
     function i() {
         if (e.data.display) return t.jsxs(t.Fragment, {
-            children: [e.data.display.map(h => t.jsx(x, {
+            children: [e.data.display.map(h => t.jsx(y, {
                 data: h
             }, Math.random())), t.jsx("div", {
                 style: {
                     marginTop: 30
                 }
             })]
         })
@@ -2910,50 +2909,52 @@
                 },
                 children: [a(), r(), i(), l(), d(), c()]
             })]
         })
     }
 
     function u() {
-        G()
+        V()
     }
 
     function o(h) {
         h.preventDefault();
-        var f = e.data.url,
+        var g = e.data.url,
             w = document.getElementById(n),
             v = new FormData(w);
         if (w.method.toUpperCase() == "GET") {
-            const B = f.indexOf("?") >= 0 ? "&" : "?";
-            f = f + B + "form=" + e.data.title + "&" + new URLSearchParams(v).toString(), v = null
+            const D = g.indexOf("?") >= 0 ? "&" : "?";
+            g = g + D + "form=" + e.data.title + "&" + new URLSearchParams(v).toString(), v = null
         }
-        L(w.method.toUpperCase(), f, function(g) {
-            if (w.querySelectorAll(".error").forEach(y => y.style.display = "none"), h.target.dataset.spinning && (h.target.querySelector("i.fa-spin").style.display = "none", h.target.querySelector("i.fa-" + h.target.dataset.spinning).style.display = "inline-block"), g.type == "response") return G(), Ke(), we(g);
-            if (g.type == "error") {
-                var j = g.text;
-                console.log(g), Object.keys(g.errors).map(function(y) {
-                    if (y == "__all__") j = g.errors[y];
+        q(w.method.toUpperCase(), g, function(m) {
+            if (w.querySelectorAll(".error").forEach(x => x.style.display = "none"), h.target.dataset.spinning && (h.target.querySelector("i.fa-spin").style.display = "none", h.target.querySelector("i.fa-" + h.target.dataset.spinning).style.display = "inline-block"), m.type == "response") m.store && Object.keys(m.store).map(function(x) {
+                m.store[x] ? localStorage.setItem(x, m.store[x]) : localStorage.removeItem(x, m.store[x])
+            }), m.redirect && m.redirect.length > 2 ? (m.message && localStorage.setItem("message", m.message), document.location.href = H(m.redirect)) : (m.message && G(m.message), m.redirect == ".." && (document.getElementsByTagName("dialog").length == 0 ? history.back() : V()), m.redirect == "." && w.reset(), m.dispose && (w.style.display = "none"), Ke());
+            else if (m.type == "error") {
+                var j = m.text;
+                console.log(m), Object.keys(m.errors).map(function(x) {
+                    if (x == "__all__") j = m.errors[x];
                     else {
-                        const D = w.querySelector("#" + y + "_error");
-                        D.querySelector("span").innerHTML = g.errors[y], D.style.display = "block"
+                        const I = w.querySelector("#" + x + "_error");
+                        I.querySelector("span").innerHTML = m.errors[x], I.style.display = "block"
                     }
-                }), te(j, !0)
+                }), G(j, !0)
             } else {
-                const y = document.querySelector("#output");
-                y.innerHTML = "", z.createRoot(y.appendChild(document.createElement("div"))).render(t.jsx(x, {
-                    data: g
+                const x = document.querySelector("#output");
+                x.innerHTML = "", W.createRoot(x.appendChild(document.createElement("div"))).render(t.jsx(y, {
+                    data: m
                 }))
             }
         }, v)
     }
     return s()
 }
 
-function Dt(e) {
-    W(`
+function It(e) {
+    F(`
         .calendar table{
             width: 100%;
             border-spacing: 0px;
             border-collapse: collapse;
             margin-top: 15px;
             margin-bottom: 15px;
         }
@@ -3091,16 +3092,16 @@
                 })]
             })]
         })
     }
     return u()
 }
 
-function It(e) {
-    W(`
+function Dt(e) {
+    F(`
       .paginator{
         display: flex;
         justify-content: space-between;
         line-height: 4rem;
         align-items: baseline;
       }
       .paginator .inline{
@@ -3199,16 +3200,16 @@
             style: a,
             children: e.total
         })
     }
     return n()
 }
 
-function qt(e) {
-    W(`
+function Nt(e) {
+    F(`
     .queryset h1, .queryset h2{
       margin: 0px;
     }
     .queryset .title{
       display: flex;
       justify-content: space-between;
       align-items: center;
@@ -3227,358 +3228,358 @@
         padding-bottom: 5px;
         padding-left: 15px;
         padding-right: 15px;
         font-weight: active ? bold : normal;
         text-decoration: none;
     }
   `), e.data.id == null && (e.data.id = Math.random());
-    const [n, a] = I.useState(e.data);
+    const [n, a] = B.useState(e.data);
 
     function r() {
         return n.attrname ? t.jsx("h2", {
-            "data-label": M(n.title),
+            "data-label": E(n.title),
             children: n.title
         }) : t.jsxs("h1", {
-            "data-label": M(n.title),
+            "data-label": E(n.title),
             children: [n.title, " ", n.total > 10 && "(" + n.total + ")"]
         })
     }
 
     function i() {
         return t.jsxs("div", {
             className: "title",
             children: [r(), t.jsx("i", {
                 id: "loader-" + e.data.id,
                 className: "fa-solid fa-circle-notch fa-spin fa-1x"
             })]
         })
     }
 
-    function l(m) {
-        document.getElementById("loader-" + e.data.id).style.display = m ? "block" : "none"
+    function l(f) {
+        document.getElementById("loader-" + e.data.id).style.display = f ? "block" : "none"
     }
 
     function d() {
         return n.subsets && t.jsx("div", {
             className: "tabs",
-            children: n.subsets.map(function(m, p) {
-                var E = n.subset === m.name || !n.subset && p == 0;
+            children: n.subsets.map(function(f, p) {
+                var M = n.subset === f.name || !n.subset && p == 0;
                 return t.jsxs(O, {
                     href: "#",
                     style: {
-                        borderBottom: E ? "solid 3px #2670e8" : 0,
+                        borderBottom: M ? "solid 3px #2670e8" : 0,
                         color: "#0c326f"
                     },
-                    onClick: function(N) {
-                        N.preventDefault(), c(m.name)
+                    onClick: function(L) {
+                        L.preventDefault(), c(f.name)
                     },
-                    dataLabel: M(m.label),
-                    children: [m.label, " ", t.jsx(Bt, {
-                        total: m.count
+                    dataLabel: E(f.label),
+                    children: [f.label, " ", t.jsx(Bt, {
+                        total: f.count
                     })]
                 }, Math.random())
             })
         })
     }
 
-    function c(m) {
+    function c(f) {
         const p = document.getElementById("subset-" + e.data.id);
-        p.value = m || "", D()
+        p.value = f || "", I()
     }
 
-    function s(m, p, E) {
-        const N = document.getElementById("form-" + e.data.id);
-        N.querySelector("input[name=" + n.calendar.field + "__day]").value = m || "", N.querySelector("input[name=" + n.calendar.field + "__month]").value = p || "", N.querySelector("input[name=" + n.calendar.field + "__year]").value = E || "", v(1)
+    function s(f, p, M) {
+        const L = document.getElementById("form-" + e.data.id);
+        L.querySelector("input[name=" + n.calendar.field + "__day]").value = f || "", L.querySelector("input[name=" + n.calendar.field + "__month]").value = p || "", L.querySelector("input[name=" + n.calendar.field + "__year]").value = M || "", v(1)
     }
 
     function u() {
-        if (n.calendar) return t.jsx(Dt, {
+        if (n.calendar) return t.jsx(It, {
             data: n.calendar,
             onChange: s
         })
     }
 
-    function o(m) {
+    function o(f) {
         const p = {
             textAlign: "left",
             verticalAlign: "top",
             lineHeight: "1.2rem",
             color: k.colors.primary,
             padding: 5
         };
         if (!(window.innerWidth < 800)) return t.jsxs("tr", {
-            children: [m.map(function(E) {
-                return E.label != "ID" && t.jsx("th", {
+            children: [f.map(function(M) {
+                return M.label != "ID" && t.jsx("th", {
                     style: p,
                     className: "bold",
-                    children: E.label
+                    children: M.label
                 }, Math.random())
             }), t.jsx("th", {
                 style: p
             })]
         })
     }
 
-    function h(m) {
+    function h(f) {
         const p = {
                 borderBottom: "solid 1px #DDD",
                 padding: 5
             },
-            E = {
+            M = {
                 borderBottom: "solid 1px #DDD",
                 lineHeight: "3rem",
                 textAlign: "right"
             };
         return window.innerWidth < 800 ? t.jsxs("tr", {
             children: [t.jsx("td", {
                 style: p,
-                children: m.title
+                children: f.title
             }, Math.random()), t.jsx("td", {
-                style: E,
+                style: M,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
                     children: t.jsx(S, {
                         icon: "chevron-right",
-                        onClick: () => Re(m.actions),
+                        onClick: () => Re(f.actions),
                         style: {
                             cursor: "pointer",
                             marginRight: 20
                         }
                     })
                 })
             })]
         }, Math.random()) : t.jsxs("tr", {
-            children: [m.data.map(function(N) {
-                return N.label != "ID" && t.jsx("td", {
+            children: [f.data.map(function(L) {
+                return L.label != "ID" && t.jsx("td", {
                     style: p,
-                    children: F(N.value)
+                    children: z(L.value)
                 }, Math.random())
             }), t.jsx("td", {
-                style: E,
+                style: M,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
-                    children: m.actions.map(function(N) {
+                    children: f.actions.map(function(L) {
                         return t.jsx(_, {
-                            data: N,
+                            data: L,
                             default: !0,
                             compact: !0
                         }, Math.random())
                     })
                 })
             })]
         }, Math.random())
     }
 
-    function f() {
+    function g() {
         return n.data.length > 0 ? (n.render == null && window.innerWidth < 800 && (n.renderer = "rows"), n.renderer ? n.renderer == "cards" ? t.jsx(P, {
             width: 300,
             alignItems: "start",
-            children: n.data.map(function(m) {
-                return m.type = n.renderer, t.jsx("div", {
-                    children: t.jsx(x, {
-                        data: m
+            children: n.data.map(function(f) {
+                return f.type = n.renderer, t.jsx("div", {
+                    children: t.jsx(y, {
+                        data: f
                     })
                 }, Math.random())
             })
         }) : t.jsx("div", {
             style: {
                 marginBottom: 15
             },
-            children: n.data.map(function(m) {
-                return m.type = n.renderer, t.jsx(x, {
-                    data: m
+            children: n.data.map(function(f) {
+                return f.type = n.renderer, t.jsx(y, {
+                    data: f
                 }, Math.random())
             })
         }) : w()) : t.jsx(oe, {
             data: {
                 text: "Nenhum registro encontrado."
             }
         })
     }
 
     function w() {
-        const m = {
+        const f = {
                 width: "100%",
                 overflowX: "auto"
             },
             p = {
                 width: "100%",
                 lineHeight: "2rem",
                 borderSpacing: 0
             };
         return t.jsx("div", {
-            style: m,
+            style: f,
             children: t.jsxs("table", {
                 style: p,
                 children: [t.jsx("thead", {
                     children: o(n.data[0].data)
                 }), t.jsx("tbody", {
-                    children: n.data.map(function(E) {
-                        return h(E)
+                    children: n.data.map(function(M) {
+                        return h(M)
                     })
                 })]
             })
         })
     }
 
-    function v(m) {
-        const E = document.getElementById("form-" + e.data.id).querySelector("input[name=page]");
-        E && (E.value = m), D(), j()
+    function v(f) {
+        const M = document.getElementById("form-" + e.data.id).querySelector("input[name=page]");
+        M && (M.value = f), I(), j()
     }
 
-    function B() {
-        const m = document.getElementById("form-" + e.data.id);
-        if (m) {
-            const p = m.querySelector("input[name=page]");
+    function D() {
+        const f = document.getElementById("form-" + e.data.id);
+        if (f) {
+            const p = f.querySelector("input[name=page]");
             p && (p.value = n.pagination.page.current)
         }
-        return t.jsx(It, {
+        return t.jsx(Dt, {
             data: n.pagination,
             onChange: v,
             total: n.total
         })
     }
 
-    function g() {
+    function m() {
         return t.jsx("div", {
             align: "right",
             style: {
                 marginTop: 20,
                 marginBottom: 20
             },
-            children: n.actions.map(function(m) {
+            children: n.actions.map(function(f) {
                 return t.jsx(_, {
-                    data: m,
+                    data: f,
                     primary: !0
                 }, Math.random())
             })
         })
     }
 
     function j() {
-        const m = document.getElementById(e.data.id).getBoundingClientRect().top + window.scrollY;
-        console.log(m), console.log(e.data.id), window.scrollTo({
-            top: m,
+        const f = document.getElementById(e.data.id).getBoundingClientRect().top + window.scrollY;
+        console.log(f), console.log(e.data.id), window.scrollTo({
+            top: f,
             behavior: "smooth"
         })
     }
 
-    function y() {
-        const m = {
+    function x() {
+        const f = {
                 backgroundColor: "#f8f8f8",
                 borderBottom: "solid 1px #DDD",
                 marginBottom: 10,
                 padding: 10
             },
             p = n.search.length > 0,
-            E = n.filters.length > 0;
-        if ((n.bi || n.data.length >= 0) && (p || E)) {
-            const N = {
+            M = n.filters.length > 0;
+        if ((n.bi || n.data.length >= 0) && (p || M)) {
+            const L = {
                 name: "q",
                 mask: null,
                 type: "text",
                 label: "Palavras-chaves",
                 value: n.q
             };
             return t.jsxs("div", {
-                style: m,
+                style: f,
                 children: [t.jsxs(P, {
                     width: 250,
                     children: [p && t.jsx("div", {
-                        children: t.jsx(Z, {
-                            data: N
+                        children: t.jsx(ee, {
+                            data: L
                         })
-                    }), E && n.filters.map(function(q) {
-                        return q.type != "hidden" && t.jsx("div", {
-                            children: t.jsx(Z, {
-                                data: q
+                    }), M && n.filters.map(function(N) {
+                        return N.type != "hidden" && t.jsx("div", {
+                            children: t.jsx(ee, {
+                                data: N
                             })
                         }, Math.random())
                     }), t.jsx("div", {
                         children: t.jsx(R, {
-                            onClick: D,
+                            onClick: I,
                             label: "Filtrar",
                             icon: "filter"
                         })
                     })]
-                }), E && n.filters.map(function(q) {
-                    return q.type == "hidden" && t.jsx("div", {
-                        children: t.jsx(Z, {
-                            data: q
+                }), M && n.filters.map(function(N) {
+                    return N.type == "hidden" && t.jsx("div", {
+                        children: t.jsx(ee, {
+                            data: N
                         })
                     }, Math.random())
                 })]
             })
         }
     }
 
-    function D() {
+    function I() {
         l(!0);
-        var m;
+        var f;
         const p = new URLSearchParams(new FormData(document.getElementById("form-" + e.data.id))).toString();
-        e.data.url.indexOf("?") > 0 ? m = e.data.url + "&" + p : m = e.data.url + "?" + p, L("GET", m, function(E) {
-            a(E), l(!1)
+        e.data.url.indexOf("?") > 0 ? f = e.data.url + "&" + p : f = e.data.url + "?" + p, q("GET", f, function(M) {
+            a(M), l(!1)
         })
     }
 
     function b() {
-        const m = {
+        const f = {
             color: k.colors.primary
         };
         return e.data.reloadable && t.jsxs("div", {
             align: "center",
             children: [t.jsxs("i", {
                 children: ["Ultima atualização em ", new Date().toLocaleTimeString()]
             }), t.jsx("div", {
                 children: t.jsx(O, {
-                    style: m,
+                    style: f,
                     onClick: p => {
-                        p.preventDefault(), D()
+                        p.preventDefault(), I()
                     },
                     children: "Atualizar agora"
                 })
             })]
         })
     }
 
     function C() {
         return n.bi ? t.jsxs(t.Fragment, {
-            children: [y(), n.bi.map(function(m) {
+            children: [x(), n.bi.map(function(f) {
                 return t.jsx(P, {
                     width: 300,
                     alignItems: "start",
-                    children: m.map(function(p) {
+                    children: f.map(function(p) {
                         return t.jsx("div", {
-                            children: t.jsx(x, {
+                            children: t.jsx(y, {
                                 data: p
                             })
                         }, Math.random())
                     })
                 }, Math.random())
             })]
         }) : t.jsxs("div", {
             className: "content",
-            children: [b(), g(), d(), y(), u(), f(), B()]
+            children: [b(), m(), d(), x(), u(), g(), D()]
         })
     }
 
     function T() {
-        window[e.data.id] = () => D();
-        const m = {
+        window[e.data.id] = () => I();
+        const f = {
             backgroundColor: "white",
             padding: 20
         };
         return t.jsx("div", {
             className: "reloadable queryset",
             id: e.data.id,
-            sytle: m,
+            sytle: f,
             children: t.jsxs("form", {
                 id: "form-" + e.data.id,
                 children: [t.jsx("div", {
                     children: !1
                 }), t.jsx("input", {
                     type: "hidden",
                     name: "subset",
@@ -3686,31 +3687,31 @@
         return t.jsx(ne, {
             option: i
         })
     }
     return r()
 }
 
-function Lt(e) {
+function qt(e) {
     return t.jsx(he, {
         donut: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function Nt(e) {
+function Lt(e) {
     return t.jsx(he, {
         area: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function H(e) {
+function U(e) {
     var n = e.invert || !1,
         a = e.type || "bar",
         r = e.stack,
         i = {
             type: "value"
         },
         l = {
@@ -3785,55 +3786,55 @@
             option: o
         })
     }
     return u()
 }
 
 function At(e) {
-    return t.jsx(H, {
+    return t.jsx(U, {
         headers: e.headers,
         rows: e.rows
     })
 }
 
 function Rt(e) {
-    return t.jsx(H, {
+    return t.jsx(U, {
         type: "line",
         headers: e.headers,
         rows: e.rows
     })
 }
 
 function Ot(e) {
-    return t.jsx(H, {
+    return t.jsx(U, {
         area: !0,
         type: "line",
         headers: e.headers,
         rows: e.rows
     })
 }
 
 function _t(e) {
-    return t.jsx(H, {
+    return t.jsx(U, {
         stack: "1",
         headers: e.headers,
         rows: e.rows
     })
 }
 
 function Ft(e) {
-    return t.jsx(H, {
+    return t.jsx(U, {
         invert: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
 function zt(e) {
-    return t.jsx(H, {
+    return t.jsx(U, {
         invert: !0,
         stack: "1",
         headers: e.headers,
         rows: e.rows
     })
 }
 
@@ -3934,29 +3935,29 @@
         return t.jsx(ne, {
             option: a
         })
     }
     return n()
 }
 
-function ve(e) {
+function be(e) {
     function n() {
         switch (e.type) {
             case "pie":
                 return t.jsx(he, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "polar":
-                return t.jsx(Nt, {
+                return t.jsx(Lt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "donut":
-                return t.jsx(Lt, {
+                return t.jsx(qt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "bar":
                 return t.jsx(At, {
                     headers: e.headers,
                     rows: e.rows
@@ -3993,15 +3994,15 @@
                 });
             case "progress":
                 return t.jsx(Pt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             default:
-                return t.jsx(H, {
+                return t.jsx(U, {
                     headers: e.headers,
                     rows: e.rows
                 })
         }
     }
 
     function a() {
@@ -4016,95 +4017,110 @@
             }), n()]
         })
     }
     return a()
 }
 
 function Ht(e) {
+    F(`
+    .statistics .odd {
+      background-color: #EEE;
+    }
+  `);
+
     function n() {
         for (var r = [], i = 0; i < e.data.series.length; i++) r.push([e.data.series[i][0], e.data.series[i][1]]);
-        return e.data.chart ? t.jsx(ve, {
+        return e.data.chart ? t.jsx(be, {
             type: e.data.chart,
             title: e.data.title,
             rows: r
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
-                "data-label": M(e.data.title),
+                "data-label": E(e.data.title),
                 children: e.data.title
             }), t.jsx("table", {
                 style: {
-                    width: "100%"
+                    width: "100%",
+                    borderSpacing: 0
                 },
                 children: t.jsx("tbody", {
-                    children: r.map(l => t.jsx("tr", {
-                        children: l.map((d, c) => c == 0 ? t.jsx("th", {
+                    children: r.map((l, d) => t.jsx("tr", {
+                        children: l.map((c, s) => s == 0 ? t.jsx("th", {
                             style: {
                                 textAlign: "left",
-                                lineHeight: "2rem"
+                                lineHeight: "2rem",
+                                padding: 5
                             },
-                            children: d
+                            className: d % 2 == 0 ? "even" : "odd",
+                            children: c
                         }, Math.random()) : t.jsx("td", {
-                            children: F(d)
+                            className: d % 2 == 0 ? "even" : "odd",
+                            children: z(c)
                         }, Math.random()))
                     }, Math.random()))
                 })
             })]
         })
     }
 
     function a() {
         for (var r = [], i = [], l = Object.keys(e.data.series), d = [], c = 0; c < l.length; c++) {
             c == 0 && r.push("");
             for (var s = [l[c]], u = 0, o = 0; o < e.data.series[l[c]].length; o++) {
                 var h = e.data.series[l[c]];
                 c == 0 && r.push(h[o][0]), s.push(h[o][1]), u += h[o][1], l.length > 1 && (c == 0 ? d.push(h[o][1]) : d[o] += h[o][1], o > 0 && o == e.data.series[l[c]].length - 1 && (c == 0 ? d.push(u) : d[o + 1] += u))
             }
-            s.length > 2 && (c == 0 && r.push("TOTAL"), s.push(u)), i.push(s)
+            s.length > 2 && (c == 0 && r.push(""), s.push(u)), i.push(s)
         }
-        return e.data.chart ? t.jsx(ve, {
+        return e.data.chart ? t.jsx(be, {
             type: e.data.chart,
             title: e.data.title,
             headers: r,
             rows: i
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
-                "data-label": M(e.data.title),
+                "data-label": E(e.data.title),
                 children: e.data.title
             }), t.jsxs("table", {
                 style: {
-                    width: "100%"
+                    width: "100%",
+                    borderSpacing: 0
                 },
                 children: [r && t.jsx("thead", {
                     children: t.jsx("tr", {
-                        children: r.map(f => t.jsx("th", {
-                            children: f
+                        children: r.map(g => t.jsx("th", {
+                            className: "bold",
+                            style: {
+                                textAlign: "left",
+                                padding: 5
+                            },
+                            children: g
                         }, Math.random()))
                     })
                 }), t.jsxs("tbody", {
-                    children: [i.map(f => t.jsx("tr", {
-                        children: f.map((w, v) => v == 0 ? t.jsx("th", {
-                            children: w
-                        }, Math.random()) : t.jsx("td", {
-                            align: "center",
+                    children: [i.map((g, w) => t.jsx("tr", {
+                        children: g.map((v, D) => D == 0 ? t.jsx("th", {
+                            className: w % 2 == 0 ? "even" : "odd",
                             style: {
-                                backgroundColor: v == f.length - 1 && r && r[r.length - 1] == "TOTAL" ? "var(--info-color)" : "inherite"
+                                textAlign: "left",
+                                padding: 5
                             },
-                            children: F(w)
+                            children: v
+                        }, Math.random()) : t.jsx("td", {
+                            align: "center",
+                            className: (D == g.length - 1 && r && r[r.length - 1] == "" ? "bold" : "") + " " + (w % 2 == 0 ? "even" : "odd"),
+                            children: z(v)
                         }, Math.random()))
                     }, Math.random())), d.length > 0 && t.jsxs("tr", {
-                        children: [t.jsx("th", {
-                            children: "TOTAL"
-                        }), d.map(f => t.jsxs("td", {
+                        children: [t.jsx("th", {}), d.map(g => t.jsxs("td", {
                             align: "center",
-                            style: {
-                                backgroundColor: "var(--info-color)"
-                            },
-                            children: [F(f), " "]
+                            className: "bold",
+                            children: [z(g), " "]
                         }, Math.random()))]
                     }, Math.random())]
                 })]
             })]
         })
     }
     return Array.isArray(e.data.series) ? n() : a()
@@ -4174,27 +4190,27 @@
             };
         return l.url ? t.jsx("li", {
             style: c,
             onClick: n,
             className: "item",
             children: t.jsxs(O, {
                 href: l.url,
-                dataLabel: M(l.label),
+                dataLabel: E(l.label),
                 style: {
                     textDecoration: "none"
                 },
                 children: [d == 0 && t.jsx(S, {
                     icon: l.icon || "dot-circle",
                     style: s
                 }), l.label]
             })
         }, Math.random()) : l.items.length > 0 && t.jsxs("li", {
             onClick: n,
             style: c,
-            "data-label": M(l.label),
+            "data-label": E(l.label),
             children: [d == 0 && t.jsx(S, {
                 icon: l.icon || "dot-circle",
                 style: s
             }), l.label, t.jsx(S, {
                 icon: "chevron-right",
                 style: {
                     float: "right",
@@ -4258,15 +4274,15 @@
                 l.pushManager.subscribe({
                     userVisibleOnly: !0,
                     applicationServerKey: d
                 }).then(function(c) {
                     if (console.log(c), n = JSON.stringify(c), console.log(n), c) {
                         alert("Notificação ativada com sucesso.");
                         var s = new FormData;
-                        s.append("subscription", n), L("POST", "/api/pushsubscribe/", function(u) {
+                        s.append("subscription", n), q("POST", "/api/pushsubscribe/", function(u) {
                             console.log(u)
                         }, s)
                     } else {
                         alert("Problema ao ativar notificações.");
                         return
                     }
                 }).catch(function(c) {
@@ -4275,15 +4291,15 @@
             } else console.log("No registered service worker.")
         }).catch(function(l) {
             alert("Erro"), console.error("Service Worker Error", l)
         }) : alert("Push messaging is not supported")
     }
 
     function i() {
-        if (window.Notification == null || window.Notification.permission !== "granted") return t.jsx(S, {
+        return t.jsx(S, {
             onClick: r,
             icon: "bell",
             style: {
                 cursor: "pointer",
                 color: k.colors.primary
             }
         })
@@ -4337,37 +4353,37 @@
             })]
         })
     }
     return n()
 }
 
 function $t(e) {
-    const [n, a] = I.useState(e.data);
+    const [n, a] = B.useState(e.data);
     window.loaddata = i => a(i);
 
     function r() {
         const i = {
             minHeight: 400,
             margin: window.innerWidth > 800 ? 20 : 5
         };
         return t.jsx("div", {
             style: i,
             id: "container",
-            children: t.jsx(x, {
+            children: t.jsx(y, {
                 data: n
             }, Math.random())
         })
     }
     return r()
 }
 
 function Jt(e) {
-    I.useEffect(() => {
+    B.useEffect(() => {
         const o = localStorage.getItem("message");
-        o && (localStorage.removeItem("message"), te(o)), window.addEventListener("resize", () => {
+        o && (localStorage.removeItem("message"), G(o)), window.addEventListener("resize", () => {
             const h = document.querySelector("aside");
             h && (h.style.display = window.innerWidth < 800 ? "none" : "block")
         })
     }, []);
 
     function a() {
         const o = document.querySelector("aside");
@@ -4436,91 +4452,91 @@
                     display: "flex",
                     alignItems: "center"
                 },
                 children: [e.data.navbar.adder.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(K, {
+                    children: t.jsx(Z, {
                         actions: e.data.navbar.adder,
                         position: {},
                         dataLabel: "plus",
                         children: t.jsx(S, {
                             icon: "plus"
                         })
                     })
                 }), t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx(Gt, {})
                 }), e.data.navbar.toolbar && window.innerWidth > 800 && e.data.navbar.toolbar.length > 0 && t.jsx("div", {
                     className: "toolbar",
-                    children: e.data.navbar.toolbar.map(function(f) {
+                    children: e.data.navbar.toolbar.map(function(g) {
                         return t.jsx(_, {
-                            data: f,
+                            data: g,
                             primary: !0,
                             compact: !0
                         }, Math.random())
                     })
-                }), e.data.navbar.actions && e.data.navbar.actions.length > 0 && e.data.navbar.actions.map(function(f) {
-                    return f.url == "/api/login/" && (e.data.navbar.user || document.location.pathname == "/app/login/") ? null : t.jsx("div", {
+                }), e.data.navbar.actions && e.data.navbar.actions.length > 0 && e.data.navbar.actions.map(function(g) {
+                    return g.url == "/api/login/" && (e.data.navbar.user || document.location.pathname == "/app/login/") ? null : t.jsx("div", {
                         children: t.jsx(_, {
-                            data: f,
+                            data: g,
                             primary: !0
                         }, Math.random())
                     }, Math.random())
-                }), e.data.oauth && e.data.oauth.length > 0 && e.data.navbar.user == null && e.data.oauth.map(function(f) {
+                }), e.data.oauth && e.data.oauth.length > 0 && e.data.navbar.user == null && e.data.oauth.map(function(g) {
                     return t.jsx(O, {
-                        href: f.url,
+                        href: g.url,
                         style: {
                             marginRight: 10
                         },
-                        children: f.label
+                        children: g.label
                     }, Math.random())
                 }), e.data.navbar.tools.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(K, {
+                    children: t.jsx(Z, {
                         actions: e.data.navbar.tools,
                         position: {},
                         dataLabel: "tools",
                         children: t.jsx(S, {
                             icon: "tools"
                         })
                     })
                 }), e.data.navbar.settings.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(K, {
+                    children: t.jsx(Z, {
                         actions: e.data.navbar.settings,
                         position: {},
                         dataLabel: "gear",
                         children: t.jsx(S, {
                             icon: "gear"
                         })
                     })
                 }), window.innerWidth > 800 && e.data.navbar.user && t.jsx("div", {
-                    children: t.jsx(Ee, {
+                    children: t.jsx(Me, {
                         data: h,
                         style: {
                             padding: 10
                         },
-                        onSelect: f => document.location.href = U(f.id)
+                        onSelect: g => document.location.href = H(g.id)
                     })
                 }), e.data.navbar.user && e.data.navbar.usermenu.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
-                    children: t.jsx(K, {
+                    children: t.jsx(Z, {
                         actions: e.data.navbar.usermenu,
                         position: {},
-                        dataLabel: M(e.data.navbar.user),
+                        dataLabel: E(e.data.navbar.user),
                         children: t.jsx("img", {
                             src: "/static/images/user.svg",
                             style: {
                                 width: 30,
                                 height: 30,
                                 borderRadius: "50%",
                                 objectFit: "cover",
@@ -4632,47 +4648,47 @@
                 mandatory: {
                     OfferToReceiveAudio: !0,
                     OfferToReceiveVideo: !0
                 },
                 offerToReceiveAudio: 1,
                 offerToReceiveVideo: 1
             },
-            sdpTransform: g => g.replace("a=fmtp:111 minptime=10;useinbandfec=1", "a=fmtp:111 ptime=5;useinbandfec=1;stereo=1;maxplaybackrate=48000;maxaveragebitrat=128000;sprop-stereo=1")
+            sdpTransform: m => m.replace("a=fmtp:111 minptime=10;useinbandfec=1", "a=fmtp:111 ptime=5;useinbandfec=1;stereo=1;maxplaybackrate=48000;maxaveragebitrat=128000;sprop-stereo=1")
         };
-    I.useEffect(() => {
-        n = new Peer("123456" + e.data.caller.replaceAll(".", "")), n.on("open", function(g) {
+    B.useEffect(() => {
+        n = new Peer("123456" + e.data.caller.replaceAll(".", "")), n.on("open", function(m) {
             document.getElementById("callerid").innerHTML = e.data.caller
-        }), n.on("call", function(g) {
+        }), n.on("call", function(m) {
             i({
                 video: {
                     width: {
                         exact: 320
                     },
                     height: {
                         exact: 240
                     }
                 },
                 audio: !0
             }, function(j) {
                 a = j;
-                var y = document.getElementById("video2");
-                y.addEventListener("loadedmetadata", function(D) {
-                    y.style.width = this.videoWidth / 4 + "px", y.style.height = this.videoHeight / 4 + "px", y.style.marginLeft = -this.videoWidth / 4 + "px", y.style.visibility = "visible"
-                }, !1), y.srcObject = a, g.answer(j), g.on("stream", function(D) {
-                    r = D, document.getElementById("video1").srcObject = r
-                }), g.on("close", function() {
+                var x = document.getElementById("video2");
+                x.addEventListener("loadedmetadata", function(I) {
+                    x.style.width = this.videoWidth / 4 + "px", x.style.height = this.videoHeight / 4 + "px", x.style.marginLeft = -this.videoWidth / 4 + "px", x.style.visibility = "visible"
+                }, !1), x.srcObject = a, m.answer(j), m.on("stream", function(I) {
+                    r = I, document.getElementById("video1").srcObject = r
+                }), m.on("close", function() {
                     s()
-                }), n.on("error", function(D) {
+                }), n.on("error", function(I) {
                     s()
                 })
             }, function(j) {
                 console.log("Failed to get local stream", j)
             })
-        }), n.on("error", function(g) {
-            g.type == "browser-incompatible" ? alert("Navegador incompatível.") : g.type == "invalid-id" ? alert("Usuário inexistente.") : g.type == "network" ? alert("Problema na conexão do usuário.") : g.type == "peer-unavailable" && alert("Usuário indisponível.")
+        }), n.on("error", function(m) {
+            m.type == "browser-incompatible" ? alert("Navegador incompatível.") : m.type == "invalid-id" ? alert("Usuário inexistente.") : m.type == "network" ? alert("Problema na conexão do usuário.") : m.type == "peer-unavailable" && alert("Usuário indisponível.")
         })
     }, []);
 
     function d() {
         o(a, "audio"), o(a, "video"), o(r, "audio"), o(r, "video")
     }
 
@@ -4680,42 +4696,42 @@
         h(a, "audio"), h(a, "video"), h(r, "audio"), h(r, "video")
     }
 
     function s() {
         u(a, "audio"), u(a, "video"), u(r, "audio"), u(r, "video"), a = null, r = null, document.getElementById("video1").srcObject = null, document.getElementById("video2").srcObject = null, console.log("Stopped!")
     }
 
-    function u(g, j) {
-        g != null && g.getTracks().forEach(y => {
-            y.readyState == "live" && y.kind === j && y.stop()
+    function u(m, j) {
+        m != null && m.getTracks().forEach(x => {
+            x.readyState == "live" && x.kind === j && x.stop()
         })
     }
 
-    function o(g, j) {
-        g != null && g.getTracks().forEach(y => {
-            y.readyState == "live" && y.kind === j && (y.enabled = !1)
+    function o(m, j) {
+        m != null && m.getTracks().forEach(x => {
+            x.readyState == "live" && x.kind === j && (x.enabled = !1)
         })
     }
 
-    function h(g, j) {
-        g != null && g.getTracks().forEach(y => {
-            y.readyState == "live" && y.kind === j && (y.enabled = !0)
+    function h(m, j) {
+        m != null && m.getTracks().forEach(x => {
+            x.readyState == "live" && x.kind === j && (x.enabled = !0)
         })
     }
 
-    function f() {
-        var g = document.getElementById("video1");
-        g.style.width == "" ? g.style.width = "400px" : g.style.width = ""
+    function g() {
+        var m = document.getElementById("video1");
+        m.style.width == "" ? m.style.width = "400px" : m.style.width = ""
     }
 
     function w() {
-        var g = n.call("123456" + e.data.receiver.replaceAll(".", ""), a, l);
-        g.on("stream", function(j) {
+        var m = n.call("123456" + e.data.receiver.replaceAll(".", ""), a, l);
+        m.on("stream", function(j) {
             r = j, document.getElementById("video1").srcObject = r
-        }), g.on("close", function() {
+        }), m.on("close", function() {
             s()
         }), n.on("error", function(j) {
             s()
         })
     }
 
     function v() {
@@ -4736,89 +4752,89 @@
                 echoCancellation: !1,
                 latency: 0,
                 noiseSuppression: !1,
                 sampleRate: 48e3,
                 sampleSize: 16,
                 volume: 1
             }
-        }, function(g) {
-            a = g;
+        }, function(m) {
+            a = m;
             var j = document.getElementById("video2");
-            j.addEventListener("loadedmetadata", function(y) {
+            j.addEventListener("loadedmetadata", function(x) {
                 j.style.width = this.videoWidth / 4 + "px", j.style.height = this.videoHeight / 4 + "px", j.style.marginLeft = -this.videoWidth / 4 + "px", j.style.visibility = "visible"
             }, !1), j.srcObject = a, w()
-        }, function(g) {
+        }, function(m) {
             alert("Failed to get local stream.")
         })
     }
 
-    function B() {
-        var g = {
+    function D() {
+        var m = {
                 width: "fit-content",
                 margin: "auto"
             },
             j = {
                 position: "absolute",
                 color: "white",
                 padding: "5px"
             },
-            y = {
+            x = {
                 color: "white",
                 backgroundColor: "black",
                 padding: 2
             },
-            D = {
+            I = {
                 position: "absolute",
                 marginTop: "-30px"
             },
             b = {
                 backgroundColor: "black"
             },
             C = {
                 visibility: "hidden",
                 width: "0px"
             };
         return t.jsxs("div", {
-            style: g,
+            style: m,
             children: [t.jsx("div", {
                 id: "callerid",
                 style: j
             }), t.jsx("video", {
                 id: "video1",
                 style: b,
                 playsInline: !0,
                 autoPlay: !0
             }), t.jsx("video", {
                 id: "video2",
                 style: C,
                 playsInline: !0,
                 autoPlay: !0
             }), t.jsxs("div", {
-                style: D,
+                style: I,
                 children: [t.jsx(S, {
-                    style: y,
+                    style: x,
                     onClick: v,
                     icon: "play"
                 }), t.jsx(S, {
-                    style: y,
+                    style: x,
                     onClick: d,
                     icon: "pause"
                 }), t.jsx(S, {
-                    style: y,
+                    style: x,
                     onClick: s,
                     icon: "stop"
                 }), t.jsx(S, {
-                    style: y,
-                    onClick: f,
+                    style: x,
+                    onClick: g,
                     icon: "maximize"
                 })]
             })]
         })
     }
-    return B()
+    return D()
 }
 
 function Qt(e) {
     const n = {
         color: e.data.color
     };
 
@@ -4826,92 +4842,92 @@
         return t.jsx("div", {
             style: n,
             children: e.data.text
         })
     }
     return a()
 }
-var ee, me = {};
+var te, me = {};
 const Xt = "/api/application/",
-    be = localStorage.getItem("application");
+    we = localStorage.getItem("application");
 
-function x(e) {
+function y(e) {
     const n = me[e.data.type];
     return n ? Te.createElement(n, {
         data: e.data
     }) : t.jsx("div", {
         children: JSON.stringify(e.data)
     })
 }
-x.register = function(e, n) {
+y.register = function(e, n) {
     me[n.toLowerCase()] = e
 };
-x.render = function(e) {
-    ee = e, document.location.pathname == "/" ? localStorage.getItem("token") ? window.reload("/app/dashboard/") : window.reload("/app/home/") : document.location.pathname == "/app/login/" && (localStorage.getItem("token") || localStorage.getItem("application")) ? (localStorage.removeItem("token"), localStorage.removeItem("application"), document.location.reload()) : window.reload(document.location.href)
+y.render = function(e) {
+    te = e, document.location.pathname == "/" ? localStorage.getItem("token") ? window.reload("/app/dashboard/") : window.reload("/app/home/") : document.location.pathname == "/app/login/" && (localStorage.getItem("token") || localStorage.getItem("application")) ? (localStorage.removeItem("token"), localStorage.removeItem("application"), document.location.reload()) : window.reload(document.location.href)
 };
-x.register(ht, "Counter");
-x.register(Tt, "Form");
-x.register(qt, "QuerySet");
-x.register(Ge, "Fieldset");
-x.register(V, "Field");
-x.register(Je, "Object");
-x.register(Ye, "Section");
-x.register(Xe, "Group");
-x.register(Ht, "Statistics");
-x.register(et, "Image");
-x.register(Ze, "Banner");
-x.register(tt, "Map");
-x.register(nt, "Steps");
-x.register(st, "QrCode");
-x.register(Se, "Badge");
-x.register(rt, "Status");
-x.register(at, "Progress");
-x.register(De, "Color");
-x.register(it, "Boxes");
-x.register(ct, "Indicators");
-x.register(lt, "Shell");
-x.register(ot, "FileLink");
-x.register(dt, "FilePreview");
-x.register(Ne, "Response");
-x.register(Jt, "Application");
-x.register(Ie, "IconSet");
-x.register(ut, "Grid");
-x.register(Pe, "Rows");
-x.register(He, "Cards");
-x.register(Ue, "Timeline");
-x.register(Ce, "Scheduler");
-x.register(Yt, "WebConf");
-x.register(Qt, "Text");
+y.register(ht, "Counter");
+y.register(Tt, "Form");
+y.register(Nt, "QuerySet");
+y.register(Ge, "Fieldset");
+y.register($, "Field");
+y.register(Je, "Object");
+y.register(Ye, "Section");
+y.register(Xe, "Group");
+y.register(Ht, "Statistics");
+y.register(et, "Image");
+y.register(Ze, "Banner");
+y.register(tt, "Map");
+y.register(nt, "Steps");
+y.register(st, "QrCode");
+y.register(Se, "Badge");
+y.register(rt, "Status");
+y.register(at, "Progress");
+y.register(Ie, "Color");
+y.register(it, "Boxes");
+y.register(ct, "Indicators");
+y.register(lt, "Shell");
+y.register(ot, "FileLink");
+y.register(dt, "FilePreview");
+y.register(Le, "Response");
+y.register(Jt, "Application");
+y.register(De, "IconSet");
+y.register(ut, "Grid");
+y.register(Pe, "Rows");
+y.register(He, "Cards");
+y.register(Ue, "Timeline");
+y.register(Ce, "Scheduler");
+y.register(Yt, "WebConf");
+y.register(Qt, "Text");
 window.addEventListener("popstate", e => {
     window.reload(e.currentTarget.location.href)
 });
 window.reload = function(e) {
     const n = e.split("/app/")[1].split("/")[0];
-    me[n] ? L("GET", A(e), function(a) {
-        ee.render(t.jsx(x, {
+    me[n] ? q("GET", A(e), function(a) {
+        te.render(t.jsx(y, {
             data: {
                 type: n,
                 data: a
             }
         }))
     }) : (e != document.location.href && window.history.pushState({
         url: e
-    }, "", e), be ? (window.application = JSON.parse(be), L("GET", A(e), function(a) {
-        window.application.content = a, ee.render(t.jsx(x, {
+    }, "", e), we ? (window.application = JSON.parse(we), q("GET", A(e), function(a) {
+        window.application.content = a, te.render(t.jsx(y, {
             data: window.application
         }, Math.random()))
-    })) : L("GET", Xt, function(r) {
-        window.application = r, localStorage.setItem("application", JSON.stringify(window.application)), L("GET", A(e), function(i) {
-            window.application.content = i, ee.render(t.jsx(x, {
+    })) : q("GET", Xt, function(r) {
+        window.application = r, localStorage.setItem("application", JSON.stringify(window.application)), q("GET", A(e), function(i) {
+            window.application.content = i, te.render(t.jsx(y, {
                 data: window.application
             }, Math.random()))
         })
     }))
 };
 window.load = function(e) {
     e.indexOf(window.origin) >= 0 || e.startsWith("/") ? (e != document.location.href && e != document.location.pathname && window.history.pushState({
         url: e
-    }, "", e), L("GET", A(e), function(n) {
+    }, "", e), q("GET", A(e), function(n) {
         window.loaddata(n)
     })) : document.location.href = e
 };
-x.render(z.createRoot(document.getElementById("root")));
+y.render(W.createRoot(document.getElementById("root")));
```

### Comparing `pyslth-0.3.3/slth/static/js/vanilla-masker.js` & `pyslth-0.3.4/slth/static/js/vanilla-masker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/static/js/vanilla-masker.min.js` & `pyslth-0.3.4/slth/static/js/vanilla-masker.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/statistics.py` & `pyslth-0.3.4/slth/statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,17 +62,17 @@
         self._xdict = {}
         self._ydict = {}
         self._values_dict = None
 
     def calc(self):
         self._values_dict = {}
         if self.y:
-            values_list = self.qs.values_list(self.x, self.y).annotate(self.func(self.z))
+            values_list = self.qs.values_list(self.x, self.y).order_by(self.x, self.y).annotate(self.func(self.z))
         else:
-            values_list = self.qs.values_list(self.x).annotate(self.func(self.z))
+            values_list = self.qs.values_list(self.x).order_by(self.x).annotate(self.func(self.z))
 
         self._xfield = self.qs.model.get_field(self.x.replace('__year', '').replace('__month', ''))
         if self._xdict == {}:
             xvalues = self.qs.values_list(self.x, flat=True).order_by(self.x).distinct()
             if self._xfield.related_model:
                 if hasattr(self._xfield.related_model, 'cor'):
                     self.colors = {pk: color for pk, color in self._xfield.related_model.objects.values_list('id', 'cor')}
```

### Comparing `pyslth-0.3.3/slth/templates/index.html` & `pyslth-0.3.4/slth/templates/index.html`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/templates/service-worker.js` & `pyslth-0.3.4/slth/templates/service-worker.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,42 @@
 'use strict';
 
 self.addEventListener('push', function(event) {
     console.log('[Service Worker] Push Received.');
+    console.log(event.data);
     console.log(`[Service Worker] Push had this data: "${event.data.text()}"`);
-    var tokens = event.data.text().split('>>>');
-    const title = tokens[0]
+    const data = JSON.parse(event.data.text())
+    console.log(data);
     const options = {
-        body: tokens[1],
+        body: data.message,
+        icon: data.icon,
+        data: {
+            url: data.url
+        }
     };
-
-    event.waitUntil(self.registration.showNotification(title, options));
+    event.waitUntil(self.registration.showNotification(data.title, options));
 });
 
 self.addEventListener('notificationclick', function(event) {
     console.log('[Service Worker] Notification click Received.');
+    console.log(event.notification);
+    var url = event.notification.data && event.notification.data.url;
+    if (url) {
+        url = url.replace('/api/', '/app/');
+        event.waitUntil(clients.matchAll({
+            type: 'window'
+        }).then(function(clientList) {
+            var matchFound = false;
+            for (var client of clientList) {
+                var clientUrl = new URL(client.url);
+                var targetUrl = new URL(url.startsWith("/") ? clientUrl.origin + url : url);
+                if (clientUrl.host === targetUrl.host && 'focus' in client) {
+                    client.navigate(url);
+                    client.focus();
+                    matchFound = true;
+                }
+            }
+            if (!matchFound) event.waitUntil(clients.openWindow(url));
+        }));
+    }
     event.notification.close();
-    //event.waitUntil(clients.openWindow('http://petshop.aplicativo.click/app/login/'));
 });
```

### Comparing `pyslth-0.3.3/slth/tests.py` & `pyslth-0.3.4/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/urls.py` & `pyslth-0.3.4/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/utils.py` & `pyslth-0.3.4/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.3/slth/views.py` & `pyslth-0.3.4/slth/views.py`

 * *Files identical despite different names*

