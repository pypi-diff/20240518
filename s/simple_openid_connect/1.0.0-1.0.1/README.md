# Comparing `tmp/simple_openid_connect-1.0.0.tar.gz` & `tmp/simple_openid_connect-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_openid_connect-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "simple_openid_connect-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `simple_openid_connect-1.0.0.tar` & `simple_openid_connect-1.0.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0       50 2023-05-11 13:50:35.101827 simple_openid_connect-1.0.0/.gitattributes
--rw-r--r--   0        0        0     1761 2024-01-26 15:29:34.203943 simple_openid_connect-1.0.0/.github/workflows/checks.yml
--rw-r--r--   0        0        0      136 2023-05-11 13:50:35.101827 simple_openid_connect-1.0.0/.gitignore
--rw-r--r--   0        0        0      795 2023-05-11 13:50:35.101827 simple_openid_connect-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      177 2023-05-11 13:50:35.101827 simple_openid_connect-1.0.0/.readthedocs.yaml
--rw-r--r--   0        0        0     2315 2023-12-19 13:46:23.738527 simple_openid_connect-1.0.0/DEVELOPMENT.md
--rw-r--r--   0        0        0     1116 2023-05-11 13:50:35.101827 simple_openid_connect-1.0.0/LICENSE
--rw-r--r--   0        0        0     4447 2024-01-26 15:29:34.203943 simple_openid_connect-1.0.0/README.md
--rw-r--r--   0        0        0      679 2023-05-11 13:50:35.105827 simple_openid_connect-1.0.0/docs/Makefile
--rw-r--r--   0        0        0        0 2023-05-11 13:50:35.105827 simple_openid_connect-1.0.0/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-11 13:50:35.105827 simple_openid_connect-1.0.0/docs/_templates/.gitkeep
--rw-r--r--   0        0        0      320 2023-05-11 13:50:35.105827 simple_openid_connect-1.0.0/docs/api.rst
--rw-r--r--   0        0        0     1790 2023-05-11 13:50:35.105827 simple_openid_connect-1.0.0/docs/conf.py
--rw-r--r--   0        0        0     7053 2024-02-08 14:47:00.588785 simple_openid_connect-1.0.0/docs/django-integration.rst
--rw-r--r--   0        0        0     2615 2023-05-11 13:50:35.105827 simple_openid_connect-1.0.0/docs/drf-integration.rst
--rw-r--r--   0        0        0      708 2023-05-11 13:50:35.105827 simple_openid_connect-1.0.0/docs/index.rst
--rw-r--r--   0        0        0     1247 2023-05-11 13:50:35.105827 simple_openid_connect-1.0.0/docs/installation.rst
--rw-r--r--   0        0        0     4868 2023-05-11 13:50:35.105827 simple_openid_connect-1.0.0/docs/usage.rst
--rw-r--r--   0        0        0     2385 2024-02-08 14:54:01.448780 simple_openid_connect-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      211 2024-01-26 15:29:36.363598 simple_openid_connect-1.0.0/requirements.dev.txt
--rw-r--r--   0        0        0      127 2024-02-08 14:54:27.240779 simple_openid_connect-1.0.0/src/simple_openid_connect/__init__.py
--rw-r--r--   0        0        0     3855 2023-12-19 13:46:23.738527 simple_openid_connect-1.0.0/src/simple_openid_connect/base_data.py
--rw-r--r--   0        0        0    13420 2024-02-08 13:51:32.192825 simple_openid_connect-1.0.0/src/simple_openid_connect/client.py
--rw-r--r--   0        0        0     3443 2023-06-13 10:15:12.994409 simple_openid_connect-1.0.0/src/simple_openid_connect/client_authentication.py
--rw-r--r--   0        0        0    63268 2024-02-08 14:54:01.448780 simple_openid_connect-1.0.0/src/simple_openid_connect/data.py
--rw-r--r--   0        0        0     1819 2023-06-13 10:15:12.998409 simple_openid_connect-1.0.0/src/simple_openid_connect/discovery.py
--rw-r--r--   0        0        0     1174 2023-06-13 10:15:12.998409 simple_openid_connect-1.0.0/src/simple_openid_connect/exceptions.py
--rw-r--r--   0        0        0      343 2023-06-13 10:15:12.998409 simple_openid_connect-1.0.0/src/simple_openid_connect/flows/__init__.py
--rw-r--r--   0        0        0     5631 2023-06-13 10:15:12.998409 simple_openid_connect-1.0.0/src/simple_openid_connect/flows/authorization_code_flow/__init__.py
--rw-r--r--   0        0        0     5823 2023-06-13 10:15:12.998409 simple_openid_connect-1.0.0/src/simple_openid_connect/flows/authorization_code_flow/client.py
--rw-r--r--   0        0        0     1827 2023-10-04 15:24:00.514545 simple_openid_connect-1.0.0/src/simple_openid_connect/flows/client_credentials_grant/__init__.py
--rw-r--r--   0        0        0     1549 2023-10-04 15:24:00.514545 simple_openid_connect-1.0.0/src/simple_openid_connect/flows/client_credentials_grant/client.py
--rw-r--r--   0        0        0     2208 2023-05-11 13:50:35.109827 simple_openid_connect-1.0.0/src/simple_openid_connect/flows/direct_access_grant/__init__.py
--rw-r--r--   0        0        0     1583 2023-05-11 13:50:35.109827 simple_openid_connect-1.0.0/src/simple_openid_connect/flows/direct_access_grant/client.py
--rw-r--r--   0        0        0       53 2023-06-13 10:15:12.998409 simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/__init__.py
--rw-r--r--   0        0        0       61 2023-06-13 10:15:12.998409 simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/__init__.py
--rw-r--r--   0        0        0     6892 2024-02-08 14:54:01.448780 simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/apps.py
--rw-r--r--   0        0        0     3553 2023-12-19 13:46:23.742527 simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/decorators.py
--rw-r--r--   0        0        0     1792 2024-01-26 15:29:36.367597 simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/middleware.py
--rw-r--r--   0        0        0     2630 2023-06-13 10:15:12.998409 simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/migrations/0001_initial.py
--rw-r--r--   0        0        0      657 2023-12-19 13:46:23.742527 simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/migrations/0002_move_sessions_id_token.py
--rw-r--r--   0        0        0      418 2024-02-08 14:46:54.848785 simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/migrations/0003_openidsession_add_raw_id_token.py
--rw-r--r--   0        0        0        0 2023-06-13 10:15:13.002409 simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/migrations/__init__.py
--rw-r--r--   0        0        0     4442 2024-02-08 14:46:54.848785 simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/models.py
--rw-r--r--   0        0        0      381 2023-06-13 10:15:13.002409 simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/templates/simple_openid_connect/login_failed.html
--rw-r--r--   0        0        0      729 2023-06-13 10:15:13.002409 simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/urls.py
--rw-r--r--   0        0        0    11558 2024-02-08 14:47:00.592785 simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/user_mapping.py
--rw-r--r--   0        0        0     5137 2024-02-08 14:46:54.848785 simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/views.py
--rw-r--r--   0        0        0      306 2023-06-13 10:15:13.002409 simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/djangorestframework/__init__.py
--rw-r--r--   0        0        0     2623 2023-12-19 13:46:23.742527 simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/djangorestframework/authentication.py
--rw-r--r--   0        0        0      957 2023-06-13 10:15:13.002409 simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/djangorestframework/drf_spectacular_schema.py
--rw-r--r--   0        0        0     3836 2023-12-19 13:46:23.742527 simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/djangorestframework/permissions.py
--rw-r--r--   0        0        0      472 2023-06-13 10:15:13.002409 simple_openid_connect-1.0.0/src/simple_openid_connect/jwk.py
--rw-r--r--   0        0        0      621 2023-06-13 10:15:13.006409 simple_openid_connect-1.0.0/src/simple_openid_connect/rp_initiated_logout.py
--rw-r--r--   0        0        0     1509 2023-06-13 10:15:13.006409 simple_openid_connect-1.0.0/src/simple_openid_connect/token_introspection.py
--rw-r--r--   0        0        0     1566 2023-06-13 10:15:13.006409 simple_openid_connect-1.0.0/src/simple_openid_connect/token_refresh.py
--rw-r--r--   0        0        0     1393 2023-06-13 10:15:13.006409 simple_openid_connect-1.0.0/src/simple_openid_connect/userinfo.py
--rw-r--r--   0        0        0      781 2023-06-13 10:15:13.006409 simple_openid_connect-1.0.0/src/simple_openid_connect/utils.py
--rw-r--r--   0        0        0    16998 2023-12-19 13:46:23.742527 simple_openid_connect-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.0/tests/django_test_project/django_test_project/__init__.py
--rw-r--r--   0        0        0     2806 2023-12-19 13:46:23.742527 simple_openid_connect-1.0.0/tests/django_test_project/django_test_project/settings.py
--rw-r--r--   0        0        0     2572 2023-12-19 13:46:23.742527 simple_openid_connect-1.0.0/tests/django_test_project/django_test_project/tests/conftest.py
--rw-r--r--   0        0        0     1560 2023-12-19 13:46:23.742527 simple_openid_connect-1.0.0/tests/django_test_project/django_test_project/tests/test_access_token_protected_view.py
--rw-r--r--   0        0        0      633 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.0/tests/django_test_project/django_test_project/tests/test_frontchannel_logout_notifications.py
--rw-r--r--   0        0        0     5247 2023-06-01 11:14:39.765067 simple_openid_connect-1.0.0/tests/django_test_project/django_test_project/tests/test_login.py
--rw-r--r--   0        0        0      687 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.0/tests/django_test_project/django_test_project/tests/test_logout.py
--rw-r--r--   0        0        0     1248 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.0/tests/django_test_project/django_test_project/urls.py
--rw-r--r--   0        0        0      639 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.0/tests/django_test_project/django_test_project/views.py
--rw-r--r--   0        0        0      415 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.0/tests/django_test_project/django_test_project/wsgi.py
--rwxr-xr-x   0        0        0      675 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.0/tests/django_test_project/manage.py
--rw-r--r--   0        0        0     1746 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.0/tests/interactive_tests/conftest.py
--rw-r--r--   0        0        0     2001 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.0/tests/interactive_tests/test_google.py
--rw-r--r--   0        0        0     1693 2023-12-19 13:46:23.742527 simple_openid_connect-1.0.0/tests/test_authorization_code_flow.py
--rw-r--r--   0        0        0     3125 2023-12-19 13:46:23.742527 simple_openid_connect-1.0.0/tests/test_client.py
--rw-r--r--   0        0        0      934 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.0/tests/test_client_auth.py
--rw-r--r--   0        0        0     1227 2023-10-04 15:24:00.514545 simple_openid_connect-1.0.0/tests/test_client_credentials_grant.py
--rw-r--r--   0        0        0     1378 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.0/tests/test_direct_access_grant.py
--rw-r--r--   0        0        0     1541 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.0/tests/test_discovery.py
--rw-r--r--   0        0        0      590 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.0/tests/test_jwk.py
--rw-r--r--   0        0        0     2274 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.0/tests/test_message_encoding.py
--rw-r--r--   0        0        0      581 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.0/tests/test_rp_initiated_logout.py
--rw-r--r--   0        0        0     5754 1970-01-01 00:00:00.000000 simple_openid_connect-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-05-11 13:50:35.101827 simple_openid_connect-1.0.1/.gitattributes
+-rw-r--r--   0        0        0     1761 2024-01-26 15:29:34.203943 simple_openid_connect-1.0.1/.github/workflows/checks.yml
+-rw-r--r--   0        0        0      136 2023-05-11 13:50:35.101827 simple_openid_connect-1.0.1/.gitignore
+-rw-r--r--   0        0        0      795 2023-05-11 13:50:35.101827 simple_openid_connect-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      177 2023-05-11 13:50:35.101827 simple_openid_connect-1.0.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     2315 2023-12-19 13:46:23.738527 simple_openid_connect-1.0.1/DEVELOPMENT.md
+-rw-r--r--   0        0        0     1116 2023-05-11 13:50:35.101827 simple_openid_connect-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4447 2024-01-26 15:29:34.203943 simple_openid_connect-1.0.1/README.md
+-rw-r--r--   0        0        0      679 2023-05-11 13:50:35.105827 simple_openid_connect-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0        0 2023-05-11 13:50:35.105827 simple_openid_connect-1.0.1/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-11 13:50:35.105827 simple_openid_connect-1.0.1/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0      320 2023-05-11 13:50:35.105827 simple_openid_connect-1.0.1/docs/api.rst
+-rw-r--r--   0        0        0     2122 2024-05-18 08:57:29.442322 simple_openid_connect-1.0.1/docs/conf.py
+-rw-r--r--   0        0        0     7480 2024-05-18 08:57:29.442322 simple_openid_connect-1.0.1/docs/django-integration.rst
+-rw-r--r--   0        0        0     2615 2023-05-11 13:50:35.105827 simple_openid_connect-1.0.1/docs/drf-integration.rst
+-rw-r--r--   0        0        0      708 2023-05-11 13:50:35.105827 simple_openid_connect-1.0.1/docs/index.rst
+-rw-r--r--   0        0        0     1247 2023-05-11 13:50:35.105827 simple_openid_connect-1.0.1/docs/installation.rst
+-rw-r--r--   0        0        0     4868 2023-05-11 13:50:35.105827 simple_openid_connect-1.0.1/docs/usage.rst
+-rw-r--r--   0        0        0     2385 2024-02-08 14:54:01.448780 simple_openid_connect-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      211 2024-01-26 15:29:36.363598 simple_openid_connect-1.0.1/requirements.dev.txt
+-rw-r--r--   0        0        0      127 2024-05-18 08:58:17.782766 simple_openid_connect-1.0.1/src/simple_openid_connect/__init__.py
+-rw-r--r--   0        0        0     3855 2023-12-19 13:46:23.738527 simple_openid_connect-1.0.1/src/simple_openid_connect/base_data.py
+-rw-r--r--   0        0        0    13420 2024-02-08 13:51:32.192825 simple_openid_connect-1.0.1/src/simple_openid_connect/client.py
+-rw-r--r--   0        0        0     3443 2023-06-13 10:15:12.994409 simple_openid_connect-1.0.1/src/simple_openid_connect/client_authentication.py
+-rw-r--r--   0        0        0    63268 2024-02-08 14:54:01.448780 simple_openid_connect-1.0.1/src/simple_openid_connect/data.py
+-rw-r--r--   0        0        0     1819 2023-06-13 10:15:12.998409 simple_openid_connect-1.0.1/src/simple_openid_connect/discovery.py
+-rw-r--r--   0        0        0     1174 2023-06-13 10:15:12.998409 simple_openid_connect-1.0.1/src/simple_openid_connect/exceptions.py
+-rw-r--r--   0        0        0      343 2023-06-13 10:15:12.998409 simple_openid_connect-1.0.1/src/simple_openid_connect/flows/__init__.py
+-rw-r--r--   0        0        0     5631 2023-06-13 10:15:12.998409 simple_openid_connect-1.0.1/src/simple_openid_connect/flows/authorization_code_flow/__init__.py
+-rw-r--r--   0        0        0     5823 2023-06-13 10:15:12.998409 simple_openid_connect-1.0.1/src/simple_openid_connect/flows/authorization_code_flow/client.py
+-rw-r--r--   0        0        0     1827 2023-10-04 15:24:00.514545 simple_openid_connect-1.0.1/src/simple_openid_connect/flows/client_credentials_grant/__init__.py
+-rw-r--r--   0        0        0     1549 2023-10-04 15:24:00.514545 simple_openid_connect-1.0.1/src/simple_openid_connect/flows/client_credentials_grant/client.py
+-rw-r--r--   0        0        0     2208 2023-05-11 13:50:35.109827 simple_openid_connect-1.0.1/src/simple_openid_connect/flows/direct_access_grant/__init__.py
+-rw-r--r--   0        0        0     1583 2023-05-11 13:50:35.109827 simple_openid_connect-1.0.1/src/simple_openid_connect/flows/direct_access_grant/client.py
+-rw-r--r--   0        0        0       53 2023-06-13 10:15:12.998409 simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-13 10:15:12.998409 simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/__init__.py
+-rw-r--r--   0        0        0     8022 2024-05-18 08:57:29.442322 simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/apps.py
+-rw-r--r--   0        0        0     3553 2023-12-19 13:46:23.742527 simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/decorators.py
+-rw-r--r--   0        0        0     2298 2024-05-18 08:57:29.442322 simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/middleware.py
+-rw-r--r--   0        0        0     2630 2023-06-13 10:15:12.998409 simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/migrations/0001_initial.py
+-rw-r--r--   0        0        0      657 2023-12-19 13:46:23.742527 simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/migrations/0002_move_sessions_id_token.py
+-rw-r--r--   0        0        0      418 2024-02-08 14:46:54.848785 simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/migrations/0003_openidsession_add_raw_id_token.py
+-rw-r--r--   0        0        0        0 2023-06-13 10:15:13.002409 simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/migrations/__init__.py
+-rw-r--r--   0        0        0     4442 2024-02-08 14:46:54.848785 simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/models.py
+-rw-r--r--   0        0        0      381 2023-06-13 10:15:13.002409 simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/templates/simple_openid_connect/login_failed.html
+-rw-r--r--   0        0        0      729 2023-06-13 10:15:13.002409 simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/urls.py
+-rw-r--r--   0        0        0    11558 2024-02-08 14:47:00.592785 simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/user_mapping.py
+-rw-r--r--   0        0        0     5137 2024-02-08 14:46:54.848785 simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/views.py
+-rw-r--r--   0        0        0      306 2023-06-13 10:15:13.002409 simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/djangorestframework/__init__.py
+-rw-r--r--   0        0        0     2623 2023-12-19 13:46:23.742527 simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/djangorestframework/authentication.py
+-rw-r--r--   0        0        0      957 2023-06-13 10:15:13.002409 simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/djangorestframework/drf_spectacular_schema.py
+-rw-r--r--   0        0        0     3836 2023-12-19 13:46:23.742527 simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/djangorestframework/permissions.py
+-rw-r--r--   0        0        0      472 2023-06-13 10:15:13.002409 simple_openid_connect-1.0.1/src/simple_openid_connect/jwk.py
+-rw-r--r--   0        0        0      621 2023-06-13 10:15:13.006409 simple_openid_connect-1.0.1/src/simple_openid_connect/rp_initiated_logout.py
+-rw-r--r--   0        0        0     1509 2023-06-13 10:15:13.006409 simple_openid_connect-1.0.1/src/simple_openid_connect/token_introspection.py
+-rw-r--r--   0        0        0     1566 2023-06-13 10:15:13.006409 simple_openid_connect-1.0.1/src/simple_openid_connect/token_refresh.py
+-rw-r--r--   0        0        0     1393 2023-06-13 10:15:13.006409 simple_openid_connect-1.0.1/src/simple_openid_connect/userinfo.py
+-rw-r--r--   0        0        0      781 2023-06-13 10:15:13.006409 simple_openid_connect-1.0.1/src/simple_openid_connect/utils.py
+-rw-r--r--   0        0        0    16998 2023-12-19 13:46:23.742527 simple_openid_connect-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.1/tests/django_test_project/django_test_project/__init__.py
+-rw-r--r--   0        0        0     2806 2023-12-19 13:46:23.742527 simple_openid_connect-1.0.1/tests/django_test_project/django_test_project/settings.py
+-rw-r--r--   0        0        0     2572 2023-12-19 13:46:23.742527 simple_openid_connect-1.0.1/tests/django_test_project/django_test_project/tests/conftest.py
+-rw-r--r--   0        0        0     1560 2023-12-19 13:46:23.742527 simple_openid_connect-1.0.1/tests/django_test_project/django_test_project/tests/test_access_token_protected_view.py
+-rw-r--r--   0        0        0      633 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.1/tests/django_test_project/django_test_project/tests/test_frontchannel_logout_notifications.py
+-rw-r--r--   0        0        0     5247 2023-06-01 11:14:39.765067 simple_openid_connect-1.0.1/tests/django_test_project/django_test_project/tests/test_login.py
+-rw-r--r--   0        0        0      687 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.1/tests/django_test_project/django_test_project/tests/test_logout.py
+-rw-r--r--   0        0        0     1248 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.1/tests/django_test_project/django_test_project/urls.py
+-rw-r--r--   0        0        0      639 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.1/tests/django_test_project/django_test_project/views.py
+-rw-r--r--   0        0        0      415 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.1/tests/django_test_project/django_test_project/wsgi.py
+-rwxr-xr-x   0        0        0      675 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.1/tests/django_test_project/manage.py
+-rw-r--r--   0        0        0     1746 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.1/tests/interactive_tests/conftest.py
+-rw-r--r--   0        0        0     2001 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.1/tests/interactive_tests/test_google.py
+-rw-r--r--   0        0        0     1693 2023-12-19 13:46:23.742527 simple_openid_connect-1.0.1/tests/test_authorization_code_flow.py
+-rw-r--r--   0        0        0     3125 2023-12-19 13:46:23.742527 simple_openid_connect-1.0.1/tests/test_client.py
+-rw-r--r--   0        0        0      934 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.1/tests/test_client_auth.py
+-rw-r--r--   0        0        0     1227 2023-10-04 15:24:00.514545 simple_openid_connect-1.0.1/tests/test_client_credentials_grant.py
+-rw-r--r--   0        0        0     1378 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.1/tests/test_direct_access_grant.py
+-rw-r--r--   0        0        0     1541 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.1/tests/test_discovery.py
+-rw-r--r--   0        0        0      590 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.1/tests/test_jwk.py
+-rw-r--r--   0        0        0     2274 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.1/tests/test_message_encoding.py
+-rw-r--r--   0        0        0      581 2023-05-11 13:50:35.117828 simple_openid_connect-1.0.1/tests/test_rp_initiated_logout.py
+-rw-r--r--   0        0        0     5754 1970-01-01 00:00:00.000000 simple_openid_connect-1.0.1/PKG-INFO
```

### Comparing `simple_openid_connect-1.0.0/.github/workflows/checks.yml` & `simple_openid_connect-1.0.1/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/.pre-commit-config.yaml` & `simple_openid_connect-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/DEVELOPMENT.md` & `simple_openid_connect-1.0.1/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/LICENSE` & `simple_openid_connect-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/README.md` & `simple_openid_connect-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/docs/Makefile` & `simple_openid_connect-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/docs/django-integration.rst` & `simple_openid_connect-1.0.1/docs/django-integration.rst`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 ``simple_openid_connect.integrations.django.TokenVerificationMiddleware`` should also be added to the middleware stack.
 This middleware makes sure that access tokens of users are still valid. It is not required if the library is only used as a Resource Server (see below)::
 
     # settings.py
     MIDDLEWARE = [
         ...,
-        "simple_openid_connect.integrations.django.TokenVerificationMiddleware",
+        "simple_openid_connect.integrations.django.middleware.TokenVerificationMiddleware",
     ]
 
 Add url routes
 --------------
 
 Django needs to be told how to route Openid related login views.
 To do so, include this libraries urls into yours::
@@ -65,17 +65,26 @@
     The Openid scopes which are requested from the provider when a user logs in.
     It should be a list of scopes as space separated string and should contain the ``openid`` scope.
 
 - ``LOGIN_URL`` (`django LOGIN_URL docs <https://docs.djangoproject.com/en/dev/ref/settings/#login-url>`_)
     This is recommended to be set to ``simple_openid_connect:login`` to serve this libraries login page which handles Openid authentication.
     If additional authentication methods are also used, don't do this.
 
