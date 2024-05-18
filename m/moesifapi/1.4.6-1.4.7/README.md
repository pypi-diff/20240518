# Comparing `tmp/moesifapi-1.4.6.tar.gz` & `tmp/moesifapi-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moesifapi-1.4.6.tar", last modified: Wed May  8 23:10:57 2024, max compression
+gzip compressed data, was "moesifapi-1.4.7.tar", last modified: Fri May 17 05:26:35 2024, max compression
```

## Comparing `moesifapi-1.4.6.tar` & `moesifapi-1.4.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:10:57.845313 moesifapi-1.4.6/
--rwxr-xr-x   0 keyur      (501) staff       (20)    11918 2020-05-11 16:17:23.000000 moesifapi-1.4.6/LICENSE
--rw-r--r--   0 keyur      (501) staff       (20)       61 2020-05-11 16:17:23.000000 moesifapi-1.4.6/MANIFEST.in
--rw-r--r--   0 keyur      (501) staff       (20)    13737 2024-05-08 23:10:57.845555 moesifapi-1.4.6/PKG-INFO
--rwxr-xr-x   0 keyur      (501) staff       (20)    12654 2024-03-29 18:28:28.000000 moesifapi-1.4.6/README.md
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:10:57.786080 moesifapi-1.4.6/moesifapi/
--rwxr-xr-x   0 keyur      (501) staff       (20)      209 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/__init__.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     5538 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/api_helper.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:10:57.790691 moesifapi-1.4.6/moesifapi/app_config/
--rw-r--r--   0 keyur      (501) staff       (20)       25 2024-04-06 01:03:24.000000 moesifapi-1.4.6/moesifapi/app_config/__init__.py
--rw-r--r--   0 keyur      (501) staff       (20)     2688 2024-04-06 01:03:24.000000 moesifapi-1.4.6/moesifapi/app_config/app_config.py
--rw-r--r--   0 keyur      (501) staff       (20)     4028 2024-04-06 01:03:24.000000 moesifapi-1.4.6/moesifapi/app_config/regex_config_helper.py
--rw-r--r--   0 keyur      (501) staff       (20)     5064 2024-04-06 01:03:24.000000 moesifapi-1.4.6/moesifapi/config_manager.py
--rwxr-xr-x   0 keyur      (501) staff       (20)      343 2024-05-08 23:09:55.000000 moesifapi-1.4.6/moesifapi/configuration.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:10:57.795658 moesifapi-1.4.6/moesifapi/controllers/
--rwxr-xr-x   0 keyur      (501) staff       (20)       94 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/controllers/__init__.py
--rwxr-xr-x   0 keyur      (501) staff       (20)    19878 2024-05-08 23:09:55.000000 moesifapi-1.4.6/moesifapi/controllers/api_controller.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     1493 2024-03-29 18:28:28.000000 moesifapi-1.4.6/moesifapi/controllers/base_controller.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     2342 2021-02-17 05:27:26.000000 moesifapi-1.4.6/moesifapi/controllers/health_controller.py
--rwxr-xr-x   0 keyur      (501) staff       (20)      409 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/decorators.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:10:57.797738 moesifapi-1.4.6/moesifapi/exceptions/
--rwxr-xr-x   0 keyur      (501) staff       (20)       29 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/exceptions/__init__.py
--rwxr-xr-x   0 keyur      (501) staff       (20)      827 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/exceptions/api_exception.py
--rw-r--r--   0 keyur      (501) staff       (20)    11182 2024-05-08 18:35:25.000000 moesifapi-1.4.6/moesifapi/governance_manager.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:10:57.833772 moesifapi-1.4.6/moesifapi/http/
--rwxr-xr-x   0 keyur      (501) staff       (20)      205 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/http/__init__.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     1117 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/http/http_call_back.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     7690 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/http/http_client.py
--rwxr-xr-x   0 keyur      (501) staff       (20)      962 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/http/http_context.py
--rwxr-xr-x   0 keyur      (501) staff       (20)      791 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/http/http_method_enum.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     2343 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/http/http_request.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     1004 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/http/http_response.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     3291 2024-05-08 23:09:55.000000 moesifapi-1.4.6/moesifapi/http/requests_client.py
--rw-r--r--   0 keyur      (501) staff       (20)      148 2024-04-06 01:03:24.000000 moesifapi-1.4.6/moesifapi/logger_helper.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:10:57.841401 moesifapi-1.4.6/moesifapi/models/
--rwxr-xr-x   0 keyur      (501) staff       (20)      245 2024-03-29 18:28:28.000000 moesifapi-1.4.6/moesifapi/models/__init__.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     1836 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/models/base_model.py
--rw-r--r--   0 keyur      (501) staff       (20)     3002 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/models/campaign_model.py
--rw-r--r--   0 keyur      (501) staff       (20)     3182 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/models/company_model.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     4135 2024-03-29 18:28:28.000000 moesifapi-1.4.6/moesifapi/models/event_model.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     3141 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/models/event_request_model.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     2638 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/models/event_response_model.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     1525 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/models/status_model.py
--rw-r--r--   0 keyur      (501) staff       (20)     3047 2024-03-29 18:28:28.000000 moesifapi-1.4.6/moesifapi/models/subscription_model.py
--rw-r--r--   0 keyur      (501) staff       (20)     3470 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/models/user_model.py
--rwxr-xr-x   0 keyur      (501) staff       (20)      461 2020-05-11 16:17:23.000000 moesifapi-1.4.6/moesifapi/moesif_api_client.py
--rw-r--r--   0 keyur      (501) staff       (20)     2344 2024-04-06 01:03:24.000000 moesifapi-1.4.6/moesifapi/parse_body.py
--rw-r--r--   0 keyur      (501) staff       (20)     8043 2024-04-06 01:03:24.000000 moesifapi-1.4.6/moesifapi/update_companies.py
--rw-r--r--   0 keyur      (501) staff       (20)     7784 2024-04-06 01:03:24.000000 moesifapi-1.4.6/moesifapi/update_users.py
--rw-r--r--   0 keyur      (501) staff       (20)     8502 2024-04-06 01:03:24.000000 moesifapi-1.4.6/moesifapi/workers.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:10:57.788787 moesifapi-1.4.6/moesifapi.egg-info/
--rw-r--r--   0 keyur      (501) staff       (20)    13737 2024-05-08 23:10:57.000000 moesifapi-1.4.6/moesifapi.egg-info/PKG-INFO
--rw-r--r--   0 keyur      (501) staff       (20)     1637 2024-05-08 23:10:57.000000 moesifapi-1.4.6/moesifapi.egg-info/SOURCES.txt
--rw-r--r--   0 keyur      (501) staff       (20)        1 2024-05-08 23:10:57.000000 moesifapi-1.4.6/moesifapi.egg-info/dependency_links.txt
--rw-r--r--   0 keyur      (501) staff       (20)       45 2024-05-08 23:10:57.000000 moesifapi-1.4.6/moesifapi.egg-info/entry_points.txt
--rw-r--r--   0 keyur      (501) staff       (20)      119 2024-05-08 23:10:57.000000 moesifapi-1.4.6/moesifapi.egg-info/requires.txt
--rw-r--r--   0 keyur      (501) staff       (20)       16 2024-05-08 23:10:57.000000 moesifapi-1.4.6/moesifapi.egg-info/top_level.txt
--rw-r--r--   0 keyur      (501) staff       (20)       67 2024-05-08 23:10:57.846238 moesifapi-1.4.6/setup.cfg
--rw-r--r--   0 keyur      (501) staff       (20)     3724 2024-05-08 23:09:55.000000 moesifapi-1.4.6/setup.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:10:57.842225 moesifapi-1.4.6/tests/
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:10:57.844234 moesifapi-1.4.6/tests/controllers/
--rwxr-xr-x   0 keyur      (501) staff       (20)        0 2020-05-11 16:17:23.000000 moesifapi-1.4.6/tests/controllers/__init__.py
--rwxr-xr-x   0 keyur      (501) staff       (20)      887 2024-04-06 01:04:20.000000 moesifapi-1.4.6/tests/controllers/controller_test_base.py
--rwxr-xr-x   0 keyur      (501) staff       (20)    17361 2024-03-29 18:28:28.000000 moesifapi-1.4.6/tests/controllers/test_api_controller.py
--rwxr-xr-x   0 keyur      (501) staff       (20)     4922 2020-05-11 16:17:23.000000 moesifapi-1.4.6/tests/test_helper.py
+drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-05-17 05:26:35.239655 moesifapi-1.4.7/
+-rwxr-xr-x   0 praveen    (501) staff       (20)    11918 2023-11-09 16:30:27.000000 moesifapi-1.4.7/LICENSE
+-rw-rw-r--   0 praveen    (501) staff       (20)       61 2022-08-18 23:33:42.000000 moesifapi-1.4.7/MANIFEST.in
+-rw-r--r--   0 praveen    (501) staff       (20)    13963 2024-05-17 05:26:35.239438 moesifapi-1.4.7/PKG-INFO
+-rwxr-xr-x   0 praveen    (501) staff       (20)    12654 2024-02-29 20:25:49.000000 moesifapi-1.4.7/README.md
+drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-05-17 05:26:35.221526 moesifapi-1.4.7/moesifapi/
+-rwxr-xr-x   0 praveen    (501) staff       (20)      209 2023-11-09 16:30:27.000000 moesifapi-1.4.7/moesifapi/__init__.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)     5538 2023-11-09 16:30:27.000000 moesifapi-1.4.7/moesifapi/api_helper.py
+drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-05-17 05:26:35.223731 moesifapi-1.4.7/moesifapi/app_config/
+-rw-r--r--   0 praveen    (501) staff       (20)       25 2024-05-07 00:03:07.000000 moesifapi-1.4.7/moesifapi/app_config/__init__.py
+-rw-r--r--   0 praveen    (501) staff       (20)     2688 2024-05-07 00:03:07.000000 moesifapi-1.4.7/moesifapi/app_config/app_config.py
+-rw-r--r--   0 praveen    (501) staff       (20)     4028 2024-05-07 00:03:07.000000 moesifapi-1.4.7/moesifapi/app_config/regex_config_helper.py
+-rw-r--r--   0 praveen    (501) staff       (20)     5064 2024-05-07 00:03:07.000000 moesifapi-1.4.7/moesifapi/config_manager.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)      343 2024-05-17 05:25:28.000000 moesifapi-1.4.7/moesifapi/configuration.py
+drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-05-17 05:26:35.227599 moesifapi-1.4.7/moesifapi/controllers/
+-rwxr-xr-x   0 praveen    (501) staff       (20)       94 2023-11-09 16:30:27.000000 moesifapi-1.4.7/moesifapi/controllers/__init__.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)    19878 2024-05-17 05:25:28.000000 moesifapi-1.4.7/moesifapi/controllers/api_controller.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)     1493 2024-01-10 04:21:31.000000 moesifapi-1.4.7/moesifapi/controllers/base_controller.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)     2342 2023-11-09 16:30:27.000000 moesifapi-1.4.7/moesifapi/controllers/health_controller.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)      409 2023-11-09 16:30:27.000000 moesifapi-1.4.7/moesifapi/decorators.py
+drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-05-17 05:26:35.228497 moesifapi-1.4.7/moesifapi/exceptions/
+-rwxr-xr-x   0 praveen    (501) staff       (20)       29 2023-11-09 16:30:27.000000 moesifapi-1.4.7/moesifapi/exceptions/__init__.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)      827 2023-11-09 16:30:27.000000 moesifapi-1.4.7/moesifapi/exceptions/api_exception.py
+-rw-r--r--   0 praveen    (501) staff       (20)    11182 2024-05-07 00:03:07.000000 moesifapi-1.4.7/moesifapi/governance_manager.py
+drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-05-17 05:26:35.232946 moesifapi-1.4.7/moesifapi/http/
+-rwxr-xr-x   0 praveen    (501) staff       (20)      205 2023-11-09 16:30:27.000000 moesifapi-1.4.7/moesifapi/http/__init__.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)     1117 2023-11-09 16:30:27.000000 moesifapi-1.4.7/moesifapi/http/http_call_back.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)     7690 2023-11-09 16:30:27.000000 moesifapi-1.4.7/moesifapi/http/http_client.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)      962 2023-11-09 16:30:27.000000 moesifapi-1.4.7/moesifapi/http/http_context.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)      791 2023-11-09 16:30:27.000000 moesifapi-1.4.7/moesifapi/http/http_method_enum.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)     2343 2023-11-09 16:30:27.000000 moesifapi-1.4.7/moesifapi/http/http_request.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)     1004 2023-11-09 16:30:27.000000 moesifapi-1.4.7/moesifapi/http/http_response.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)     3291 2024-05-17 05:25:28.000000 moesifapi-1.4.7/moesifapi/http/requests_client.py
+-rw-r--r--   0 praveen    (501) staff       (20)      148 2024-05-07 00:03:07.000000 moesifapi-1.4.7/moesifapi/logger_helper.py
+drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-05-17 05:26:35.236364 moesifapi-1.4.7/moesifapi/models/
+-rwxr-xr-x   0 praveen    (501) staff       (20)      245 2024-02-29 20:25:49.000000 moesifapi-1.4.7/moesifapi/models/__init__.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)     1836 2023-11-09 16:30:27.000000 moesifapi-1.4.7/moesifapi/models/base_model.py
+-rw-rw-r--   0 praveen    (501) staff       (20)     3002 2022-08-18 23:33:42.000000 moesifapi-1.4.7/moesifapi/models/campaign_model.py
+-rw-rw-r--   0 praveen    (501) staff       (20)     3182 2022-08-18 23:33:42.000000 moesifapi-1.4.7/moesifapi/models/company_model.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)     4135 2024-01-10 04:21:31.000000 moesifapi-1.4.7/moesifapi/models/event_model.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)     3141 2023-11-09 16:30:27.000000 moesifapi-1.4.7/moesifapi/models/event_request_model.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)     2638 2023-11-09 16:30:27.000000 moesifapi-1.4.7/moesifapi/models/event_response_model.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)     1525 2023-11-09 16:30:27.000000 moesifapi-1.4.7/moesifapi/models/status_model.py
+-rw-r--r--   0 praveen    (501) staff       (20)     3047 2024-02-29 20:25:49.000000 moesifapi-1.4.7/moesifapi/models/subscription_model.py
+-rw-rw-r--   0 praveen    (501) staff       (20)     3470 2022-08-18 23:33:42.000000 moesifapi-1.4.7/moesifapi/models/user_model.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)      461 2023-11-09 16:30:27.000000 moesifapi-1.4.7/moesifapi/moesif_api_client.py
+-rw-r--r--   0 praveen    (501) staff       (20)     2877 2024-05-17 05:25:28.000000 moesifapi-1.4.7/moesifapi/parse_body.py
+-rw-r--r--   0 praveen    (501) staff       (20)     8043 2024-05-07 00:03:07.000000 moesifapi-1.4.7/moesifapi/update_companies.py
+-rw-r--r--   0 praveen    (501) staff       (20)     7784 2024-05-07 00:03:07.000000 moesifapi-1.4.7/moesifapi/update_users.py
+-rw-r--r--   0 praveen    (501) staff       (20)     8502 2024-05-07 00:03:07.000000 moesifapi-1.4.7/moesifapi/workers.py
+drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-05-17 05:26:35.239004 moesifapi-1.4.7/moesifapi.egg-info/
+-rw-r--r--   0 praveen    (501) staff       (20)    13963 2024-05-17 05:26:35.000000 moesifapi-1.4.7/moesifapi.egg-info/PKG-INFO
+-rw-rw-r--   0 praveen    (501) staff       (20)     1637 2024-05-17 05:26:35.000000 moesifapi-1.4.7/moesifapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 praveen    (501) staff       (20)        1 2024-05-17 05:26:35.000000 moesifapi-1.4.7/moesifapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 praveen    (501) staff       (20)       45 2024-05-17 05:26:35.000000 moesifapi-1.4.7/moesifapi.egg-info/entry_points.txt
+-rw-rw-r--   0 praveen    (501) staff       (20)      119 2024-05-17 05:26:35.000000 moesifapi-1.4.7/moesifapi.egg-info/requires.txt
+-rw-rw-r--   0 praveen    (501) staff       (20)       16 2024-05-17 05:26:35.000000 moesifapi-1.4.7/moesifapi.egg-info/top_level.txt
+-rw-rw-r--   0 praveen    (501) staff       (20)       67 2024-05-17 05:26:35.239934 moesifapi-1.4.7/setup.cfg
+-rw-r--r--   0 praveen    (501) staff       (20)     3724 2024-05-17 05:25:28.000000 moesifapi-1.4.7/setup.py
+drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-05-17 05:26:35.237444 moesifapi-1.4.7/tests/
+drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-05-17 05:26:35.238353 moesifapi-1.4.7/tests/controllers/
+-rwxr-xr-x   0 praveen    (501) staff       (20)        0 2023-11-09 16:30:27.000000 moesifapi-1.4.7/tests/controllers/__init__.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)      887 2023-11-09 16:30:27.000000 moesifapi-1.4.7/tests/controllers/controller_test_base.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)    17361 2024-02-29 20:25:49.000000 moesifapi-1.4.7/tests/controllers/test_api_controller.py
+-rwxr-xr-x   0 praveen    (501) staff       (20)     4922 2023-11-09 16:30:27.000000 moesifapi-1.4.7/tests/test_helper.py
```

### Comparing `moesifapi-1.4.6/LICENSE` & `moesifapi-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/PKG-INFO` & `moesifapi-1.4.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moesifapi
-Version: 1.4.6
+Version: 1.4.7
 Summary: Moesif API Lib for Python
 Home-page: https://www.moesif.com/docs/api?python#api-libs
 Author: Moesif, Inc
 Author-email: derric@moesif.com
 License: Apache Software License
 Keywords: log analysis restful api development debug
 Classifier: Development Status :: 4 - Beta
@@ -18,17 +18,24 @@
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: jsonpickle
+Requires-Dist: python-dateutil
+Requires-Dist: isodatetimehandler
+Requires-Dist: readerwriterlock>=1.0.9
+Requires-Dist: apscheduler>=3.10.4
 Provides-Extra: dev
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: nose; extra == "test"
 
 # MoesifApi Lib for Python
 
 [![Built For][ico-built-for]][link-built-for]
 [![Latest Version][ico-version]][link-package]
 [![Language Versions][ico-language]][link-language]
 [![Software License][ico-license]][link-license]
```

### Comparing `moesifapi-1.4.6/README.md` & `moesifapi-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/api_helper.py` & `moesifapi-1.4.7/moesifapi/api_helper.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/app_config/app_config.py` & `moesifapi-1.4.7/moesifapi/app_config/app_config.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/app_config/regex_config_helper.py` & `moesifapi-1.4.7/moesifapi/app_config/regex_config_helper.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/config_manager.py` & `moesifapi-1.4.7/moesifapi/config_manager.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/controllers/api_controller.py` & `moesifapi-1.4.7/moesifapi/controllers/api_controller.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/controllers/base_controller.py` & `moesifapi-1.4.7/moesifapi/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/controllers/health_controller.py` & `moesifapi-1.4.7/moesifapi/controllers/health_controller.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/exceptions/api_exception.py` & `moesifapi-1.4.7/moesifapi/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/governance_manager.py` & `moesifapi-1.4.7/moesifapi/governance_manager.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/http/http_call_back.py` & `moesifapi-1.4.7/moesifapi/http/http_call_back.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/http/http_client.py` & `moesifapi-1.4.7/moesifapi/http/http_client.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/http/http_context.py` & `moesifapi-1.4.7/moesifapi/http/http_context.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/http/http_method_enum.py` & `moesifapi-1.4.7/moesifapi/http/http_method_enum.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/http/http_request.py` & `moesifapi-1.4.7/moesifapi/http/http_request.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/http/http_response.py` & `moesifapi-1.4.7/moesifapi/http/http_response.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/http/requests_client.py` & `moesifapi-1.4.7/moesifapi/http/requests_client.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/models/base_model.py` & `moesifapi-1.4.7/moesifapi/models/base_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/models/campaign_model.py` & `moesifapi-1.4.7/moesifapi/models/campaign_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/models/company_model.py` & `moesifapi-1.4.7/moesifapi/models/company_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/models/event_model.py` & `moesifapi-1.4.7/moesifapi/models/event_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/models/event_request_model.py` & `moesifapi-1.4.7/moesifapi/models/event_request_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/models/event_response_model.py` & `moesifapi-1.4.7/moesifapi/models/event_response_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/models/status_model.py` & `moesifapi-1.4.7/moesifapi/models/status_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/models/subscription_model.py` & `moesifapi-1.4.7/moesifapi/models/subscription_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/models/user_model.py` & `moesifapi-1.4.7/moesifapi/models/user_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/parse_body.py` & `moesifapi-1.4.7/moesifapi/parse_body.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,32 @@
     def transform_headers(cls, headers):
         return {k.lower(): v for k, v in headers.items()}
 
     @classmethod
     def base64_body(cls, body):
         return base64.standard_b64encode(body).decode(encoding="UTF-8"), "base64"
 