+- ``LOGIN_REDIRECT_URL`` (`django LOGIN_REDIRECT_URL docs <https://docs.djangoproject.com/en/dev/ref/settings/#login-redirect-url>`_)
+    This is the URL to which a user is redirected after a successful login.
+
 - ``LOGOUT_REDIRECT_URL`` (`django LOGOUT_REDIRECT_URL docs <https://docs.djangoproject.com/en/dev/ref/settings/#logout-redirect-url>`_)
     This is the url the user is redirected to after logging out. If it is not set, some Openid providers do not redirect the user back to the application.
 
+Settings Reference
+------------------
+
+For a list of all settings that are read by *simple_openid_connect*, see the :class:`SettingsModel <simple_openid_connect.integrations.django.apps.SettingsModel>`.
+
+
 Usage
 =====
 
 After setup is done, this library is very *hands off*.
 It authenticates users using Openid-Connect, parses retrieved user information, automatically creates or updates user
 objects as required and then authenticates the current session.
 It interoperates with Django's builtin authentication so things like the ``login_required`` decorator can still be used.
```

### Comparing `simple_openid_connect-1.0.0/docs/drf-integration.rst` & `simple_openid_connect-1.0.1/docs/drf-integration.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/docs/index.rst` & `simple_openid_connect-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/docs/installation.rst` & `simple_openid_connect-1.0.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/docs/usage.rst` & `simple_openid_connect-1.0.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/pyproject.toml` & `simple_openid_connect-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/base_data.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/base_data.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/client.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/client.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/client_authentication.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/client_authentication.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/data.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/data.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/discovery.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/discovery.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/exceptions.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/exceptions.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/flows/authorization_code_flow/__init__.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/flows/authorization_code_flow/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/flows/authorization_code_flow/client.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/flows/authorization_code_flow/client.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/flows/client_credentials_grant/__init__.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/flows/client_credentials_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/flows/client_credentials_grant/client.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/flows/client_credentials_grant/client.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/flows/direct_access_grant/__init__.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/flows/direct_access_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/flows/direct_access_grant/client.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/flows/direct_access_grant/client.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/apps.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/apps.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,25 +28,42 @@
     """
     A pydantic model used to validate django settings
     """
 
     model_config = ConfigDict(from_attributes=True)
 
     OPENID_ISSUER: str
+    "The Openid issuer to use. This is required to be an `https` url and an Openid discovery document should be served under ``{issuer}/.well-known/openid-configuration``."
+
     OPENID_CLIENT_ID: str
+    "The client id that was issued to you from your OpenId provider."
+
     OPENID_CLIENT_SECRET: Optional[str] = None
+    "The client secret that was issued to you from your OpenId provider if this is a confidential client."
+
     OPENID_SCOPE: str = "openid"
+    "The Openid scopes which are requested from the provider when a user logs in. It should be a list of scopes as space separated string and should contain the ``openid`` scope."
+
     OPENID_REDIRECT_URI: Optional[str] = "simple_openid_connect:login-callback"
+    "The URL or ``named URL pattern <https://docs.djangoproject.com/en/dev/topics/http/urls/#naming-url-patterns>``_ where users are redirected to from the OpenId provider and at which the authentication result is processed.\nThis is sometimes also called a callback uri."
+
     OPENID_BASE_URI: Optional[str] = None
+    "The absolute base uri of this application. This is used to construct valid redirect urls to the current application."
+
     OPENID_USER_MAPPER: str = (
         "simple_openid_connect.integrations.django.user_mapping.UserMapper"
     )
+    "An string specifying a class that inherits from :class:`simple_openid_connect.integrations.django.user_mapping.UserMapper`."
 
 
 class OpenidAppConfig(AppConfig):