+    @staticmethod
+    def get_content_type(headers):
+        try:
+            return headers['content-type']
+        except KeyError:
+            try:
+                return headers['Content-Type']
+            except KeyError:
+                pass
+        return None
+
+    def is_multi_part_upload(self, headers):
+        if not headers:
+            return False
+
+        content_type_header = self.get_content_type(headers)
+        return bool(content_type_header and content_type_header.lower().startswith('multipart/form-data'))
+
     def parse_bytes_body(self, body, content_encoding, headers):
         try:
             if content_encoding is not None and "gzip" in content_encoding.lower() or \
                     (headers is not None and "content-encoding" in headers and headers["content-encoding"] is not None
                      and "gzip" in (headers["content-encoding"]).lower()):
                 parsed_body, transfer_encoding = self.base64_body(gzip.decompress(body))
             else:
```

### Comparing `moesifapi-1.4.6/moesifapi/update_companies.py` & `moesifapi-1.4.7/moesifapi/update_companies.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/update_users.py` & `moesifapi-1.4.7/moesifapi/update_users.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi/workers.py` & `moesifapi-1.4.7/moesifapi/workers.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/moesifapi.egg-info/PKG-INFO` & `moesifapi-1.4.7/moesifapi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moesifapi
-Version: 1.4.6
+Version: 1.4.7
 Summary: Moesif API Lib for Python
 Home-page: https://www.moesif.com/docs/api?python#api-libs
 Author: Moesif, Inc
 Author-email: derric@moesif.com
 License: Apache Software License
 Keywords: log analysis restful api development debug
 Classifier: Development Status :: 4 - Beta