+    """
+    The Django AppConfig for simple_openid_connect
+    """
+
     name = "simple_openid_connect.integrations.django"
     label = "simple_openid_connect_django"
 
     default_auto_field = "django.db.models.BigAutoField"
 
     def ready(self) -> None:
         """
```

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/decorators.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/decorators.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/middleware.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/middleware.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,30 +16,40 @@
 
 class TokenVerificationMiddleware:
     def __init__(self, get_response: Callable[[HttpRequest], HttpResponse]) -> None:
         self.get_response = get_response
 
     def __call__(self, request: HttpRequest) -> HttpResponse:
         response = self.get_response(request)
+
+        # if we are already trying to log in, no redirect should happen
+        if request.path == resolve_url(settings.LOGIN_URL):
+            return response
+
+        # if the user is not logged in, also no redirect should happen
         openid_session_id = request.session.get("openid_session")
         if not openid_session_id:
             return response
 
+        # the refresh token has a long validity, the access token expires quickly
         openid_session = OpenidSession.objects.get(id=openid_session_id)
         refresh_token = openid_session.refresh_token
         session_valid_until = openid_session.access_token_expiry
         access_token_valid = (
             session_valid_until is not None
             and session_valid_until > datetime.now(timezone.utc)
         )
+        # if the access token is valid, everything is fine
         if access_token_valid:
             return response
 
+        # try to refresh the access token with the refresh token
         logger.debug("access token expired, trying to refresh")
         client = OpenidAppConfig.get_instance().get_client(request)
         exchange_response = client.exchange_refresh_token(refresh_token)
         if isinstance(exchange_response, TokenSuccessResponse):
             openid_session.update_session(exchange_response)
             openid_session.save()
             return response
         else:
+            # the refresh token is also expired, redirect to login
             return HttpResponseRedirect(resolve_url(settings.LOGIN_URL))
```

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/migrations/0001_initial.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/migrations/0002_move_sessions_id_token.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/migrations/0002_move_sessions_id_token.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/models.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/models.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/urls.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/urls.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/user_mapping.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/user_mapping.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/django/views.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/django/views.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/djangorestframework/authentication.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/djangorestframework/authentication.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/djangorestframework/drf_spectacular_schema.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/djangorestframework/drf_spectacular_schema.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/integrations/djangorestframework/permissions.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/integrations/djangorestframework/permissions.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/rp_initiated_logout.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/rp_initiated_logout.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/token_introspection.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/token_introspection.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/token_refresh.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/token_refresh.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/userinfo.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/userinfo.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/src/simple_openid_connect/utils.py` & `simple_openid_connect-1.0.1/src/simple_openid_connect/utils.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/conftest.py` & `simple_openid_connect-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/django_test_project/django_test_project/settings.py` & `simple_openid_connect-1.0.1/tests/django_test_project/django_test_project/settings.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/django_test_project/django_test_project/tests/conftest.py` & `simple_openid_connect-1.0.1/tests/django_test_project/django_test_project/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/django_test_project/django_test_project/tests/test_access_token_protected_view.py` & `simple_openid_connect-1.0.1/tests/django_test_project/django_test_project/tests/test_access_token_protected_view.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/django_test_project/django_test_project/tests/test_frontchannel_logout_notifications.py` & `simple_openid_connect-1.0.1/tests/django_test_project/django_test_project/tests/test_frontchannel_logout_notifications.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/django_test_project/django_test_project/tests/test_login.py` & `simple_openid_connect-1.0.1/tests/django_test_project/django_test_project/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/django_test_project/django_test_project/tests/test_logout.py` & `simple_openid_connect-1.0.1/tests/django_test_project/django_test_project/tests/test_logout.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/django_test_project/django_test_project/urls.py` & `simple_openid_connect-1.0.1/tests/django_test_project/django_test_project/urls.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/django_test_project/django_test_project/views.py` & `simple_openid_connect-1.0.1/tests/django_test_project/django_test_project/views.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/django_test_project/manage.py` & `simple_openid_connect-1.0.1/tests/django_test_project/manage.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/interactive_tests/conftest.py` & `simple_openid_connect-1.0.1/tests/interactive_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/interactive_tests/test_google.py` & `simple_openid_connect-1.0.1/tests/interactive_tests/test_google.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/test_authorization_code_flow.py` & `simple_openid_connect-1.0.1/tests/test_authorization_code_flow.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/test_client.py` & `simple_openid_connect-1.0.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/test_client_auth.py` & `simple_openid_connect-1.0.1/tests/test_client_auth.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/test_client_credentials_grant.py` & `simple_openid_connect-1.0.1/tests/test_client_credentials_grant.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/test_direct_access_grant.py` & `simple_openid_connect-1.0.1/tests/test_direct_access_grant.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/test_discovery.py` & `simple_openid_connect-1.0.1/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/test_jwk.py` & `simple_openid_connect-1.0.1/tests/test_jwk.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/test_message_encoding.py` & `simple_openid_connect-1.0.1/tests/test_message_encoding.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/tests/test_rp_initiated_logout.py` & `simple_openid_connect-1.0.1/tests/test_rp_initiated_logout.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-1.0.0/PKG-INFO` & `simple_openid_connect-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_openid_connect
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple and opinionated OpenID-Connect relying party and resource server implementation
 Author-email: Finn-Thorben Sell <dev@finn-thorben.me>
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
```