@@ -18,17 +18,24 @@
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: jsonpickle
+Requires-Dist: python-dateutil
+Requires-Dist: isodatetimehandler
+Requires-Dist: readerwriterlock>=1.0.9
+Requires-Dist: apscheduler>=3.10.4
 Provides-Extra: dev
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: nose; extra == "test"
 
 # MoesifApi Lib for Python
 
 [![Built For][ico-built-for]][link-built-for]
 [![Latest Version][ico-version]][link-package]
 [![Language Versions][ico-language]][link-language]
 [![Software License][ico-license]][link-license]
```

### Comparing `moesifapi-1.4.6/moesifapi.egg-info/SOURCES.txt` & `moesifapi-1.4.7/moesifapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/setup.py` & `moesifapi-1.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 setup(
     name='moesifapi',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.4.6',
+    version='1.4.7',
 
     description='Moesif API Lib for Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://www.moesif.com/docs/api?python#api-libs',
```

### Comparing `moesifapi-1.4.6/tests/controllers/controller_test_base.py` & `moesifapi-1.4.7/tests/controllers/controller_test_base.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/tests/controllers/test_api_controller.py` & `moesifapi-1.4.7/tests/controllers/test_api_controller.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.6/tests/test_helper.py` & `moesifapi-1.4.7/tests/test_helper.py`

 * *Files identical despite different names*

