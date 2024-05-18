# Comparing `tmp/linked_services-1.2.1.tar.gz` & `tmp/linked_services-1.2.2.tar.gz`

## Comparing `linked_services-1.2.1.tar` & `linked_services-1.2.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 linked_services-1.2.1/.coveragerc
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 linked_services-1.2.1/.flake8
--rw-r--r--   0        0        0    22308 2020-02-02 00:00:00.000000 linked_services-1.2.1/conftest.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 linked_services-1.2.1/mkdocs.yml
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 linked_services-1.2.1/.github/workflows/workflow.yml
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 linked_services-1.2.1/.vscode/settings.json
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 linked_services-1.2.1/docs/index.md
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 linked_services-1.2.1/docs/css/custom.css
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 linked_services-1.2.1/docs/extending-scope/rest-frameworks.md
--rw-r--r--   0        0        0    15649 2020-02-02 00:00:00.000000 linked_services-1.2.1/docs/extending-service/http-clients.md
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 linked_services-1.2.1/docs/extending-service/rest-frameworks.md
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 linked_services-1.2.1/docs/getting-started/installation.md
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 linked_services-1.2.1/docs/getting-started/scopes.md
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 linked_services-1.2.1/docs/getting-started/services.md
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 linked_services-1.2.1/docs/getting-started/set-up.md
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 linked_services-1.2.1/docs/getting-started/views.md
--rwxr-xr-x   0        0        0      727 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/manage.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/__about__.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/admin.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/apps.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/models.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/settings.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/core/actions.py
--rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/core/decorators.py
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/core/exceptions.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/core/i18n.py
--rw-r--r--   0        0        0    27289 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/core/service.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/core/settings.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/core/shorteners.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/core/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/django/__init__.py
--rw-r--r--   0        0        0    12495 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/django/actions.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/django/admin.py
--rw-r--r--   0        0        0    14095 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/django/models.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/django/receivers.py
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/django/service.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/django/signals.py
--rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/django/tasks.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/django/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/management/commands/__init__.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/management/commands/first_party_webhooks.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/management/commands/get_first_party_ids.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/management/commands/sign_jwt.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/management/commands/sign_request.py
--rw-r--r--   0        0        0    13376 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/rest_framework/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/rest_framework/decorators.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/rest_framework/types.py
--rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/rest_framework/views.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/templates/app-not-found.html
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/templates/authorize.html
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/templates/button.html
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/templates/scopes.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/templatetags/__init__.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/templatetags/button.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 linked_services-1.2.1/src/linked_services/templatetags/scopes.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/__init__.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/django/__init__.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/django/actions/__init__.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/django/actions/test_acreate_user.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/django/actions/test_aget_user.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/django/actions/test_create_user.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/django/actions/test_get_user.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/django/tasks/__init__.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/django/tasks/test_check_credentials.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/django/tasks/test_first_party_webhooks.py
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/django/tasks/test_import_external_user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/management/commands/__init__.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/management/commands/test_sign_jwt.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/management/commands/test_sign_request.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/rest_framework/__init__.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/rest_framework/views/__init__.py
--rw-r--r--   0        0        0    19550 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/rest_framework/views/test_authorize_view.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/utils/__init__.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/utils/argument_parser.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/utils/create_models.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/utils/exceptions.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/utils/get_list.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/utils/is_valid.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 linked_services-1.2.1/tests/utils/just_one.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 linked_services-1.2.1/.gitignore
--rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 linked_services-1.2.1/LICENSE.txt
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 linked_services-1.2.1/README.md
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 linked_services-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 linked_services-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 linked_services-1.2.2/.coveragerc
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 linked_services-1.2.2/.flake8
+-rw-r--r--   0        0        0    23011 2020-02-02 00:00:00.000000 linked_services-1.2.2/conftest.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 linked_services-1.2.2/mkdocs.yml
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 linked_services-1.2.2/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 linked_services-1.2.2/.vscode/settings.json
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 linked_services-1.2.2/docs/index.md
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 linked_services-1.2.2/docs/css/custom.css
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 linked_services-1.2.2/docs/extending-scope/rest-frameworks.md
+-rw-r--r--   0        0        0    16120 2020-02-02 00:00:00.000000 linked_services-1.2.2/docs/extending-service/http-clients.md
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 linked_services-1.2.2/docs/extending-service/rest-frameworks.md
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 linked_services-1.2.2/docs/getting-started/installation.md
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 linked_services-1.2.2/docs/getting-started/scopes.md
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 linked_services-1.2.2/docs/getting-started/services.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 linked_services-1.2.2/docs/getting-started/set-up.md
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 linked_services-1.2.2/docs/getting-started/views.md
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/manage.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/__about__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/admin.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/apps.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/models.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/settings.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/core/actions.py
+-rw-r--r--   0        0        0    14688 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/core/decorators.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/core/exceptions.py
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/core/i18n.py
+-rw-r--r--   0        0        0    28163 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/core/service.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/core/settings.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/core/shorteners.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/core/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/django/__init__.py
+-rw-r--r--   0        0        0    12955 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/django/actions.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/django/admin.py
+-rw-r--r--   0        0        0    14519 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/django/models.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/django/receivers.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/django/service.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/django/signals.py
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/django/tasks.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/django/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/management/commands/__init__.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/management/commands/first_party_webhooks.py
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/management/commands/get_first_party_ids.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/management/commands/sign_jwt.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/management/commands/sign_request.py
+-rw-r--r--   0        0        0    13691 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/rest_framework/__init__.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/rest_framework/decorators.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/rest_framework/types.py
+-rw-r--r--   0        0        0     7899 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/rest_framework/views.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/templates/app-not-found.html
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/templates/authorize.html
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/templates/button.html
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/templates/scopes.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/templatetags/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/templatetags/button.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/templatetags/scopes.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/__init__.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/django/__init__.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/django/actions/__init__.py
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/django/actions/test_acreate_user.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/django/actions/test_aget_user.py
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/django/actions/test_create_user.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/django/actions/test_get_user.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/django/tasks/__init__.py
+-rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/django/tasks/test_check_credentials.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/django/tasks/test_first_party_webhooks.py
+-rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/django/tasks/test_import_external_user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/management/commands/__init__.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/management/commands/test_sign_jwt.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/management/commands/test_sign_request.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/rest_framework/__init__.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/rest_framework/views/__init__.py
+-rw-r--r--   0        0        0    20163 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/rest_framework/views/test_authorize_view.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/utils/argument_parser.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/utils/create_models.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/utils/exceptions.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/utils/get_list.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/utils/is_valid.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/utils/just_one.py
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 linked_services-1.2.2/.gitignore
+-rw-r--r--   0        0        0     7783 2020-02-02 00:00:00.000000 linked_services-1.2.2/LICENSE.txt
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 linked_services-1.2.2/README.md
+-rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 linked_services-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 linked_services-1.2.2/PKG-INFO
```

### Comparing `linked_services-1.2.1/.github/workflows/workflow.yml` & `linked_services-1.2.2/.github/workflows/workflow.yml`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-# This workflow will install Python dependencies, run tests and lint with a single version of Python
-# For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
-
-name: Check
-
-on:
-  push: {}
-  pull_request: {}
-
-env:
-  PYTHON_VERSION: 3.11.8
-  PYTHONUNBUFFERED: 1
-
-jobs:
-  tests:
-    runs-on: ubuntu-latest
-
-    steps:
-      - name: Checkout code
-        uses: actions/checkout@v4
-
-      - name: Set up Python
-        uses: actions/setup-python@v5
-        with:
-          python-version: ${{ env.PYTHON_VERSION }}
-          cache: "pip"
-
-      - name: Install dependencies
-        run: |
-          pip install hatch
-
-      - name: Run tests
-        run: |
-          hatch run test
-
-      - uses: codecov/codecov-action@v4
-        if: ${{ github.event_name == 'pull_request' || github.repository == 'breatheco-de/apiv2' }}
-        with:
-          token: ${{ secrets.CODECOV_TOKEN }} # not required for public repos
-          files: ./coverage.xml # optional
-          flags: unittests # optional
-          name: codecov-umbrella # optional
-          fail_ci_if_error: true # optional (default = false)
-          verbose: true # optional (default = false)
-
-      - name: Upload coverage data to coveralls.io
-        if: ${{ github.event_name == 'pull_request' || github.repository == 'breatheco-de/apiv2' }}
-        run: |
-          hatch run coveralls --service=github
-        env:
-          GITHUB_TOKEN: ${{ github.token }}
-
-  pages:
-    if: >-
-      github.repository == 'breatheco-de/linked-services-django-plugin' &&
-      github.event_name == 'push' &&
-      github.ref == 'refs/heads/main'
-
-    runs-on: ubuntu-latest
-    steps:
-      - name: Checkout code
-        uses: actions/checkout@v4
-
-      - name: Set up Python
-        uses: actions/setup-python@v5
-        with:
-          python-version: ${{ env.PYTHON_VERSION }}
-          cache: "pip"
-
-      - name: Install dependencies
-        run: |
-          pip install hatch
-
-      - name: Deploy docs
-        run: hatch run mkdocs gh-deploy --force
+# This workflow will install Python dependencies, run tests and lint with a single version of Python
+# For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
+
+name: Check
+
+on:
+  push: {}
+  pull_request: {}
+
+env:
+  PYTHON_VERSION: 3.11.8
+  PYTHONUNBUFFERED: 1
+
+jobs:
+  tests:
+    runs-on: ubuntu-latest
+
+    steps:
+      - name: Checkout code
+        uses: actions/checkout@v4
+
+      - name: Set up Python
+        uses: actions/setup-python@v5
+        with:
+          python-version: ${{ env.PYTHON_VERSION }}
+          cache: "pip"
+
+      - name: Install dependencies
+        run: |
+          pip install hatch
+
+      - name: Run tests
+        run: |
+          hatch run test
+
+      - uses: codecov/codecov-action@v4
+        if: ${{ github.event_name == 'pull_request' || github.repository == 'breatheco-de/apiv2' }}
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }} # not required for public repos
+          files: ./coverage.xml # optional
+          flags: unittests # optional
+          name: codecov-umbrella # optional
+          fail_ci_if_error: true # optional (default = false)
+          verbose: true # optional (default = false)
+
+      - name: Upload coverage data to coveralls.io
+        if: ${{ github.event_name == 'pull_request' || github.repository == 'breatheco-de/apiv2' }}
+        run: |
+          hatch run coveralls --service=github
+        env:
+          GITHUB_TOKEN: ${{ github.token }}
+
+  pages:
+    if: >-
+      github.repository == 'breatheco-de/linked-services-django-plugin' &&
+      github.event_name == 'push' &&
+      github.ref == 'refs/heads/main'
+
+    runs-on: ubuntu-latest
+    steps:
+      - name: Checkout code
+        uses: actions/checkout@v4
+
+      - name: Set up Python
+        uses: actions/setup-python@v5
+        with:
+          python-version: ${{ env.PYTHON_VERSION }}
+          cache: "pip"
+
+      - name: Install dependencies
+        run: |
+          pip install hatch
+
+      - name: Deploy docs
+        run: hatch run mkdocs gh-deploy --force
```

### Comparing `linked_services-1.2.1/docs/extending-service/http-clients.md` & `linked_services-1.2.2/docs/extending-service/http-clients.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,471 +1,471 @@
-# HTTP clients
-
-You could write a new implementation for a HTTP client here `src/linked_services/core/service.py`.
-
-## HTTP client preference
-
-### Async
-
-1. `aiohttp`.
-2. `httpx`.
-3. `requests`.
-
-### Sync
-
-1. `httpx`.
-2. `requests`.
-
-### Which are supported right now
-
-- `aiohttp`.
-- `requests`.
-
-### `SyncService` methods
-
-- `__enter__`: called when it gets entered into an sync context.
-- `__exit__`: called when it gets exited from an sync context.
-- `_sync_proxy`: called when it requires that the response be a REST framework response.
-- `_sync_get`: called when it tries to do a get request, it returns a HTTP response or a Rest response.
-- `_sync_options`: called when it tries to do a options request, it returns a HTTP response or a Rest response.
-- `_sync_head`: called when it tries to do a head request, it returns a HTTP response or a Rest response.
-- `_sync_post`: called when it tries to do a post request, it returns a HTTP response or a Rest response.
-- `_sync_webhook`: called when it tries to trigger an webhook, it returns a HTTP response or a Rest response.
-- `_sync_put`: called when it tries to do a put request, it returns a HTTP response or a Rest response.
-- `_sync_patch`: called when it tries to do a patch request, it returns a HTTP response or a Rest response.
-- `_sync_delete`: called when it tries to do a delete request, it returns a HTTP response or a Rest response.
-- `_sync_request`: called when it tries to do a generic request, it returns a HTTP response or a Rest response.
-
-### `AsyncService` methods
-
-- `__aenter__`: called when it gets entered into an async context.
-- `__aexit__`: called when it gets exited from an async context.
-- `_async_proxy`: called when it requires that the response be a REST framework response.
-- `_async_get`: called when it tries to do a get request, it returns a HTTP response or a Rest response.
-- `_async_options`: called when it tries to do a options request, it returns a HTTP response or a Rest response.
-- `_async_head`: called when it tries to do a head request, it returns a HTTP response or a Rest response.
-- `_async_post`: called when it tries to do a post request, it returns a HTTP response or a Rest response.
-- `_async_webhook`: called when it tries to trigger an webhook, it returns a HTTP response or a Rest response.
-- `_async_put`: called when it tries to do a put request, it returns a HTTP response or a Rest response.
-- `_async_patch`: called when it tries to do a patch request, it returns a HTTP response or a Rest response.
-- `_async_delete`: called when it tries to do a delete request, it returns a HTTP response or a Rest response.
-- `_async_request`: called when it tries to do a generic request, it returns a HTTP response or a Rest response.
-
-### How to implement a new HTTP client
-
-You must implement an `SyncService` and `AsyncService` for your new library.
-
-#### Detecting your new client
-
-First, you need to add an import test here, it will tell to the rest of the code which clients are available.
-
-```py
-LIBRARIES = {
-    "requests": False,
-    "aiohttp": False,  # no implemented yet
-    "httpx": False,
-}
-
-try:
-    import requests
-
-    LIBRARIES["requests"] = True
-
-except ImportError:
-    pass
-
-try:
-    from aiohttp.client_reqrep import ClientResponse
-
-    LIBRARIES["aiohttp"] = True
-
-except ImportError:
-    pass
-
-try:
-    import httpx  # noqa: F401
-
-    LIBRARIES["httpx"] = True
-
-except ImportError:
-    pass
-```
-
-#### Implementing `SyncService` and `AsyncService`
-
-You must use `elif LIBRARIES["your-client"]:` to check if your library is available, also, you must remind each client has a different relevance, so, sort them by relevance.
-
-#### `SyncService` example
-
-Implementing `requests` library.
-
-```py
-if LIBRARIES["requests"]:
-
-    class SyncService:
-
-        def __enter__(self) -> "Service":
-
-            self.sync = True
-
-            if isinstance(self.app_pk, self._get_app_cls()):
-                self.app = self.app_pk
-                return self
-
-            try:
-                self.app = self._get_app(self.app_pk)
-
-            except Exception:
-                raise AppNotFound(f"App {self.app_pk} not found")
-
-            return self
-
-        def __exit__(
-            self,
-            exc_type: Optional[Type[BaseException]],
-            exc_val: Optional[BaseException],
-            exc_tb: Optional[TracebackType],
-        ) -> None:
-            pass
-
-        def _sync_proxy(self, request: Callable[[], requests.Response], stream: bool) -> StreamingHttpResponse:
-            try:
-                response = request()
-
-            except Exception as e:
-                raise ValidationException("Unexpected error: " + str(e), code=500, slug="unexpected-error")
-
-            header_keys = [x for x in response.headers.keys() if x not in self.banned_keys]
-
-            if stream:
-                resource = StreamingHttpResponse(
-                    response.raw,
-                    status=response.status_code,
-                    reason=response.reason,
-                )
-
-                for header in header_keys:
-                    resource[header] = response.headers[header]
-
-                return resource
-
-            headers = {}
-
-            for header in header_keys:
-                headers[header] = response.headers[header]
-
-            return HttpResponse(response.content, status=response.status_code, headers=headers)
-
-        def _sync_get(self, url, params=None, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-
-            if self.sync is False:
-                params = kwargs.pop("params", None)
-
-            headers = self._authenticate("get", params=params, **kwargs)
-
-            def request() -> requests.Response:
-                return requests.get(url, params=params, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._sync_proxy(request, kwargs.get("stream", False))
-
-            res = request()
-
-            return res
-
-        def _sync_options(self, url, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("options", **kwargs)
-
-            def request() -> requests.Response:
-                return requests.options(url, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._sync_proxy(request, kwargs.get("stream", False))
-
-            res = request()
-
-            return res
-
-        def _sync_head(self, url, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("head", **kwargs)
-
-            def request() -> requests.Response:
-                return requests.head(url, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._sync_proxy(request, kwargs.get("stream", False))
-
-            res = request()
-
-            return res
-
-        def _sync_post(self, url, data=None, json=None, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("post", data=data, json=json, **kwargs)
-
-            def request() -> requests.Response:
-                return requests.post(url, data=data, json=json, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._sync_proxy(request, kwargs.get("stream", False))
-
-            res = request()
-
-            return res
-
-        def _sync_webhook(self, url, data=None, json=None, **kwargs):
-            url = self.app.webhook_url
-            headers = self._authenticate("post", data=data, json=json, **kwargs)
-
-            def request() -> requests.Response:
-                return requests.post(url, data=data, json=json, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._sync_proxy(request, kwargs.get("stream", False))
-
-            res = request()
-
-            return res
-
-        def _sync_put(self, url, data=None, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("put", data=data, **kwargs)
-
-            def request() -> requests.Response:
-                return requests.put(url, data=data, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._sync_proxy(request, kwargs.get("stream", False))
-
-            res = request()
-
-            return res
-
-        def _sync_patch(self, url, data=None, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("patch", data=data, **kwargs)
-
-            def request() -> requests.Response:
-                return requests.patch(url, data=data, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._sync_proxy(request, kwargs.get("stream", False))
-
-            res = request()
-
-            return res
-
-        def _sync_delete(self, url, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("delete", **kwargs)
-
-            def request() -> requests.Response:
-                return requests.delete(url, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._sync_proxy(request, kwargs.get("stream", False))
-
-            res = request()
-
-            return res
-
-        def _sync_request(self, method, url, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate(method, **kwargs)
-
-            def request() -> requests.Response:
-                return requests.request(method, url, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._sync_proxy(request, kwargs.get("stream", False))
-
-            res = request()
-
-            return res
-```
-
-#### `AsyncService` example
-
-Implementing `aiohttp` library.
-
-```py
-if LIBRARIES["aiohttp"]:
-
-    class AsyncService:
-
-        async def __aenter__(self) -> "Service":
-
-            self.sync = False
-
-            if isinstance(self.app_pk, self._get_app_cls()):
-                self.app = self.app_pk
-
-            else:
-                self.app = await sync_to_async(self._get_app)(self.app_pk)
-
-            self.session = aiohttp.ClientSession()
-
-            # this should be extended
-            await self.session.__aenter__()
-
-            return self
-
-        async def __aexit__(self, *args, **kwargs) -> None:
-            for obj in self.to_close:
-                await obj.__aexit__(*args, **kwargs)
-
-            await self.session.__aexit__(*args, **kwargs)
-
-        # django does not support StreamingHttpResponse with aiohttp due to django would have to close the response
-        async def _async_proxy(self, response: Coroutine[Any, Any, ClientResponse]) -> HttpResponse:
-            try:
-                r = await response
-
-            except Exception as e:
-                raise ValidationException("Unexpected error: " + str(e), code=500, slug="unexpected-error")
-
-            header_keys = [x for x in r.headers.keys() if x not in self.banned_keys]
-
-            headers = {}
-            for header in header_keys:
-                headers[str(header)] = r.headers[header]
-
-            return HttpResponse(await r.content.read(), status=r.status, headers=headers)
-
-        def _async_get(self, url, params=None, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("get", params=params, **kwargs)
-
-            obj = self.session.get(url, params=params, **kwargs, headers=headers)
-            self.to_close.append(obj)
-
-            res = obj.__aenter__()
-
-            # wraps client response to be used within django views
-            if self.proxy:
-                return self._async_proxy(res)
-
-            return res
-
-        def _async_options(self, url, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("options", **kwargs)
-
-            obj = self.session.options(url, **kwargs, headers=headers)
-            self.to_close.append(obj)
-
-            res = obj.__aenter__()
-
-            # wraps client response to be used within django views
-            if self.proxy:
-                return self._async_proxy(res)
-
-            return res
-
-        def _async_head(self, url, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("head", **kwargs)
-
-            obj = self.session.head(url, **kwargs, headers=headers)
-            self.to_close.append(obj)
-
-            res = obj.__aenter__()
-
-            # wraps client response to be used within django views
-            if self.proxy:
-                return self._async_proxy(res)
-
-            return res
-
-        def _async_post(self, url, data=None, json=None, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("post", data=data, json=json, **kwargs)
-
-            obj = self.session.post(url, data=data, json=json, **kwargs, headers=headers)
-            self.to_close.append(obj)
-
-            res = obj.__aenter__()
-
-            # wraps client response to be used within django views
-            if self.proxy:
-                return self._async_proxy(res)
-
-            return res
-
-        def _async_webhook(self, url, data=None, json=None, **kwargs):
-            url = self.app.webhook_url
-            headers = self._authenticate("post", data=data, json=json, **kwargs)
-
-            obj = self.session.post(url, data=data, json=json, **kwargs, headers=headers)
-            self.to_close.append(obj)
-
-            res = obj.__aenter__()
-
-            # wraps client response to be used within django views
-            if self.proxy:
-                return self._async_proxy(res)
-
-            return res
-
-        def _async_put(self, url, data=None, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("put", data=data, **kwargs)
-
-            obj = self.session.put(url, data=data, **kwargs, headers=headers)
-            self.to_close.append(obj)
-
-            res = obj.__aenter__()
-
-            # wraps client response to be used within django views
-            if self.proxy:
-                return self._async_proxy(res)
-
-            return res
-
-        def _async_patch(self, url, data=None, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("patch", data=data, **kwargs)
-
-            obj = self.session.patch(url, data=data, **kwargs, headers=headers)
-            self.to_close.append(obj)
-
-            res = obj.__aenter__()
-
-            # wraps client response to be used within django views
-            if self.proxy:
-                return self._async_proxy(res)
-
-            return res
-
-        def _async_delete(self, url, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("delete", **kwargs)
-
-            obj = self.session.delete(url, **kwargs, headers=headers)
-            self.to_close.append(obj)
-
-            res = obj.__aenter__()
-
-            # wraps client response to be used within django views
-            if self.proxy:
-                return self._async_proxy(res)
-
-            return res
-
-        def _async_request(self, method, url, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate(method, **kwargs)
-
-            obj = self.session.request(method, url, **kwargs, headers=headers)
-            self.to_close.append(obj)
-
-            res = obj.__aenter__()
-
-            # wraps client response to be used within django views
-            if self.proxy:
-                return self._async_proxy(res)
-
-            return res
-```
+# HTTP clients
+
+You could write a new implementation for a HTTP client here `src/linked_services/core/service.py`.
+
+## HTTP client preference
+
+### Async
+
+1. `aiohttp`.
+2. `httpx`.
+3. `requests`.
+
+### Sync
+
+1. `httpx`.
+2. `requests`.
+
+### Which are supported right now
+
+- `aiohttp`.
+- `requests`.
+
+### `SyncService` methods
+
+- `__enter__`: called when it gets entered into an sync context.
+- `__exit__`: called when it gets exited from an sync context.
+- `_sync_proxy`: called when it requires that the response be a REST framework response.
+- `_sync_get`: called when it tries to do a get request, it returns a HTTP response or a Rest response.
+- `_sync_options`: called when it tries to do a options request, it returns a HTTP response or a Rest response.
+- `_sync_head`: called when it tries to do a head request, it returns a HTTP response or a Rest response.
+- `_sync_post`: called when it tries to do a post request, it returns a HTTP response or a Rest response.
+- `_sync_webhook`: called when it tries to trigger an webhook, it returns a HTTP response or a Rest response.
+- `_sync_put`: called when it tries to do a put request, it returns a HTTP response or a Rest response.
+- `_sync_patch`: called when it tries to do a patch request, it returns a HTTP response or a Rest response.
+- `_sync_delete`: called when it tries to do a delete request, it returns a HTTP response or a Rest response.
+- `_sync_request`: called when it tries to do a generic request, it returns a HTTP response or a Rest response.
+
+### `AsyncService` methods
+
+- `__aenter__`: called when it gets entered into an async context.
+- `__aexit__`: called when it gets exited from an async context.
+- `_async_proxy`: called when it requires that the response be a REST framework response.
+- `_async_get`: called when it tries to do a get request, it returns a HTTP response or a Rest response.
+- `_async_options`: called when it tries to do a options request, it returns a HTTP response or a Rest response.
+- `_async_head`: called when it tries to do a head request, it returns a HTTP response or a Rest response.
+- `_async_post`: called when it tries to do a post request, it returns a HTTP response or a Rest response.
+- `_async_webhook`: called when it tries to trigger an webhook, it returns a HTTP response or a Rest response.
+- `_async_put`: called when it tries to do a put request, it returns a HTTP response or a Rest response.
+- `_async_patch`: called when it tries to do a patch request, it returns a HTTP response or a Rest response.
+- `_async_delete`: called when it tries to do a delete request, it returns a HTTP response or a Rest response.
+- `_async_request`: called when it tries to do a generic request, it returns a HTTP response or a Rest response.
+
+### How to implement a new HTTP client
+
+You must implement an `SyncService` and `AsyncService` for your new library.
+
+#### Detecting your new client
+
+First, you need to add an import test here, it will tell to the rest of the code which clients are available.
+
+```py
+LIBRARIES = {
+    "requests": False,
+    "aiohttp": False,  # no implemented yet
+    "httpx": False,
+}
+
+try:
+    import requests
+
+    LIBRARIES["requests"] = True
+
+except ImportError:
+    pass
+
+try:
+    from aiohttp.client_reqrep import ClientResponse
+
+    LIBRARIES["aiohttp"] = True
+
+except ImportError:
+    pass
+
+try:
+    import httpx  # noqa: F401
+
+    LIBRARIES["httpx"] = True
+
+except ImportError:
+    pass
+```
+
+#### Implementing `SyncService` and `AsyncService`
+
+You must use `elif LIBRARIES["your-client"]:` to check if your library is available, also, you must remind each client has a different relevance, so, sort them by relevance.
+
+#### `SyncService` example
+
+Implementing `requests` library.
+
+```py
+if LIBRARIES["requests"]:
+
+    class SyncService:
+
+        def __enter__(self) -> "Service":
+
+            self.sync = True
+
+            if isinstance(self.app_pk, self._get_app_cls()):
+                self.app = self.app_pk
+                return self
+
+            try:
+                self.app = self._get_app(self.app_pk)
+
+            except Exception:
+                raise AppNotFound(f"App {self.app_pk} not found")
+
+            return self
+
+        def __exit__(
+            self,
+            exc_type: Optional[Type[BaseException]],
+            exc_val: Optional[BaseException],
+            exc_tb: Optional[TracebackType],
+        ) -> None:
+            pass
+
+        def _sync_proxy(self, request: Callable[[], requests.Response], stream: bool) -> StreamingHttpResponse:
+            try:
+                response = request()
+
+            except Exception as e:
+                raise ValidationException("Unexpected error: " + str(e), code=500, slug="unexpected-error")
+
+            header_keys = [x for x in response.headers.keys() if x not in self.banned_keys]
+
+            if stream:
+                resource = StreamingHttpResponse(
+                    response.raw,
+                    status=response.status_code,
+                    reason=response.reason,
+                )
+
+                for header in header_keys:
+                    resource[header] = response.headers[header]
+
+                return resource
+
+            headers = {}
+
+            for header in header_keys:
+                headers[header] = response.headers[header]
+
+            return HttpResponse(response.content, status=response.status_code, headers=headers)
+
+        def _sync_get(self, url, params=None, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+
+            if self.sync is False:
+                params = kwargs.pop("params", None)
+
+            headers = self._authenticate("get", params=params, **kwargs)
+
+            def request() -> requests.Response:
+                return requests.get(url, params=params, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._sync_proxy(request, kwargs.get("stream", False))
+
+            res = request()
+
+            return res
+
+        def _sync_options(self, url, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("options", **kwargs)
+
+            def request() -> requests.Response:
+                return requests.options(url, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._sync_proxy(request, kwargs.get("stream", False))
+
+            res = request()
+
+            return res
+
+        def _sync_head(self, url, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("head", **kwargs)
+
+            def request() -> requests.Response:
+                return requests.head(url, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._sync_proxy(request, kwargs.get("stream", False))
+
+            res = request()
+
+            return res
+
+        def _sync_post(self, url, data=None, json=None, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("post", data=data, json=json, **kwargs)
+
+            def request() -> requests.Response:
+                return requests.post(url, data=data, json=json, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._sync_proxy(request, kwargs.get("stream", False))
+
+            res = request()
+
+            return res
+
+        def _sync_webhook(self, url, data=None, json=None, **kwargs):
+            url = self.app.webhook_url
+            headers = self._authenticate("post", data=data, json=json, **kwargs)
+
+            def request() -> requests.Response:
+                return requests.post(url, data=data, json=json, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._sync_proxy(request, kwargs.get("stream", False))
+
+            res = request()
+
+            return res
+
+        def _sync_put(self, url, data=None, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("put", data=data, **kwargs)
+
+            def request() -> requests.Response:
+                return requests.put(url, data=data, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._sync_proxy(request, kwargs.get("stream", False))
+
+            res = request()
+
+            return res
+
+        def _sync_patch(self, url, data=None, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("patch", data=data, **kwargs)
+
+            def request() -> requests.Response:
+                return requests.patch(url, data=data, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._sync_proxy(request, kwargs.get("stream", False))
+
+            res = request()
+
+            return res
+
+        def _sync_delete(self, url, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("delete", **kwargs)
+
+            def request() -> requests.Response:
+                return requests.delete(url, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._sync_proxy(request, kwargs.get("stream", False))
+
+            res = request()
+
+            return res
+
+        def _sync_request(self, method, url, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate(method, **kwargs)
+
+            def request() -> requests.Response:
+                return requests.request(method, url, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._sync_proxy(request, kwargs.get("stream", False))
+
+            res = request()
+
+            return res
+```
+
+#### `AsyncService` example
+
+Implementing `aiohttp` library.
+
+```py
+if LIBRARIES["aiohttp"]:
+
+    class AsyncService:
+
+        async def __aenter__(self) -> "Service":
+
+            self.sync = False
+
+            if isinstance(self.app_pk, self._get_app_cls()):
+                self.app = self.app_pk
+
+            else:
+                self.app = await sync_to_async(self._get_app)(self.app_pk)
+
+            self.session = aiohttp.ClientSession()
+
+            # this should be extended
+            await self.session.__aenter__()
+
+            return self
+
+        async def __aexit__(self, *args, **kwargs) -> None:
+            for obj in self.to_close:
+                await obj.__aexit__(*args, **kwargs)
+
+            await self.session.__aexit__(*args, **kwargs)
+
+        # django does not support StreamingHttpResponse with aiohttp due to django would have to close the response
+        async def _async_proxy(self, response: Coroutine[Any, Any, ClientResponse]) -> HttpResponse:
+            try:
+                r = await response
+
+            except Exception as e:
+                raise ValidationException("Unexpected error: " + str(e), code=500, slug="unexpected-error")
+
+            header_keys = [x for x in r.headers.keys() if x not in self.banned_keys]
+
+            headers = {}
+            for header in header_keys:
+                headers[str(header)] = r.headers[header]
+
+            return HttpResponse(await r.content.read(), status=r.status, headers=headers)
+
+        def _async_get(self, url, params=None, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("get", params=params, **kwargs)
+
+            obj = self.session.get(url, params=params, **kwargs, headers=headers)
+            self.to_close.append(obj)
+
+            res = obj.__aenter__()
+
+            # wraps client response to be used within django views
+            if self.proxy:
+                return self._async_proxy(res)
+
+            return res
+
+        def _async_options(self, url, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("options", **kwargs)
+
+            obj = self.session.options(url, **kwargs, headers=headers)
+            self.to_close.append(obj)
+
+            res = obj.__aenter__()
+
+            # wraps client response to be used within django views
+            if self.proxy:
+                return self._async_proxy(res)
+
+            return res
+
+        def _async_head(self, url, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("head", **kwargs)
+
+            obj = self.session.head(url, **kwargs, headers=headers)
+            self.to_close.append(obj)
+
+            res = obj.__aenter__()
+
+            # wraps client response to be used within django views
+            if self.proxy:
+                return self._async_proxy(res)
+
+            return res
+
+        def _async_post(self, url, data=None, json=None, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("post", data=data, json=json, **kwargs)
+
+            obj = self.session.post(url, data=data, json=json, **kwargs, headers=headers)
+            self.to_close.append(obj)
+
+            res = obj.__aenter__()
+
+            # wraps client response to be used within django views
+            if self.proxy:
+                return self._async_proxy(res)
+
+            return res
+
+        def _async_webhook(self, url, data=None, json=None, **kwargs):
+            url = self.app.webhook_url
+            headers = self._authenticate("post", data=data, json=json, **kwargs)
+
+            obj = self.session.post(url, data=data, json=json, **kwargs, headers=headers)
+            self.to_close.append(obj)
+
+            res = obj.__aenter__()
+
+            # wraps client response to be used within django views
+            if self.proxy:
+                return self._async_proxy(res)
+
+            return res
+
+        def _async_put(self, url, data=None, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("put", data=data, **kwargs)
+
+            obj = self.session.put(url, data=data, **kwargs, headers=headers)
+            self.to_close.append(obj)
+
+            res = obj.__aenter__()
+
+            # wraps client response to be used within django views
+            if self.proxy:
+                return self._async_proxy(res)
+
+            return res
+
+        def _async_patch(self, url, data=None, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("patch", data=data, **kwargs)
+
+            obj = self.session.patch(url, data=data, **kwargs, headers=headers)
+            self.to_close.append(obj)
+
+            res = obj.__aenter__()
+
+            # wraps client response to be used within django views
+            if self.proxy:
+                return self._async_proxy(res)
+
+            return res
+
+        def _async_delete(self, url, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("delete", **kwargs)
+
+            obj = self.session.delete(url, **kwargs, headers=headers)
+            self.to_close.append(obj)
+
+            res = obj.__aenter__()
+
+            # wraps client response to be used within django views
+            if self.proxy:
+                return self._async_proxy(res)
+
+            return res
+
+        def _async_request(self, method, url, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate(method, **kwargs)
+
+            obj = self.session.request(method, url, **kwargs, headers=headers)
+            self.to_close.append(obj)
+
+            res = obj.__aenter__()
+
+            # wraps client response to be used within django views
+            if self.proxy:
+                return self._async_proxy(res)
+
+            return res
+```
```

### Comparing `linked_services-1.2.1/docs/extending-service/rest-frameworks.md` & `linked_services-1.2.2/docs/extending-service/rest-frameworks.md`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-# Rest frameworks
-
-You could implement a new REST framework extending `linked_services.core.service.Service`.
-
-## Methods
-
-- `__enter__`: called when it gets entered into an sync context.
-- `__aenter__`: called when it gets entered into an async context.
-- `_get_app_cls`: called when it needs to retrieve the application model class.
-- `_get_app`: called when it needs to retrieve an application instance.
-- `_get_signature`: called when it needs to retrieve a signature.
-- `_get_jwt`: called when it needs to retrieve a JWT.
-
-## Example
-
-Implementing `djangorestframework`.
-
-```py
-from typing import Any, Optional, Type
-
-from django.core.exceptions import SynchronousOnlyOperation
-
-from linked_services.core.exceptions import ValidationException
-from linked_services.core.service import AppNotFound
-from linked_services.core.service import Service as BaseService
-from linked_services.django.actions import get_app
-from linked_services.django.models import App
-
-has_sync = hasattr(BaseService, "__enter__")
-has_async = hasattr(BaseService, "__aenter__")
-
-
-class Service(BaseService):
-    if has_sync:
-
-        def __enter__(self) -> "Service":
-            try:
-                return super().__enter__()
-
-            except Exception:
-                if self.proxy:
-                    raise ValidationException(f"App {self.app_pk} not found", code=404, slug="app-not-found")
-
-                raise AppNotFound(f"App {self.app_pk} not found")
-
-    if has_async:
-
-        async def __aenter__(self) -> "Service":
-
-            try:
-                return await super().__aenter__()
-
-            except SynchronousOnlyOperation:
-                raise ValidationException(
-                    "Async is not supported by the worker",
-                    code=500,
-                    slug="no-async-support",
-                )
-
-            except Exception:
-                if self.proxy:
-                    raise ValidationException(f"App {self.app_pk} not found", code=404, slug="app-not-found")
-
-                raise AppNotFound(f"App {self.app_pk} not found")
-
-    def _get_app_cls(self) -> Type[App]:
-        return App
-
-    def _get_app(self, pk: str | int) -> App:
-        return get_app(pk)
-
-    def _get_signature(
-        self,
-        app: Any,
-        user_id: Optional[int] = None,
-        *,
-        method: str = "get",
-        params: Optional[dict] = None,
-        body: Optional[dict] = None,
-        headers: Optional[dict] = None,
-        reverse: bool = False,
-    ) -> tuple[str, str]:
-        from .actions import get_signature
-
-        return get_signature(app, user_id, method=method, params=params, body=body, headers=headers, reverse=reverse)
-
-    def _get_jwt(self, app: Any, user_id: Optional[int] = None, reverse: bool = False) -> str:
-        from .actions import get_jwt
-
-        return get_jwt(app, user_id, reverse=reverse)
-
-```
+# Rest frameworks
+
+You could implement a new REST framework extending `linked_services.core.service.Service`.
+
+## Methods
+
+- `__enter__`: called when it gets entered into an sync context.
+- `__aenter__`: called when it gets entered into an async context.
+- `_get_app_cls`: called when it needs to retrieve the application model class.
+- `_get_app`: called when it needs to retrieve an application instance.
+- `_get_signature`: called when it needs to retrieve a signature.
+- `_get_jwt`: called when it needs to retrieve a JWT.
+
+## Example
+
+Implementing `djangorestframework`.
+
+```py
+from typing import Any, Optional, Type
+
+from django.core.exceptions import SynchronousOnlyOperation
+
+from linked_services.core.exceptions import ValidationException
+from linked_services.core.service import AppNotFound
+from linked_services.core.service import Service as BaseService
+from linked_services.django.actions import get_app
+from linked_services.django.models import App
+
+has_sync = hasattr(BaseService, "__enter__")
+has_async = hasattr(BaseService, "__aenter__")
+
+
+class Service(BaseService):
+    if has_sync:
+
+        def __enter__(self) -> "Service":
+            try:
+                return super().__enter__()
+
+            except Exception:
+                if self.proxy:
+                    raise ValidationException(f"App {self.app_pk} not found", code=404, slug="app-not-found")
+
+                raise AppNotFound(f"App {self.app_pk} not found")
+
+    if has_async:
+
+        async def __aenter__(self) -> "Service":
+
+            try:
+                return await super().__aenter__()
+
+            except SynchronousOnlyOperation:
+                raise ValidationException(
+                    "Async is not supported by the worker",
+                    code=500,
+                    slug="no-async-support",
+                )
+
+            except Exception:
+                if self.proxy:
+                    raise ValidationException(f"App {self.app_pk} not found", code=404, slug="app-not-found")
+
+                raise AppNotFound(f"App {self.app_pk} not found")
+
+    def _get_app_cls(self) -> Type[App]:
+        return App
+
+    def _get_app(self, pk: str | int) -> App:
+        return get_app(pk)
+
+    def _get_signature(
+        self,
+        app: Any,
+        user_id: Optional[int] = None,
+        *,
+        method: str = "get",
+        params: Optional[dict] = None,
+        body: Optional[dict] = None,
+        headers: Optional[dict] = None,
+        reverse: bool = False,
+    ) -> tuple[str, str]:
+        from .actions import get_signature
+
+        return get_signature(app, user_id, method=method, params=params, body=body, headers=headers, reverse=reverse)
+
+    def _get_jwt(self, app: Any, user_id: Optional[int] = None, reverse: bool = False) -> str:
+        from .actions import get_jwt
+
+        return get_jwt(app, user_id, reverse=reverse)
+
+```
```

### Comparing `linked_services-1.2.1/docs/getting-started/scopes.md` & `linked_services-1.2.2/docs/getting-started/scopes.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-# Scopes
-
-`scope` and `ascope` checks automatically the auth headers provided by its pairwise. It will check if the application that made the request has those required scopes to execute the request. All applications that does not requires an agreement will be treated as if these has all availabled scopes to execute the request.
-
-## Decorators
-
-- `scope`: synchronous implementation that manages the authentication and it will checks the scopes if the current application requires an agreement.
-- `ascope`: asynchronous implementation that manages the authentication and it will checks the scopes if the current application requires an agreement.
-
-## Parameters
-
-- scopes: list of scopes.
-- mode: use an alternative option to sign the request. Default is `JWT`.
-
-## Name convention
-
-I would recommend your that you would use the following naming convention, `action_name:data_name` like `read:repo` or `data_name` like `repo`.
-
-## Get a user
-
-`scope` and `ascope` inject a function called `get_user`, it's a synchronous implementation in `scope` and an asynchronous implementation in `ascope`. `get_user` returns a user object or none if does not exist an user in this app and in the related application.
-
-## Examples
-
-### Sync
-
-You could want to use `scope` and `ascope` within a synchronous context if your framework does not support asynchronous operations.
-
-```py
-from rest_framework.views import APIView
-from rest_framework.response import Response
-
-from .serializers import AppUserSerializer
-
-class AppUserView(APIView):
-    permission_classes = [AllowAny]
-
-    @scope(['read:user'])
-    # action:data
-    def get(self, request, app: dict, token: dict, user_id=None):
-        # With the decorator I can access to the app and the token
-        extra = {}
-        if app.require_an_agreement:
-            extra['appuseragreement__app__id'] = app.id
-
-        if token.sub:
-            user = request.get_user()
-            extra['id'] = user.id
-
-        if user_id:
-            if 'id' in extra and extra['id'] != user_id:
-                raise ValidationException('This user does not have access to this resource',
-                                          code=403,
-                                          slug='user-with-no-access',
-                                          silent=True)
-
-            if 'id' not in extra:
-                extra['id'] = user_id
-
-            user = User.objects.filter(**extra).first()
-            if not user:
-                raise ValidationException('User not found',
-                                          code=404,
-                                          slug='user-not-found',
-                                          silent=True)
-
-            serializer = AppUserSerializer(user, many=False)
-            return Response(serializer.data)
-
-        # test this path
-        items = User.objects.filter(**extra)
-        serializer = AppUserSerializer(items, many=True)
-
-        return Response(serializer.data)
-```
-
-### Async
-
-This is the most convenient option if you are using some ASGI server.
-
-```py
-import asyncio
-
-from adrf.decorators import api_view
-from rest_framework.decorators import permission_classes
-from rest_framework.permissions import AllowAny
-from rest_framework.response import Response
-from linked_services.django.actions import aget_app
-from linked_services.django.models import FirstPartyWebhookLog
-from linked_services.rest_framework.decorators import ascope
-
-
-@api_view(["POST"])
-@permission_classes([AllowAny])
-@ascope(["webhook"], mode="jwt")
-async def app_webhook(request, app: dict, token: dict):
-
-    async def process_webhook(data):
-        nonlocal app, token
-
-        app = await aget_app(app.id)
-        external_id = data.get("id", None)
-        kwargs = {
-            "app": app,
-            "user_id": token.sub,
-            "external_id": external_id,
-            "type": data.get("type", "unknown"),
-        }
-        if external_id:
-            x, created = await FirstPartyWebhookLog.objects.aget_or_create(
-                **kwargs, defaults={"data": data.get("data", None)}
-            )
-            if not created:
-                x.data = data.get("data", None)
-                await x.asave()
-
-        else:
-            kwargs["data"] = data.get("data", None)
-            await FirstPartyWebhookLog.objects.acreate(**kwargs)
-
-    data = request.data if isinstance(request.data, list) else [request.data]
-
-    to_process = []
-
-    for x in data:
-        p = process_webhook(x)
-        to_process.append(p)
-
-    await asyncio.gather(*to_process)
-
-    return Response(None, status=status.HTTP_204_NO_CONTENT)
-```
+# Scopes
+
+`scope` and `ascope` checks automatically the auth headers provided by its pairwise. It will check if the application that made the request has those required scopes to execute the request. All applications that does not requires an agreement will be treated as if these has all availabled scopes to execute the request.
+
+## Decorators
+
+- `scope`: synchronous implementation that manages the authentication and it will checks the scopes if the current application requires an agreement.
+- `ascope`: asynchronous implementation that manages the authentication and it will checks the scopes if the current application requires an agreement.
+
+## Parameters
+
+- scopes: list of scopes.
+- mode: use an alternative option to sign the request. Default is `JWT`.
+
+## Name convention
+
+I would recommend your that you would use the following naming convention, `action_name:data_name` like `read:repo` or `data_name` like `repo`.
+
+## Get a user
+
+`scope` and `ascope` inject a function called `get_user`, it's a synchronous implementation in `scope` and an asynchronous implementation in `ascope`. `get_user` returns a user object or none if does not exist an user in this app and in the related application.
+
+## Examples
+
+### Sync
+
+You could want to use `scope` and `ascope` within a synchronous context if your framework does not support asynchronous operations.
+
+```py
+from rest_framework.views import APIView
+from rest_framework.response import Response
+
+from .serializers import AppUserSerializer
+
+class AppUserView(APIView):
+    permission_classes = [AllowAny]
+
+    @scope(['read:user'])
+    # action:data
+    def get(self, request, app: dict, token: dict, user_id=None):
+        # With the decorator I can access to the app and the token
+        extra = {}
+        if app.require_an_agreement:
+            extra['appuseragreement__app__id'] = app.id
+
+        if token.sub:
+            user = request.get_user()
+            extra['id'] = user.id
+
+        if user_id:
+            if 'id' in extra and extra['id'] != user_id:
+                raise ValidationException('This user does not have access to this resource',
+                                          code=403,
+                                          slug='user-with-no-access',
+                                          silent=True)
+
+            if 'id' not in extra:
+                extra['id'] = user_id
+
+            user = User.objects.filter(**extra).first()
+            if not user:
+                raise ValidationException('User not found',
+                                          code=404,
+                                          slug='user-not-found',
+                                          silent=True)
+
+            serializer = AppUserSerializer(user, many=False)
+            return Response(serializer.data)
+
+        # test this path
+        items = User.objects.filter(**extra)
+        serializer = AppUserSerializer(items, many=True)
+
+        return Response(serializer.data)
+```
+
+### Async
+
+This is the most convenient option if you are using some ASGI server.
+
+```py
+import asyncio
+
+from adrf.decorators import api_view
+from rest_framework.decorators import permission_classes
+from rest_framework.permissions import AllowAny
+from rest_framework.response import Response
+from linked_services.django.actions import aget_app
+from linked_services.django.models import FirstPartyWebhookLog
+from linked_services.rest_framework.decorators import ascope
+
+
+@api_view(["POST"])
+@permission_classes([AllowAny])
+@ascope(["webhook"], mode="jwt")
+async def app_webhook(request, app: dict, token: dict):
+
+    async def process_webhook(data):
+        nonlocal app, token
+
+        app = await aget_app(app.id)
+        external_id = data.get("id", None)
+        kwargs = {
+            "app": app,
+            "user_id": token.sub,
+            "external_id": external_id,
+            "type": data.get("type", "unknown"),
+        }
+        if external_id:
+            x, created = await FirstPartyWebhookLog.objects.aget_or_create(
+                **kwargs, defaults={"data": data.get("data", None)}
+            )
+            if not created:
+                x.data = data.get("data", None)
+                await x.asave()
+
+        else:
+            kwargs["data"] = data.get("data", None)
+            await FirstPartyWebhookLog.objects.acreate(**kwargs)
+
+    data = request.data if isinstance(request.data, list) else [request.data]
+
+    to_process = []
+
+    for x in data:
+        p = process_webhook(x)
+        to_process.append(p)
+
+    await asyncio.gather(*to_process)
+
+    return Response(None, status=status.HTTP_204_NO_CONTENT)
+```
```

### Comparing `linked_services-1.2.1/docs/getting-started/views.md` & `linked_services-1.2.2/docs/getting-started/views.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-# Views
-
-Linked services implemented `authorize_view` and `app_webhook` endpoint handlers to share the implementation between all services.
-
-## `app_webhook`
-
-It's a webhook endpoint that saves them to be processed by `first_party_webhooks` command.
-
-## `authorize_view`
-
-It's a function that return an endpoint handler.
-
-### Arguments
-
-- `login_url`: the login url. Default to `os.getenv("LOGIN_URL")`
-- `app_url`: the app url. Default to `os.getenv("APP_URL")`
-- `get_language`: a function that receives a request and returns the user language. Default to `lambda request: 'en'`
-
-## Example
-
-```py
-from django.urls import path
-from linked_services.rest_framework.views import app_webhook, authorize_view
-
-from breathecode.authenticate.actions import get_user_language
-
-
-app_name = 'authenticate'
-urlpatterns = [
-    # authorize
-    path('authorize/<str:app_slug>',
-         authorize_view(login_url='/v1/auth/view/login', get_language=get_user_language),
-         name='authorize_slug'),
-
-    path('app/webhook', app_webhook, name='app_webhook'),
-]
-```
+# Views
+
+Linked services implemented `authorize_view` and `app_webhook` endpoint handlers to share the implementation between all services.
+
+## `app_webhook`
+
+It's a webhook endpoint that saves them to be processed by `first_party_webhooks` command.
+
+## `authorize_view`
+
+It's a function that return an endpoint handler.
+
+### Arguments
+
+- `login_url`: the login url. Default to `os.getenv("LOGIN_URL")`
+- `app_url`: the app url. Default to `os.getenv("APP_URL")`
+- `get_language`: a function that receives a request and returns the user language. Default to `lambda request: 'en'`
+
+## Example
+
+```py
+from django.urls import path
+from linked_services.rest_framework.views import app_webhook, authorize_view
+
+from breathecode.authenticate.actions import get_user_language
+
+
+app_name = 'authenticate'
+urlpatterns = [
+    # authorize
+    path('authorize/<str:app_slug>',
+         authorize_view(login_url='/v1/auth/view/login', get_language=get_user_language),
+         name='authorize_slug'),
+
+    path('app/webhook', app_webhook, name='app_webhook'),
+]
+```
```

### Comparing `linked_services-1.2.1/src/manage.py` & `linked_services-1.2.2/src/manage.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-#!/usr/bin/env python
-"""Django's command-line utility for administrative tasks."""
-import os
-import sys
-
-
-def main():
-    os.environ.setdefault("DJANGO_SETTINGS_MODULE", "linked_services.settings")
-    # os.environ.setdefault("DJANGO_SETTINGS_MODULE", "task_manager.task_manager.settings")
-    try:
-        from django.core.management import execute_from_command_line
-    except ImportError as exc:
-        raise ImportError(
-            "Couldn't import Django. Are you sure it's installed and "
-            "available on your PYTHONPATH environment variable? Did you "
-            "forget to activate a virtual environment?"
-        ) from exc
-    execute_from_command_line(sys.argv)
-
-
-if __name__ == "__main__":
-    main()
+#!/usr/bin/env python
+"""Django's command-line utility for administrative tasks."""
+import os
+import sys
+
+
+def main():
+    os.environ.setdefault("DJANGO_SETTINGS_MODULE", "linked_services.settings")
+    # os.environ.setdefault("DJANGO_SETTINGS_MODULE", "task_manager.task_manager.settings")
+    try:
+        from django.core.management import execute_from_command_line
+    except ImportError as exc:
+        raise ImportError(
+            "Couldn't import Django. Are you sure it's installed and "
+            "available on your PYTHONPATH environment variable? Did you "
+            "forget to activate a virtual environment?"
+        ) from exc
+    execute_from_command_line(sys.argv)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `linked_services-1.2.1/src/linked_services/core/decorators.py` & `linked_services-1.2.2/src/linked_services/core/decorators.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,389 +1,389 @@
-import datetime as dt
-import functools
-import hashlib
-import hmac
-import logging
-import urllib.parse
-import uuid
-from datetime import datetime, timedelta
-from typing import Any, Callable, Coroutine, Optional, TypedDict
-
-import jwt
-from asgiref.sync import sync_to_async
-from django.http import HttpRequest
-from django.utils import timezone
-from rest_framework.views import APIView
-
-from linked_services.core.settings import get_setting
-from linked_services.core.utils import AttrDict
-
-from .exceptions import ProgrammingError, ValidationException
-
-__all__ = ["get_handlers", "get_decorators"]
-
-logger = logging.getLogger(__name__)
-
-
-def get_payload(app, date, signed_headers, request: HttpRequest):
-    headers = dict(request.headers)
-    headers.pop("Authorization", None)
-    payload = {
-        "timestamp": date,
-        "app": app,
-        "method": request.method,
-        "params": dict(request.GET),
-        "body": request.data if request.data is not None else None,
-        "headers": {k: v for k, v in headers.items() if k in signed_headers},
-    }
-
-    return payload
-
-
-def hmac_signature(app, date, signed_headers, request, key, fn):
-    payload = get_payload(app, date, signed_headers, request)
-
-    paybytes = urllib.parse.urlencode(payload).encode("utf8")
-
-    return hmac.new(key, paybytes, fn).hexdigest()
-
-
-TOLERANCE = 2
-
-
-Info = tuple[Any, str, str, str, bool, list[str], list[str], str, str, str]
-Key = tuple[bytes, bytes]
-
-GetUserScopesFn = Callable[[str, int], tuple[list[str], list[str]]]
-GetAppKeysFn = Callable[[str], tuple[Info, Key, Optional[Key]]]
-GetUserFn = Callable[[int | str | uuid.UUID, int | str | uuid.UUID], Any | None]
-AGetUserFn = Callable[[int | str | uuid.UUID, int | str | uuid.UUID], Coroutine[Any | None, None, None]]
-
-
-class Token(TypedDict):
-    sub: Optional[Any]
-    iss: str
-    app: str
-    aud: str
-    exp: int
-    iat: int
-    typ: str
-
-
-class App(TypedDict):
-    id: Any
-    private_key: bytes
-    public_key: bytes
-    algorithm: str
-    strategy: str
-    schema: str
-    require_an_agreement: bool
-    webhook_url: str
-    redirect_url: str
-    app_url: str
-
-
-LinkSchemaFn = Callable[[HttpRequest, list[str], str, bool], tuple[App, Token]]
-SignatureSchemaFn = Callable[[HttpRequest, list[str], str, bool], App]
-
-
-def get_handlers(get_app_keys: GetAppKeysFn, get_user_scopes: GetUserScopesFn) -> tuple[
-    LinkSchemaFn,
-    SignatureSchemaFn,
-]:
-
-    # required_scopes is really a tuple of n strings
-    def link_schema(request: HttpRequest, required_scopes: list[str], authorization: str, use_signature: bool):
-        """Authenticate the request and return a two-tuple of (user, token)."""
-
-        try:
-            authorization = dict([x.split("=") for x in authorization.split(",")])
-
-        except Exception:
-            raise ValidationException("Unauthorized", code=401, slug="authorization-header-malformed")
-
-        if sorted(authorization.keys()) != ["App", "Token"]:
-            raise ValidationException("Unauthorized", code=401, slug="authorization-header-bad-schema")
-
-        info, key, legacy_key = get_app_keys(authorization["App"])
-        (
-            app_id,
-            alg,
-            strategy,
-            schema,
-            require_an_agreement,
-            required_app_scopes,
-            optional_app_scopes,
-            webhook_url,
-            redirect_url,
-            app_url,
-        ) = info
-        public_key, private_key = key
-
-        if schema != "LINK":
-            raise ValidationException("Unauthorized", code=401, slug="authorization-header-forbidden-schema")
-
-        if strategy != "JWT":
-            raise ValidationException("Unauthorized", code=401, slug="authorization-header-forbidden-strategy")
-
-        try:
-            key = public_key if public_key else private_key
-            whoamy = get_setting("app_name")
-            payload = jwt.decode(authorization["Token"], key, algorithms=[alg], audience=whoamy)
-
-        except Exception:
-            if not legacy_key:
-                raise ValidationException("Unauthorized", code=401, slug="wrong-app-token")
-
-        if not payload:
-            try:
-                legacy_public_key, legacy_private_key = legacy_key
-
-                key = legacy_public_key if legacy_public_key else legacy_private_key
-                payload = jwt.decode(authorization["Token"], key, algorithms=[alg])
-
-            except Exception:
-                raise ValidationException("Unauthorized", code=401, slug="wrong-legacy-app-token")
-
-        if payload["sub"] and require_an_agreement:
-            required_app_scopes, optional_app_scopes = get_user_scopes(authorization["App"], payload["sub"])
-            all_scopes = required_app_scopes + optional_app_scopes
-
-            for s in required_scopes:
-                if s not in all_scopes:
-                    raise ValidationException("Unauthorized", code=401, slug="forbidden-scope")
-
-        if "exp" not in payload or payload["exp"] < timezone.now().timestamp():
-            raise ValidationException("Expired token", code=401, slug="expired")
-
-        app = {
-            "id": app_id,
-            "private_key": private_key,
-            "public_key": public_key,
-            "algorithm": alg,
-            "strategy": strategy,
-            "schema": schema,
-            "require_an_agreement": require_an_agreement,
-            "webhook_url": webhook_url,
-            "redirect_url": redirect_url,
-            "app_url": app_url,
-        }
-
-        return app, payload
-
-    # required_scopes is really a tuple of n strings
-    def signature_schema(request: HttpRequest, required_scopes: list[str], authorization: str, use_signature: bool):
-        """Authenticate the request and return a two-tuple of (user, token)."""
-
-        try:
-            authorization = dict([x.split("=") for x in authorization.split(",")])
-
-        except Exception:
-            raise ValidationException("Unauthorized", code=401, slug="authorization-header-malformed")
-
-        if sorted(authorization.keys()) != ["App", "Date", "Nonce", "SignedHeaders"]:
-            raise ValidationException("Unauthorized", code=401, slug="authorization-header-bad-schema")
-
-        info, key, legacy_key = get_app_keys(authorization["App"])
-        (
-            app_id,
-            alg,
-            strategy,
-            schema,
-            require_an_agreement,
-            required_app_scopes,
-            optional_app_scopes,
-            webhook_url,
-            redirect_url,
-            app_url,
-        ) = info
-        public_key, private_key = key
-
-        if require_an_agreement:
-            required_app_scopes, optional_app_scopes = get_user_scopes(authorization["App"])
-            all_scopes = required_app_scopes + optional_app_scopes
-
-            for s in required_scopes:
-                if s not in all_scopes:
-                    raise ValidationException("Unauthorized", code=401, slug="forbidden-scope")
-
-        if schema != "LINK":
-            raise ValidationException("Unauthorized", code=401, slug="authorization-header-forbidden-schema")
-
-        if strategy != "SIGNATURE" and not use_signature:
-            raise ValidationException("Unauthorized", code=401, slug="authorization-header-forbidden-strategy")
-
-        if alg not in ["HS256", "HS512"]:
-            raise ValidationException("Algorithm not implemented", code=401, slug="algorithm-not-implemented")
-
-        fn = hashlib.sha256 if alg == "HS256" else hashlib.sha512
-
-        key = public_key if public_key else private_key
-        if (
-            hmac_signature(
-                authorization["App"], authorization["Date"], authorization["SignedHeaders"], request, key, fn
-            )
-            != authorization["Nonce"]
-            and not legacy_key
-        ):
-            if not legacy_key:
-                raise ValidationException("Unauthorized", code=401, slug="wrong-app-token")
-
-        if legacy_key:
-            legacy_public_key, legacy_private_key = legacy_key
-            key = legacy_public_key if legacy_public_key else legacy_private_key
-            if (
-                hmac_signature(
-                    authorization["App"], authorization["Date"], authorization["SignedHeaders"], request, key, fn
-                )
-                != authorization["Nonce"]
-            ):
-                raise ValidationException("Unauthorized", code=401, slug="wrong-legacy-app-token")
-
-        try:
-            date = datetime.fromisoformat(authorization["Date"])
-            date = date.replace(tzinfo=dt.timezone.utc)
-            now = timezone.now()
-            if (now - timedelta(minutes=TOLERANCE) > date) or (now + timedelta(minutes=TOLERANCE) < date):
-                raise Exception()
-
-        except Exception:
-            raise ValidationException("Unauthorized", code=401, slug="bad-timestamp")
-
-        app = {
-            "id": app_id,
-            "private_key": private_key,
-            "public_key": public_key,
-            "algorithm": alg,
-            "strategy": strategy,
-            "schema": schema,
-            "require_an_agreement": require_an_agreement,
-            "webhook_url": webhook_url,
-            "redirect_url": redirect_url,
-            "app_url": app_url,
-        }
-
-        return app
-
-    return link_schema, signature_schema
-
-
-def get_decorators(
-    link_schema: LinkSchemaFn, signature_schema: SignatureSchemaFn, get_user: GetUserFn, aget_user: AGetUserFn
-) -> tuple[Callable, Callable]:
-    def scope(scopes: Optional[list] = None, mode: Optional[str] = None) -> callable:
-        """Check if the app has access to the scope provided."""
-
-        if scopes is None:
-            scopes = []
-
-        def decorator(function: callable) -> callable:
-
-            @functools.wraps(function)
-            def wrapper(*args, **kwargs):
-                request: HttpRequest
-
-                if isinstance(scopes, list) is False:
-                    raise ProgrammingError("Permission must be a list")
-
-                if len([x for x in scopes if not isinstance(x, str)]):
-                    raise ProgrammingError("Permission must be a list of strings")
-
-                try:
-                    if hasattr(args[0], "__class__") and isinstance(args[0], APIView):
-                        request = args[1]
-
-                    elif hasattr(args[0], "user"):
-                        request = args[0]
-
-                    else:
-                        raise IndexError()
-
-                except IndexError:
-                    raise ProgrammingError("Missing request information, use this decorator with DRF View")
-
-                authorization = request.headers.get("Authorization", "")
-                if not authorization:
-                    raise ValidationException("Unauthorized", code=401, slug="no-authorization-header")
-
-                if authorization.startswith("Link ") and mode != "signature":
-                    authorization = authorization.replace("Link ", "")
-                    app, token = link_schema(request, scopes, authorization, mode == "signature")
-
-                    cu = functools.partial(get_user, token["app"], token["sub"])
-                    setattr(request, "get_user", cu)
-
-                    return function(*args, **kwargs, token=AttrDict(**token), app=AttrDict(**app))
-
-                elif authorization.startswith("Signature ") and mode != "jwt":
-                    authorization = authorization.replace("Signature ", "")
-                    app = signature_schema(request, scopes, authorization, mode == "signature")
-                    return function(*args, **kwargs, app=AttrDict(**app))
-
-                else:
-                    raise ValidationException(
-                        "Unknown auth schema or this schema is forbidden", code=401, slug="unknown-auth-schema"
-                    )
-
-            return wrapper
-
-        return decorator
-
-    def ascope(scopes: Optional[list] = None, mode: Optional[str] = None) -> callable:
-        """Check if the app has access to the scope provided."""
-
-        if scopes is None:
-            scopes = []
-
-        def decorator(function: callable) -> callable:
-
-            @functools.wraps(function)
-            async def wrapper(*args, **kwargs):
-                request: HttpRequest
-
-                if isinstance(scopes, list) is False:
-                    raise ProgrammingError("Permission must be a list")
-
-                if len([x for x in scopes if not isinstance(x, str)]):
-                    raise ProgrammingError("Permission must be a list of strings")
-
-                try:
-                    if hasattr(args[0], "__class__") and isinstance(args[0], APIView):
-                        request = args[1]
-
-                    elif hasattr(args[0], "user"):
-                        request = args[0]
-
-                    else:
-                        raise IndexError()
-
-                except IndexError:
-                    raise ProgrammingError("Missing request information, use this decorator with DRF View")
-
-                authorization = request.headers.get("Authorization", "")
-                if not authorization:
-                    raise ValidationException("Unauthorized", code=401, slug="no-authorization-header")
-
-                if authorization.startswith("Link ") and mode != "signature":
-                    authorization = authorization.replace("Link ", "")
-                    app, token = await sync_to_async(link_schema)(request, scopes, authorization, mode == "signature")
-
-                    cu = functools.partial(get_user, token["app"], token["sub"])
-                    setattr(request, "aget_user", cu)
-
-                    return await function(*args, **kwargs, token=AttrDict(**token), app=AttrDict(**app))
-
-                elif authorization.startswith("Signature ") and mode != "jwt":
-                    authorization = authorization.replace("Signature ", "")
-                    app = await sync_to_async(signature_schema)(request, scopes, authorization, mode == "signature")
-                    return await function(*args, **kwargs, app=AttrDict(**app))
-
-                else:
-                    raise ValidationException(
-                        "Unknown auth schema or this schema is forbidden", code=401, slug="unknown-auth-schema"
-                    )
-
-            return wrapper
-
-        return decorator
-
-    return scope, ascope
+import datetime as dt
+import functools
+import hashlib
+import hmac
+import logging
+import urllib.parse
+import uuid
+from datetime import datetime, timedelta
+from typing import Any, Callable, Coroutine, Optional, TypedDict
+
+import jwt
+from asgiref.sync import sync_to_async
+from django.http import HttpRequest
+from django.utils import timezone
+from rest_framework.views import APIView
+
+from linked_services.core.settings import get_setting
+from linked_services.core.utils import AttrDict
+
+from .exceptions import ProgrammingError, ValidationException
+
+__all__ = ["get_handlers", "get_decorators"]
+
+logger = logging.getLogger(__name__)
+
+
+def get_payload(app, date, signed_headers, request: HttpRequest):
+    headers = dict(request.headers)
+    headers.pop("Authorization", None)
+    payload = {
+        "timestamp": date,
+        "app": app,
+        "method": request.method,
+        "params": dict(request.GET),
+        "body": request.data if request.data is not None else None,
+        "headers": {k: v for k, v in headers.items() if k in signed_headers},
+    }
+
+    return payload
+
+
+def hmac_signature(app, date, signed_headers, request, key, fn):
+    payload = get_payload(app, date, signed_headers, request)
+
+    paybytes = urllib.parse.urlencode(payload).encode("utf8")
+
+    return hmac.new(key, paybytes, fn).hexdigest()
+
+
+TOLERANCE = 2
+
+
+Info = tuple[Any, str, str, str, bool, list[str], list[str], str, str, str]
+Key = tuple[bytes, bytes]
+
+GetUserScopesFn = Callable[[str, int], tuple[list[str], list[str]]]
+GetAppKeysFn = Callable[[str], tuple[Info, Key, Optional[Key]]]
+GetUserFn = Callable[[int | str | uuid.UUID, int | str | uuid.UUID], Any | None]
+AGetUserFn = Callable[[int | str | uuid.UUID, int | str | uuid.UUID], Coroutine[Any | None, None, None]]
+
+
+class Token(TypedDict):
+    sub: Optional[Any]
+    iss: str
+    app: str
+    aud: str
+    exp: int
+    iat: int
+    typ: str
+
+
+class App(TypedDict):
+    id: Any
+    private_key: bytes
+    public_key: bytes
+    algorithm: str
+    strategy: str
+    schema: str
+    require_an_agreement: bool
+    webhook_url: str
+    redirect_url: str
+    app_url: str
+
+
+LinkSchemaFn = Callable[[HttpRequest, list[str], str, bool], tuple[App, Token]]
+SignatureSchemaFn = Callable[[HttpRequest, list[str], str, bool], App]
+
+
+def get_handlers(get_app_keys: GetAppKeysFn, get_user_scopes: GetUserScopesFn) -> tuple[
+    LinkSchemaFn,
+    SignatureSchemaFn,
+]:
+
+    # required_scopes is really a tuple of n strings
+    def link_schema(request: HttpRequest, required_scopes: list[str], authorization: str, use_signature: bool):
+        """Authenticate the request and return a two-tuple of (user, token)."""
+
+        try:
+            authorization = dict([x.split("=") for x in authorization.split(",")])
+
+        except Exception:
+            raise ValidationException("Unauthorized", code=401, slug="authorization-header-malformed")
+
+        if sorted(authorization.keys()) != ["App", "Token"]:
+            raise ValidationException("Unauthorized", code=401, slug="authorization-header-bad-schema")
+
+        info, key, legacy_key = get_app_keys(authorization["App"])
+        (
+            app_id,
+            alg,
+            strategy,
+            schema,
+            require_an_agreement,
+            required_app_scopes,
+            optional_app_scopes,
+            webhook_url,
+            redirect_url,
+            app_url,
+        ) = info
+        public_key, private_key = key
+
+        if schema != "LINK":
+            raise ValidationException("Unauthorized", code=401, slug="authorization-header-forbidden-schema")
+
+        if strategy != "JWT":
+            raise ValidationException("Unauthorized", code=401, slug="authorization-header-forbidden-strategy")
+
+        try:
+            key = public_key if public_key else private_key
+            whoamy = get_setting("app_name")
+            payload = jwt.decode(authorization["Token"], key, algorithms=[alg], audience=whoamy)
+
+        except Exception:
+            if not legacy_key:
+                raise ValidationException("Unauthorized", code=401, slug="wrong-app-token")
+
+        if not payload:
+            try:
+                legacy_public_key, legacy_private_key = legacy_key
+
+                key = legacy_public_key if legacy_public_key else legacy_private_key
+                payload = jwt.decode(authorization["Token"], key, algorithms=[alg])
+
+            except Exception:
+                raise ValidationException("Unauthorized", code=401, slug="wrong-legacy-app-token")
+
+        if payload["sub"] and require_an_agreement:
+            required_app_scopes, optional_app_scopes = get_user_scopes(authorization["App"], payload["sub"])
+            all_scopes = required_app_scopes + optional_app_scopes
+
+            for s in required_scopes:
+                if s not in all_scopes:
+                    raise ValidationException("Unauthorized", code=401, slug="forbidden-scope")
+
+        if "exp" not in payload or payload["exp"] < timezone.now().timestamp():
+            raise ValidationException("Expired token", code=401, slug="expired")
+
+        app = {
+            "id": app_id,
+            "private_key": private_key,
+            "public_key": public_key,
+            "algorithm": alg,
+            "strategy": strategy,
+            "schema": schema,
+            "require_an_agreement": require_an_agreement,
+            "webhook_url": webhook_url,
+            "redirect_url": redirect_url,
+            "app_url": app_url,
+        }
+
+        return app, payload
+
+    # required_scopes is really a tuple of n strings
+    def signature_schema(request: HttpRequest, required_scopes: list[str], authorization: str, use_signature: bool):
+        """Authenticate the request and return a two-tuple of (user, token)."""
+
+        try:
+            authorization = dict([x.split("=") for x in authorization.split(",")])
+
+        except Exception:
+            raise ValidationException("Unauthorized", code=401, slug="authorization-header-malformed")
+
+        if sorted(authorization.keys()) != ["App", "Date", "Nonce", "SignedHeaders"]:
+            raise ValidationException("Unauthorized", code=401, slug="authorization-header-bad-schema")
+
+        info, key, legacy_key = get_app_keys(authorization["App"])
+        (
+            app_id,
+            alg,
+            strategy,
+            schema,
+            require_an_agreement,
+            required_app_scopes,
+            optional_app_scopes,
+            webhook_url,
+            redirect_url,
+            app_url,
+        ) = info
+        public_key, private_key = key
+
+        if require_an_agreement:
+            required_app_scopes, optional_app_scopes = get_user_scopes(authorization["App"])
+            all_scopes = required_app_scopes + optional_app_scopes
+
+            for s in required_scopes:
+                if s not in all_scopes:
+                    raise ValidationException("Unauthorized", code=401, slug="forbidden-scope")
+
+        if schema != "LINK":
+            raise ValidationException("Unauthorized", code=401, slug="authorization-header-forbidden-schema")
+
+        if strategy != "SIGNATURE" and not use_signature:
+            raise ValidationException("Unauthorized", code=401, slug="authorization-header-forbidden-strategy")
+
+        if alg not in ["HS256", "HS512"]:
+            raise ValidationException("Algorithm not implemented", code=401, slug="algorithm-not-implemented")
+
+        fn = hashlib.sha256 if alg == "HS256" else hashlib.sha512
+
+        key = public_key if public_key else private_key
+        if (
+            hmac_signature(
+                authorization["App"], authorization["Date"], authorization["SignedHeaders"], request, key, fn
+            )
+            != authorization["Nonce"]
+            and not legacy_key
+        ):
+            if not legacy_key:
+                raise ValidationException("Unauthorized", code=401, slug="wrong-app-token")
+
+        if legacy_key:
+            legacy_public_key, legacy_private_key = legacy_key
+            key = legacy_public_key if legacy_public_key else legacy_private_key
+            if (
+                hmac_signature(
+                    authorization["App"], authorization["Date"], authorization["SignedHeaders"], request, key, fn
+                )
+                != authorization["Nonce"]
+            ):
+                raise ValidationException("Unauthorized", code=401, slug="wrong-legacy-app-token")
+
+        try:
+            date = datetime.fromisoformat(authorization["Date"])
+            date = date.replace(tzinfo=dt.timezone.utc)
+            now = timezone.now()
+            if (now - timedelta(minutes=TOLERANCE) > date) or (now + timedelta(minutes=TOLERANCE) < date):
+                raise Exception()
+
+        except Exception:
+            raise ValidationException("Unauthorized", code=401, slug="bad-timestamp")
+
+        app = {
+            "id": app_id,
+            "private_key": private_key,
+            "public_key": public_key,
+            "algorithm": alg,
+            "strategy": strategy,
+            "schema": schema,
+            "require_an_agreement": require_an_agreement,
+            "webhook_url": webhook_url,
+            "redirect_url": redirect_url,
+            "app_url": app_url,
+        }
+
+        return app
+
+    return link_schema, signature_schema
+
+
+def get_decorators(
+    link_schema: LinkSchemaFn, signature_schema: SignatureSchemaFn, get_user: GetUserFn, aget_user: AGetUserFn
+) -> tuple[Callable, Callable]:
+    def scope(scopes: Optional[list] = None, mode: Optional[str] = None) -> callable:
+        """Check if the app has access to the scope provided."""
+
+        if scopes is None:
+            scopes = []
+
+        def decorator(function: callable) -> callable:
+
+            @functools.wraps(function)
+            def wrapper(*args, **kwargs):
+                request: HttpRequest
+
+                if isinstance(scopes, list) is False:
+                    raise ProgrammingError("Permission must be a list")
+
+                if len([x for x in scopes if not isinstance(x, str)]):
+                    raise ProgrammingError("Permission must be a list of strings")
+
+                try:
+                    if hasattr(args[0], "__class__") and isinstance(args[0], APIView):
+                        request = args[1]
+
+                    elif hasattr(args[0], "user"):
+                        request = args[0]
+
+                    else:
+                        raise IndexError()
+
+                except IndexError:
+                    raise ProgrammingError("Missing request information, use this decorator with DRF View")
+
+                authorization = request.headers.get("Authorization", "")
+                if not authorization:
+                    raise ValidationException("Unauthorized", code=401, slug="no-authorization-header")
+
+                if authorization.startswith("Link ") and mode != "signature":
+                    authorization = authorization.replace("Link ", "")
+                    app, token = link_schema(request, scopes, authorization, mode == "signature")
+
+                    cu = functools.partial(get_user, token["app"], token["sub"])
+                    setattr(request, "get_user", cu)
+
+                    return function(*args, **kwargs, token=AttrDict(**token), app=AttrDict(**app))
+
+                elif authorization.startswith("Signature ") and mode != "jwt":
+                    authorization = authorization.replace("Signature ", "")
+                    app = signature_schema(request, scopes, authorization, mode == "signature")
+                    return function(*args, **kwargs, app=AttrDict(**app))
+
+                else:
+                    raise ValidationException(
+                        "Unknown auth schema or this schema is forbidden", code=401, slug="unknown-auth-schema"
+                    )
+
+            return wrapper
+
+        return decorator
+
+    def ascope(scopes: Optional[list] = None, mode: Optional[str] = None) -> callable:
+        """Check if the app has access to the scope provided."""
+
+        if scopes is None:
+            scopes = []
+
+        def decorator(function: callable) -> callable:
+
+            @functools.wraps(function)
+            async def wrapper(*args, **kwargs):
+                request: HttpRequest
+
+                if isinstance(scopes, list) is False:
+                    raise ProgrammingError("Permission must be a list")
+
+                if len([x for x in scopes if not isinstance(x, str)]):
+                    raise ProgrammingError("Permission must be a list of strings")
+
+                try:
+                    if hasattr(args[0], "__class__") and isinstance(args[0], APIView):
+                        request = args[1]
+
+                    elif hasattr(args[0], "user"):
+                        request = args[0]
+
+                    else:
+                        raise IndexError()
+
+                except IndexError:
+                    raise ProgrammingError("Missing request information, use this decorator with DRF View")
+
+                authorization = request.headers.get("Authorization", "")
+                if not authorization:
+                    raise ValidationException("Unauthorized", code=401, slug="no-authorization-header")
+
+                if authorization.startswith("Link ") and mode != "signature":
+                    authorization = authorization.replace("Link ", "")
+                    app, token = await sync_to_async(link_schema)(request, scopes, authorization, mode == "signature")
+
+                    cu = functools.partial(get_user, token["app"], token["sub"])
+                    setattr(request, "aget_user", cu)
+
+                    return await function(*args, **kwargs, token=AttrDict(**token), app=AttrDict(**app))
+
+                elif authorization.startswith("Signature ") and mode != "jwt":
+                    authorization = authorization.replace("Signature ", "")
+                    app = await sync_to_async(signature_schema)(request, scopes, authorization, mode == "signature")
+                    return await function(*args, **kwargs, app=AttrDict(**app))
+
+                else:
+                    raise ValidationException(
+                        "Unknown auth schema or this schema is forbidden", code=401, slug="unknown-auth-schema"
+                    )
+
+            return wrapper
+
+        return decorator
+
+    return scope, ascope
```

### Comparing `linked_services-1.2.1/src/linked_services/core/i18n.py` & `linked_services-1.2.2/src/linked_services/core/i18n.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-import logging
-import os
-from functools import cache
-from typing import Optional
-
-from .exceptions import MalformedLanguageCode
-
-__all__ = ["translation"]
-
-IS_TEST_ENV = os.getenv("ENV") == "test"
-logger = logging.getLogger(__name__)
-
-
-def get_short_code(code: str) -> str:
-    return code[:2]
-
-
-def format_and_assert_code(code: str, from_kwargs: bool = False) -> None:
-    # do not remove the assertions
-
-    is_short = len(code) == 2
-
-    # first two character only with lowercase
-    if not code[:2].islower():
-        raise MalformedLanguageCode("Lang code is not lowercase")
-
-    # last two character only with lowercase
-    if not is_short and from_kwargs and not code[3:].islower():
-        raise MalformedLanguageCode("Country code is not lowercase")
-
-    # last two character only with uppercase
-    elif not is_short and not from_kwargs and not code[2:].isupper():
-        raise MalformedLanguageCode("Country code is not uppercase")
-
-    separator = "_" if from_kwargs else "-"
-
-    # the format is en or en-US
-    if not (len(code) == 2 or (len(code) == 5 and code[2] == separator)):
-        raise MalformedLanguageCode("Code malformed")
-
-    if not from_kwargs:
-        return code.replace(separator, "_")
-
-    return code
-
-
-def format_languages(code: str) -> list:
-    """Translate the language to the local language"""
-
-    languages = set()
-
-    code.replace(" ", "")
-
-    codes = [x for x in code.split(",") if x]
-
-    for code in codes:
-        priority = 1
-        if ";q=" in code:
-            s = code.split(";q=")
-            code = s[0]
-            try:
-                priority = float(s[1])
-            except Exception:
-                raise MalformedLanguageCode(
-                    'The priority is not a float, example: "en;q=0.5"', slug="malformed-quantity-language-code"
-                )
-
-        languages.add((priority, code))
-
-    return [x[1] for x in sorted(languages, key=lambda x: (x[0], "-" in x[1], x[1]), reverse=True)]
-
-
-def try_to_translate(code, **kwargs: str) -> str | None:
-    is_short = len(code) == 2
-
-    if code.lower() in kwargs:
-        return kwargs[code.lower()]
-
-    elif not is_short and (short_code := get_short_code(code)) in kwargs:
-        return kwargs[short_code]
-
-    return None
-
-
-@cache
-def translation(code: Optional[str] = "en", slug: Optional[str] = None, **kwargs: str) -> str:
-    """Get the translation"""
-
-    if not code:
-        code = "en"
-
-    languages = [format_and_assert_code(language) for language in format_languages(code)]
-
-    # do the assertions
-    for key in kwargs:
-        format_and_assert_code(key, from_kwargs=True)
-
-    # the english if mandatory
-    if not ("en" in kwargs or "en_us" in kwargs):
-        raise MalformedLanguageCode("The english translation is mandatory")
-
-    if slug and IS_TEST_ENV:
-        return slug
-
-    for language in languages:
-        v = try_to_translate(language, **kwargs)
-
-        if v:
-            return v
-
-    if "en_us" in kwargs:
-        return kwargs["en_us"]
-
-    return kwargs["en"]
+import logging
+import os
+from functools import cache
+from typing import Optional
+
+from .exceptions import MalformedLanguageCode
+
+__all__ = ["translation"]
+
+IS_TEST_ENV = os.getenv("ENV") == "test"
+logger = logging.getLogger(__name__)
+
+
+def get_short_code(code: str) -> str:
+    return code[:2]
+
+
+def format_and_assert_code(code: str, from_kwargs: bool = False) -> None:
+    # do not remove the assertions
+
+    is_short = len(code) == 2
+
+    # first two character only with lowercase
+    if not code[:2].islower():
+        raise MalformedLanguageCode("Lang code is not lowercase")
+
+    # last two character only with lowercase
+    if not is_short and from_kwargs and not code[3:].islower():
+        raise MalformedLanguageCode("Country code is not lowercase")
+
+    # last two character only with uppercase
+    elif not is_short and not from_kwargs and not code[2:].isupper():
+        raise MalformedLanguageCode("Country code is not uppercase")
+
+    separator = "_" if from_kwargs else "-"
+
+    # the format is en or en-US
+    if not (len(code) == 2 or (len(code) == 5 and code[2] == separator)):
+        raise MalformedLanguageCode("Code malformed")
+
+    if not from_kwargs:
+        return code.replace(separator, "_")
+
+    return code
+
+
+def format_languages(code: str) -> list:
+    """Translate the language to the local language"""
+
+    languages = set()
+
+    code.replace(" ", "")
+
+    codes = [x for x in code.split(",") if x]
+
+    for code in codes:
+        priority = 1
+        if ";q=" in code:
+            s = code.split(";q=")
+            code = s[0]
+            try:
+                priority = float(s[1])
+            except Exception:
+                raise MalformedLanguageCode(
+                    'The priority is not a float, example: "en;q=0.5"', slug="malformed-quantity-language-code"
+                )
+
+        languages.add((priority, code))
+
+    return [x[1] for x in sorted(languages, key=lambda x: (x[0], "-" in x[1], x[1]), reverse=True)]
+
+
+def try_to_translate(code, **kwargs: str) -> str | None:
+    is_short = len(code) == 2
+
+    if code.lower() in kwargs:
+        return kwargs[code.lower()]
+
+    elif not is_short and (short_code := get_short_code(code)) in kwargs:
+        return kwargs[short_code]
+
+    return None
+
+
+@cache
+def translation(code: Optional[str] = "en", slug: Optional[str] = None, **kwargs: str) -> str:
+    """Get the translation"""
+
+    if not code:
+        code = "en"
+
+    languages = [format_and_assert_code(language) for language in format_languages(code)]
+
+    # do the assertions
+    for key in kwargs:
+        format_and_assert_code(key, from_kwargs=True)
+
+    # the english if mandatory
+    if not ("en" in kwargs or "en_us" in kwargs):
+        raise MalformedLanguageCode("The english translation is mandatory")
+
+    if slug and IS_TEST_ENV:
+        return slug
+
+    for language in languages:
+        v = try_to_translate(language, **kwargs)
+
+        if v:
+            return v
+
+    if "en_us" in kwargs:
+        return kwargs["en_us"]
+
+    return kwargs["en"]
```

### Comparing `linked_services-1.2.1/src/linked_services/core/service.py` & `linked_services-1.2.2/src/linked_services/core/service.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,874 +1,874 @@
-from __future__ import annotations
-
-import logging
-import os
-from types import TracebackType
-from typing import Any, Callable, Coroutine, Optional, Type
-
-import aiohttp
-from asgiref.sync import sync_to_async
-from django.http import HttpResponse, StreamingHttpResponse
-
-from linked_services.core.exceptions import ValidationException
-from linked_services.core.settings import get_setting
-
-__all__ = ["Service"]
-
-DEBUG = os.getenv("LOG_LEVEL") == "DEBUG"
-
-LIBRARIES = {
-    "requests": False,
-    "aiohttp": False,  # no implemented yet
-    "httpx": False,
-}
-
-try:
-    import requests
-
-    LIBRARIES["requests"] = True
-
-except ImportError:
-    pass
-
-try:
-    from aiohttp.client_reqrep import ClientResponse
-
-    LIBRARIES["aiohttp"] = True
-
-except ImportError:
-    pass
-
-try:
-    import httpx  # noqa: F401
-
-    LIBRARIES["httpx"] = True
-
-except ImportError:
-    pass
-
-
-class Unknown:
-    pass
-
-
-if LIBRARIES["requests"]:
-
-    class SyncService:
-
-        def __enter__(self) -> "Service":
-
-            self.sync = True
-
-            if isinstance(self.app_pk, self._get_app_cls()):
-                self.app = self.app_pk
-                return self
-
-            try:
-                self.app = self._get_app(self.app_pk)
-
-            except Exception:
-                raise AppNotFound(f"App {self.app_pk} not found")
-
-            return self
-
-        def __exit__(
-            self,
-            exc_type: Optional[Type[BaseException]],
-            exc_val: Optional[BaseException],
-            exc_tb: Optional[TracebackType],
-        ) -> None:
-            pass
-
-        def _sync_proxy(self, request: Callable[[], requests.Response], stream: bool) -> StreamingHttpResponse:
-            try:
-                response = request()
-
-            except Exception as e:
-                raise ValidationException("Unexpected error: " + str(e), code=500, slug="unexpected-error")
-
-            header_keys = [x for x in response.headers.keys() if x not in self.banned_keys]
-
-            if stream:
-                resource = StreamingHttpResponse(
-                    response.raw,
-                    status=response.status_code,
-                    reason=response.reason,
-                )
-
-                for header in header_keys:
-                    resource[header] = response.headers[header]
-
-                if DEBUG:
-                    print("Response")
-                    print("  Content: no visible due to it's a stream")
-                    print("  Headers: " + str(response.headers))
-                    print("  Status code: " + str(response.status_code))
-                    print("")
-
-                return resource
-
-            headers = {}
-
-            for header in header_keys:
-                headers[header] = response.headers[header]
-
-            if DEBUG:
-                print("Response")
-                print("  Type: Proxy")
-                print("  Content: " + response.content.decode())
-                print("  Headers: " + str(headers))
-                print("  Status code: " + str(response.status_code))
-                print("")
-
-            return HttpResponse(response.content, status=response.status_code, headers=headers)
-
-        def _sync_get(self, url, params=None, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-
-            if self.sync is False:
-                params = kwargs.pop("params", None)
-
-            headers = self._authenticate("get", params=params, **kwargs)
-
-            def request() -> requests.Response:
-                if DEBUG:
-                    print("Request")
-                    print("  Method: GET")
-                    print("  Url: " + str(url))
-                    print("")
-
-                return requests.get(url, params=params, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._sync_proxy(request, kwargs.get("stream", False))
-
-            res = request()
-
-            return res
-
-        def _sync_options(self, url, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("options", **kwargs)
-
-            def request() -> requests.Response:
-                if DEBUG:
-                    print("Request")
-                    print("  Method: OPTIONS")
-                    print("  Url: " + str(url))
-                    print("")
-
-                return requests.options(url, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._sync_proxy(request, kwargs.get("stream", False))
-
-            res = request()
-
-            return res
-
-        def _sync_head(self, url, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("head", **kwargs)
-
-            def request() -> requests.Response:
-                if DEBUG:
-                    print("Request")
-                    print("  Method: HEAD")
-                    print("  Url: " + str(url))
-                    print("")
-
-                return requests.head(url, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._sync_proxy(request, kwargs.get("stream", False))
-
-            res = request()
-
-            return res
-
-        def _sync_post(self, url, data=None, json=None, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("post", data=data, json=json, **kwargs)
-
-            def request() -> requests.Response:
-                if DEBUG:
-                    print("Request")
-                    print("  Method: POST")
-                    print("  Url: " + str(url))
-                    print("")
-
-                return requests.post(url, data=data, json=json, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._sync_proxy(request, kwargs.get("stream", False))
-
-            res = request()
-
-            return res
-
-        def _sync_webhook(self, url, data=None, json=None, **kwargs):
-            url = self.app.webhook_url
-            headers = self._authenticate("post", data=data, json=json, **kwargs)
-
-            def request() -> requests.Response:
-                if DEBUG:
-                    print("Request")
-                    print("  Type: Webhook")
-                    print("  Url: " + str(url))
-                    print("")
-
-                return requests.post(url, data=data, json=json, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._sync_proxy(request, kwargs.get("stream", False))
-
-            res = request()
-
-            return res
-
-        def _sync_put(self, url, data=None, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("put", data=data, **kwargs)
-
-            def request() -> requests.Response:
-                if DEBUG:
-                    print("Request")
-                    print("  Method: PUT")
-                    print("  Url: " + str(url))
-                    print("")
-
-                return requests.put(url, data=data, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._sync_proxy(request, kwargs.get("stream", False))
-
-            res = request()
-
-            return res
-
-        def _sync_patch(self, url, data=None, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("patch", data=data, **kwargs)
-
-            def request() -> requests.Response:
-                if DEBUG:
-                    print("Request")
-                    print("  Method: PATCH")
-                    print("  Url: " + str(url))
-                    print("")
-
-                return requests.patch(url, data=data, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._sync_proxy(request, kwargs.get("stream", False))
-
-            res = request()
-
-            return res
-
-        def _sync_delete(self, url, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("delete", **kwargs)
-
-            def request() -> requests.Response:
-                if DEBUG:
-                    print("Request")
-                    print("  Method: DELETE")
-                    print("  Url: " + str(url))
-                    print("")
-
-                return requests.delete(url, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._sync_proxy(request, kwargs.get("stream", False))
-
-            res = request()
-
-            return res
-
-        def _sync_request(self, method, url, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate(method, **kwargs)
-
-            def request() -> requests.Response:
-                if DEBUG:
-                    print("Request")
-                    print("  Method: " + str(method).upper())
-                    print("  Url: " + str(url))
-                    print("")
-
-                return requests.request(method, url, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._sync_proxy(request, kwargs.get("stream", False))
-
-            res = request()
-
-            return res
-
-else:
-
-    class SyncService:
-        pass
-
-
-if LIBRARIES["aiohttp"]:
-
-    class AsyncService:
-        to_close: list
-
-        async def __aenter__(self) -> "Service":
-
-            self.sync = False
-
-            if isinstance(self.app_pk, self._get_app_cls()):
-                self.app = self.app_pk
-
-            else:
-                self.app = await sync_to_async(self._get_app)(self.app_pk)
-
-            self.session = aiohttp.ClientSession()
-
-            # this should be extended
-            await self.session.__aenter__()
-
-            return self
-
-        async def __aexit__(self, *args, **kwargs) -> None:
-            for obj in self.to_close:
-                try:
-                    await obj.__aexit__(*args, **kwargs)
-
-                except Exception:
-                    pass
-
-            try:
-                await self.session.__aexit__(*args, **kwargs)
-
-            except Exception:
-                pass
-
-        # django does not support StreamingHttpResponse with aiohttp due to django would have to close the response
-        async def _async_proxy(self, response: Coroutine[Any, Any, ClientResponse]) -> HttpResponse:
-            try:
-                r = await response
-
-            except Exception as e:
-                raise ValidationException("Unexpected error: " + str(e), code=500, slug="unexpected-error")
-
-            header_keys = [x for x in r.headers.keys() if x not in self.banned_keys]
-
-            headers = {}
-            for header in header_keys:
-                headers[str(header)] = r.headers[header]
-
-            content = await r.content.read()
-
-            if DEBUG:
-                print("Response")
-                print("  Type: Proxy")
-                print("  Content: " + content.decode())
-                print("  Headers: " + str(headers))
-                print("  Status code: " + str(r.status))
-                print("")
-
-            return HttpResponse(content, status=r.status, headers=headers)
-
-        def _async_get(self, url, params=None, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("get", params=params, **kwargs)
-
-            obj = self.session.get(url, params=params, **kwargs, headers=headers)
-            self.to_close.append(obj)
-
-            res = obj.__aenter__()
-
-            if DEBUG:
-                print("Request")
-                print("  Method: GET")
-                print("  Url: " + str(url))
-                print("")
-
-            # wraps client response to be used within django views
-            if self.proxy:
-                return self._async_proxy(res)
-
-            return res
-
-        def _async_options(self, url, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("options", **kwargs)
-
-            obj = self.session.options(url, **kwargs, headers=headers)
-            self.to_close.append(obj)
-
-            res = obj.__aenter__()
-
-            if DEBUG:
-                print("Request")
-                print("  Method: OPTIONS")
-                print("  Url: " + str(url))
-                print("")
-
-            # wraps client response to be used within django views
-            if self.proxy:
-                return self._async_proxy(res)
-
-            return res
-
-        def _async_head(self, url, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("head", **kwargs)
-
-            obj = self.session.head(url, **kwargs, headers=headers)
-            self.to_close.append(obj)
-
-            res = obj.__aenter__()
-
-            if DEBUG:
-                print("Request")
-                print("  Method: HEAD")
-                print("  Url: " + str(url))
-                print("")
-
-            # wraps client response to be used within django views
-            if self.proxy:
-                return self._async_proxy(res)
-
-            return res
-
-        def _async_post(self, url, data=None, json=None, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("post", data=data, json=json, **kwargs)
-
-            obj = self.session.post(url, data=data, json=json, **kwargs, headers=headers)
-            self.to_close.append(obj)
-
-            res = obj.__aenter__()
-
-            if DEBUG:
-                print("Request")
-                print("  Method: POST")
-                print("  Url: " + str(url))
-                print("")
-
-            # wraps client response to be used within django views
-            if self.proxy:
-                return self._async_proxy(res)
-
-            return res
-
-        def _async_webhook(self, url, data=None, json=None, **kwargs):
-            url = self.app.webhook_url
-            headers = self._authenticate("post", data=data, json=json, **kwargs)
-
-            obj = self.session.post(url, data=data, json=json, **kwargs, headers=headers)
-            self.to_close.append(obj)
-
-            res = obj.__aenter__()
-
-            if DEBUG:
-                print("Request")
-                print("  Type: Webhook")
-                print("  Url: " + str(url))
-                print("")
-
-            # wraps client response to be used within django views
-            if self.proxy:
-                return self._async_proxy(res)
-
-            return res
-
-        def _async_put(self, url, data=None, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("put", data=data, **kwargs)
-
-            obj = self.session.put(url, data=data, **kwargs, headers=headers)
-            self.to_close.append(obj)
-
-            res = obj.__aenter__()
-
-            if DEBUG:
-                print("Request")
-                print("  Method: PUT")
-                print("  Url: " + str(url))
-                print("")
-
-            # wraps client response to be used within django views
-            if self.proxy:
-                return self._async_proxy(res)
-
-            return res
-
-        def _async_patch(self, url, data=None, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("patch", data=data, **kwargs)
-
-            obj = self.session.patch(url, data=data, **kwargs, headers=headers)
-            self.to_close.append(obj)
-
-            res = obj.__aenter__()
-
-            if DEBUG:
-                print("Request")
-                print("  Method: PATCH")
-                print("  Url: " + str(url))
-                print("")
-
-            # wraps client response to be used within django views
-            if self.proxy:
-                return self._async_proxy(res)
-
-            return res
-
-        def _async_delete(self, url, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("delete", **kwargs)
-
-            obj = self.session.delete(url, **kwargs, headers=headers)
-            self.to_close.append(obj)
-
-            res = obj.__aenter__()
-
-            if DEBUG:
-                print("Request")
-                print("  Method: DELETE")
-                print("  Url: " + str(url))
-                print("")
-
-            # wraps client response to be used within django views
-            if self.proxy:
-                return self._async_proxy(res)
-
-            return res
-
-        def _async_request(self, method, url, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate(method, **kwargs)
-
-            obj = self.session.request(method, url, **kwargs, headers=headers)
-            self.to_close.append(obj)
-
-            res = obj.__aenter__()
-
-            if DEBUG:
-                print("Request")
-                print("  Method: " + str(method).upper())
-                print("  Url: " + str(url))
-                print("")
-
-            # wraps client response to be used within django views
-            if self.proxy:
-                return self._async_proxy(res)
-
-            return res
-
-elif LIBRARIES["requests"]:
-
-    class AsyncService:
-
-        async def __aenter__(self) -> "Service":
-
-            self.sync = True
-
-            if isinstance(self.app_pk, self._get_app_cls()):
-                self.app = self.app_pk
-                return self
-
-            self.app = await sync_to_async(self._get_app)(self.app_pk)
-
-            return self
-
-        async def __aexit__(self, *args, **kwargs) -> None:
-            pass
-
-        def _async_proxy(self, response: requests.Response, stream: bool) -> StreamingHttpResponse:
-            header_keys = [x for x in response.headers.keys() if x not in self.banned_keys]
-
-            if stream:
-                resource = StreamingHttpResponse(
-                    response.raw,
-                    status=response.status_code,
-                    reason=response.reason,
-                )
-
-                for header in header_keys:
-                    resource[header] = response.headers[header]
-
-                if DEBUG:
-                    print("Response")
-                    print("  Content: no visible due to it's a stream")
-                    print("  Headers: " + str(response.headers))
-                    print("  Status code: " + str(response.status_code))
-                    print("")
-
-                return resource
-
-            headers = {}
-
-            for header in header_keys:
-                headers[header] = response.headers[header]
-
-            if DEBUG:
-                print("Response")
-                print("  Type: Proxy")
-                print("  Content: " + response.content.decode())
-                print("  Headers: " + str(headers))
-                print("  Status code: " + str(response.status_code))
-                print("")
-
-            return HttpResponse(response.content, status=response.status_code, headers=headers)
-
-        async def _async_get(self, url, params=None, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-
-            if self.sync is False:
-                params = kwargs.pop("params", None)
-
-            headers = self._authenticate("get", params=params, **kwargs)
-            res = requests.get(url, params=params, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._async_proxy(res, kwargs.get("stream", False))
-
-            return res
-
-        async def _async_options(self, url, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("options", **kwargs)
-            res = requests.options(url, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._async_proxy(res, kwargs.get("stream", False))
-
-            return res
-
-        async def _async_head(self, url, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("head", **kwargs)
-            res = requests.head(url, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._async_proxy(res, kwargs.get("stream", False))
-
-            return res
-
-        async def _async_post(self, url, data=None, json=None, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("post", data=data, json=json, **kwargs)
-            res = requests.post(url, data=data, json=json, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._async_proxy(res, kwargs.get("stream", False))
-
-            return res
-
-        async def _async_webhook(self, url, data=None, json=None, **kwargs):
-            url = self.app.webhook_url
-            headers = self._authenticate("post", data=data, json=json, **kwargs)
-            res = requests.post(url, data=data, json=json, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._async_proxy(res, kwargs.get("stream", False))
-
-            return res
-
-        async def _async_put(self, url, data=None, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("put", data=data, **kwargs)
-            res = requests.put(url, data=data, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._async_proxy(res, kwargs.get("stream", False))
-
-            return res
-
-        async def _async_patch(self, url, data=None, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("patch", data=data, **kwargs)
-            res = requests.patch(url, data=data, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._async_proxy(res, kwargs.get("stream", False))
-
-            return res
-
-        async def _async_delete(self, url, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate("delete", **kwargs)
-            res = requests.delete(url, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._async_proxy(res, kwargs.get("stream", False))
-
-            return res
-
-        async def _async_request(self, method, url, **kwargs):
-            url = self.app.app_url + self._fix_url(url)
-            headers = self._authenticate(method, **kwargs)
-            res = requests.request(method, url, **kwargs, headers=headers)
-
-            if self.proxy:
-                return self._async_proxy(res, kwargs.get("stream", False))
-
-            return res
-
-else:
-
-    class AsyncService:
-        pass
-
-
-class Service(SyncService, AsyncService):
-    session: aiohttp.ClientSession
-
-    def __init__(
-        self,
-        app_pk: str | int,
-        user_pk: Optional[str | int] = None,
-        *,
-        mode: Optional[str] = None,
-        proxy: bool = False,
-    ):
-        self.app_pk = app_pk
-        self.user_pk = user_pk
-        self.mode = mode
-        self.to_close = []
-        self.proxy = proxy
-        self.banned_keys = [
-            "Transfer-Encoding",
-            "Content-Encoding",
-            "Keep-Alive",
-            "Connection",
-            "Content-Length",
-            "Upgrade",
-        ]
-
-    def _get_app_cls(self) -> Type[Unknown]:
-        raise NotImplementedError("This method should be implemented")
-
-    def _get_app(self, pk: str | int) -> Unknown:
-        raise NotImplementedError("This method should be implemented")
-
-    def _get_signature(
-        self,
-        app: Any,
-        user_id: Optional[int] = None,
-        *,
-        method: str = "get",
-        params: Optional[dict] = None,
-        body: Optional[dict] = None,
-        headers: Optional[dict] = None,
-        reverse: bool = False,
-    ) -> tuple[str, str]:
-        raise NotImplementedError("This method should be implemented")
-
-    def _get_jwt(self, app: Any, user_id: Optional[int] = None, reverse: bool = False) -> str:
-        raise NotImplementedError("This method should be implemented")
-
-    def _sign(self, method, params=None, data=None, json=None, **kwargs) -> requests.Request:
-        # from breathecode.authenticate.actions import get_signature
-
-        headers = kwargs.pop("headers", {})
-        headers.pop("Authorization", None)
-
-        sign, now = self._get_signature(
-            self.app,
-            self.user_pk,
-            method=method,
-            params=params,
-            body=data if data is not None else json,
-            headers=headers,
-        )
-
-        whoamy = get_setting("app_name")
-        headers["Authorization"] = (
-            f"Signature App={whoamy}," f"Nonce={sign}," f'SignedHeaders={";".join(headers.keys())},' f"Date={now}"
-        )
-
-        return headers
-
-    def _jwt(self, method, **kwargs) -> requests.Request:
-        # from .actions import get_jwt
-
-        headers = kwargs.pop("headers", {})
-
-        token = self._get_jwt(self.app, self.user_pk)
-
-        whoamy = get_setting("app_name")
-        headers["Authorization"] = f"Link App={whoamy}," f"Token={token}"
-
-        return headers
-
-    def _authenticate(self, method, params=None, data=None, json=None, **kwargs) -> requests.Request:
-        if self.mode == "signature" or self.app.strategy == "SIGNATURE":
-            return self._sign(method, params=params, data=data, json=json, **kwargs)
-
-        elif self.mode == "jwt" or self.app.strategy == "JWT":
-            return self._jwt(method, **kwargs)
-
-        raise Exception("Strategy not implemented")
-
-    def _fix_url(self, url):
-        if url[0] != "/":
-            url = f"/{url}"
-
-        return url
-
-    def get(self, url, params=None, **kwargs):
-        if self.sync:
-            return self._sync_get(url, params=params, **kwargs)
-
-        return self._async_get(url, params=params, **kwargs)
-
-    def options(self, url, **kwargs):
-        if self.sync:
-            return self._sync_options(url, **kwargs)
-
-        return self._async_options(url, **kwargs)
-
-    def head(self, url, **kwargs):
-        if self.sync:
-            return self._sync_head(url, **kwargs)
-
-        return self._async_head(url, **kwargs)
-
-    def post(self, url, data=None, json=None, **kwargs):
-        if self.sync:
-            return self._sync_post(url, data=data, json=json, **kwargs)
-
-        return self._async_post(url, data=data, json=json, **kwargs)
-
-    def webhook(self, url, data=None, json=None, **kwargs):
-        if self.sync:
-            return self._sync_webhook(url, data=data, json=json, **kwargs)
-
-        return self._async_webhook(url, data=data, json=json, **kwargs)
-
-    def put(self, url, data=None, **kwargs):
-        if self.sync:
-            return self._sync_put(url, data=data, **kwargs)
-
-        return self._async_put(url, data=data, **kwargs)
-
-    def patch(self, url, data=None, **kwargs):
-        if self.sync:
-            return self._sync_patch(url, data=data, **kwargs)
-
-        return self._async_patch(url, data=data, **kwargs)
-
-    def delete(self, url, **kwargs):
-        if self.sync:
-            return self._sync_delete(url, **kwargs)
-
-        return self._async_delete(url, **kwargs)
-
-    def request(self, method, url, **kwargs):
-        if self.sync:
-            return self._sync_request(method, url, **kwargs)
-
-        return self._async_request(method, url, **kwargs)
-
-
-class AppNotFound(Exception):
-    pass
+from __future__ import annotations
+
+import logging
+import os
+from types import TracebackType
+from typing import Any, Callable, Coroutine, Optional, Type
+
+import aiohttp
+from asgiref.sync import sync_to_async
+from django.http import HttpResponse, StreamingHttpResponse
+
+from linked_services.core.exceptions import ValidationException
+from linked_services.core.settings import get_setting
+
+__all__ = ["Service"]
+
+DEBUG = os.getenv("LOG_LEVEL") == "DEBUG"
+
+LIBRARIES = {
+    "requests": False,
+    "aiohttp": False,  # no implemented yet
+    "httpx": False,
+}
+
+try:
+    import requests
+
+    LIBRARIES["requests"] = True
+
+except ImportError:
+    pass
+
+try:
+    from aiohttp.client_reqrep import ClientResponse
+
+    LIBRARIES["aiohttp"] = True
+
+except ImportError:
+    pass
+
+try:
+    import httpx  # noqa: F401
+
+    LIBRARIES["httpx"] = True
+
+except ImportError:
+    pass
+
+
+class Unknown:
+    pass
+
+
+if LIBRARIES["requests"]:
+
+    class SyncService:
+
+        def __enter__(self) -> "Service":
+
+            self.sync = True
+
+            if isinstance(self.app_pk, self._get_app_cls()):
+                self.app = self.app_pk
+                return self
+
+            try:
+                self.app = self._get_app(self.app_pk)
+
+            except Exception:
+                raise AppNotFound(f"App {self.app_pk} not found")
+
+            return self
+
+        def __exit__(
+            self,
+            exc_type: Optional[Type[BaseException]],
+            exc_val: Optional[BaseException],
+            exc_tb: Optional[TracebackType],
+        ) -> None:
+            pass
+
+        def _sync_proxy(self, request: Callable[[], requests.Response], stream: bool) -> StreamingHttpResponse:
+            try:
+                response = request()
+
+            except Exception as e:
+                raise ValidationException("Unexpected error: " + str(e), code=500, slug="unexpected-error")
+
+            header_keys = [x for x in response.headers.keys() if x not in self.banned_keys]
+
+            if stream:
+                resource = StreamingHttpResponse(
+                    response.raw,
+                    status=response.status_code,
+                    reason=response.reason,
+                )
+
+                for header in header_keys:
+                    resource[header] = response.headers[header]
+
+                if DEBUG:
+                    print("Response")
+                    print("  Content: no visible due to it's a stream")
+                    print("  Headers: " + str(response.headers))
+                    print("  Status code: " + str(response.status_code))
+                    print("")
+
+                return resource
+
+            headers = {}
+
+            for header in header_keys:
+                headers[header] = response.headers[header]
+
+            if DEBUG:
+                print("Response")
+                print("  Type: Proxy")
+                print("  Content: " + response.content.decode())
+                print("  Headers: " + str(headers))
+                print("  Status code: " + str(response.status_code))
+                print("")
+
+            return HttpResponse(response.content, status=response.status_code, headers=headers)
+
+        def _sync_get(self, url, params=None, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+
+            if self.sync is False:
+                params = kwargs.pop("params", None)
+
+            headers = self._authenticate("get", params=params, **kwargs)
+
+            def request() -> requests.Response:
+                if DEBUG:
+                    print("Request")
+                    print("  Method: GET")
+                    print("  Url: " + str(url))
+                    print("")
+
+                return requests.get(url, params=params, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._sync_proxy(request, kwargs.get("stream", False))
+
+            res = request()
+
+            return res
+
+        def _sync_options(self, url, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("options", **kwargs)
+
+            def request() -> requests.Response:
+                if DEBUG:
+                    print("Request")
+                    print("  Method: OPTIONS")
+                    print("  Url: " + str(url))
+                    print("")
+
+                return requests.options(url, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._sync_proxy(request, kwargs.get("stream", False))
+
+            res = request()
+
+            return res
+
+        def _sync_head(self, url, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("head", **kwargs)
+
+            def request() -> requests.Response:
+                if DEBUG:
+                    print("Request")
+                    print("  Method: HEAD")
+                    print("  Url: " + str(url))
+                    print("")
+
+                return requests.head(url, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._sync_proxy(request, kwargs.get("stream", False))
+
+            res = request()
+
+            return res
+
+        def _sync_post(self, url, data=None, json=None, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("post", data=data, json=json, **kwargs)
+
+            def request() -> requests.Response:
+                if DEBUG:
+                    print("Request")
+                    print("  Method: POST")
+                    print("  Url: " + str(url))
+                    print("")
+
+                return requests.post(url, data=data, json=json, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._sync_proxy(request, kwargs.get("stream", False))
+
+            res = request()
+
+            return res
+
+        def _sync_webhook(self, url, data=None, json=None, **kwargs):
+            url = self.app.webhook_url
+            headers = self._authenticate("post", data=data, json=json, **kwargs)
+
+            def request() -> requests.Response:
+                if DEBUG:
+                    print("Request")
+                    print("  Type: Webhook")
+                    print("  Url: " + str(url))
+                    print("")
+
+                return requests.post(url, data=data, json=json, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._sync_proxy(request, kwargs.get("stream", False))
+
+            res = request()
+
+            return res
+
+        def _sync_put(self, url, data=None, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("put", data=data, **kwargs)
+
+            def request() -> requests.Response:
+                if DEBUG:
+                    print("Request")
+                    print("  Method: PUT")
+                    print("  Url: " + str(url))
+                    print("")
+
+                return requests.put(url, data=data, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._sync_proxy(request, kwargs.get("stream", False))
+
+            res = request()
+
+            return res
+
+        def _sync_patch(self, url, data=None, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("patch", data=data, **kwargs)
+
+            def request() -> requests.Response:
+                if DEBUG:
+                    print("Request")
+                    print("  Method: PATCH")
+                    print("  Url: " + str(url))
+                    print("")
+
+                return requests.patch(url, data=data, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._sync_proxy(request, kwargs.get("stream", False))
+
+            res = request()
+
+            return res
+
+        def _sync_delete(self, url, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("delete", **kwargs)
+
+            def request() -> requests.Response:
+                if DEBUG:
+                    print("Request")
+                    print("  Method: DELETE")
+                    print("  Url: " + str(url))
+                    print("")
+
+                return requests.delete(url, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._sync_proxy(request, kwargs.get("stream", False))
+
+            res = request()
+
+            return res
+
+        def _sync_request(self, method, url, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate(method, **kwargs)
+
+            def request() -> requests.Response:
+                if DEBUG:
+                    print("Request")
+                    print("  Method: " + str(method).upper())
+                    print("  Url: " + str(url))
+                    print("")
+
+                return requests.request(method, url, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._sync_proxy(request, kwargs.get("stream", False))
+
+            res = request()
+
+            return res
+
+else:
+
+    class SyncService:
+        pass
+
+
+if LIBRARIES["aiohttp"]:
+
+    class AsyncService:
+        to_close: list
+
+        async def __aenter__(self) -> "Service":
+
+            self.sync = False
+
+            if isinstance(self.app_pk, self._get_app_cls()):
+                self.app = self.app_pk
+
+            else:
+                self.app = await sync_to_async(self._get_app)(self.app_pk)
+
+            self.session = aiohttp.ClientSession()
+
+            # this should be extended
+            await self.session.__aenter__()
+
+            return self
+
+        async def __aexit__(self, *args, **kwargs) -> None:
+            for obj in self.to_close:
+                try:
+                    await obj.__aexit__(*args, **kwargs)
+
+                except Exception:
+                    pass
+
+            try:
+                await self.session.__aexit__(*args, **kwargs)
+
+            except Exception:
+                pass
+
+        # django does not support StreamingHttpResponse with aiohttp due to django would have to close the response
+        async def _async_proxy(self, response: Coroutine[Any, Any, ClientResponse]) -> HttpResponse:
+            try:
+                r = await response
+
+            except Exception as e:
+                raise ValidationException("Unexpected error: " + str(e), code=500, slug="unexpected-error")
+
+            header_keys = [x for x in r.headers.keys() if x not in self.banned_keys]
+
+            headers = {}
+            for header in header_keys:
+                headers[str(header)] = r.headers[header]
+
+            content = await r.content.read()
+
+            if DEBUG:
+                print("Response")
+                print("  Type: Proxy")
+                print("  Content: " + content.decode())
+                print("  Headers: " + str(headers))
+                print("  Status code: " + str(r.status))
+                print("")
+
+            return HttpResponse(content, status=r.status, headers=headers)
+
+        def _async_get(self, url, params=None, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("get", params=params, **kwargs)
+
+            obj = self.session.get(url, params=params, **kwargs, headers=headers)
+            self.to_close.append(obj)
+
+            res = obj.__aenter__()
+
+            if DEBUG:
+                print("Request")
+                print("  Method: GET")
+                print("  Url: " + str(url))
+                print("")
+
+            # wraps client response to be used within django views
+            if self.proxy:
+                return self._async_proxy(res)
+
+            return res
+
+        def _async_options(self, url, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("options", **kwargs)
+
+            obj = self.session.options(url, **kwargs, headers=headers)
+            self.to_close.append(obj)
+
+            res = obj.__aenter__()
+
+            if DEBUG:
+                print("Request")
+                print("  Method: OPTIONS")
+                print("  Url: " + str(url))
+                print("")
+
+            # wraps client response to be used within django views
+            if self.proxy:
+                return self._async_proxy(res)
+
+            return res
+
+        def _async_head(self, url, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("head", **kwargs)
+
+            obj = self.session.head(url, **kwargs, headers=headers)
+            self.to_close.append(obj)
+
+            res = obj.__aenter__()
+
+            if DEBUG:
+                print("Request")
+                print("  Method: HEAD")
+                print("  Url: " + str(url))
+                print("")
+
+            # wraps client response to be used within django views
+            if self.proxy:
+                return self._async_proxy(res)
+
+            return res
+
+        def _async_post(self, url, data=None, json=None, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("post", data=data, json=json, **kwargs)
+
+            obj = self.session.post(url, data=data, json=json, **kwargs, headers=headers)
+            self.to_close.append(obj)
+
+            res = obj.__aenter__()
+
+            if DEBUG:
+                print("Request")
+                print("  Method: POST")
+                print("  Url: " + str(url))
+                print("")
+
+            # wraps client response to be used within django views
+            if self.proxy:
+                return self._async_proxy(res)
+
+            return res
+
+        def _async_webhook(self, url, data=None, json=None, **kwargs):
+            url = self.app.webhook_url
+            headers = self._authenticate("post", data=data, json=json, **kwargs)
+
+            obj = self.session.post(url, data=data, json=json, **kwargs, headers=headers)
+            self.to_close.append(obj)
+
+            res = obj.__aenter__()
+
+            if DEBUG:
+                print("Request")
+                print("  Type: Webhook")
+                print("  Url: " + str(url))
+                print("")
+
+            # wraps client response to be used within django views
+            if self.proxy:
+                return self._async_proxy(res)
+
+            return res
+
+        def _async_put(self, url, data=None, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("put", data=data, **kwargs)
+
+            obj = self.session.put(url, data=data, **kwargs, headers=headers)
+            self.to_close.append(obj)
+
+            res = obj.__aenter__()
+
+            if DEBUG:
+                print("Request")
+                print("  Method: PUT")
+                print("  Url: " + str(url))
+                print("")
+
+            # wraps client response to be used within django views
+            if self.proxy:
+                return self._async_proxy(res)
+
+            return res
+
+        def _async_patch(self, url, data=None, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("patch", data=data, **kwargs)
+
+            obj = self.session.patch(url, data=data, **kwargs, headers=headers)
+            self.to_close.append(obj)
+
+            res = obj.__aenter__()
+
+            if DEBUG:
+                print("Request")
+                print("  Method: PATCH")
+                print("  Url: " + str(url))
+                print("")
+
+            # wraps client response to be used within django views
+            if self.proxy:
+                return self._async_proxy(res)
+
+            return res
+
+        def _async_delete(self, url, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("delete", **kwargs)
+
+            obj = self.session.delete(url, **kwargs, headers=headers)
+            self.to_close.append(obj)
+
+            res = obj.__aenter__()
+
+            if DEBUG:
+                print("Request")
+                print("  Method: DELETE")
+                print("  Url: " + str(url))
+                print("")
+
+            # wraps client response to be used within django views
+            if self.proxy:
+                return self._async_proxy(res)
+
+            return res
+
+        def _async_request(self, method, url, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate(method, **kwargs)
+
+            obj = self.session.request(method, url, **kwargs, headers=headers)
+            self.to_close.append(obj)
+
+            res = obj.__aenter__()
+
+            if DEBUG:
+                print("Request")
+                print("  Method: " + str(method).upper())
+                print("  Url: " + str(url))
+                print("")
+
+            # wraps client response to be used within django views
+            if self.proxy:
+                return self._async_proxy(res)
+
+            return res
+
+elif LIBRARIES["requests"]:
+
+    class AsyncService:
+
+        async def __aenter__(self) -> "Service":
+
+            self.sync = True
+
+            if isinstance(self.app_pk, self._get_app_cls()):
+                self.app = self.app_pk
+                return self
+
+            self.app = await sync_to_async(self._get_app)(self.app_pk)
+
+            return self
+
+        async def __aexit__(self, *args, **kwargs) -> None:
+            pass
+
+        def _async_proxy(self, response: requests.Response, stream: bool) -> StreamingHttpResponse:
+            header_keys = [x for x in response.headers.keys() if x not in self.banned_keys]
+
+            if stream:
+                resource = StreamingHttpResponse(
+                    response.raw,
+                    status=response.status_code,
+                    reason=response.reason,
+                )
+
+                for header in header_keys:
+                    resource[header] = response.headers[header]
+
+                if DEBUG:
+                    print("Response")
+                    print("  Content: no visible due to it's a stream")
+                    print("  Headers: " + str(response.headers))
+                    print("  Status code: " + str(response.status_code))
+                    print("")
+
+                return resource
+
+            headers = {}
+
+            for header in header_keys:
+                headers[header] = response.headers[header]
+
+            if DEBUG:
+                print("Response")
+                print("  Type: Proxy")
+                print("  Content: " + response.content.decode())
+                print("  Headers: " + str(headers))
+                print("  Status code: " + str(response.status_code))
+                print("")
+
+            return HttpResponse(response.content, status=response.status_code, headers=headers)
+
+        async def _async_get(self, url, params=None, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+
+            if self.sync is False:
+                params = kwargs.pop("params", None)
+
+            headers = self._authenticate("get", params=params, **kwargs)
+            res = requests.get(url, params=params, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._async_proxy(res, kwargs.get("stream", False))
+
+            return res
+
+        async def _async_options(self, url, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("options", **kwargs)
+            res = requests.options(url, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._async_proxy(res, kwargs.get("stream", False))
+
+            return res
+
+        async def _async_head(self, url, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("head", **kwargs)
+            res = requests.head(url, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._async_proxy(res, kwargs.get("stream", False))
+
+            return res
+
+        async def _async_post(self, url, data=None, json=None, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("post", data=data, json=json, **kwargs)
+            res = requests.post(url, data=data, json=json, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._async_proxy(res, kwargs.get("stream", False))
+
+            return res
+
+        async def _async_webhook(self, url, data=None, json=None, **kwargs):
+            url = self.app.webhook_url
+            headers = self._authenticate("post", data=data, json=json, **kwargs)
+            res = requests.post(url, data=data, json=json, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._async_proxy(res, kwargs.get("stream", False))
+
+            return res
+
+        async def _async_put(self, url, data=None, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("put", data=data, **kwargs)
+            res = requests.put(url, data=data, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._async_proxy(res, kwargs.get("stream", False))
+
+            return res
+
+        async def _async_patch(self, url, data=None, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("patch", data=data, **kwargs)
+            res = requests.patch(url, data=data, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._async_proxy(res, kwargs.get("stream", False))
+
+            return res
+
+        async def _async_delete(self, url, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate("delete", **kwargs)
+            res = requests.delete(url, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._async_proxy(res, kwargs.get("stream", False))
+
+            return res
+
+        async def _async_request(self, method, url, **kwargs):
+            url = self.app.app_url + self._fix_url(url)
+            headers = self._authenticate(method, **kwargs)
+            res = requests.request(method, url, **kwargs, headers=headers)
+
+            if self.proxy:
+                return self._async_proxy(res, kwargs.get("stream", False))
+
+            return res
+
+else:
+
+    class AsyncService:
+        pass
+
+
+class Service(SyncService, AsyncService):
+    session: aiohttp.ClientSession
+
+    def __init__(
+        self,
+        app_pk: str | int,
+        user_pk: Optional[str | int] = None,
+        *,
+        mode: Optional[str] = None,
+        proxy: bool = False,
+    ):
+        self.app_pk = app_pk
+        self.user_pk = user_pk
+        self.mode = mode
+        self.to_close = []
+        self.proxy = proxy
+        self.banned_keys = [
+            "Transfer-Encoding",
+            "Content-Encoding",
+            "Keep-Alive",
+            "Connection",
+            "Content-Length",
+            "Upgrade",
+        ]
+
+    def _get_app_cls(self) -> Type[Unknown]:
+        raise NotImplementedError("This method should be implemented")
+
+    def _get_app(self, pk: str | int) -> Unknown:
+        raise NotImplementedError("This method should be implemented")
+
+    def _get_signature(
+        self,
+        app: Any,
+        user_id: Optional[int] = None,
+        *,
+        method: str = "get",
+        params: Optional[dict] = None,
+        body: Optional[dict] = None,
+        headers: Optional[dict] = None,
+        reverse: bool = False,
+    ) -> tuple[str, str]:
+        raise NotImplementedError("This method should be implemented")
+
+    def _get_jwt(self, app: Any, user_id: Optional[int] = None, reverse: bool = False) -> str:
+        raise NotImplementedError("This method should be implemented")
+
+    def _sign(self, method, params=None, data=None, json=None, **kwargs) -> requests.Request:
+        # from breathecode.authenticate.actions import get_signature
+
+        headers = kwargs.pop("headers", {})
+        headers.pop("Authorization", None)
+
+        sign, now = self._get_signature(
+            self.app,
+            self.user_pk,
+            method=method,
+            params=params,
+            body=data if data is not None else json,
+            headers=headers,
+        )
+
+        whoamy = get_setting("app_name")
+        headers["Authorization"] = (
+            f"Signature App={whoamy}," f"Nonce={sign}," f'SignedHeaders={";".join(headers.keys())},' f"Date={now}"
+        )
+
+        return headers
+
+    def _jwt(self, method, **kwargs) -> requests.Request:
+        # from .actions import get_jwt
+
+        headers = kwargs.pop("headers", {})
+
+        token = self._get_jwt(self.app, self.user_pk)
+
+        whoamy = get_setting("app_name")
+        headers["Authorization"] = f"Link App={whoamy}," f"Token={token}"
+
+        return headers
+
+    def _authenticate(self, method, params=None, data=None, json=None, **kwargs) -> requests.Request:
+        if self.mode == "signature" or self.app.strategy == "SIGNATURE":
+            return self._sign(method, params=params, data=data, json=json, **kwargs)
+
+        elif self.mode == "jwt" or self.app.strategy == "JWT":
+            return self._jwt(method, **kwargs)
+
+        raise Exception("Strategy not implemented")
+
+    def _fix_url(self, url):
+        if url[0] != "/":
+            url = f"/{url}"
+
+        return url
+
+    def get(self, url, params=None, **kwargs):
+        if self.sync:
+            return self._sync_get(url, params=params, **kwargs)
+
+        return self._async_get(url, params=params, **kwargs)
+
+    def options(self, url, **kwargs):
+        if self.sync:
+            return self._sync_options(url, **kwargs)
+
+        return self._async_options(url, **kwargs)
+
+    def head(self, url, **kwargs):
+        if self.sync:
+            return self._sync_head(url, **kwargs)
+
+        return self._async_head(url, **kwargs)
+
+    def post(self, url, data=None, json=None, **kwargs):
+        if self.sync:
+            return self._sync_post(url, data=data, json=json, **kwargs)
+
+        return self._async_post(url, data=data, json=json, **kwargs)
+
+    def webhook(self, url, data=None, json=None, **kwargs):
+        if self.sync:
+            return self._sync_webhook(url, data=data, json=json, **kwargs)
+
+        return self._async_webhook(url, data=data, json=json, **kwargs)
+
+    def put(self, url, data=None, **kwargs):
+        if self.sync:
+            return self._sync_put(url, data=data, **kwargs)
+
+        return self._async_put(url, data=data, **kwargs)
+
+    def patch(self, url, data=None, **kwargs):
+        if self.sync:
+            return self._sync_patch(url, data=data, **kwargs)
+
+        return self._async_patch(url, data=data, **kwargs)
+
+    def delete(self, url, **kwargs):
+        if self.sync:
+            return self._sync_delete(url, **kwargs)
+
+        return self._async_delete(url, **kwargs)
+
+    def request(self, method, url, **kwargs):
+        if self.sync:
+            return self._sync_request(method, url, **kwargs)
+
+        return self._async_request(method, url, **kwargs)
+
+
+class AppNotFound(Exception):
+    pass
```

### Comparing `linked_services-1.2.1/src/linked_services/django/actions.py` & `linked_services-1.2.2/src/linked_services/django/actions.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,460 +1,460 @@
-import hashlib
-import hmac
-import os
-import secrets
-import urllib.parse
-import uuid
-from functools import lru_cache
-from typing import Optional
-
-import jwt
-from asgiref.sync import sync_to_async
-from cryptography.hazmat.primitives.asymmetric.ed25519 import Ed25519PrivateKey
-from cryptography.hazmat.primitives.serialization import (
-    Encoding,
-    NoEncryption,
-    PrivateFormat,
-    PublicFormat,
-)
-from django.contrib.auth.models import User
-from django.utils import timezone
-
-from linked_services.core.exceptions import ValidationException
-from linked_services.core.settings import get_setting
-from linked_services.django.models import (
-    App,
-    FirstPartyCredentials,
-    FirstPartyWebhookLog,
-)
-
-JWT_LIFETIME = 10
-
-
-def get_jwt(app: App, user_id: Optional[int] = None, reverse: bool = False):
-    from datetime import datetime, timedelta
-
-    now = datetime.utcnow()
-    whoamy = get_setting("app_name")
-
-    # https://datatracker.ietf.org/doc/html/rfc7519#section-4
-    payload = {
-        "sub": user_id,
-        "iss": os.getenv("API_URL", "http://localhost:8000"),
-        "app": whoamy,
-        "aud": app.slug,
-        "exp": datetime.timestamp(now + timedelta(minutes=JWT_LIFETIME)),
-        "iat": datetime.timestamp(now) - 1,
-        "typ": "JWT",
-    }
-
-    if reverse:
-        payload["app"] = app.slug
-        payload["aud"] = whoamy
-
-    if app.algorithm == "HMAC_SHA256":
-
-        token = jwt.encode(payload, bytes.fromhex(app.private_key), algorithm="HS256")
-
-    elif app.algorithm == "HMAC_SHA512":
-        token = jwt.encode(payload, bytes.fromhex(app.private_key), algorithm="HS512")
-
-    elif app.algorithm == "ED25519":
-        token = jwt.encode(payload, bytes.fromhex(app.private_key), algorithm="EdDSA")
-
-    else:
-        raise Exception("Algorithm not implemented")
-
-    return token
-
-
-def get_signature(
-    app: App,
-    user_id: Optional[int] = None,
-    *,
-    method: str = "get",
-    params: Optional[dict] = None,
-    body: Optional[dict] = None,
-    headers: Optional[dict] = None,
-    reverse: bool = False,
-):
-    now = timezone.now().isoformat()
-    whoamy = get_setting("app_name")
-
-    if headers is None:
-        headers = {}
-
-    if params is None:
-        params = {}
-
-    payload = {
-        "timestamp": now,
-        "app": whoamy,
-        "method": method.upper(),
-        "params": params or {},
-        "body": body,
-        "headers": headers or {},
-    }
-
-    if reverse:
-        payload["app"] = app.slug
-
-    paybytes = urllib.parse.urlencode(payload).encode("utf8")
-
-    if app.algorithm == "HMAC_SHA256":
-        sign = hmac.new(bytes.fromhex(app.private_key), paybytes, hashlib.sha256).hexdigest()
-
-    elif app.algorithm == "HMAC_SHA512":
-        sign = hmac.new(bytes.fromhex(app.private_key), paybytes, hashlib.sha512).hexdigest()
-
-    else:
-        raise Exception("Algorithm not implemented")
-
-    return sign, now
-
-
-def generate_auth_keys(algorithm) -> tuple[bytes, bytes]:
-    public_key = None
-    key = Ed25519PrivateKey.generate()
-
-    if algorithm == "HMAC_SHA256" or algorithm == "HMAC_SHA512":
-        private_key = secrets.token_hex(64)
-
-    elif algorithm == "ED25519":
-        private_key = key.private_bytes(
-            encoding=Encoding.PEM,
-            format=PrivateFormat.PKCS8,
-            encryption_algorithm=NoEncryption(),
-        ).hex()
-
-        public_key = (
-            key.public_key().public_bytes(encoding=Encoding.PEM, format=PublicFormat.SubjectPublicKeyInfo).hex()
-        )
-
-    return public_key, private_key
-
-
-@lru_cache(maxsize=100)
-def get_optional_scopes_set(scope_set_id):
-    from .models import OptionalScopeSet
-
-    scope_set = OptionalScopeSet.objects.filter(id=scope_set_id).first()
-    if scope_set is None:
-        raise Exception(f"Invalid scope set id: {scope_set_id}")
-
-    # use structure that use lower memory
-    return tuple(sorted(x for x in scope_set.optional_scopes.all()))
-
-
-def get_user_scopes(app_slug, user_id=None):
-    from .models import AppUserAgreement
-
-    info, _, _ = get_app_keys(app_slug)
-    (_, _, _, _, require_an_agreement, required_scopes, optional_scopes, _, _, _) = info
-
-    if user_id and require_an_agreement:
-        agreement = AppUserAgreement.objects.filter(app__slug=app_slug, user__id=user_id).first()
-        if not agreement:
-            raise ValidationException(
-                "User has not accepted the agreement",
-                slug="agreement-not-accepted",
-                silent=True,
-                data={"app_slug": app_slug, "user_id": user_id},
-            )
-
-        optional_scopes = get_optional_scopes_set(agreement.optional_scope_set.id)
-
-    # use structure that use lower memory
-    return required_scopes, optional_scopes
-
-
-@lru_cache(maxsize=100)
-def get_app_keys(app_slug):
-    from .models import App, Scope
-
-    app = App.objects.filter(slug=app_slug).first()
-
-    if app is None:
-        raise ValidationException("Unauthorized", code=401, slug="app-not-found")
-
-    if app.algorithm == "HMAC_SHA256":
-        alg = "HS256"
-
-    elif app.algorithm == "HMAC_SHA512":
-        alg = "HS512"
-
-    elif app.algorithm == "ED25519":
-        alg = "EdDSA"
-
-    else:
-        raise ValidationException("Algorithm not implemented", code=401, slug="algorithm-not-implemented")
-
-    legacy_public_key = None
-    legacy_private_key = None
-    legacy_key = None
-    if hasattr(app, "legacy_key"):
-        legacy_public_key = bytes.fromhex(app.legacy_key.public_key) if app.legacy_key.public_key else None
-        legacy_private_key = bytes.fromhex(app.legacy_key.private_key)
-        legacy_key = (
-            legacy_public_key,
-            legacy_private_key,
-        )
-
-    info = (
-        app.id,
-        alg,
-        app.strategy,
-        app.schema,
-        app.require_an_agreement,
-        tuple(sorted(x.slug for x in Scope.objects.filter(m2m_required_scopes__app=app))),
-        tuple(sorted(x.slug for x in Scope.objects.filter(m2m_optional_scopes__app=app))),
-        app.webhook_url,
-        app.redirect_url,
-        app.app_url,
-    )
-    key = (
-        bytes.fromhex(app.public_key) if app.public_key else None,
-        bytes.fromhex(app.private_key),
-    )
-
-    # use structure that use lower memory
-    return info, key, legacy_key
-
-
-def reset_app_cache():
-    get_app.cache_clear()
-    get_app_keys.cache_clear()
-    get_optional_scopes_set.cache_clear()
-
-
-def reset_app_user_cache():
-    get_optional_scopes_set.cache_clear()
-
-
-@lru_cache(maxsize=100)
-def get_app(pk: str | int) -> App:
-    kwargs = {}
-
-    if isinstance(pk, int):
-        kwargs["id"] = pk
-
-    elif isinstance(pk, str):
-        kwargs["slug"] = pk
-
-    else:
-        raise Exception("Invalid pk type")
-
-    if not (app := App.objects.filter(**kwargs).first()):
-        raise Exception("App not found")
-
-    return app
-
-
-async def aget_app(pk: str | int) -> App:
-    return await sync_to_async(get_app)(pk)
-
-
-class WebhookException(Exception):
-    pass
-
-
-async def send_webhook(
-    app: str | int | App,
-    type: str,
-    data: Optional[dict | list] = None,
-    user: Optional[str | int | User] = None,
-):
-    from .service import Service
-
-    if not isinstance(app, App):
-        app = await aget_app(app)
-
-    if user and not isinstance(user, User):
-        user = await User.objects.filter(id=user).afirst()
-        if user is None:
-            raise Exception("User not found")
-
-    x = await FirstPartyWebhookLog.objects.acreate(app=app, type=type, data=data)
-    payload = {
-        "type": type,
-        "external_id": x.id,
-        "data": data,
-    }
-
-    user_id = None
-    if user:
-        user_id = user.id
-
-    try:
-        async with Service(app, user_id, proxy=True) as s:
-            response = await s.webhook(payload)
-            if response.status != 200:
-                msg = f"Error calling webhook {app.webhook_url} with status {response.status}"
-
-                # this has relation with a reveived signal not implemented yet
-                x.processed = True
-                x.status = "ERROR"
-                x.status_text = msg
-                x.save()
-
-                raise WebhookException(msg)
-
-    except WebhookException as e:
-        raise e
-
-    except Exception as e:
-        x.delete()
-        raise e
-
-    # this has relation with a reveived signal not implemented yet
-    x.processed = True
-    # this will keep PENDING in the future
-    x.status = "DONE"
-    x.save()
-
-
-def get_user(app: str | int | uuid.UUID, sub: str | int | uuid.UUID) -> User | None:
-    credentials = FirstPartyCredentials.objects.filter(**{f"app__{app}": sub}).select_related("user").first()
-
-    if credentials:
-        return credentials.user
-
-    return create_user(app, sub)
-
-
-async def aget_user(app: str | int | uuid.UUID, sub: str | int | uuid.UUID) -> User | None:
-    credentials = await FirstPartyCredentials.objects.filter(**{f"app__{app}": sub}).select_related("user").afirst()
-
-    if credentials:
-        return credentials.user
-
-    return await acreate_user(app, sub)
-
-
-def create_user(app: str | int | uuid.UUID, sub: str | int | uuid.UUID) -> User | None:
-    from linked_services.django.service import Service
-
-    with Service(app) as s:
-        url = s.app.users_path
-        if url[-1] == "/":
-            url += str(sub)
-
-        else:
-            url += f"/{sub}"
-
-        response = s.get(url)
-
-        if response.status_code >= 300:
-            return None
-
-        data = response.json()
-        mandatory_fields = ["username", "email"]
-        optional_fields = ["first_name", "last_name"]
-        mandatory_attrs = {}
-        optional_attrs = {}
-        errors = []
-
-        if "id" not in data:
-            errors.append("id not provided")
-
-        else:
-            id = data.get("id")
-
-        for field in mandatory_fields:
-            if field in data:
-                mandatory_attrs[field] = data.get(field)
-
-            else:
-                errors.append(f"{field} not provided")
-
-        for field in optional_fields:
-            optional_attrs[field] = data.get(field, "")
-
-        if errors:
-            raise ValidationException(", ".join(errors), slug="missing-required-fields")
-
-        user, created = User.objects.get_or_create(**mandatory_attrs, defaults=optional_attrs)
-        if created:
-            for field in optional_fields:
-                setattr(user, field, optional_attrs[field])
-
-            user.save()
-
-        credentials, created = FirstPartyCredentials.objects.get_or_create(
-            user=user,
-            defaults={
-                "app": {
-                    s.app.slug: id,
-                },
-            },
-        )
-
-        if created is False:
-            credentials.app[s.app.slug] = id
-            credentials.save()
-
-        return user
-
-
-async def acreate_user(app: str | int | uuid.UUID, sub: str | int | uuid.UUID) -> User | None:
-    from linked_services.django.service import Service
-
-    async with Service(app) as s:
-        url = s.app.users_path
-        if url[-1] == "/":
-            url += str(sub)
-
-        else:
-            url += f"/{sub}"
-
-        response = await s.get(url)
-
-        if response.status_code >= 300:
-            return None
-
-        data = await response.json()
-        mandatory_fields = ["username", "email"]
-        optional_fields = ["first_name", "last_name"]
-        mandatory_attrs = {}
-        optional_attrs = {}
-        errors = []
-
-        if "id" not in data:
-            errors.append("id not provided")
-
-        else:
-            id = data.get("id")
-
-        for field in mandatory_fields:
-            if field in data:
-                mandatory_attrs[field] = data.get(field)
-
-            else:
-                errors.append(f"{field} not provided")
-
-        for field in optional_fields:
-            optional_attrs[field] = data.get(field, "")
-
-        if errors:
-            raise ValidationException(", ".join(errors), slug="missing-required-fields")
-
-        user, created = await User.objects.aget_or_create(**mandatory_attrs, defaults=optional_attrs)
-        if created:
-            for field in optional_fields:
-                setattr(user, field, optional_attrs[field])
-
-            await user.asave()
-
-        credentials, created = await FirstPartyCredentials.objects.aget_or_create(
-            user=user,
-            defaults={
-                "app": {
-                    s.app.slug: id,
-                },
-            },
-        )
-
-        if created is False:
-            credentials.app[s.app.slug] = id
-            await credentials.asave()
-
-        return user
+import hashlib
+import hmac
+import os
+import secrets
+import urllib.parse
+import uuid
+from functools import lru_cache
+from typing import Optional
+
+import jwt
+from asgiref.sync import sync_to_async
+from cryptography.hazmat.primitives.asymmetric.ed25519 import Ed25519PrivateKey
+from cryptography.hazmat.primitives.serialization import (
+    Encoding,
+    NoEncryption,
+    PrivateFormat,
+    PublicFormat,
+)
+from django.contrib.auth.models import User
+from django.utils import timezone
+
+from linked_services.core.exceptions import ValidationException
+from linked_services.core.settings import get_setting
+from linked_services.django.models import (
+    App,
+    FirstPartyCredentials,
+    FirstPartyWebhookLog,
+)
+
+JWT_LIFETIME = 10
+
+
+def get_jwt(app: App, user_id: Optional[int] = None, reverse: bool = False):
+    from datetime import datetime, timedelta
+
+    now = datetime.utcnow()
+    whoamy = get_setting("app_name")
+
+    # https://datatracker.ietf.org/doc/html/rfc7519#section-4
+    payload = {
+        "sub": user_id,
+        "iss": os.getenv("API_URL", "http://localhost:8000"),
+        "app": whoamy,
+        "aud": app.slug,
+        "exp": datetime.timestamp(now + timedelta(minutes=JWT_LIFETIME)),
+        "iat": datetime.timestamp(now) - 1,
+        "typ": "JWT",
+    }
+
+    if reverse:
+        payload["app"] = app.slug
+        payload["aud"] = whoamy
+
+    if app.algorithm == "HMAC_SHA256":
+
+        token = jwt.encode(payload, bytes.fromhex(app.private_key), algorithm="HS256")
+
+    elif app.algorithm == "HMAC_SHA512":
+        token = jwt.encode(payload, bytes.fromhex(app.private_key), algorithm="HS512")
+
+    elif app.algorithm == "ED25519":
+        token = jwt.encode(payload, bytes.fromhex(app.private_key), algorithm="EdDSA")
+
+    else:
+        raise Exception("Algorithm not implemented")
+
+    return token
+
+
+def get_signature(
+    app: App,
+    user_id: Optional[int] = None,
+    *,
+    method: str = "get",
+    params: Optional[dict] = None,
+    body: Optional[dict] = None,
+    headers: Optional[dict] = None,
+    reverse: bool = False,
+):
+    now = timezone.now().isoformat()
+    whoamy = get_setting("app_name")
+
+    if headers is None:
+        headers = {}
+
+    if params is None:
+        params = {}
+
+    payload = {
+        "timestamp": now,
+        "app": whoamy,
+        "method": method.upper(),
+        "params": params or {},
+        "body": body,
+        "headers": headers or {},
+    }
+
+    if reverse:
+        payload["app"] = app.slug
+
+    paybytes = urllib.parse.urlencode(payload).encode("utf8")
+
+    if app.algorithm == "HMAC_SHA256":
+        sign = hmac.new(bytes.fromhex(app.private_key), paybytes, hashlib.sha256).hexdigest()
+
+    elif app.algorithm == "HMAC_SHA512":
+        sign = hmac.new(bytes.fromhex(app.private_key), paybytes, hashlib.sha512).hexdigest()
+
+    else:
+        raise Exception("Algorithm not implemented")
+
+    return sign, now
+
+
+def generate_auth_keys(algorithm) -> tuple[bytes, bytes]:
+    public_key = None
+    key = Ed25519PrivateKey.generate()
+
+    if algorithm == "HMAC_SHA256" or algorithm == "HMAC_SHA512":
+        private_key = secrets.token_hex(64)
+
+    elif algorithm == "ED25519":
+        private_key = key.private_bytes(
+            encoding=Encoding.PEM,
+            format=PrivateFormat.PKCS8,
+            encryption_algorithm=NoEncryption(),
+        ).hex()
+
+        public_key = (
+            key.public_key().public_bytes(encoding=Encoding.PEM, format=PublicFormat.SubjectPublicKeyInfo).hex()
+        )
+
+    return public_key, private_key
+
+
+@lru_cache(maxsize=100)
+def get_optional_scopes_set(scope_set_id):
+    from .models import OptionalScopeSet
+
+    scope_set = OptionalScopeSet.objects.filter(id=scope_set_id).first()
+    if scope_set is None:
+        raise Exception(f"Invalid scope set id: {scope_set_id}")
+
+    # use structure that use lower memory
+    return tuple(sorted(x for x in scope_set.optional_scopes.all()))
+
+
+def get_user_scopes(app_slug, user_id=None):
+    from .models import AppUserAgreement
+
+    info, _, _ = get_app_keys(app_slug)
+    (_, _, _, _, require_an_agreement, required_scopes, optional_scopes, _, _, _) = info
+
+    if user_id and require_an_agreement:
+        agreement = AppUserAgreement.objects.filter(app__slug=app_slug, user__id=user_id).first()
+        if not agreement:
+            raise ValidationException(
+                "User has not accepted the agreement",
+                slug="agreement-not-accepted",
+                silent=True,
+                data={"app_slug": app_slug, "user_id": user_id},
+            )
+
+        optional_scopes = get_optional_scopes_set(agreement.optional_scope_set.id)
+
+    # use structure that use lower memory
+    return required_scopes, optional_scopes
+
+
+@lru_cache(maxsize=100)
+def get_app_keys(app_slug):
+    from .models import App, Scope
+
+    app = App.objects.filter(slug=app_slug).first()
+
+    if app is None:
+        raise ValidationException("Unauthorized", code=401, slug="app-not-found")
+
+    if app.algorithm == "HMAC_SHA256":
+        alg = "HS256"
+
+    elif app.algorithm == "HMAC_SHA512":
+        alg = "HS512"
+
+    elif app.algorithm == "ED25519":
+        alg = "EdDSA"
+
+    else:
+        raise ValidationException("Algorithm not implemented", code=401, slug="algorithm-not-implemented")
+
+    legacy_public_key = None
+    legacy_private_key = None
+    legacy_key = None
+    if hasattr(app, "legacy_key"):
+        legacy_public_key = bytes.fromhex(app.legacy_key.public_key) if app.legacy_key.public_key else None
+        legacy_private_key = bytes.fromhex(app.legacy_key.private_key)
+        legacy_key = (
+            legacy_public_key,
+            legacy_private_key,
+        )
+
+    info = (
+        app.id,
+        alg,
+        app.strategy,
+        app.schema,
+        app.require_an_agreement,
+        tuple(sorted(x.slug for x in Scope.objects.filter(m2m_required_scopes__app=app))),
+        tuple(sorted(x.slug for x in Scope.objects.filter(m2m_optional_scopes__app=app))),
+        app.webhook_url,
+        app.redirect_url,
+        app.app_url,
+    )
+    key = (
+        bytes.fromhex(app.public_key) if app.public_key else None,
+        bytes.fromhex(app.private_key),
+    )
+
+    # use structure that use lower memory
+    return info, key, legacy_key
+
+
+def reset_app_cache():
+    get_app.cache_clear()
+    get_app_keys.cache_clear()
+    get_optional_scopes_set.cache_clear()
+
+
+def reset_app_user_cache():
+    get_optional_scopes_set.cache_clear()
+
+
+@lru_cache(maxsize=100)
+def get_app(pk: str | int) -> App:
+    kwargs = {}
+
+    if isinstance(pk, int):
+        kwargs["id"] = pk
+
+    elif isinstance(pk, str):
+        kwargs["slug"] = pk
+
+    else:
+        raise Exception("Invalid pk type")
+
+    if not (app := App.objects.filter(**kwargs).first()):
+        raise Exception("App not found")
+
+    return app
+
+
+async def aget_app(pk: str | int) -> App:
+    return await sync_to_async(get_app)(pk)
+
+
+class WebhookException(Exception):
+    pass
+
+
+async def send_webhook(
+    app: str | int | App,
+    type: str,
+    data: Optional[dict | list] = None,
+    user: Optional[str | int | User] = None,
+):
+    from .service import Service
+
+    if not isinstance(app, App):
+        app = await aget_app(app)
+
+    if user and not isinstance(user, User):
+        user = await User.objects.filter(id=user).afirst()
+        if user is None:
+            raise Exception("User not found")
+
+    x = await FirstPartyWebhookLog.objects.acreate(app=app, type=type, data=data)
+    payload = {
+        "type": type,
+        "external_id": x.id,
+        "data": data,
+    }
+
+    user_id = None
+    if user:
+        user_id = user.id
+
+    try:
+        async with Service(app, user_id, proxy=True) as s:
+            response = await s.webhook(payload)
+            if response.status != 200:
+                msg = f"Error calling webhook {app.webhook_url} with status {response.status}"
+
+                # this has relation with a reveived signal not implemented yet
+                x.processed = True
+                x.status = "ERROR"
+                x.status_text = msg
+                x.save()
+
+                raise WebhookException(msg)
+
+    except WebhookException as e:
+        raise e
+
+    except Exception as e:
+        x.delete()
+        raise e
+
+    # this has relation with a reveived signal not implemented yet
+    x.processed = True
+    # this will keep PENDING in the future
+    x.status = "DONE"
+    x.save()
+
+
+def get_user(app: str | int | uuid.UUID, sub: str | int | uuid.UUID) -> User | None:
+    credentials = FirstPartyCredentials.objects.filter(**{f"app__{app}": sub}).select_related("user").first()
+
+    if credentials:
+        return credentials.user
+
+    return create_user(app, sub)
+
+
+async def aget_user(app: str | int | uuid.UUID, sub: str | int | uuid.UUID) -> User | None:
+    credentials = await FirstPartyCredentials.objects.filter(**{f"app__{app}": sub}).select_related("user").afirst()
+
+    if credentials:
+        return credentials.user
+
+    return await acreate_user(app, sub)
+
+
+def create_user(app: str | int | uuid.UUID, sub: str | int | uuid.UUID) -> User | None:
+    from linked_services.django.service import Service
+
+    with Service(app) as s:
+        url = s.app.users_path
+        if url[-1] == "/":
+            url += str(sub)
+
+        else:
+            url += f"/{sub}"
+
+        response = s.get(url)
+
+        if response.status_code >= 300:
+            return None
+
+        data = response.json()
+        mandatory_fields = ["username", "email"]
+        optional_fields = ["first_name", "last_name"]
+        mandatory_attrs = {}
+        optional_attrs = {}
+        errors = []
+
+        if "id" not in data:
+            errors.append("id not provided")
+
+        else:
+            id = data.get("id")
+
+        for field in mandatory_fields:
+            if field in data:
+                mandatory_attrs[field] = data.get(field)
+
+            else:
+                errors.append(f"{field} not provided")
+
+        for field in optional_fields:
+            optional_attrs[field] = data.get(field, "")
+
+        if errors:
+            raise ValidationException(", ".join(errors), slug="missing-required-fields")
+
+        user, created = User.objects.get_or_create(**mandatory_attrs, defaults=optional_attrs)
+        if created:
+            for field in optional_fields:
+                setattr(user, field, optional_attrs[field])
+
+            user.save()
+
+        credentials, created = FirstPartyCredentials.objects.get_or_create(
+            user=user,
+            defaults={
+                "app": {
+                    s.app.slug: id,
+                },
+            },
+        )
+
+        if created is False:
+            credentials.app[s.app.slug] = id
+            credentials.save()
+
+        return user
+
+
+async def acreate_user(app: str | int | uuid.UUID, sub: str | int | uuid.UUID) -> User | None:
+    from linked_services.django.service import Service
+
+    async with Service(app) as s:
+        url = s.app.users_path
+        if url[-1] == "/":
+            url += str(sub)
+
+        else:
+            url += f"/{sub}"
+
+        response = await s.get(url)
+
+        if response.status_code >= 300:
+            return None
+
+        data = await response.json()
+        mandatory_fields = ["username", "email"]
+        optional_fields = ["first_name", "last_name"]
+        mandatory_attrs = {}
+        optional_attrs = {}
+        errors = []
+
+        if "id" not in data:
+            errors.append("id not provided")
+
+        else:
+            id = data.get("id")
+
+        for field in mandatory_fields:
+            if field in data:
+                mandatory_attrs[field] = data.get(field)
+
+            else:
+                errors.append(f"{field} not provided")
+
+        for field in optional_fields:
+            optional_attrs[field] = data.get(field, "")
+
+        if errors:
+            raise ValidationException(", ".join(errors), slug="missing-required-fields")
+
+        user, created = await User.objects.aget_or_create(**mandatory_attrs, defaults=optional_attrs)
+        if created:
+            for field in optional_fields:
+                setattr(user, field, optional_attrs[field])
+
+            await user.asave()
+
+        credentials, created = await FirstPartyCredentials.objects.aget_or_create(
+            user=user,
+            defaults={
+                "app": {
+                    s.app.slug: id,
+                },
+            },
+        )
+
+        if created is False:
+            credentials.app[s.app.slug] = id
+            await credentials.asave()
+
+        return user
```

### Comparing `linked_services-1.2.1/src/linked_services/django/admin.py` & `linked_services-1.2.2/src/linked_services/django/admin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,80 @@
-from django.contrib import admin
-
-from .models import (
-    App,
-    AppOptionalScope,
-    AppRequiredScope,
-    AppUserAgreement,
-    LegacyKey,
-    OptionalScopeSet,
-    Scope,
-)
-
-
-@admin.register(Scope)
-class ScopeAdmin(admin.ModelAdmin):
-    list_display = ("name", "slug")
-    search_fields = ["name", "slug"]
-    actions = []
-
-
-@admin.register(App)
-class AppAdmin(admin.ModelAdmin):
-    list_display = ("name", "slug", "algorithm", "strategy", "schema", "agreement_version", "require_an_agreement")
-    search_fields = ["name", "slug"]
-    list_filter = ["algorithm", "strategy", "schema", "require_an_agreement"]
-
-
-@admin.register(AppRequiredScope)
-class AppRequiredScopeAdmin(admin.ModelAdmin):
-    list_display = ("app", "scope", "agreed_at")
-    search_fields = ["app__name", "app__slug", "scope__name", "scope__slug"]
-    list_filter = ["app", "scope"]
-
-
-@admin.register(AppOptionalScope)
-class AppOptionalScopeAdmin(admin.ModelAdmin):
-    list_display = ("app", "scope", "agreed_at")
-    search_fields = ["app__name", "app__slug", "scope__name", "scope__slug"]
-    list_filter = ["app", "scope"]
-
-
-@admin.register(LegacyKey)
-class LegacyKeyAdmin(admin.ModelAdmin):
-    list_display = ("app", "algorithm", "strategy", "schema")
-    search_fields = ["app__name", "app__slug"]
-    list_filter = ["algorithm", "strategy", "schema"]
-    actions = []
-
-
-@admin.register(OptionalScopeSet)
-class OptionalScopeSetAdmin(admin.ModelAdmin):
-    list_display = ("id",)
-    search_fields = ["optional_scopes__name", "optional_scopes__slug"]
-    actions = []
-
-
-@admin.register(AppUserAgreement)
-class AppUserAgreementAdmin(admin.ModelAdmin):
-    list_display = ("id", "user", "app", "optional_scope_set", "agreement_version")
-    search_fields = ["user__username", "user__email", "user__first_name", "user__last_name", "app__name", "app__slug"]
-    list_filter = ["app"]
-    actions = []
+from django.contrib import admin
+
+from .models import (
+    App,
+    AppOptionalScope,
+    AppRequiredScope,
+    AppUserAgreement,
+    FirstPartyCredentials,
+    FirstPartyWebhookLog,
+    LegacyKey,
+    OptionalScopeSet,
+    Scope,
+)
+
+
+@admin.register(Scope)
+class ScopeAdmin(admin.ModelAdmin):
+    list_display = ("name", "slug")
+    search_fields = ["name", "slug"]
+    actions = []
+
+
+@admin.register(App)
+class AppAdmin(admin.ModelAdmin):
+    list_display = ("name", "slug", "algorithm", "strategy", "schema", "agreement_version", "require_an_agreement")
+    search_fields = ["name", "slug"]
+    list_filter = ["algorithm", "strategy", "schema", "require_an_agreement"]
+
+
+@admin.register(AppRequiredScope)
+class AppRequiredScopeAdmin(admin.ModelAdmin):
+    list_display = ("app", "scope", "agreed_at")
+    search_fields = ["app__name", "app__slug", "scope__name", "scope__slug"]
+    list_filter = ["app", "scope"]
+
+
+@admin.register(AppOptionalScope)
+class AppOptionalScopeAdmin(admin.ModelAdmin):
+    list_display = ("app", "scope", "agreed_at")
+    search_fields = ["app__name", "app__slug", "scope__name", "scope__slug"]
+    list_filter = ["app", "scope"]
+
+
+@admin.register(LegacyKey)
+class LegacyKeyAdmin(admin.ModelAdmin):
+    list_display = ("app", "algorithm", "strategy", "schema")
+    search_fields = ["app__name", "app__slug"]
+    list_filter = ["algorithm", "strategy", "schema"]
+    actions = []
+
+
+@admin.register(OptionalScopeSet)
+class OptionalScopeSetAdmin(admin.ModelAdmin):
+    list_display = ("id",)
+    search_fields = ["optional_scopes__name", "optional_scopes__slug"]
+    actions = []
+
+
+@admin.register(AppUserAgreement)
+class AppUserAgreementAdmin(admin.ModelAdmin):
+    list_display = ("id", "user", "app", "optional_scope_set", "agreement_version")
+    search_fields = ["user__username", "user__email", "user__first_name", "user__last_name", "app__name", "app__slug"]
+    list_filter = ["app"]
+    actions = []
+
+
+@admin.register(FirstPartyWebhookLog)
+class FirstPartyWebhookLogAdmin(admin.ModelAdmin):
+    list_display = ("id", "app", "type", "user_id", "external_id", "url", "processed", "attempts", "status")
+    search_fields = ["user_id", "external_id", "url", "app__name", "app__slug"]
+    list_filter = ["app", "admin", "processed", "status"]
+    actions = []
+
+
+@admin.register(FirstPartyCredentials)
+class FirstPartyCredentialsAdmin(admin.ModelAdmin):
+    list_display = ("id", "user", "app")
+    search_fields = ["user__username", "user__email", "user__first_name", "user__last_name", "app__name", "app__slug"]
+    list_filter = ["app"]
+    actions = []
```

### Comparing `linked_services-1.2.1/src/linked_services/django/models.py` & `linked_services-1.2.2/src/linked_services/django/models.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,424 +1,424 @@
-import re
-import uuid
-from datetime import datetime, timedelta
-
-from django import forms
-from django.contrib.auth.models import User
-from django.db import models
-from slugify import slugify
-
-LEGACY_KEY_LIFETIME = timedelta(minutes=2)
-
-
-class Scope(models.Model):
-    name = models.CharField(
-        max_length=25, unique=True, help_text="Descriptive and unique name that appears on the authorize UI"
-    )
-    slug = models.CharField(max_length=15, unique=True, help_text="{action}:{data} for example read:repo")
-    description = models.CharField(max_length=255, help_text="Description of the scope")
-
-    def clean(self) -> None:
-        if not self.slug:
-            self.slug = slugify(self.name)
-
-        if not self.description:
-            raise forms.ValidationError("Scope description is required")
-
-        if (
-            not self.slug
-            or not re.findall(r"^[a-z_:]+$", self.slug)
-            or (0 < self.slug.count(":") > 1)
-            or self.slug.count("__") > 0
-        ):
-            raise forms.ValidationError(
-                'Scope slug must be in the format "action_name:data_name" or "data_name" example '
-                '"read:repo" or "repo"'
-            )
-
-        return super().clean()
-
-    def save(self, *args, **kwargs):
-        self.full_clean()
-        super().save(*args, **kwargs)
-
-    def __str__(self):
-        return f"{self.name} ({self.slug})"
-
-
-HMAC_SHA256 = "HMAC_SHA256"
-HMAC_SHA512 = "HMAC_SHA512"
-ED25519 = "ED25519"
-AUTH_ALGORITHM = (
-    (HMAC_SHA256, "HMAC-SHA256"),
-    (HMAC_SHA512, "HMAC_SHA512"),
-    (ED25519, "ED25519"),
-)
-
-JWT = "JWT"
-SIGNATURE = "SIGNATURE"
-AUTH_STRATEGY = (
-    (JWT, "Json Web Token"),
-    (SIGNATURE, "Signature"),
-)
-
-LINK = "LINK"
-AUTH_SCHEMA = ((LINK, "Link"),)
-
-SYMMETRIC_ALGORITHMS = [HMAC_SHA256, HMAC_SHA512]
-ASYMMETRIC_ALGORITHMS = [ED25519]
-
-
-class App(models.Model):
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        self._algorithm = self.algorithm
-        self._strategy = self.strategy
-        self._schema = self.schema
-
-        self._private_key = self.private_key
-        self._public_key = self.public_key
-
-        self._webhook_url = self.webhook_url
-        self._redirect_url = self.redirect_url
-
-    name = models.CharField(max_length=25, unique=True, help_text="Descriptive and unique name of the app")
-    slug = models.SlugField(
-        unique=True, help_text="Unique slug for the app, it must be url friendly and please avoid to change it"
-    )
-    description = models.CharField(
-        max_length=255, help_text="Description of the app, it will appear on the authorize UI"
-    )
-
-    algorithm = models.CharField(max_length=11, choices=AUTH_ALGORITHM, default=HMAC_SHA512)
-    strategy = models.CharField(max_length=9, choices=AUTH_STRATEGY, default=JWT)
-    schema = models.CharField(
-        max_length=4,
-        choices=AUTH_SCHEMA,
-        default=LINK,
-        help_text="Schema to use for the auth process to r2epresent how the apps will communicate",
-    )
-
-    required_scopes = models.ManyToManyField(
-        Scope,
-        blank=True,
-        through="AppRequiredScope",
-        through_fields=("app", "scope"),
-        related_name="app_required_scopes",
-    )
-    optional_scopes = models.ManyToManyField(
-        Scope,
-        blank=True,
-        through="AppOptionalScope",
-        through_fields=("app", "scope"),
-        related_name="app_optional_scopes",
-    )
-    agreement_version = models.IntegerField(default=1, help_text="Version of the agreement, based in the scopes")
-
-    private_key = models.CharField(max_length=255, blank=True, null=False)
-    public_key = models.CharField(max_length=255, blank=True, null=True, default=None)
-    require_an_agreement = models.BooleanField(
-        default=True, help_text="If true, the user will be required to accept an agreement"
-    )
-
-    users_path = models.CharField(
-        max_length=200, default="/v1/auth/app/user/", blank=True, help_text="URL path to consult the users"
-    )
-    webhook_url = models.URLField(help_text="URL to receive webhooks")
-    redirect_url = models.URLField(help_text="URL to redirect the user after the authorization")
-    app_url = models.URLField(help_text="URL to the app")
-
-    created_at = models.DateTimeField(auto_now_add=True, editable=False)
-    updated_at = models.DateTimeField(auto_now=True, editable=False)
-
-    def __str__(self):
-        return f"{self.name} ({self.slug})"
-
-    def clean(self) -> None:
-        from .actions import generate_auth_keys
-
-        if not self.slug:
-            self.slug = slugify(self.name)
-
-        if self.public_key and self.algorithm in SYMMETRIC_ALGORITHMS:
-            raise forms.ValidationError("Public key is not required for symmetric algorithms")
-
-        if not self.public_key and not self.private_key:
-            self.public_key, self.private_key = generate_auth_keys(self.algorithm)
-
-        if self.app_url.endswith("/"):
-            self.app_url = self.app_url[:-1]
-
-        return super().clean()
-
-    def save(self, *args, **kwargs):
-        from .actions import reset_app_cache
-
-        had_pk = self.pk
-
-        self.full_clean()
-        super().save(*args, **kwargs)
-
-        if had_pk and (
-            self.private_key != self._private_key
-            or self.public_key != self._public_key
-            or self.algorithm != self._algorithm
-        ):
-            key = LegacyKey()
-            key.app = self
-
-            key.algorithm = self._algorithm
-            key.strategy = self._strategy
-            key.schema = self._schema
-
-            key.private_key = self._private_key
-            key.public_key = self._public_key
-
-            key.webhook_url = self._webhook_url
-            key.redirect_url = self._redirect_url
-
-            key.save()
-
-        if had_pk:
-            reset_app_cache()
-
-        self._algorithm = self.algorithm
-        self._strategy = self.strategy
-        self._schema = self.schema
-
-        self._private_key = self.private_key
-        self._public_key = self.public_key
-
-        self._webhook_url = self.webhook_url
-        self._redirect_url = self.redirect_url
-
-
-class AppRequiredScope(models.Model):
-    app = models.ForeignKey(App, on_delete=models.CASCADE, related_name="m2m_required_scopes")
-    scope = models.ForeignKey(Scope, on_delete=models.CASCADE, related_name="m2m_required_scopes")
-    agreed_at = models.DateTimeField(auto_now_add=True, editable=False)
-
-    def __str__(self):
-        try:
-            return f"{self.app.name} ({self.app.slug}) -> {self.scope.name} ({self.scope.slug})"
-
-        except Exception:
-            return self.pk
-
-
-class AppOptionalScope(models.Model):
-    app = models.ForeignKey(App, on_delete=models.CASCADE, related_name="m2m_optional_scopes")
-    scope = models.ForeignKey(Scope, on_delete=models.CASCADE, related_name="m2m_optional_scopes")
-    agreed_at = models.DateTimeField(auto_now_add=True, editable=False)
-
-    def __str__(self):
-        try:
-            return f"{self.app.name} ({self.app.slug}) -> {self.scope.name} ({self.scope.slug})"
-
-        except Exception:
-            return self.pk
-
-
-class OptionalScopeSet(models.Model):
-    optional_scopes = models.ManyToManyField(Scope, blank=True)
-
-    def save(self, *args, **kwargs):
-        from .actions import reset_app_user_cache
-
-        had_pk = self.pk
-
-        self.full_clean()
-        super().save(*args, **kwargs)
-
-        self.__class__.objects.exclude(app_user_agreement__id__gte=1).exclude(id=self.id).delete()
-
-        if had_pk:
-            reset_app_user_cache()
-
-
-class AppUserAgreement(models.Model):
-
-    user = models.ForeignKey(User, on_delete=models.CASCADE)
-    app = models.ForeignKey(App, on_delete=models.CASCADE)
-    optional_scope_set = models.ForeignKey(
-        OptionalScopeSet, on_delete=models.CASCADE, related_name="app_user_agreement"
-    )
-    agreement_version = models.IntegerField(default=1, help_text="Version of the agreement that was accepted")
-    agreed_at = models.DateTimeField()
-
-    def save(self, *args, **kwargs):
-        from .actions import reset_app_user_cache
-
-        had_pk = self.pk
-
-        self.full_clean()
-        super().save(*args, **kwargs)
-
-        if had_pk:
-            reset_app_user_cache()
-
-
-class LegacyKey(models.Model):
-
-    app = models.OneToOneField(App, on_delete=models.CASCADE, related_name="legacy_key")
-
-    algorithm = models.CharField(max_length=11, choices=AUTH_ALGORITHM)
-    strategy = models.CharField(max_length=9, choices=AUTH_STRATEGY)
-    schema = models.CharField(max_length=4, choices=AUTH_SCHEMA)
-
-    private_key = models.CharField(max_length=255, blank=True, null=False)
-    public_key = models.CharField(max_length=255, blank=True, null=True, default=None)
-
-    webhook_url = models.URLField()
-    redirect_url = models.URLField()
-
-    created_at = models.DateTimeField(auto_now_add=True, editable=False)
-    updated_at = models.DateTimeField(auto_now=True, editable=False)
-
-    def __str__(self):
-        return f"{self.app.name} ({self.app.slug})"
-
-    def clean(self) -> None:
-        if self.public_key and self.algorithm in SYMMETRIC_ALGORITHMS:
-            raise forms.ValidationError("Public key is not required for symmetric algorithms")
-
-        if not self.public_key and not self.private_key:
-            raise forms.ValidationError("Public and private keys are required")
-
-        return super().clean()
-
-    def save(self, *args, **kwargs):
-        from . import tasks
-
-        self.full_clean()
-        super().save(*args, **kwargs)
-
-        tasks.destroy_legacy_key.apply_async(args=(self.id,), eta=datetime.utcnow() + LEGACY_KEY_LIFETIME)
-
-    def delete(self, *args, **kwargs):
-        from . import actions
-
-        r = super().delete(*args, **kwargs)
-        actions.reset_app_cache()
-        return r
-
-
-PENDING = "PENDING"
-# SENT = 'SENT'
-DONE = "DONE"
-ERROR = "ERROR"
-WEBHOOK_STATUSES = (
-    (PENDING, "Pending"),
-    # (SENT, 'Sent'),
-    (DONE, "Done"),
-    (ERROR, "Error"),
-)
-
-
-class FirstPartyWebhookLog(models.Model):
-    """First party credentials."""
-
-    app = models.ForeignKey(App, on_delete=models.CASCADE, help_text="App that triggered or will receive the webhook")
-
-    type = models.CharField(max_length=50, blank=True, default="unknown", help_text="Type of the webhook")
-
-    user_id = models.IntegerField(default=None, null=True, blank=True, help_text="User ID who triggered the webhook")
-    external_id = models.IntegerField(
-        default=None, null=True, blank=True, help_text="External ID where the webhook was triggered"
-    )
-
-    url = models.URLField(default=None, null=True, blank=True, help_text="URL to consult the content")
-    data = models.JSONField(default=dict, blank=True, null=True, help_text="Data received")
-
-    processed = models.BooleanField(default=False, blank=True, help_text="If true, the webhook has been processed")
-    attempts = models.IntegerField(default=0, blank=True, help_text="Number of attempts to process the webhook")
-
-    status = models.CharField(max_length=9, choices=WEBHOOK_STATUSES, default=PENDING, blank=True)
-    status_text = models.CharField(max_length=255, default=None, null=True, blank=True)
-
-    created_at = models.DateTimeField(auto_now_add=True, editable=False)
-    updated_at = models.DateTimeField(auto_now=True, editable=False)
-
-    def clean(self) -> None:
-        from linked_services.core.settings import get_setting
-
-        if self.data and not isinstance(self.data, dict) and not isinstance(self.data, list):
-            raise forms.ValidationError("Data must be a dictionary or a list")
-
-        app_name = get_setting("app_name")
-
-        if self.app and self.app.slug == app_name:
-            raise forms.ValidationError(f"You can't use {app_name} as app")
-
-        if self.attempts < 0:
-            raise forms.ValidationError("Attempts must be a positive integer")
-
-        if self.user_id and self.user_id < 1:
-            raise forms.ValidationError("User ID must be a positive integer")
-
-        if self.type is None:
-            self.type = "unknown"
-
-        return super().clean()
-
-    def save(self, *args, **kwargs):
-        self.full_clean()
-
-        super().save(*args, **kwargs)
-
-
-class FirstPartyCredentials(models.Model):
-    """First party credentials for 4geeks, like Rigobot."""
-
-    user = models.OneToOneField(User, on_delete=models.CASCADE, related_name="credentials")
-    app = models.JSONField(default=dict, blank=True, help_text="Credentials in each app")
-    health_status = models.JSONField(default=dict, blank=True, help_text="Health status of each credentials")
-
-    def clean(self) -> None:
-        from linked_services.core.settings import get_setting
-
-        if not isinstance(self.app, dict):
-            raise forms.ValidationError("App must be a dictionary")
-
-        apps = self.app.keys()
-        app_name = get_setting("app_name")
-        for app in apps:
-            t = type(self.app[app])
-            if app == app_name:
-                raise forms.ValidationError(f"You can't use {app_name} as app, app names must be unique")
-
-            if t not in [int, str, uuid.UUID]:
-                raise forms.ValidationError(
-                    f"app['{app}'] credential must be an integer, string or UUID, but got {t.__name__}"
-                )
-
-            if t is int and self.app[app] < 1:
-                raise forms.ValidationError(f"app['{app}'] credential must be a positive integer")
-
-        self._apps = apps
-
-        return super().clean()
-
-    def save(self, *args, **kwargs):
-        from linked_services.django import tasks
-
-        if not self.health_status:
-            self.health_status = {}
-
-        self.full_clean()
-
-        super().save(*args, **kwargs)
-
-        to_check = []
-
-        for app in self._apps:
-            if (
-                app not in self.health_status
-                or self.health_status[app]["id"] != self.app[app]
-                or self.health_status[app]["status"] != "HEALTHY"
-            ):
-                to_check.append(app)
-
-        if to_check:
-            tasks.check_credentials.delay(self.user.id, to_check)
+import re
+import uuid
+from datetime import datetime, timedelta
+
+from django import forms
+from django.contrib.auth.models import User
+from django.db import models
+from slugify import slugify
+
+LEGACY_KEY_LIFETIME = timedelta(minutes=2)
+
+
+class Scope(models.Model):
+    name = models.CharField(
+        max_length=25, unique=True, help_text="Descriptive and unique name that appears on the authorize UI"
+    )
+    slug = models.CharField(max_length=15, unique=True, help_text="{action}:{data} for example read:repo")
+    description = models.CharField(max_length=255, help_text="Description of the scope")
+
+    def clean(self) -> None:
+        if not self.slug:
+            self.slug = slugify(self.name)
+
+        if not self.description:
+            raise forms.ValidationError("Scope description is required")
+
+        if (
+            not self.slug
+            or not re.findall(r"^[a-z_:]+$", self.slug)
+            or (0 < self.slug.count(":") > 1)
+            or self.slug.count("__") > 0
+        ):
+            raise forms.ValidationError(
+                'Scope slug must be in the format "action_name:data_name" or "data_name" example '
+                '"read:repo" or "repo"'
+            )
+
+        return super().clean()
+
+    def save(self, *args, **kwargs):
+        self.full_clean()
+        super().save(*args, **kwargs)
+
+    def __str__(self):
+        return f"{self.name} ({self.slug})"
+
+
+HMAC_SHA256 = "HMAC_SHA256"
+HMAC_SHA512 = "HMAC_SHA512"
+ED25519 = "ED25519"
+AUTH_ALGORITHM = (
+    (HMAC_SHA256, "HMAC-SHA256"),
+    (HMAC_SHA512, "HMAC_SHA512"),
+    (ED25519, "ED25519"),
+)
+
+JWT = "JWT"
+SIGNATURE = "SIGNATURE"
+AUTH_STRATEGY = (
+    (JWT, "Json Web Token"),
+    (SIGNATURE, "Signature"),
+)
+
+LINK = "LINK"
+AUTH_SCHEMA = ((LINK, "Link"),)
+
+SYMMETRIC_ALGORITHMS = [HMAC_SHA256, HMAC_SHA512]
+ASYMMETRIC_ALGORITHMS = [ED25519]
+
+
+class App(models.Model):
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self._algorithm = self.algorithm
+        self._strategy = self.strategy
+        self._schema = self.schema
+
+        self._private_key = self.private_key
+        self._public_key = self.public_key
+
+        self._webhook_url = self.webhook_url
+        self._redirect_url = self.redirect_url
+
+    name = models.CharField(max_length=25, unique=True, help_text="Descriptive and unique name of the app")
+    slug = models.SlugField(
+        unique=True, help_text="Unique slug for the app, it must be url friendly and please avoid to change it"
+    )
+    description = models.CharField(
+        max_length=255, help_text="Description of the app, it will appear on the authorize UI"
+    )
+
+    algorithm = models.CharField(max_length=11, choices=AUTH_ALGORITHM, default=HMAC_SHA512)
+    strategy = models.CharField(max_length=9, choices=AUTH_STRATEGY, default=JWT)
+    schema = models.CharField(
+        max_length=4,
+        choices=AUTH_SCHEMA,
+        default=LINK,
+        help_text="Schema to use for the auth process to r2epresent how the apps will communicate",
+    )
+
+    required_scopes = models.ManyToManyField(
+        Scope,
+        blank=True,
+        through="AppRequiredScope",
+        through_fields=("app", "scope"),
+        related_name="app_required_scopes",
+    )
+    optional_scopes = models.ManyToManyField(
+        Scope,
+        blank=True,
+        through="AppOptionalScope",
+        through_fields=("app", "scope"),
+        related_name="app_optional_scopes",
+    )
+    agreement_version = models.IntegerField(default=1, help_text="Version of the agreement, based in the scopes")
+
+    private_key = models.CharField(max_length=255, blank=True, null=False)
+    public_key = models.CharField(max_length=255, blank=True, null=True, default=None)
+    require_an_agreement = models.BooleanField(
+        default=True, help_text="If true, the user will be required to accept an agreement"
+    )
+
+    users_path = models.CharField(
+        max_length=200, default="/v1/auth/app/user/", blank=True, help_text="URL path to consult the users"
+    )
+    webhook_url = models.URLField(help_text="URL to receive webhooks")
+    redirect_url = models.URLField(help_text="URL to redirect the user after the authorization")
+    app_url = models.URLField(help_text="URL to the app")
+
+    created_at = models.DateTimeField(auto_now_add=True, editable=False)
+    updated_at = models.DateTimeField(auto_now=True, editable=False)
+
+    def __str__(self):
+        return f"{self.name} ({self.slug})"
+
+    def clean(self) -> None:
+        from .actions import generate_auth_keys
+
+        if not self.slug:
+            self.slug = slugify(self.name)
+
+        if self.public_key and self.algorithm in SYMMETRIC_ALGORITHMS:
+            raise forms.ValidationError("Public key is not required for symmetric algorithms")
+
+        if not self.public_key and not self.private_key:
+            self.public_key, self.private_key = generate_auth_keys(self.algorithm)
+
+        if self.app_url.endswith("/"):
+            self.app_url = self.app_url[:-1]
+
+        return super().clean()
+
+    def save(self, *args, **kwargs):
+        from .actions import reset_app_cache
+
+        had_pk = self.pk
+
+        self.full_clean()
+        super().save(*args, **kwargs)
+
+        if had_pk and (
+            self.private_key != self._private_key
+            or self.public_key != self._public_key
+            or self.algorithm != self._algorithm
+        ):
+            key = LegacyKey()
+            key.app = self
+
+            key.algorithm = self._algorithm
+            key.strategy = self._strategy
+            key.schema = self._schema
+
+            key.private_key = self._private_key
+            key.public_key = self._public_key
+
+            key.webhook_url = self._webhook_url
+            key.redirect_url = self._redirect_url
+
+            key.save()
+
+        if had_pk:
+            reset_app_cache()
+
+        self._algorithm = self.algorithm
+        self._strategy = self.strategy
+        self._schema = self.schema
+
+        self._private_key = self.private_key
+        self._public_key = self.public_key
+
+        self._webhook_url = self.webhook_url
+        self._redirect_url = self.redirect_url
+
+
+class AppRequiredScope(models.Model):
+    app = models.ForeignKey(App, on_delete=models.CASCADE, related_name="m2m_required_scopes")
+    scope = models.ForeignKey(Scope, on_delete=models.CASCADE, related_name="m2m_required_scopes")
+    agreed_at = models.DateTimeField(auto_now_add=True, editable=False)
+
+    def __str__(self):
+        try:
+            return f"{self.app.name} ({self.app.slug}) -> {self.scope.name} ({self.scope.slug})"
+
+        except Exception:
+            return self.pk
+
+
+class AppOptionalScope(models.Model):
+    app = models.ForeignKey(App, on_delete=models.CASCADE, related_name="m2m_optional_scopes")
+    scope = models.ForeignKey(Scope, on_delete=models.CASCADE, related_name="m2m_optional_scopes")
+    agreed_at = models.DateTimeField(auto_now_add=True, editable=False)
+
+    def __str__(self):
+        try:
+            return f"{self.app.name} ({self.app.slug}) -> {self.scope.name} ({self.scope.slug})"
+
+        except Exception:
+            return self.pk
+
+
+class OptionalScopeSet(models.Model):
+    optional_scopes = models.ManyToManyField(Scope, blank=True)
+
+    def save(self, *args, **kwargs):
+        from .actions import reset_app_user_cache
+
+        had_pk = self.pk
+
+        self.full_clean()
+        super().save(*args, **kwargs)
+
+        self.__class__.objects.exclude(app_user_agreement__id__gte=1).exclude(id=self.id).delete()
+
+        if had_pk:
+            reset_app_user_cache()
+
+
+class AppUserAgreement(models.Model):
+
+    user = models.ForeignKey(User, on_delete=models.CASCADE)
+    app = models.ForeignKey(App, on_delete=models.CASCADE)
+    optional_scope_set = models.ForeignKey(
+        OptionalScopeSet, on_delete=models.CASCADE, related_name="app_user_agreement"
+    )
+    agreement_version = models.IntegerField(default=1, help_text="Version of the agreement that was accepted")
+    agreed_at = models.DateTimeField()
+
+    def save(self, *args, **kwargs):
+        from .actions import reset_app_user_cache
+
+        had_pk = self.pk
+
+        self.full_clean()
+        super().save(*args, **kwargs)
+
+        if had_pk:
+            reset_app_user_cache()
+
+
+class LegacyKey(models.Model):
+
+    app = models.OneToOneField(App, on_delete=models.CASCADE, related_name="legacy_key")
+
+    algorithm = models.CharField(max_length=11, choices=AUTH_ALGORITHM)
+    strategy = models.CharField(max_length=9, choices=AUTH_STRATEGY)
+    schema = models.CharField(max_length=4, choices=AUTH_SCHEMA)
+
+    private_key = models.CharField(max_length=255, blank=True, null=False)
+    public_key = models.CharField(max_length=255, blank=True, null=True, default=None)
+
+    webhook_url = models.URLField()
+    redirect_url = models.URLField()
+
+    created_at = models.DateTimeField(auto_now_add=True, editable=False)
+    updated_at = models.DateTimeField(auto_now=True, editable=False)
+
+    def __str__(self):
+        return f"{self.app.name} ({self.app.slug})"
+
+    def clean(self) -> None:
+        if self.public_key and self.algorithm in SYMMETRIC_ALGORITHMS:
+            raise forms.ValidationError("Public key is not required for symmetric algorithms")
+
+        if not self.public_key and not self.private_key:
+            raise forms.ValidationError("Public and private keys are required")
+
+        return super().clean()
+
+    def save(self, *args, **kwargs):
+        from . import tasks
+
+        self.full_clean()
+        super().save(*args, **kwargs)
+
+        tasks.destroy_legacy_key.apply_async(args=(self.id,), eta=datetime.utcnow() + LEGACY_KEY_LIFETIME)
+
+    def delete(self, *args, **kwargs):
+        from . import actions
+
+        r = super().delete(*args, **kwargs)
+        actions.reset_app_cache()
+        return r
+
+
+PENDING = "PENDING"
+# SENT = 'SENT'
+DONE = "DONE"
+ERROR = "ERROR"
+WEBHOOK_STATUSES = (
+    (PENDING, "Pending"),
+    # (SENT, 'Sent'),
+    (DONE, "Done"),
+    (ERROR, "Error"),
+)
+
+
+class FirstPartyWebhookLog(models.Model):
+    """First party credentials."""
+
+    app = models.ForeignKey(App, on_delete=models.CASCADE, help_text="App that triggered or will receive the webhook")
+
+    type = models.CharField(max_length=50, blank=True, default="unknown", help_text="Type of the webhook")
+
+    user_id = models.IntegerField(default=None, null=True, blank=True, help_text="User ID who triggered the webhook")
+    external_id = models.IntegerField(
+        default=None, null=True, blank=True, help_text="External ID where the webhook was triggered"
+    )
+
+    url = models.URLField(default=None, null=True, blank=True, help_text="URL to consult the content")
+    data = models.JSONField(default=dict, blank=True, null=True, help_text="Data received")
+
+    processed = models.BooleanField(default=False, blank=True, help_text="If true, the webhook has been processed")
+    attempts = models.IntegerField(default=0, blank=True, help_text="Number of attempts to process the webhook")
+
+    status = models.CharField(max_length=9, choices=WEBHOOK_STATUSES, default=PENDING, blank=True)
+    status_text = models.CharField(max_length=255, default=None, null=True, blank=True)
+
+    created_at = models.DateTimeField(auto_now_add=True, editable=False)
+    updated_at = models.DateTimeField(auto_now=True, editable=False)
+
+    def clean(self) -> None:
+        from linked_services.core.settings import get_setting
+
+        if self.data and not isinstance(self.data, dict) and not isinstance(self.data, list):
+            raise forms.ValidationError("Data must be a dictionary or a list")
+
+        app_name = get_setting("app_name")
+
+        if self.app and self.app.slug == app_name:
+            raise forms.ValidationError(f"You can't use {app_name} as app")
+
+        if self.attempts < 0:
+            raise forms.ValidationError("Attempts must be a positive integer")
+
+        if self.user_id and self.user_id < 1:
+            raise forms.ValidationError("User ID must be a positive integer")
+
+        if self.type is None:
+            self.type = "unknown"
+
+        return super().clean()
+
+    def save(self, *args, **kwargs):
+        self.full_clean()
+
+        super().save(*args, **kwargs)
+
+
+class FirstPartyCredentials(models.Model):
+    """First party credentials for 4geeks, like Rigobot."""
+
+    user = models.OneToOneField(User, on_delete=models.CASCADE, related_name="credentials")
+    app = models.JSONField(default=dict, blank=True, help_text="Credentials in each app")
+    health_status = models.JSONField(default=dict, blank=True, help_text="Health status of each credentials")
+
+    def clean(self) -> None:
+        from linked_services.core.settings import get_setting
+
+        if not isinstance(self.app, dict):
+            raise forms.ValidationError("App must be a dictionary")
+
+        apps = self.app.keys()
+        app_name = get_setting("app_name")
+        for app in apps:
+            t = type(self.app[app])
+            if app == app_name:
+                raise forms.ValidationError(f"You can't use {app_name} as app, app names must be unique")
+
+            if t not in [int, str, uuid.UUID]:
+                raise forms.ValidationError(
+                    f"app['{app}'] credential must be an integer, string or UUID, but got {t.__name__}"
+                )
+
+            if t is int and self.app[app] < 1:
+                raise forms.ValidationError(f"app['{app}'] credential must be a positive integer")
+
+        self._apps = apps
+
+        return super().clean()
+
+    def save(self, *args, **kwargs):
+        from linked_services.django import tasks
+
+        if not self.health_status:
+            self.health_status = {}
+
+        self.full_clean()
+
+        super().save(*args, **kwargs)
+
+        to_check = []
+
+        for app in self._apps:
+            if (
+                app not in self.health_status
+                or self.health_status[app]["id"] != self.app[app]
+                or self.health_status[app]["status"] != "HEALTHY"
+            ):
+                to_check.append(app)
+
+        if to_check:
+            tasks.check_credentials.delay(self.user.id, to_check)
```

### Comparing `linked_services-1.2.1/src/linked_services/django/receivers.py` & `linked_services-1.2.2/src/linked_services/django/receivers.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from typing import Type
-
-from django.db.models.signals import post_save, pre_delete
-from django.dispatch import receiver
-
-from .models import AppOptionalScope, AppRequiredScope, AppUserAgreement
-from .signals import app_scope_updated
-
-
-@receiver(post_save, sender=AppRequiredScope)
-def increment_on_update_required_scope(sender: Type[AppRequiredScope], instance: AppRequiredScope, **_):
-    app_scope_updated.send(sender=sender, instance=instance)
-
-
-@receiver(post_save, sender=AppOptionalScope)
-def increment_on_update_optional_scope(sender: Type[AppOptionalScope], instance: AppOptionalScope, **_):
-    app_scope_updated.send(sender=sender, instance=instance)
-
-
-@receiver(pre_delete, sender=AppRequiredScope)
-def increment_on_delete_required_scope(sender: Type[AppRequiredScope], instance: AppRequiredScope, **_):
-    app_scope_updated.send(sender=sender, instance=instance)
-
-
-@receiver(pre_delete, sender=AppOptionalScope)
-def increment_on_delete_optional_scope(sender: Type[AppOptionalScope], instance: AppOptionalScope, **_):
-    app_scope_updated.send(sender=sender, instance=instance)
-
-
-@receiver(app_scope_updated)
-def update_app_scope(
-    sender: Type[AppOptionalScope | AppRequiredScope], instance: AppOptionalScope | AppRequiredScope, **_
-):
-    if AppUserAgreement.objects.filter(app=instance.app, agreement_version=instance.app.agreement_version).exists():
-        instance.app.agreement_version += 1
-        instance.app.save()
+from typing import Type
+
+from django.db.models.signals import post_save, pre_delete
+from django.dispatch import receiver
+
+from .models import AppOptionalScope, AppRequiredScope, AppUserAgreement
+from .signals import app_scope_updated
+
+
+@receiver(post_save, sender=AppRequiredScope)
+def increment_on_update_required_scope(sender: Type[AppRequiredScope], instance: AppRequiredScope, **_):
+    app_scope_updated.send(sender=sender, instance=instance)
+
+
+@receiver(post_save, sender=AppOptionalScope)
+def increment_on_update_optional_scope(sender: Type[AppOptionalScope], instance: AppOptionalScope, **_):
+    app_scope_updated.send(sender=sender, instance=instance)
+
+
+@receiver(pre_delete, sender=AppRequiredScope)
+def increment_on_delete_required_scope(sender: Type[AppRequiredScope], instance: AppRequiredScope, **_):
+    app_scope_updated.send(sender=sender, instance=instance)
+
+
+@receiver(pre_delete, sender=AppOptionalScope)
+def increment_on_delete_optional_scope(sender: Type[AppOptionalScope], instance: AppOptionalScope, **_):
+    app_scope_updated.send(sender=sender, instance=instance)
+
+
+@receiver(app_scope_updated)
+def update_app_scope(
+    sender: Type[AppOptionalScope | AppRequiredScope], instance: AppOptionalScope | AppRequiredScope, **_
+):
+    if AppUserAgreement.objects.filter(app=instance.app, agreement_version=instance.app.agreement_version).exists():
+        instance.app.agreement_version += 1
+        instance.app.save()
```

### Comparing `linked_services-1.2.1/src/linked_services/django/tasks.py` & `linked_services-1.2.2/src/linked_services/django/tasks.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-import logging
-import os
-
-from django.contrib.auth.models import User
-from task_manager.core.exceptions import AbortTask, RetryTask
-from task_manager.django.decorators import task
-
-from linked_services.django.actions import get_app
-from linked_services.django.models import FirstPartyCredentials, FirstPartyWebhookLog
-from linked_services.django.service import Service
-
-logger = logging.getLogger(__name__)
-settings = {}
-
-if p := os.getenv("OAUTH_CREDENTIALS_PRIORITY"):
-    settings["priority"] = int(p)
-
-else:
-    settings["priority"] = 5
-
-
-@task(**settings)
-def destroy_legacy_key(legacy_key_id, **_):
-    from .models import LegacyKey
-
-    LegacyKey.objects.filter(id=legacy_key_id).delete()
-
-
-@task(**settings)
-def check_credentials(user_id: int, check=None, **_):
-
-    def error(app_name: str, credentials: FirstPartyCredentials, status="NOT_FOUND"):
-        credentials.health_status[app_name] = {"id": credentials.app[app_name], "status": status}
-        del credentials.app[app_name]
-        credentials.save()
-
-    logger.info("Running check_credentials task")
-
-    if check is None:
-        raise AbortTask("Nothing to check")
-
-    if not (
-        credentials := FirstPartyCredentials.objects.filter(user__id=user_id)
-        .only("health_status", "app", "user__email")
-        .first()
-    ):
-        raise RetryTask("FirstPartyCredentials not found")
-
-    for app_name in check:
-        if credentials.app.get(app_name, None) is None:
-            save = False
-            if app_name in credentials.health_status:
-                del credentials.health_status[app_name]
-                save = True
-
-            if app_name in credentials.app:
-                del credentials.app[app_name]
-                save = True
-
-            if save:
-                credentials.save()
-
-            return
-
-        else:
-            try:
-                app = get_app(app_name)
-
-            except Exception:
-                # logger.error(f"App {app_name} not found")
-                error(app_name, credentials, status="APP_NOT_FOUND")
-                continue
-
-            with Service(app) as s:
-                response = s.get(f"{s.app.users_path}?email={credentials.user.email}&id={credentials.app[app_name]}")
-
-                if response.status_code != 200:
-                    return error(app_name, credentials)
-
-                json = response.json()
-                if not isinstance(json, list) or len(json) == 0:
-                    return error(app_name, credentials)
-
-                else:
-                    credentials.health_status[app_name] = {"id": credentials.app[app_name], "status": "HEALTHY"}
-                    credentials.save()
-
-
-@task(**settings)
-def import_external_user(webhook_id: int, **_):
-    logger.info("Running check_credentials task")
-
-    webhook = FirstPartyWebhookLog.objects.filter(id=webhook_id).first()
-    if webhook is None:
-        raise AbortTask("Webhook not found")
-
-    if webhook.data is None or not isinstance(webhook.data, dict):
-        logger.error(f"Webhook {webhook.type} requires a data field as json")
-        return
-
-    errors = []
-    for field in ["id", "email", "first_name", "last_name"]:
-        if field not in webhook.data:
-            errors.append(field)
-
-    if len(errors) > 0:
-        format = ", ".join(["data." + x for x in errors])
-        logger.error(f"Webhook {webhook.type} requires a data field as json with the following fields: {format}")
-        return
-
-    app = webhook.app
-
-    if User.objects.filter(**{f"credentials__app__{app.slug}": webhook.data["id"]}).exists():
-        return
-
-    user = User.objects.filter(email=webhook.data["email"]).first()
-    if user is None:
-        user = User.objects.create(
-            email=webhook.data["email"],
-            username=webhook.data["email"],
-            first_name=webhook.data["first_name"],
-            last_name=webhook.data["last_name"],
-            is_active=True,
-        )
-
-        instance, created = FirstPartyCredentials.objects.get_or_create(
-            user=user,
-            defaults={
-                "app": {
-                    app.slug: webhook.data["id"],
-                },
-            },
-        )
-
-        if not created:
-            instance.app[app.slug] = webhook.data["id"]
-            instance.save()
+import logging
+import os
+
+from django.contrib.auth.models import User
+from task_manager.core.exceptions import AbortTask, RetryTask
+from task_manager.django.decorators import task
+
+from linked_services.django.actions import get_app
+from linked_services.django.models import FirstPartyCredentials, FirstPartyWebhookLog
+from linked_services.django.service import Service
+
+logger = logging.getLogger(__name__)
+settings = {}
+
+if p := os.getenv("OAUTH_CREDENTIALS_PRIORITY"):
+    settings["priority"] = int(p)
+
+else:
+    settings["priority"] = 5
+
+
+@task(**settings)
+def destroy_legacy_key(legacy_key_id, **_):
+    from .models import LegacyKey
+
+    LegacyKey.objects.filter(id=legacy_key_id).delete()
+
+
+@task(**settings)
+def check_credentials(user_id: int, check=None, **_):
+
+    def error(app_name: str, credentials: FirstPartyCredentials, status="NOT_FOUND"):
+        credentials.health_status[app_name] = {"id": credentials.app[app_name], "status": status}
+        del credentials.app[app_name]
+        credentials.save()
+
+    logger.info("Running check_credentials task")
+
+    if check is None:
+        raise AbortTask("Nothing to check")
+
+    if not (
+        credentials := FirstPartyCredentials.objects.filter(user__id=user_id)
+        .only("health_status", "app", "user__email")
+        .first()
+    ):
+        raise RetryTask("FirstPartyCredentials not found")
+
+    for app_name in check:
+        if credentials.app.get(app_name, None) is None:
+            save = False
+            if app_name in credentials.health_status:
+                del credentials.health_status[app_name]
+                save = True
+
+            if app_name in credentials.app:
+                del credentials.app[app_name]
+                save = True
+
+            if save:
+                credentials.save()
+
+            return
+
+        else:
+            try:
+                app = get_app(app_name)
+
+            except Exception:
+                # logger.error(f"App {app_name} not found")
+                error(app_name, credentials, status="APP_NOT_FOUND")
+                continue
+
+            with Service(app) as s:
+                response = s.get(f"{s.app.users_path}?email={credentials.user.email}&id={credentials.app[app_name]}")
+
+                if response.status_code != 200:
+                    return error(app_name, credentials)
+
+                json = response.json()
+                if not isinstance(json, list) or len(json) == 0:
+                    return error(app_name, credentials)
+
+                else:
+                    credentials.health_status[app_name] = {"id": credentials.app[app_name], "status": "HEALTHY"}
+                    credentials.save()
+
+
+@task(**settings)
+def import_external_user(webhook_id: int, **_):
+    logger.info("Running check_credentials task")
+
+    webhook = FirstPartyWebhookLog.objects.filter(id=webhook_id).first()
+    if webhook is None:
+        raise AbortTask("Webhook not found")
+
+    if webhook.data is None or not isinstance(webhook.data, dict):
+        logger.error(f"Webhook {webhook.type} requires a data field as json")
+        return
+
+    errors = []
+    for field in ["id", "email", "first_name", "last_name"]:
+        if field not in webhook.data:
+            errors.append(field)
+
+    if len(errors) > 0:
+        format = ", ".join(["data." + x for x in errors])
+        logger.error(f"Webhook {webhook.type} requires a data field as json with the following fields: {format}")
+        return
+
+    app = webhook.app
+
+    if User.objects.filter(**{f"credentials__app__{app.slug}": webhook.data["id"]}).exists():
+        return
+
+    user = User.objects.filter(email=webhook.data["email"]).first()
+    if user is None:
+        user = User.objects.create(
+            email=webhook.data["email"],
+            username=webhook.data["email"],
+            first_name=webhook.data["first_name"],
+            last_name=webhook.data["last_name"],
+            is_active=True,
+        )
+
+        instance, created = FirstPartyCredentials.objects.get_or_create(
+            user=user,
+            defaults={
+                "app": {
+                    app.slug: webhook.data["id"],
+                },
+            },
+        )
+
+        if not created:
+            instance.app[app.slug] = webhook.data["id"]
+            instance.save()
```

### Comparing `linked_services-1.2.1/src/linked_services/management/commands/first_party_webhooks.py` & `linked_services-1.2.2/src/linked_services/management/commands/first_party_webhooks.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import logging
-from datetime import timedelta
-
-from django.core.management.base import BaseCommand
-from django.db.models import Q
-from django.utils import timezone
-
-from linked_services.django import tasks
-from linked_services.django.models import FirstPartyWebhookLog
-
-logger = logging.getLogger(__name__)
-
-
-class Command(BaseCommand):
-    help = "Manage first party webhooks"
-
-    def route(self, webhook: FirstPartyWebhookLog):
-        if webhook.type == "user.created" or webhook.type == "user.updated":
-            return tasks.import_external_user.delay(webhook.id)
-
-        webhook.status = "ERROR"
-        webhook.status_text = "Invalid webhook type"
-        webhook.save()
-
-    def handle(self, *args, **options):
-        now = timezone.now()
-
-        newest = FirstPartyWebhookLog.objects.filter(attempts=0, status="PENDING", external_id__isnull=False).only(
-            "id", "type"
-        )
-        retries = (
-            FirstPartyWebhookLog.objects.filter(
-                updated_at__lte=now - timedelta(minutes=20), status="PENDING", external_id__isnull=False
-            )
-            .exclude(Q(attempts__gt=5) | Q(attempts=0))
-            .only("id", "type")
-        )
-
-        for retry in retries:
-            self.route(retry)
-
-        for new in newest:
-            self.route(new)
+import logging
+from datetime import timedelta
+
+from django.core.management.base import BaseCommand
+from django.db.models import Q
+from django.utils import timezone
+
+from linked_services.django import tasks
+from linked_services.django.models import FirstPartyWebhookLog
+
+logger = logging.getLogger(__name__)
+
+
+class Command(BaseCommand):
+    help = "Manage first party webhooks"
+
+    def route(self, webhook: FirstPartyWebhookLog):
+        if webhook.type == "user.created" or webhook.type == "user.updated":
+            return tasks.import_external_user.delay(webhook.id)
+
+        webhook.status = "ERROR"
+        webhook.status_text = "Invalid webhook type"
+        webhook.save()
+
+    def handle(self, *args, **options):
+        now = timezone.now()
+
+        newest = FirstPartyWebhookLog.objects.filter(attempts=0, status="PENDING", external_id__isnull=False).only(
+            "id", "type"
+        )
+        retries = (
+            FirstPartyWebhookLog.objects.filter(
+                updated_at__lte=now - timedelta(minutes=20), status="PENDING", external_id__isnull=False
+            )
+            .exclude(Q(attempts__gt=5) | Q(attempts=0))
+            .only("id", "type")
+        )
+
+        for retry in retries:
+            self.route(retry)
+
+        for new in newest:
+            self.route(new)
```

### Comparing `linked_services-1.2.1/src/linked_services/management/commands/sign_request.py` & `linked_services-1.2.2/src/linked_services/management/commands/sign_request.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from django.core.management.base import BaseCommand
-
-
-class Command(BaseCommand):
-    help = "Sign a request with a symmetric key"
-
-    def add_arguments(self, parser):
-        parser.add_argument("app", nargs="?", type=int)
-        parser.add_argument("user", nargs="?", type=int)
-        parser.add_argument("method", nargs="?", type=str)
-        parser.add_argument("params", nargs="?", type=str)
-        parser.add_argument("body", nargs="?", type=str)
-        parser.add_argument("headers", nargs="?", type=str)
-
-    def handle(self, *args, **options):
-        from linked_services.django.actions import get_signature
-
-        from ...models import App
-
-        if not options["app"]:
-            raise Exception("Missing app id")
-
-        options["method"] = options["method"] if options["method"] is not None else "get"
-        options["params"] = eval(options["params"]) if options["params"] is not None else {}
-        options["body"] = eval(options["body"]) if options["body"] is not None else None
-        options["headers"] = eval(options["headers"]) if options["headers"] is not None else {}
-
-        try:
-            app = App.objects.get(id=options["app"])
-
-        except App.DoesNotExist:
-            self.stderr.write(self.style.ERROR(f'App {options["app"]} not found'))
-            return
-
-        sign, now = get_signature(
-            app,
-            options["user"],
-            method=options["method"],
-            params=options["params"],
-            body=options["body"],
-            headers=options["headers"],
-            reverse=True,
-        )
-
-        self.stdout.write(
-            f"Authorization: Signature App={app.slug},"
-            f"Nonce={sign},"
-            f'SignedHeaders={";".join(options["headers"])},'
-            f"Date={now}"
-        )
+from django.core.management.base import BaseCommand
+
+
+class Command(BaseCommand):
+    help = "Sign a request with a symmetric key"
+
+    def add_arguments(self, parser):
+        parser.add_argument("app", nargs="?", type=int)
+        parser.add_argument("user", nargs="?", type=int)
+        parser.add_argument("method", nargs="?", type=str)
+        parser.add_argument("params", nargs="?", type=str)
+        parser.add_argument("body", nargs="?", type=str)
+        parser.add_argument("headers", nargs="?", type=str)
+
+    def handle(self, *args, **options):
+        from linked_services.django.actions import get_signature
+
+        from ...models import App
+
+        if not options["app"]:
+            raise Exception("Missing app id")
+
+        options["method"] = options["method"] if options["method"] is not None else "get"
+        options["params"] = eval(options["params"]) if options["params"] is not None else {}
+        options["body"] = eval(options["body"]) if options["body"] is not None else None
+        options["headers"] = eval(options["headers"]) if options["headers"] is not None else {}
+
+        try:
+            app = App.objects.get(id=options["app"])
+
+        except App.DoesNotExist:
+            self.stderr.write(self.style.ERROR(f'App {options["app"]} not found'))
+            return
+
+        sign, now = get_signature(
+            app,
+            options["user"],
+            method=options["method"],
+            params=options["params"],
+            body=options["body"],
+            headers=options["headers"],
+            reverse=True,
+        )
+
+        self.stdout.write(
+            f"Authorization: Signature App={app.slug},"
+            f"Nonce={sign},"
+            f'SignedHeaders={";".join(options["headers"])},'
+            f"Date={now}"
+        )
```

### Comparing `linked_services-1.2.1/src/linked_services/rest_framework/types.py` & `linked_services-1.2.2/src/linked_services/rest_framework/types.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-import uuid
-
-from adrf.requests import AsyncRequest as BaseAsyncRequest
-from django.contrib.auth.models import User
-from django.http.request import HttpRequest as BaseHttpRequest
-
-
-class AsyncLinkedHttpRequest(BaseAsyncRequest):
-    def __init__(self, *args, **kwargs):
-        raise Exception("This AsyncRequest class cannot be instantiated, you must use adrf.requests.AsyncRequest")
-
-    async def get_user() -> User | None:
-        pass
-
-
-class LinkedHttpRequest(BaseHttpRequest):
-    def __init__(self, *args, **kwargs):
-        raise Exception("This AsyncRequest class cannot be instantiated, you must use django.http.request.HttpRequest")
-
-    def get_user() -> User | None:
-        pass
-
-
-class LinkedToken:
-    def __init__(self, *args, **kwargs):
-        raise Exception("This class cannot be instantiated")
-
-    sub: int | str | uuid.UUID
-    iss: str
-    app: str
-    aud: str
-    exp: float
-    iat: float
-    typ: str
-
-
-class LinkedApp:
-    def __init__(self, *args, **kwargs):
-        raise Exception("This class cannot be instantiated")
-
-    id: int | str | uuid.UUID
-    private_key: bytes
-    public_key: bytes | None
-    algorithm: str
-    strategy: str
-    schema: str
-    schema: str
-    require_an_agreement: bool
-    webhook_url: float
-    redirect_url: float
-    app_url: float
-
-
-class LinkedApplication(LinkedApp):
-    pass
+import uuid
+
+from adrf.requests import AsyncRequest as BaseAsyncRequest
+from django.contrib.auth.models import User
+from django.http.request import HttpRequest as BaseHttpRequest
+
+
+class AsyncLinkedHttpRequest(BaseAsyncRequest):
+    def __init__(self, *args, **kwargs):
+        raise Exception("This AsyncRequest class cannot be instantiated, you must use adrf.requests.AsyncRequest")
+
+    async def get_user() -> User | None:
+        pass
+
+
+class LinkedHttpRequest(BaseHttpRequest):
+    def __init__(self, *args, **kwargs):
+        raise Exception("This AsyncRequest class cannot be instantiated, you must use django.http.request.HttpRequest")
+
+    def get_user() -> User | None:
+        pass
+
+
+class LinkedToken:
+    def __init__(self, *args, **kwargs):
+        raise Exception("This class cannot be instantiated")
+
+    sub: int | str | uuid.UUID
+    iss: str
+    app: str
+    aud: str
+    exp: float
+    iat: float
+    typ: str
+
+
+class LinkedApp:
+    def __init__(self, *args, **kwargs):
+        raise Exception("This class cannot be instantiated")
+
+    id: int | str | uuid.UUID
+    private_key: bytes
+    public_key: bytes | None
+    algorithm: str
+    strategy: str
+    schema: str
+    schema: str
+    require_an_agreement: bool
+    webhook_url: float
+    redirect_url: float
+    app_url: float
+
+
+class LinkedApplication(LinkedApp):
+    pass
```

### Comparing `linked_services-1.2.1/src/linked_services/rest_framework/views.py` & `linked_services-1.2.2/src/linked_services/rest_framework/views.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,236 +1,236 @@
-import asyncio
-import base64
-import logging
-import os
-from typing import Callable, Optional
-
-from adrf.decorators import api_view
-from asgiref.sync import sync_to_async
-from django.db.models import Q
-from django.http import HttpRequest
-from django.shortcuts import redirect, render
-from django.utils import timezone
-from rest_framework import status
-from rest_framework.decorators import permission_classes
-from rest_framework.permissions import AllowAny
-from rest_framework.response import Response
-
-from linked_services.core.actions import set_query_parameter
-from linked_services.core.i18n import translation
-from linked_services.core.settings import get_setting
-from linked_services.django.actions import aget_app
-from linked_services.django.models import (
-    AppUserAgreement,
-    FirstPartyWebhookLog,
-    OptionalScopeSet,
-    Scope,
-)
-from linked_services.rest_framework.decorators import ascope
-
-logger = logging.getLogger(__name__)
-
-
-# app/webhook
-@api_view(["POST"])
-@permission_classes([AllowAny])
-@ascope(["webhook"], mode="jwt")
-async def app_webhook(request, app: dict, token: dict):
-
-    async def process_webhook(data):
-        nonlocal app, token
-
-        app = await aget_app(app.id)
-        external_id = data.get("id", None)
-        kwargs = {
-            "app": app,
-            "user_id": token.sub,
-            "external_id": external_id,
-            "type": data.get("type", "unknown"),
-        }
-        if external_id:
-            x, created = await FirstPartyWebhookLog.objects.aget_or_create(
-                **kwargs, defaults={"data": data.get("data", None)}
-            )
-            if not created:
-                x.data = data.get("data", None)
-                await x.asave()
-
-        else:
-            kwargs["data"] = data.get("data", None)
-            await FirstPartyWebhookLog.objects.acreate(**kwargs)
-
-    data = request.data if isinstance(request.data, list) else [request.data]
-
-    to_process = []
-
-    for x in data:
-        p = process_webhook(x)
-        to_process.append(p)
-
-    await asyncio.gather(*to_process)
-
-    return Response(None, status=status.HTTP_204_NO_CONTENT)
-
-
-def authorize_view(
-    login_url: Optional[str] = None,
-    app_url: Optional[str] = None,
-    get_language: Optional[Callable[[HttpRequest], str]] = None,
-):
-    non_valid_envs = []
-    if login_url is None:
-        login_url = os.getenv("LOGIN_URL")
-
-    if app_url is None:
-        app_url = os.getenv("APP_URL")
-
-    if login_url is None:
-        non_valid_envs.append("LOGIN_URL")
-
-    if app_url is None:
-        non_valid_envs.append("APP_URL")
-
-    if non_valid_envs:
-        raise Exception(f"Missing environment variables: {', '.join(non_valid_envs)}")
-
-    if get_language is None:
-
-        def get_language(request: HttpRequest) -> str:
-            return "en"
-
-    @sync_to_async
-    def aget_user(request: HttpRequest):
-        return request.user
-
-    @api_view(["GET", "POST"])
-    @permission_classes([AllowAny])
-    async def wrapper(request: HttpRequest, app_slug=None):
-        user = await aget_user(request)
-
-        if user.is_anonymous:
-
-            # base64 encode
-            forward = str(base64.b64encode(request.get_full_path().encode("utf-8")), "utf-8")
-            url = set_query_parameter(login_url, url=forward)
-            return redirect(url)
-
-        lang = get_language(request)
-
-        try:
-            app = await aget_app(app_slug)
-
-        except Exception:
-            return render(
-                request,
-                "app-not-found.html",
-                {
-                    "app_url": app_url,
-                    "title": translation(lang, en="Not found", es="No encontrado"),
-                    "description": translation(lang, en="The app was not found", es="La app no fue encontrada"),
-                    "btn": translation(lang, en="Go back", es="Volver"),
-                },
-                status=404,
-            )
-
-        if not app.require_an_agreement:
-            return render(
-                request,
-                "app-not-found.html",
-                {
-                    "app_url": app_url,
-                    "title": translation(lang, en="Not found", es="No encontrado"),
-                    "description": translation(lang, en="The app was not found", es="La app no fue encontrada"),
-                    "btn": translation(lang, en="Go back", es="Volver"),
-                },
-                status=404,
-            )
-
-        agreement = (
-            await AppUserAgreement.objects.filter(app=app, user=request.user)
-            .select_related("optional_scope_set")
-            .afirst()
-        )
-        selected_scopes = (
-            [x.slug async for x in agreement.optional_scope_set.optional_scopes.filter()] if agreement else []
-        )
-
-        required_scopes = [x async for x in Scope.objects.filter(m2m_required_scopes__app=app)]
-        optional_scopes = [x async for x in Scope.objects.filter(m2m_optional_scopes__app=app)]
-
-        new_scopes = (
-            [
-                x.slug
-                async for x in Scope.objects.filter(
-                    Q(m2m_required_scopes__app=app, m2m_required_scopes__agreed_at__gt=agreement.agreed_at)
-                    | Q(m2m_optional_scopes__app=app, m2m_optional_scopes__agreed_at__gt=agreement.agreed_at),
-                )
-            ]
-            if agreement
-            else []
-        )
-
-        whoamy = get_setting("app_name")
-
-        if request.method == "GET":
-            whoamy = get_setting("app_name")
-            return render(
-                request,
-                "authorize.html",
-                {
-                    "app": app,
-                    "required_scopes": required_scopes,
-                    "optional_scopes": optional_scopes,
-                    "selected_scopes": selected_scopes,
-                    "new_scopes": new_scopes,
-                    "reject_url": app.redirect_url + f"?app={whoamy}&status=rejected",
-                },
-            )
-
-        if request.method == "POST":
-            items = set()
-            for key in request.POST:
-                if key == "csrfmiddlewaretoken":
-                    continue
-
-                items.add(key)
-
-            items = sorted(list(items))
-            query = Q()
-
-            for item in items:
-                query |= Q(optional_scopes__slug=item)
-
-            created = False
-            cache = await OptionalScopeSet.objects.filter(query).afirst()
-            if cache is None or await cache.optional_scopes.acount() != len(items):
-                cache = OptionalScopeSet()
-                await cache.asave()
-
-                created = True
-
-                for s in items:
-                    scope = await Scope.objects.filter(slug=s).afirst()
-                    await cache.optional_scopes.aadd(scope)
-
-            if agreement := await AppUserAgreement.objects.filter(app=app, user=request.user).afirst():
-                if created:
-                    agreement.agreed_at = timezone.now()
-
-                agreement.optional_scope_set = cache
-                agreement.agreement_version = app.agreement_version
-                await agreement.asave()
-
-            else:
-                user = await aget_user(request)
-                agreement = await AppUserAgreement.objects.acreate(
-                    app=app,
-                    user=user,
-                    agreed_at=timezone.now(),
-                    agreement_version=app.agreement_version,
-                    optional_scope_set=cache,
-                )
-
-            whoamy = get_setting("app_name")
-            return redirect(app.redirect_url + f"?app={whoamy}&status=authorized")
-
-    return wrapper
+import asyncio
+import base64
+import logging
+import os
+from typing import Callable, Optional
+
+from adrf.decorators import api_view
+from asgiref.sync import sync_to_async
+from django.db.models import Q
+from django.http import HttpRequest
+from django.shortcuts import redirect, render
+from django.utils import timezone
+from rest_framework import status
+from rest_framework.decorators import permission_classes
+from rest_framework.permissions import AllowAny
+from rest_framework.response import Response
+
+from linked_services.core.actions import set_query_parameter
+from linked_services.core.i18n import translation
+from linked_services.core.settings import get_setting
+from linked_services.django.actions import aget_app
+from linked_services.django.models import (
+    AppUserAgreement,
+    FirstPartyWebhookLog,
+    OptionalScopeSet,
+    Scope,
+)
+from linked_services.rest_framework.decorators import ascope
+
+logger = logging.getLogger(__name__)
+
+
+# app/webhook
+@api_view(["POST"])
+@permission_classes([AllowAny])
+@ascope(["webhook"], mode="jwt")
+async def app_webhook(request, app: dict, token: dict):
+
+    async def process_webhook(data):
+        nonlocal app, token
+
+        app = await aget_app(app.id)
+        external_id = data.get("id", None)
+        kwargs = {
+            "app": app,
+            "user_id": token.sub,
+            "external_id": external_id,
+            "type": data.get("type", "unknown"),
+        }
+        if external_id:
+            x, created = await FirstPartyWebhookLog.objects.aget_or_create(
+                **kwargs, defaults={"data": data.get("data", None)}
+            )
+            if not created:
+                x.data = data.get("data", None)
+                await x.asave()
+
+        else:
+            kwargs["data"] = data.get("data", None)
+            await FirstPartyWebhookLog.objects.acreate(**kwargs)
+
+    data = request.data if isinstance(request.data, list) else [request.data]
+
+    to_process = []
+
+    for x in data:
+        p = process_webhook(x)
+        to_process.append(p)
+
+    await asyncio.gather(*to_process)
+
+    return Response(None, status=status.HTTP_204_NO_CONTENT)
+
+
+def authorize_view(
+    login_url: Optional[str] = None,
+    app_url: Optional[str] = None,
+    get_language: Optional[Callable[[HttpRequest], str]] = None,
+):
+    non_valid_envs = []
+    if login_url is None:
+        login_url = os.getenv("LOGIN_URL")
+
+    if app_url is None:
+        app_url = os.getenv("APP_URL")
+
+    if login_url is None:
+        non_valid_envs.append("LOGIN_URL")
+
+    if app_url is None:
+        non_valid_envs.append("APP_URL")
+
+    if non_valid_envs:
+        raise Exception(f"Missing environment variables: {', '.join(non_valid_envs)}")
+
+    if get_language is None:
+
+        def get_language(request: HttpRequest) -> str:
+            return "en"
+
+    @sync_to_async
+    def aget_user(request: HttpRequest):
+        return request.user
+
+    @api_view(["GET", "POST"])
+    @permission_classes([AllowAny])
+    async def wrapper(request: HttpRequest, app_slug=None):
+        user = await aget_user(request)
+
+        if user.is_anonymous:
+
+            # base64 encode
+            forward = str(base64.b64encode(request.get_full_path().encode("utf-8")), "utf-8")
+            url = set_query_parameter(login_url, url=forward)
+            return redirect(url)
+
+        lang = get_language(request)
+
+        try:
+            app = await aget_app(app_slug)
+
+        except Exception:
+            return render(
+                request,
+                "app-not-found.html",
+                {
+                    "app_url": app_url,
+                    "title": translation(lang, en="Not found", es="No encontrado"),
+                    "description": translation(lang, en="The app was not found", es="La app no fue encontrada"),
+                    "btn": translation(lang, en="Go back", es="Volver"),
+                },
+                status=404,
+            )
+
+        if not app.require_an_agreement:
+            return render(
+                request,
+                "app-not-found.html",
+                {
+                    "app_url": app_url,
+                    "title": translation(lang, en="Not found", es="No encontrado"),
+                    "description": translation(lang, en="The app was not found", es="La app no fue encontrada"),
+                    "btn": translation(lang, en="Go back", es="Volver"),
+                },
+                status=404,
+            )
+
+        agreement = (
+            await AppUserAgreement.objects.filter(app=app, user=request.user)
+            .select_related("optional_scope_set")
+            .afirst()
+        )
+        selected_scopes = (
+            [x.slug async for x in agreement.optional_scope_set.optional_scopes.filter()] if agreement else []
+        )
+
+        required_scopes = [x async for x in Scope.objects.filter(m2m_required_scopes__app=app)]
+        optional_scopes = [x async for x in Scope.objects.filter(m2m_optional_scopes__app=app)]
+
+        new_scopes = (
+            [
+                x.slug
+                async for x in Scope.objects.filter(
+                    Q(m2m_required_scopes__app=app, m2m_required_scopes__agreed_at__gt=agreement.agreed_at)
+                    | Q(m2m_optional_scopes__app=app, m2m_optional_scopes__agreed_at__gt=agreement.agreed_at),
+                )
+            ]
+            if agreement
+            else []
+        )
+
+        whoamy = get_setting("app_name")
+
+        if request.method == "GET":
+            whoamy = get_setting("app_name")
+            return render(
+                request,
+                "authorize.html",
+                {
+                    "app": app,
+                    "required_scopes": required_scopes,
+                    "optional_scopes": optional_scopes,
+                    "selected_scopes": selected_scopes,
+                    "new_scopes": new_scopes,
+                    "reject_url": app.redirect_url + f"?app={whoamy}&status=rejected",
+                },
+            )
+
+        if request.method == "POST":
+            items = set()
+            for key in request.POST:
+                if key == "csrfmiddlewaretoken":
+                    continue
+
+                items.add(key)
+
+            items = sorted(list(items))
+            query = Q()
+
+            for item in items:
+                query |= Q(optional_scopes__slug=item)
+
+            created = False
+            cache = await OptionalScopeSet.objects.filter(query).afirst()
+            if cache is None or await cache.optional_scopes.acount() != len(items):
+                cache = OptionalScopeSet()
+                await cache.asave()
+
+                created = True
+
+                for s in items:
+                    scope = await Scope.objects.filter(slug=s).afirst()
+                    await cache.optional_scopes.aadd(scope)
+
+            if agreement := await AppUserAgreement.objects.filter(app=app, user=request.user).afirst():
+                if created:
+                    agreement.agreed_at = timezone.now()
+
+                agreement.optional_scope_set = cache
+                agreement.agreement_version = app.agreement_version
+                await agreement.asave()
+
+            else:
+                user = await aget_user(request)
+                agreement = await AppUserAgreement.objects.acreate(
+                    app=app,
+                    user=user,
+                    agreed_at=timezone.now(),
+                    agreement_version=app.agreement_version,
+                    optional_scope_set=cache,
+                )
+
+            whoamy = get_setting("app_name")
+            return redirect(app.redirect_url + f"?app={whoamy}&status=authorized")
+
+    return wrapper
```

### Comparing `linked_services-1.2.1/src/linked_services/templates/authorize.html` & `linked_services-1.2.2/src/linked_services/templates/authorize.html`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-{% load button %}
-{% load scopes %}
-<!DOCTYPE html>
-<html lang="en">
-
-<head>
-    <meta charset="UTF-8">
-    <meta name="viewport" content="width=device-width, initial-scale=1">
-    <title>Academy Invite</title>
-    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/css/bootstrap.min.css" rel="stylesheet"
-        integrity="sha384-4bw+/aepP/YC94hEpVNVgiZdgIC5+VKNBQNGCHeKRQN+PtmoHDEXuppvnDJzQIu9" crossorigin="anonymous">
-    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.0/font/bootstrap-icons.css">
-    <style>
-        .buttons {
-            margin-top: 16px;
-        }
-
-        .question {
-            margin-top: 3px;
-            font-size: 10px;
-            vertical-align: top;
-        }
-
-        .disable-shadow:focus {
-            box-shadow: inset 0 calc(-1 * var(--bs-accordion-border-width)) 0 var(--bs-accordion-border-color);
-        }
-
-        .disable-shadow.collapsed:focus {
-            box-shadow: inset 0 0 0 var(--bs-accordion-border-color);
-        }
-
-        .container-sm {
-            max-width: 540px;
-            padding-top: 50px;
-        }
-
-        .accordion-button:focus {
-            outline: none;
-        }
-
-        .accordion-button:not(.collapsed) {
-            color: var(--bs-accordion-btn-color);
-            background-color: var(--bs-accordion-btn-bg);
-
-        }
-
-        .text-justify {
-            text-align: justify;
-        }
-    </style>
-
-</html>
-
-<body>
-    <div class="container-sm">
-        <form method="post">
-            {% csrf_token %}
-            <h1 class="text-center">
-                <span class="badge bg-secondary">{{app.name}}</span>
-            </h1>
-
-            <p class="fw-normal text-center">
-                This app is requesting permission to access your account.
-            </p>
-
-            <p class="fw-lighter text-justify">
-                {{app.description}}
-            </p>
-
-            {% scopes scopes=required_scopes id='required' title='Required permissions' disabled=True new_scopes=new_scopes %}
-            {% scopes scopes=optional_scopes id='optional' title='Optional permissions' disabled=False new_scopes=new_scopes selected_scopes=selected_scopes %}
-
-            <div class="gap-2 d-md-flex buttons">
-                {% button type="link" className="btn-danger offset-2 col-4" href=reject_url value="Reject" %}
-                {% button type="submit" className="btn-primary col-4" value="Accept" %}
-            </div>
-        </form>
-    </div>
-
-    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/js/bootstrap.bundle.min.js"
-        integrity="sha384-HwwvtgBNo3bZJJLYd8oVXjrBZt8cqVSpeBNS5n7C8IVInixGAoxmnlMuBnhbgrkm"
-        crossorigin="anonymous"></script>
-
-    <script>
-        var popoverTriggerList = [].slice.call(document.querySelectorAll('[data-bs-toggle="popover"]'))
-        var popoverList = popoverTriggerList.map(function (popoverTriggerEl) {
-            return new bootstrap.Popover(popoverTriggerEl)
-        })
-    </script>
-</body>
+{% load button %}
+{% load scopes %}
+<!DOCTYPE html>
+<html lang="en">
+
+<head>
+    <meta charset="UTF-8">
+    <meta name="viewport" content="width=device-width, initial-scale=1">
+    <title>Academy Invite</title>
+    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/css/bootstrap.min.css" rel="stylesheet"
+        integrity="sha384-4bw+/aepP/YC94hEpVNVgiZdgIC5+VKNBQNGCHeKRQN+PtmoHDEXuppvnDJzQIu9" crossorigin="anonymous">
+    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.0/font/bootstrap-icons.css">
+    <style>
+        .buttons {
+            margin-top: 16px;
+        }
+
+        .question {
+            margin-top: 3px;
+            font-size: 10px;
+            vertical-align: top;
+        }
+
+        .disable-shadow:focus {
+            box-shadow: inset 0 calc(-1 * var(--bs-accordion-border-width)) 0 var(--bs-accordion-border-color);
+        }
+
+        .disable-shadow.collapsed:focus {
+            box-shadow: inset 0 0 0 var(--bs-accordion-border-color);
+        }
+
+        .container-sm {
+            max-width: 540px;
+            padding-top: 50px;
+        }
+
+        .accordion-button:focus {
+            outline: none;
+        }
+
+        .accordion-button:not(.collapsed) {
+            color: var(--bs-accordion-btn-color);
+            background-color: var(--bs-accordion-btn-bg);
+
+        }
+
+        .text-justify {
+            text-align: justify;
+        }
+    </style>
+
+</html>
+
+<body>
+    <div class="container-sm">
+        <form method="post">
+            {% csrf_token %}
+            <h1 class="text-center">
+                <span class="badge bg-secondary">{{app.name}}</span>
+            </h1>
+
+            <p class="fw-normal text-center">
+                This app is requesting permission to access your account.
+            </p>
+
+            <p class="fw-lighter text-justify">
+                {{app.description}}
+            </p>
+
+            {% scopes scopes=required_scopes id='required' title='Required permissions' disabled=True new_scopes=new_scopes %}
+            {% scopes scopes=optional_scopes id='optional' title='Optional permissions' disabled=False new_scopes=new_scopes selected_scopes=selected_scopes %}
+
+            <div class="gap-2 d-md-flex buttons">
+                {% button type="link" className="btn-danger offset-2 col-4" href=reject_url value="Reject" %}
+                {% button type="submit" className="btn-primary col-4" value="Accept" %}
+            </div>
+        </form>
+    </div>
+
+    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/js/bootstrap.bundle.min.js"
+        integrity="sha384-HwwvtgBNo3bZJJLYd8oVXjrBZt8cqVSpeBNS5n7C8IVInixGAoxmnlMuBnhbgrkm"
+        crossorigin="anonymous"></script>
+
+    <script>
+        var popoverTriggerList = [].slice.call(document.querySelectorAll('[data-bs-toggle="popover"]'))
+        var popoverList = popoverTriggerList.map(function (popoverTriggerEl) {
+            return new bootstrap.Popover(popoverTriggerEl)
+        })
+    </script>
+</body>
```

### Comparing `linked_services-1.2.1/tests/django/actions/test_acreate_user.py` & `linked_services-1.2.2/tests/django/actions/test_acreate_user.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-import random
-import secrets
-from datetime import datetime
-from unittest.mock import AsyncMock, MagicMock
-
-import pytest
-
-from linked_services.core.exceptions import ValidationException
-from linked_services.core.service import AppNotFound
-from linked_services.core.settings import set_settings
-from linked_services.django import actions
-
-
-@pytest.fixture(autouse=True)
-def setup(db, monkeypatch):
-    set_settings(app_name="breathecode")
-    monkeypatch.setattr("logging.Logger.error", MagicMock())
-    monkeypatch.setattr("linked_services.django.tasks.check_credentials.delay", MagicMock())
-
-    yield
-
-
-class ResponseMock:
-
-    def __init__(self, data, status):
-        self.status_code = status
-        self.data = data
-
-    async def json(self):
-        return self.data
-
-
-@pytest.fixture
-def patch_request(monkeypatch):
-
-    def wrapper(data, status):
-        monkeypatch.setattr(
-            "linked_services.core.service.Service.get", AsyncMock(return_value=ResponseMock(data, status))
-        )
-        return MagicMock()
-
-    yield wrapper
-
-
-@pytest.mark.asyncio
-@pytest.mark.django_db(reset_sequences=True)
-async def test_app_not_found(fake, database):
-    app_slug = fake.slug()
-
-    with pytest.raises(AppNotFound):
-        await actions.acreate_user(app_slug, 1)
-
-    assert await database.alist_of("linked_services.FirstPartyCredentials") == []
-    assert await database.alist_of("auth.User") == []
-
-
-@pytest.mark.asyncio
-@pytest.mark.django_db(reset_sequences=True)
-async def test_required_fields_not_provided(fake, database, patch_request):
-    patch_request({}, 200)
-    app_slug = fake.slug()
-    await database.acreate(
-        app={
-            "slug": app_slug,
-            "private_key": secrets.token_hex(64),
-        }
-    )
-
-    with pytest.raises(ValidationException, match="id not provided, username not provided, email not provided"):
-        await actions.acreate_user(app_slug, 1)
-
-    assert await database.alist_of("linked_services.FirstPartyCredentials") == []
-    assert await database.alist_of("auth.User") == []
-
-
-@pytest.mark.asyncio
-@pytest.mark.django_db(reset_sequences=True)
-@pytest.mark.parametrize("optional_fields", [{}, {"first_name": "John", "last_name": "Silla 🪑"}])
-async def test_all_fine(fake, database, patch_request, optional_fields):
-    data = {
-        "id": random.randint(1, 100),
-        "username": fake.slug(),
-        "email": fake.email(),
-    }
-    if optional_fields:
-        data.update(optional_fields)
-
-    patch_request(data, 200)
-    app_slug = fake.slug()
-    await database.acreate(
-        app={
-            "slug": app_slug,
-            "private_key": secrets.token_hex(64),
-        }
-    )
-
-    await actions.acreate_user(app_slug, 1)
-
-    assert await database.alist_of("linked_services.FirstPartyCredentials") == [
-        {
-            "app": {app_slug: data["id"]},
-            "health_status": {},
-            "id": 1,
-            "user_id": 1,
-        },
-    ]
-    users_db = [
-        x
-        for x in await database.alist_of("auth.User")
-        if isinstance(x["date_joined"], datetime) and x.pop("date_joined")
-    ]
-    assert users_db == [
-        {
-            "email": data["email"],
-            "first_name": data.get("first_name", ""),
-            "id": 1,
-            "is_active": True,
-            "is_staff": False,
-            "is_superuser": False,
-            "last_login": None,
-            "last_name": data.get("last_name", ""),
-            "password": "",
-            "username": data["username"],
-        }
-    ]
+import random
+import secrets
+from datetime import datetime
+from unittest.mock import AsyncMock, MagicMock
+
+import pytest
+
+from linked_services.core.exceptions import ValidationException
+from linked_services.core.service import AppNotFound
+from linked_services.core.settings import set_settings
+from linked_services.django import actions
+
+
+@pytest.fixture(autouse=True)
+def setup(db, monkeypatch):
+    set_settings(app_name="breathecode")
+    monkeypatch.setattr("logging.Logger.error", MagicMock())
+    monkeypatch.setattr("linked_services.django.tasks.check_credentials.delay", MagicMock())
+
+    yield
+
+
+class ResponseMock:
+
+    def __init__(self, data, status):
+        self.status_code = status
+        self.data = data
+
+    async def json(self):
+        return self.data
+
+
+@pytest.fixture
+def patch_request(monkeypatch):
+
+    def wrapper(data, status):
+        monkeypatch.setattr(
+            "linked_services.core.service.Service.get", AsyncMock(return_value=ResponseMock(data, status))
+        )
+        return MagicMock()
+
+    yield wrapper
+
+
+@pytest.mark.asyncio
+@pytest.mark.django_db(reset_sequences=True)
+async def test_app_not_found(fake, database):
+    app_slug = fake.slug()
+
+    with pytest.raises(AppNotFound):
+        await actions.acreate_user(app_slug, 1)
+
+    assert await database.alist_of("linked_services.FirstPartyCredentials") == []
+    assert await database.alist_of("auth.User") == []
+
+
+@pytest.mark.asyncio
+@pytest.mark.django_db(reset_sequences=True)
+async def test_required_fields_not_provided(fake, database, patch_request):
+    patch_request({}, 200)
+    app_slug = fake.slug()
+    await database.acreate(
+        app={
+            "slug": app_slug,
+            "private_key": secrets.token_hex(64),
+        }
+    )
+
+    with pytest.raises(ValidationException, match="id not provided, username not provided, email not provided"):
+        await actions.acreate_user(app_slug, 1)
+
+    assert await database.alist_of("linked_services.FirstPartyCredentials") == []
+    assert await database.alist_of("auth.User") == []
+
+
+@pytest.mark.asyncio
+@pytest.mark.django_db(reset_sequences=True)
+@pytest.mark.parametrize("optional_fields", [{}, {"first_name": "John", "last_name": "Silla 🪑"}])
+async def test_all_fine(fake, database, patch_request, optional_fields):
+    data = {
+        "id": random.randint(1, 100),
+        "username": fake.slug(),
+        "email": fake.email(),
+    }
+    if optional_fields:
+        data.update(optional_fields)
+
+    patch_request(data, 200)
+    app_slug = fake.slug()
+    await database.acreate(
+        app={
+            "slug": app_slug,
+            "private_key": secrets.token_hex(64),
+        }
+    )
+
+    await actions.acreate_user(app_slug, 1)
+
+    assert await database.alist_of("linked_services.FirstPartyCredentials") == [
+        {
+            "app": {app_slug: data["id"]},
+            "health_status": {},
+            "id": 1,
+            "user_id": 1,
+        },
+    ]
+    users_db = [
+        x
+        for x in await database.alist_of("auth.User")
+        if isinstance(x["date_joined"], datetime) and x.pop("date_joined")
+    ]
+    assert users_db == [
+        {
+            "email": data["email"],
+            "first_name": data.get("first_name", ""),
+            "id": 1,
+            "is_active": True,
+            "is_staff": False,
+            "is_superuser": False,
+            "last_login": None,
+            "last_name": data.get("last_name", ""),
+            "password": "",
+            "username": data["username"],
+        }
+    ]
```

### Comparing `linked_services-1.2.1/tests/django/actions/test_aget_user.py` & `linked_services-1.2.2/tests/django/actions/test_aget_user.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-from unittest.mock import AsyncMock, call
-
-import pytest
-
-from linked_services.core.settings import set_settings
-from linked_services.django import actions
-
-
-@pytest.fixture(autouse=True)
-def patch(db, monkeypatch):
-    from linked_services.django.actions import reset_app_cache
-
-    m1 = AsyncMock()
-
-    set_settings(app_name="breathecode")
-    reset_app_cache()
-
-    monkeypatch.setattr("linked_services.django.tasks.check_credentials.delay", AsyncMock())
-    monkeypatch.setattr("linked_services.django.actions.acreate_user", m1)
-
-    yield m1
-
-
-@pytest.mark.asyncio
-@pytest.mark.django_db(reset_sequences=True)
-@pytest.mark.parametrize("user", [0, 1])
-async def test_no_first_party_credentials(patch, fake, database, user):
-    app_slug = fake.slug()
-    await database.acreate(user=user, app={"slug": app_slug})
-    v = fake.slug()
-    create_use_mock = patch
-    create_use_mock.return_value = v
-
-    res = await actions.aget_user(app_slug, 1)
-
-    assert res == v
-    assert actions.acreate_user.call_args_list == [call(app_slug, 1)]
-    assert await database.alist_of("linked_services.FirstPartyCredentials") == []
-
-
-@pytest.mark.asyncio
-@pytest.mark.django_db(reset_sequences=True)
-async def test_with_first_party_credentials(patch, fake, database, get_json_obj):
-    app_slug = fake.slug()
-    model = await database.acreate(user=1, first_party_credentials={"app": {app_slug: 1}})
-
-    v = fake.slug()
-    create_use_mock = patch
-    create_use_mock.return_value = v
-
-    res = await actions.aget_user(app_slug, 1)
-
-    assert res == model.user
-    assert actions.acreate_user.call_args_list == []
-    assert await database.alist_of("linked_services.FirstPartyCredentials") == [
-        get_json_obj(model.first_party_credentials)
-    ]
+from unittest.mock import AsyncMock, call
+
+import pytest
+
+from linked_services.core.settings import set_settings
+from linked_services.django import actions
+
+
+@pytest.fixture(autouse=True)
+def patch(db, monkeypatch):
+    from linked_services.django.actions import reset_app_cache
+
+    m1 = AsyncMock()
+
+    set_settings(app_name="breathecode")
+    reset_app_cache()
+
+    monkeypatch.setattr("linked_services.django.tasks.check_credentials.delay", AsyncMock())
+    monkeypatch.setattr("linked_services.django.actions.acreate_user", m1)
+
+    yield m1
+
+
+@pytest.mark.asyncio
+@pytest.mark.django_db(reset_sequences=True)
+@pytest.mark.parametrize("user", [0, 1])
+async def test_no_first_party_credentials(patch, fake, database, user):
+    app_slug = fake.slug()
+    await database.acreate(user=user, app={"slug": app_slug})
+    v = fake.slug()
+    create_use_mock = patch
+    create_use_mock.return_value = v
+
+    res = await actions.aget_user(app_slug, 1)
+
+    assert res == v
+    assert actions.acreate_user.call_args_list == [call(app_slug, 1)]
+    assert await database.alist_of("linked_services.FirstPartyCredentials") == []
+
+
+@pytest.mark.asyncio
+@pytest.mark.django_db(reset_sequences=True)
+async def test_with_first_party_credentials(patch, fake, database, get_json_obj):
+    app_slug = fake.slug()
+    model = await database.acreate(user=1, first_party_credentials={"app": {app_slug: 1}})
+
+    v = fake.slug()
+    create_use_mock = patch
+    create_use_mock.return_value = v
+
+    res = await actions.aget_user(app_slug, 1)
+
+    assert res == model.user
+    assert actions.acreate_user.call_args_list == []
+    assert await database.alist_of("linked_services.FirstPartyCredentials") == [
+        get_json_obj(model.first_party_credentials)
+    ]
```

### Comparing `linked_services-1.2.1/tests/django/actions/test_get_user.py` & `linked_services-1.2.2/tests/django/actions/test_get_user.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import secrets
-from unittest.mock import MagicMock, call
-
-import pytest
-
-from linked_services.core.settings import set_settings
-from linked_services.django import actions
-
-
-@pytest.fixture(autouse=True)
-def patch(db, monkeypatch):
-    from linked_services.django.actions import reset_app_cache
-
-    m1 = MagicMock()
-
-    set_settings(app_name="breathecode")
-    reset_app_cache()
-
-    monkeypatch.setattr("linked_services.django.tasks.check_credentials.delay", MagicMock())
-    monkeypatch.setattr("linked_services.django.actions.create_user", m1)
-
-    yield m1
-
-
-@pytest.mark.parametrize("user", [0, 1])
-def test_no_first_party_credentials(patch, fake, database, user):
-    database.create(user=user)
-    v = fake.slug()
-    create_use_mock = patch
-    create_use_mock.return_value = v
-
-    res = actions.get_user("breathecode", 1)
-
-    assert res == v
-    assert actions.create_user.call_args_list == [call("breathecode", 1)]
-    assert database.list_of("linked_services.FirstPartyCredentials") == []
-
-
-def test_with_first_party_credentials(patch, fake, database, get_json_obj):
-    app_slug = fake.slug()
-    model = database.create(
-        user=1,
-        first_party_credentials={
-            "app": {app_slug: 1},
-        },
-    )
-
-    v = fake.slug()
-    create_use_mock = patch
-    create_use_mock.return_value = v
-
-    res = actions.get_user(app_slug, 1)
-
-    assert res == model.user
-    assert actions.create_user.call_args_list == []
-    assert database.list_of("linked_services.FirstPartyCredentials") == [get_json_obj(model.first_party_credentials)]
+import secrets
+from unittest.mock import MagicMock, call
+
+import pytest
+
+from linked_services.core.settings import set_settings
+from linked_services.django import actions
+
+
+@pytest.fixture(autouse=True)
+def patch(db, monkeypatch):
+    from linked_services.django.actions import reset_app_cache
+
+    m1 = MagicMock()
+
+    set_settings(app_name="breathecode")
+    reset_app_cache()
+
+    monkeypatch.setattr("linked_services.django.tasks.check_credentials.delay", MagicMock())
+    monkeypatch.setattr("linked_services.django.actions.create_user", m1)
+
+    yield m1
+
+
+@pytest.mark.parametrize("user", [0, 1])
+def test_no_first_party_credentials(patch, fake, database, user):
+    database.create(user=user)
+    v = fake.slug()
+    create_use_mock = patch
+    create_use_mock.return_value = v
+
+    res = actions.get_user("breathecode", 1)
+
+    assert res == v
+    assert actions.create_user.call_args_list == [call("breathecode", 1)]
+    assert database.list_of("linked_services.FirstPartyCredentials") == []
+
+
+def test_with_first_party_credentials(patch, fake, database, get_json_obj):
+    app_slug = fake.slug()
+    model = database.create(
+        user=1,
+        first_party_credentials={
+            "app": {app_slug: 1},
+        },
+    )
+
+    v = fake.slug()
+    create_use_mock = patch
+    create_use_mock.return_value = v
+
+    res = actions.get_user(app_slug, 1)
+
+    assert res == model.user
+    assert actions.create_user.call_args_list == []
+    assert database.list_of("linked_services.FirstPartyCredentials") == [get_json_obj(model.first_party_credentials)]
```

### Comparing `linked_services-1.2.1/tests/django/tasks/test_check_credentials.py` & `linked_services-1.2.2/tests/django/tasks/test_check_credentials.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,186 +1,186 @@
-import logging
-import random
-from unittest.mock import MagicMock, call, patch
-
-import pytest
-
-from linked_services.core.settings import set_settings
-from linked_services.django.service import Service
-from linked_services.django.tasks import check_credentials
-
-
-@pytest.fixture(autouse=True)
-def setup(db, monkeypatch):
-    set_settings(app_name="breathecode")
-    monkeypatch.setattr("logging.Logger.error", MagicMock())
-
-    yield
-
-
-class ResponseMock:
-
-    def __init__(self, data, status):
-        self.status_code = status
-        self.data = data
-
-    def json(self):
-        return self.data
-
-
-@pytest.fixture
-def patch_request(monkeypatch):
-
-    def wrapper(data, status):
-        monkeypatch.setattr(
-            "linked_services.core.service.Service.get", MagicMock(return_value=ResponseMock(data, status))
-        )
-        return MagicMock()
-
-    yield wrapper
-
-
-def test_nothing_to_check(database, get_json_obj):
-    check_credentials.delay(1)
-
-    assert database.list_of("linked_services.FirstPartyCredentials") == []
-
-    assert logging.Logger.error.call_args_list == [
-        call("Nothing to check", exc_info=True),
-    ]
-
-
-# you should parametrize these tests to check with another apps
-
-
-def test_not_found(database, get_json_obj):
-    check_credentials.delay(1, ["rigobot"])
-
-    assert database.list_of("linked_services.FirstPartyCredentials") == []
-
-    assert logging.Logger.error.call_args_list == [
-        call("FirstPartyCredentials not found", exc_info=True),
-    ]
-
-
-def test_if_rigobot_id_is_null_remove_its_related_log(database, get_json_obj):
-    with patch("linked_services.django.tasks.check_credentials.delay", MagicMock()):
-        model = database.create(
-            first_party_credentials={
-                "app": {},
-                "health_status": {
-                    "rigobot": {
-                        "random": "value",
-                    },
-                },
-            }
-        )
-    check_credentials.delay(1, ["rigobot"])
-
-    assert database.list_of("linked_services.FirstPartyCredentials") == [
-        {
-            **get_json_obj(model.first_party_credentials),
-            "health_status": {},
-        },
-    ]
-
-    assert logging.Logger.error.call_args_list == []
-
-
-def test_app_not_found(database, get_json_obj):
-    id = random.randint(1, 100)
-    with patch("linked_services.django.tasks.check_credentials.delay", MagicMock()):
-        model = database.create(
-            first_party_credentials={
-                "app": {
-                    "rigobot": id,
-                },
-            },
-        )
-
-    check_credentials.delay(1, ["rigobot"])
-
-    assert database.list_of("linked_services.FirstPartyCredentials") == [
-        {
-            **get_json_obj(model.first_party_credentials),
-            "app": {},
-            "health_status": {
-                "rigobot": {
-                    "id": id,
-                    "status": "APP_NOT_FOUND",
-                },
-            },
-        },
-    ]
-
-    assert logging.Logger.error.call_args_list == []
-
-
-@pytest.mark.parametrize("status,data", [(404, []), (200, {}), (200, [])])
-def test_not_found_on_rigobot(database, get_json_obj, patch_request, status, data):
-    patch_request(data, status)
-    id = random.randint(1, 100)
-
-    with patch("linked_services.django.tasks.check_credentials.delay", MagicMock()):
-        model = database.create(
-            first_party_credentials={
-                "app": {
-                    "rigobot": id,
-                },
-            },
-            app={"slug": "rigobot"},
-        )
-
-    check_credentials.delay(1, ["rigobot"])
-
-    assert database.list_of("linked_services.FirstPartyCredentials") == [
-        {
-            **get_json_obj(model.first_party_credentials),
-            "health_status": {
-                "rigobot": {
-                    "id": id,
-                    "status": "NOT_FOUND",
-                },
-            },
-            "app": {},
-        },
-    ]
-
-    assert logging.Logger.error.call_args_list == []
-    assert Service.get.call_args_list == [
-        call(f"/v1/auth/app/user/?email={model.user.email}&id={id}"),
-    ]
-
-
-def test_found_on_rigobot(database, get_json_obj, patch_request):
-    patch_request([1], 200)
-    id = random.randint(1, 100)
-
-    with patch("linked_services.django.tasks.check_credentials.delay", MagicMock()):
-        model = database.create(
-            first_party_credentials={
-                "app": {
-                    "rigobot": id,
-                },
-            },
-            app={"slug": "rigobot"},
-        )
-
-    check_credentials.delay(1, ["rigobot"])
-
-    assert database.list_of("linked_services.FirstPartyCredentials") == [
-        {
-            **get_json_obj(model.first_party_credentials),
-            "health_status": {
-                "rigobot": {
-                    "id": id,
-                    "status": "HEALTHY",
-                },
-            },
-            "app": {"rigobot": id},
-        },
-    ]
-
-    assert logging.Logger.error.call_args_list == []
-    assert Service.get.call_args_list == [
-        call(f"/v1/auth/app/user/?email={model.user.email}&id={id}"),
-    ]
+import logging
+import random
+from unittest.mock import MagicMock, call, patch
+
+import pytest
+
+from linked_services.core.settings import set_settings
+from linked_services.django.service import Service
+from linked_services.django.tasks import check_credentials
+
+
+@pytest.fixture(autouse=True)
+def setup(db, monkeypatch):
+    set_settings(app_name="breathecode")
+    monkeypatch.setattr("logging.Logger.error", MagicMock())
+
+    yield
+
+
+class ResponseMock:
+
+    def __init__(self, data, status):
+        self.status_code = status
+        self.data = data
+
+    def json(self):
+        return self.data
+
+
+@pytest.fixture
+def patch_request(monkeypatch):
+
+    def wrapper(data, status):
+        monkeypatch.setattr(
+            "linked_services.core.service.Service.get", MagicMock(return_value=ResponseMock(data, status))
+        )
+        return MagicMock()
+
+    yield wrapper
+
+
+def test_nothing_to_check(database, get_json_obj):
+    check_credentials.delay(1)
+
+    assert database.list_of("linked_services.FirstPartyCredentials") == []
+
+    assert logging.Logger.error.call_args_list == [
+        call("Nothing to check", exc_info=True),
+    ]
+
+
+# you should parametrize these tests to check with another apps
+
+
+def test_not_found(database, get_json_obj):
+    check_credentials.delay(1, ["rigobot"])
+
+    assert database.list_of("linked_services.FirstPartyCredentials") == []
+
+    assert logging.Logger.error.call_args_list == [
+        call("FirstPartyCredentials not found", exc_info=True),
+    ]
+
+
+def test_if_rigobot_id_is_null_remove_its_related_log(database, get_json_obj):
+    with patch("linked_services.django.tasks.check_credentials.delay", MagicMock()):
+        model = database.create(
+            first_party_credentials={
+                "app": {},
+                "health_status": {
+                    "rigobot": {
+                        "random": "value",
+                    },
+                },
+            }
+        )
+    check_credentials.delay(1, ["rigobot"])
+
+    assert database.list_of("linked_services.FirstPartyCredentials") == [
+        {
+            **get_json_obj(model.first_party_credentials),
+            "health_status": {},
+        },
+    ]
+
+    assert logging.Logger.error.call_args_list == []
+
+
+def test_app_not_found(database, get_json_obj):
+    id = random.randint(1, 100)
+    with patch("linked_services.django.tasks.check_credentials.delay", MagicMock()):
+        model = database.create(
+            first_party_credentials={
+                "app": {
+                    "rigobot": id,
+                },
+            },
+        )
+
+    check_credentials.delay(1, ["rigobot"])
+
+    assert database.list_of("linked_services.FirstPartyCredentials") == [
+        {
+            **get_json_obj(model.first_party_credentials),
+            "app": {},
+            "health_status": {
+                "rigobot": {
+                    "id": id,
+                    "status": "APP_NOT_FOUND",
+                },
+            },
+        },
+    ]
+
+    assert logging.Logger.error.call_args_list == []
+
+
+@pytest.mark.parametrize("status,data", [(404, []), (200, {}), (200, [])])
+def test_not_found_on_rigobot(database, get_json_obj, patch_request, status, data):
+    patch_request(data, status)
+    id = random.randint(1, 100)
+
+    with patch("linked_services.django.tasks.check_credentials.delay", MagicMock()):
+        model = database.create(
+            first_party_credentials={
+                "app": {
+                    "rigobot": id,
+                },
+            },
+            app={"slug": "rigobot"},
+        )
+
+    check_credentials.delay(1, ["rigobot"])
+
+    assert database.list_of("linked_services.FirstPartyCredentials") == [
+        {
+            **get_json_obj(model.first_party_credentials),
+            "health_status": {
+                "rigobot": {
+                    "id": id,
+                    "status": "NOT_FOUND",
+                },
+            },
+            "app": {},
+        },
+    ]
+
+    assert logging.Logger.error.call_args_list == []
+    assert Service.get.call_args_list == [
+        call(f"/v1/auth/app/user/?email={model.user.email}&id={id}"),
+    ]
+
+
+def test_found_on_rigobot(database, get_json_obj, patch_request):
+    patch_request([1], 200)
+    id = random.randint(1, 100)
+
+    with patch("linked_services.django.tasks.check_credentials.delay", MagicMock()):
+        model = database.create(
+            first_party_credentials={
+                "app": {
+                    "rigobot": id,
+                },
+            },
+            app={"slug": "rigobot"},
+        )
+
+    check_credentials.delay(1, ["rigobot"])
+
+    assert database.list_of("linked_services.FirstPartyCredentials") == [
+        {
+            **get_json_obj(model.first_party_credentials),
+            "health_status": {
+                "rigobot": {
+                    "id": id,
+                    "status": "HEALTHY",
+                },
+            },
+            "app": {"rigobot": id},
+        },
+    ]
+
+    assert logging.Logger.error.call_args_list == []
+    assert Service.get.call_args_list == [
+        call(f"/v1/auth/app/user/?email={model.user.email}&id={id}"),
+    ]
```

### Comparing `linked_services-1.2.1/tests/django/tasks/test_first_party_webhooks.py` & `linked_services-1.2.2/tests/django/tasks/test_first_party_webhooks.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-from datetime import timedelta
-from unittest.mock import MagicMock, call
-
-import pytest
-from django.utils import timezone
-
-from linked_services.core.settings import set_settings
-from linked_services.management.commands.first_party_webhooks import Command
-
-T1 = timezone.now()
-
-
-@pytest.fixture(autouse=True)
-def patch(db, monkeypatch):
-    set_settings(app_name="breathecode")
-    # from breathecode.authenticate import tasks
-    # return tasks.import_external_user.delay(webhook.id)
-    m1 = MagicMock()
-
-    monkeypatch.setattr("linked_services.django.tasks.import_external_user.delay", m1)
-    # monkeypatch.setattr('django.utils.timezone.now', lambda: T1)
-
-    yield m1
-
-
-@pytest.fixture
-def freeze_time(monkeypatch):
-
-    def wrapper(time=T1):
-        monkeypatch.setattr("django.utils.timezone.now", lambda: time)
-
-    yield wrapper
-
-
-def test__nothing_to_migrate(database, patch):
-    import_external_user = patch
-    command = Command()
-    command.handle()
-
-    assert database.list_of("linked_services.FirstPartyWebhookLog") == []
-    assert import_external_user.call_args_list == []
-
-
-def test__no_calls__breathecode_log(database, patch, get_json_obj):
-    model = database.create(first_party_webhook_log=(2, {"attempts": 0}))
-    import_external_user = patch
-    command = Command()
-    command.handle()
-
-    db = get_json_obj(model.first_party_webhook_log)
-    assert database.list_of("linked_services.FirstPartyWebhookLog") == db
-    assert import_external_user.call_args_list == []
-
-
-@pytest.mark.parametrize(
-    "delta,attempts",
-    [
-        (timedelta(0), 0),
-        (timedelta(minutes=21), 1),
-        (timedelta(minutes=22), 2),
-        (timedelta(minutes=23), 3),
-        (timedelta(minutes=24), 4),
-        (timedelta(minutes=25), 5),
-    ],
-)
-def test__no_calls__rigobot_requests(database, patch, freeze_time, delta, attempts, get_json_obj):
-    import_external_user = patch
-
-    model = database.create(first_party_webhook_log=(2, {"attempts": attempts, "external_id": 1}))
-
-    freeze_time(T1 + delta)
-
-    command = Command()
-    command.handle()
-
-    assert database.list_of("linked_services.FirstPartyWebhookLog") == [
-        {
-            **get_json_obj(model.first_party_webhook_log[0]),
-            "status": "ERROR",
-            "status_text": "Invalid webhook type",
-        },
-        {
-            **get_json_obj(model.first_party_webhook_log[1]),
-            "status": "ERROR",
-            "status_text": "Invalid webhook type",
-        },
-    ]
-    assert import_external_user.call_args_list == []
-
-
-@pytest.mark.parametrize(
-    "delta,attempts,type",
-    [
-        (timedelta(0), 0, "user.created"),
-        (timedelta(0), 0, "user.updated"),
-        (timedelta(minutes=21), 1, "user.created"),
-        (timedelta(minutes=22), 2, "user.updated"),
-        (timedelta(minutes=23), 3, "user.created"),
-        (timedelta(minutes=24), 4, "user.updated"),
-        (timedelta(minutes=25), 5, "user.created"),
-    ],
-)
-def test__user_events_scheduled(database, patch, freeze_time, delta, attempts, type, get_json_obj):
-    import_external_user = patch
-
-    model = database.create(first_party_webhook_log=(2, {"attempts": attempts, "external_id": 1, "type": type}))
-
-    freeze_time(T1 + delta)
-
-    command = Command()
-    command.handle()
-
-    assert database.list_of("linked_services.FirstPartyWebhookLog") == [
-        {
-            **get_json_obj(model.first_party_webhook_log[0]),
-            "status": "PENDING",
-        },
-        {
-            **get_json_obj(model.first_party_webhook_log[1]),
-            "status": "PENDING",
-        },
-    ]
-    assert import_external_user.call_args_list == [call(1), call(2)]
+from datetime import timedelta
+from unittest.mock import MagicMock, call
+
+import pytest
+from django.utils import timezone
+
+from linked_services.core.settings import set_settings
+from linked_services.management.commands.first_party_webhooks import Command
+
+T1 = timezone.now()
+
+
+@pytest.fixture(autouse=True)
+def patch(db, monkeypatch):
+    set_settings(app_name="breathecode")
+    # from breathecode.authenticate import tasks
+    # return tasks.import_external_user.delay(webhook.id)
+    m1 = MagicMock()
+
+    monkeypatch.setattr("linked_services.django.tasks.import_external_user.delay", m1)
+    # monkeypatch.setattr('django.utils.timezone.now', lambda: T1)
+
+    yield m1
+
+
+@pytest.fixture
+def freeze_time(monkeypatch):
+
+    def wrapper(time=T1):
+        monkeypatch.setattr("django.utils.timezone.now", lambda: time)
+
+    yield wrapper
+
+
+def test__nothing_to_migrate(database, patch):
+    import_external_user = patch
+    command = Command()
+    command.handle()
+
+    assert database.list_of("linked_services.FirstPartyWebhookLog") == []
+    assert import_external_user.call_args_list == []
+
+
+def test__no_calls__breathecode_log(database, patch, get_json_obj):
+    model = database.create(first_party_webhook_log=(2, {"attempts": 0}))
+    import_external_user = patch
+    command = Command()
+    command.handle()
+
+    db = get_json_obj(model.first_party_webhook_log)
+    assert database.list_of("linked_services.FirstPartyWebhookLog") == db
+    assert import_external_user.call_args_list == []
+
+
+@pytest.mark.parametrize(
+    "delta,attempts",
+    [
+        (timedelta(0), 0),
+        (timedelta(minutes=21), 1),
+        (timedelta(minutes=22), 2),
+        (timedelta(minutes=23), 3),
+        (timedelta(minutes=24), 4),
+        (timedelta(minutes=25), 5),
+    ],
+)
+def test__no_calls__rigobot_requests(database, patch, freeze_time, delta, attempts, get_json_obj):
+    import_external_user = patch
+
+    model = database.create(first_party_webhook_log=(2, {"attempts": attempts, "external_id": 1}))
+
+    freeze_time(T1 + delta)
+
+    command = Command()
+    command.handle()
+
+    assert database.list_of("linked_services.FirstPartyWebhookLog") == [
+        {
+            **get_json_obj(model.first_party_webhook_log[0]),
+            "status": "ERROR",
+            "status_text": "Invalid webhook type",
+        },
+        {
+            **get_json_obj(model.first_party_webhook_log[1]),
+            "status": "ERROR",
+            "status_text": "Invalid webhook type",
+        },
+    ]
+    assert import_external_user.call_args_list == []
+
+
+@pytest.mark.parametrize(
+    "delta,attempts,type",
+    [
+        (timedelta(0), 0, "user.created"),
+        (timedelta(0), 0, "user.updated"),
+        (timedelta(minutes=21), 1, "user.created"),
+        (timedelta(minutes=22), 2, "user.updated"),
+        (timedelta(minutes=23), 3, "user.created"),
+        (timedelta(minutes=24), 4, "user.updated"),
+        (timedelta(minutes=25), 5, "user.created"),
+    ],
+)
+def test__user_events_scheduled(database, patch, freeze_time, delta, attempts, type, get_json_obj):
+    import_external_user = patch
+
+    model = database.create(first_party_webhook_log=(2, {"attempts": attempts, "external_id": 1, "type": type}))
+
+    freeze_time(T1 + delta)
+
+    command = Command()
+    command.handle()
+
+    assert database.list_of("linked_services.FirstPartyWebhookLog") == [
+        {
+            **get_json_obj(model.first_party_webhook_log[0]),
+            "status": "PENDING",
+        },
+        {
+            **get_json_obj(model.first_party_webhook_log[1]),
+            "status": "PENDING",
+        },
+    ]
+    assert import_external_user.call_args_list == [call(1), call(2)]
```

### Comparing `linked_services-1.2.1/tests/management/commands/test_sign_jwt.py` & `linked_services-1.2.2/tests/management/commands/test_sign_jwt.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-"""
-Test /academy/cohort
-"""
-
-from unittest.mock import MagicMock, call, patch
-
-import pytest
-from django.core.management.base import OutputWrapper
-
-from linked_services.management.commands.sign_jwt import Command
-
-
-@pytest.fixture(autouse=True)
-def setup(db, monkeypatch):
-    monkeypatch.setattr("django.core.management.base.OutputWrapper.write", MagicMock())
-    yield
-
-
-# When: No app
-# Then: Shouldn't do anything
-def test_no_app(database, fake):
-    command = Command()
-    result = command.handle(app="1", user=None)
-
-    assert result is None
-    assert database.list_of("linked_services.App") == []
-    assert OutputWrapper.write.call_args_list == [
-        call("App 1 not found"),
-    ]
-
-
-# When: With app
-# Then: Print the token
-def test_sign_jwt(database, fake, get_json_obj, monkeypatch):
-    private_key = fake.slug()
-    model = database.create(app={"private_key": private_key.encode().hex()})
-
-    command = Command()
-
-    token = fake.slug()
-    monkeypatch.setattr("jwt.encode", MagicMock(return_value=token))
-
-    result = command.handle(app="1", user=None)
-
-    assert result is None
-    assert database.list_of("linked_services.App") == [get_json_obj(model.app)]
-    assert OutputWrapper.write.call_args_list == [
-        call(f"Authorization: Link App={model.app.slug}," f"Token={token}"),
-    ]
+"""
+Test /academy/cohort
+"""
+
+from unittest.mock import MagicMock, call, patch
+
+import pytest
+from django.core.management.base import OutputWrapper
+
+from linked_services.management.commands.sign_jwt import Command
+
+
+@pytest.fixture(autouse=True)
+def setup(db, monkeypatch):
+    monkeypatch.setattr("django.core.management.base.OutputWrapper.write", MagicMock())
+    yield
+
+
+# When: No app
+# Then: Shouldn't do anything
+def test_no_app(database, fake):
+    command = Command()
+    result = command.handle(app="1", user=None)
+
+    assert result is None
+    assert database.list_of("linked_services.App") == []
+    assert OutputWrapper.write.call_args_list == [
+        call("App 1 not found"),
+    ]
+
+
+# When: With app
+# Then: Print the token
+def test_sign_jwt(database, fake, get_json_obj, monkeypatch):
+    private_key = fake.slug()
+    model = database.create(app={"private_key": private_key.encode().hex()})
+
+    command = Command()
+
+    token = fake.slug()
+    monkeypatch.setattr("jwt.encode", MagicMock(return_value=token))
+
+    result = command.handle(app="1", user=None)
+
+    assert result is None
+    assert database.list_of("linked_services.App") == [get_json_obj(model.app)]
+    assert OutputWrapper.write.call_args_list == [
+        call(f"Authorization: Link App={model.app.slug}," f"Token={token}"),
+    ]
```

### Comparing `linked_services-1.2.1/tests/management/commands/test_sign_request.py` & `linked_services-1.2.2/tests/management/commands/test_sign_request.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-"""
-Test /academy/cohort
-"""
-
-from datetime import datetime
-from unittest.mock import MagicMock, call, patch
-
-import pytest
-from django.core.management.base import OutputWrapper
-
-from linked_services.management.commands.sign_request import Command
-
-
-@pytest.fixture(autouse=True)
-def setup(db, monkeypatch):
-    monkeypatch.setattr("django.core.management.base.OutputWrapper.write", MagicMock())
-    yield
-
-
-"""
-🔽🔽🔽 With zero Profile
-"""
-
-
-# When: No app
-# Then: Shouldn't do anything
-def test_no_app(database):
-    command = Command()
-    result = command.handle(app="1", user=None, method=None, params=None, body=None, headers=None)
-
-    assert result is None
-    assert database.list_of("linked_services.App") == []
-    assert OutputWrapper.write.call_args_list == [
-        call("App 1 not found"),
-    ]
-
-
-# When: With app
-# Then: Print the signature
-def test_sign_jwt(database, fake, monkeypatch, get_json_obj):
-    headers = {
-        fake.slug(): fake.slug(),
-        fake.slug(): fake.slug(),
-        fake.slug(): fake.slug(),
-    }
-    private_key = fake.slug()
-    model = database.create(app={"private_key": private_key.encode().hex()})
-
-    command = Command()
-
-    token = fake.slug()
-    d = datetime(2023, 8, 3, 4, 2, 58, 992939)
-
-    monkeypatch.setattr("hmac.HMAC.hexdigest", MagicMock(return_value=token))
-    monkeypatch.setattr("django.utils.timezone.now", MagicMock(return_value=d))
-
-    result = command.handle(
-        app="1",
-        user=None,
-        method=f"{headers}",
-        params=f"{headers}",
-        body=f"{headers}",
-        headers=f"{headers}",
-    )
-
-    assert result is None
-    assert database.list_of("linked_services.App") == [get_json_obj(model.app)]
-    assert OutputWrapper.write.call_args_list == [
-        call(
-            f"Authorization: Signature App={model.app.slug},"
-            f"Nonce={token},"
-            f'SignedHeaders={";".join(headers.keys())},'
-            f"Date={d.isoformat()}"
-        ),
-    ]
+"""
+Test /academy/cohort
+"""
+
+from datetime import datetime
+from unittest.mock import MagicMock, call, patch
+
+import pytest
+from django.core.management.base import OutputWrapper
+
+from linked_services.management.commands.sign_request import Command
+
+
+@pytest.fixture(autouse=True)
+def setup(db, monkeypatch):
+    monkeypatch.setattr("django.core.management.base.OutputWrapper.write", MagicMock())
+    yield
+
+
+"""
+🔽🔽🔽 With zero Profile
+"""
+
+
+# When: No app
+# Then: Shouldn't do anything
+def test_no_app(database):
+    command = Command()
+    result = command.handle(app="1", user=None, method=None, params=None, body=None, headers=None)
+
+    assert result is None
+    assert database.list_of("linked_services.App") == []
+    assert OutputWrapper.write.call_args_list == [
+        call("App 1 not found"),
+    ]
+
+
+# When: With app
+# Then: Print the signature
+def test_sign_jwt(database, fake, monkeypatch, get_json_obj):
+    headers = {
+        fake.slug(): fake.slug(),
+        fake.slug(): fake.slug(),
+        fake.slug(): fake.slug(),
+    }
+    private_key = fake.slug()
+    model = database.create(app={"private_key": private_key.encode().hex()})
+
+    command = Command()
+
+    token = fake.slug()
+    d = datetime(2023, 8, 3, 4, 2, 58, 992939)
+
+    monkeypatch.setattr("hmac.HMAC.hexdigest", MagicMock(return_value=token))
+    monkeypatch.setattr("django.utils.timezone.now", MagicMock(return_value=d))
+
+    result = command.handle(
+        app="1",
+        user=None,
+        method=f"{headers}",
+        params=f"{headers}",
+        body=f"{headers}",
+        headers=f"{headers}",
+    )
+
+    assert result is None
+    assert database.list_of("linked_services.App") == [get_json_obj(model.app)]
+    assert OutputWrapper.write.call_args_list == [
+        call(
+            f"Authorization: Signature App={model.app.slug},"
+            f"Nonce={token},"
+            f'SignedHeaders={";".join(headers.keys())},'
+            f"Date={d.isoformat()}"
+        ),
+    ]
```

### Comparing `linked_services-1.2.1/tests/rest_framework/views/test_authorize_view.py` & `linked_services-1.2.2/tests/rest_framework/views/test_authorize_view.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,613 +1,613 @@
-import base64
-import os
-import random
-import urllib.parse
-from datetime import timedelta
-from unittest.mock import MagicMock, patch
-
-import pytest
-from django.http import HttpRequest
-from django.shortcuts import redirect, render
-from django.test import RequestFactory
-from django.utils import timezone
-from rest_framework.test import APIRequestFactory, force_authenticate
-
-from linked_services.core.settings import set_settings
-from linked_services.rest_framework.views import authorize_view
-
-
-async def fix_data(apps=[], scopes=[]):
-
-    def fixer(s):
-        for word in ["permissions", "required", "optional", "checked", "New", "new"]:
-            s = s.replace(word, "x")
-
-        return s
-
-    for app in apps:
-        app.name = fixer(app.name)
-        app.slug = fixer(app.slug)
-        app.description = fixer(app.description)
-        await app.asave()
-
-    for scope in scopes:
-        scope.name = fixer(scope.name)
-        scope.slug = fixer(scope.slug)
-        scope.description = fixer(scope.description)
-        await scope.asave()
-
-
-@pytest.fixture(autouse=True)
-def setup(db: None, database, set_env, fake, monkeypatch: pytest.MonkeyPatch):
-    set_settings(app_name="breathecode")
-    set_env(LOGIN_URL=fake.url(), APP_URL=fake.url())
-
-    def get_scopes(n=0):
-        for n in range(n):
-            slug = fake.slug().replace("-", "_")[:7]
-
-            if random.randint(0, 1):
-                slug += ":" + fake.slug().replace("-", "_")[:7]
-
-            yield {"slug": slug}
-        ...
-
-    async def fn(
-        user=0, app=0, optional_scope_set=0, app_user_agreement=0, scopes=0, optional_scopes=0, required_scopes=0
-    ):
-        # app = {'require_an_agreement': True}
-        # optional_scope_set = {"optional_scopes": []}
-        # import timezone from django
-
-        now = timezone.now()
-        # app_user_agreement = {"agreed_at": now - timedelta(days=1)}
-
-        scopes = [*get_scopes(scopes)]
-
-        if app and isinstance(optional_scopes, list) and isinstance(required_scopes, list):
-            app_required_scopes = required_scopes
-            app_optional_scopes = optional_scopes
-
-        elif app and len(scopes) >= optional_scopes + required_scopes:
-            app_optional_scopes = [
-                {
-                    "app_id": 1,
-                    "scope_id": n + 1,
-                    "agreed_at": now,
-                }
-                for n in range(optional_scopes)
-            ]
-
-            app_required_scopes = [
-                {
-                    "app_id": 1,
-                    "scope_id": optional_scopes + n + 1,
-                    "agreed_at": now,
-                }
-                for n in range(required_scopes)
-            ]
-
-        elif app and optional_scopes + required_scopes != 0:
-            raise Exception("Invalid number of scopes")
-
-        else:
-            app_required_scopes = []
-            app_optional_scopes = []
-
-        model = await database.acreate(
-            user=user,
-            app=app,
-            scope=scopes,
-            app_user_agreement=app_user_agreement,
-            optional_scope_set=optional_scope_set,
-            app_required_scope=app_required_scopes,
-            app_optional_scope=app_optional_scopes,
-        )
-
-        apps = []
-        scopes = []
-
-        if "app" in model:
-            if isinstance(model.app, list):
-                apps = model.app
-            else:
-                apps = [model.app]
-
-        if "scope" in model:
-            if isinstance(model.scope, list):
-                scopes = model.scope
-            else:
-                scopes = [model.scope]
-
-        await fix_data(apps=apps, scopes=scopes)
-        return model
-
-    with patch("django.template.context_processors.get_token", MagicMock(return_value="predicabletoken")):
-        yield fn
-
-
-# class AnonymousUser:
-#     def __init__(self):
-#         self.is_authenticated = False
-
-
-# class RequestMock:
-#     def __init__(self, method="GET", user=AnonymousUser()):
-#         self.method = method
-#         self.user = user
-
-#     async def auser(self):
-#         return self.user
-
-
-def encode(s):
-    return str(base64.b64encode(s.encode("utf-8")), "utf-8")
-
-
-def get_es_translations(request):
-    return "es"
-
-
-def get_en_translations(request):
-    return "en"
-
-
-class TestGet:
-
-    @pytest.mark.asyncio
-    @pytest.mark.django_db(reset_sequences=True)
-    @pytest.mark.parametrize("value", [None, "https://www.google.com"])
-    async def test_no_auth(self, fake, value):
-        view = authorize_view(login_url=value)
-        request = HttpRequest()
-        request.method = "GET"
-        request.path = fake.url()
-
-        response = await view(request, app_slug=fake.slug())
-        assert response.status_code == 302
-        assert response.content == b""
-
-        if value is None:
-            value = os.getenv("LOGIN_URL")
-
-        assert response.url == value + "?url=" + urllib.parse.quote(encode(request.get_full_path()))
-
-    @pytest.mark.asyncio
-    @pytest.mark.django_db(reset_sequences=True)
-    @pytest.mark.parametrize(
-        "value, get_language, translations",
-        [
-            (
-                None,
-                None,
-                {
-                    "title": "Not found",
-                    "description": "The app was not found",
-                    "btn": "Go back",
-                },
-            ),
-            (
-                "https://www.google.com",
-                get_es_translations,
-                {
-                    "title": "No encontrado",
-                    "description": "La app no fue encontrada",
-                    "btn": "Volver",
-                },
-            ),
-            (
-                "https://manageyourpig.com",
-                get_en_translations,
-                {
-                    "title": "Not found",
-                    "description": "The app was not found",
-                    "btn": "Go back",
-                },
-            ),
-        ],
-    )
-    async def test_app_not_found(self, fake, setup, value, get_language, translations):
-
-        view = authorize_view(app_url=value, get_language=get_language)
-        request = HttpRequest()
-        request.method = "GET"
-        model = await setup(user=1)
-        request.user = model.user
-        request.path = fake.url()
-
-        request_factory = APIRequestFactory()
-        request = request_factory.get(fake.url())  # Specify the path you need
-
-        force_authenticate(request, user=model.user)
-
-        response = await view(request, app_slug=fake.slug())
-
-        if value is None:
-            value = os.getenv("APP_URL")
-
-        expected = render(
-            request,
-            "app-not-found.html",
-            {
-                "app_url": value,
-                **translations,
-            },
-            status=404,
-        )
-
-        assert response.content == expected.content
-        assert response.status_code == expected.status_code
-
-    @pytest.mark.asyncio
-    @pytest.mark.django_db(reset_sequences=True)
-    async def test_agreement_message_without_any_scope(self, fake, database, setup):
-
-        view = authorize_view()
-        request = HttpRequest()
-        request.method = "GET"
-        model = await setup(user=1, app=1)
-        request.user = model.user
-        request.path = fake.url()
-
-        request_factory = APIRequestFactory()
-        request = request_factory.get(fake.url())  # Specify the path you need
-
-        force_authenticate(request, user=model.user)
-
-        response = await view(request, app_slug=model.app.slug)
-
-        expected = render(
-            request,
-            "authorize.html",
-            {
-                "app": model.app,
-                "required_scopes": [],
-                "optional_scopes": [],
-                "selected_scopes": [],
-                "new_scopes": [],
-                "reject_url": model.app.redirect_url + "?app=breathecode&status=rejected",
-            },
-        )
-
-        assert response.content == expected.content
-        assert response.status_code == expected.status_code
-
-    @pytest.mark.asyncio
-    @pytest.mark.django_db(reset_sequences=True)
-    @pytest.mark.parametrize("agreement, optional_scopes, required_scopes", [(True, 3, 3), (False, 0, 3), (True, 3, 0)])
-    async def test_agreement_message_with_some_scopes(self, fake, setup, agreement, optional_scopes, required_scopes):
-        extra = {}
-
-        if agreement:
-            extra = {"app_user_agreement": {"agreed_at": timezone.now() + timedelta(days=1)}}
-
-        view = authorize_view()
-        scopes = optional_scopes + required_scopes
-        model = await setup(
-            user=1, app=1, scopes=scopes, optional_scopes=optional_scopes, required_scopes=required_scopes, **extra
-        )
-
-        request = HttpRequest()
-        request.method = "GET"
-        request.user = model.user
-        request.path = fake.url()
-
-        request_factory = APIRequestFactory()
-        request = request_factory.get(fake.url())  # Specify the path you need
-
-        force_authenticate(request, user=model.user)
-
-        response = await view(request, app_slug=model.app.slug)
-
-        if scopes:
-            scopes = model.scope
-
-        required_scopes_list = []
-        optional_scopes_list = []
-
-        if required_scopes:
-            required_scopes_list = model.scope[optional_scopes : optional_scopes + required_scopes]
-
-        if optional_scopes:
-            optional_scopes_list = model.scope[:optional_scopes]
-
-        expected = render(
-            request,
-            "authorize.html",
-            {
-                "app": model.app,
-                "required_scopes": required_scopes_list,
-                "optional_scopes": optional_scopes_list,
-                "selected_scopes": [],
-                "new_scopes": [],
-                "reject_url": model.app.redirect_url + "?app=breathecode&status=rejected",
-            },
-        )
-
-        if response.content != expected.content or True:
-            with open("content.html", "w") as f:
-                f.write(response.content.decode("utf-8"))
-
-            with open("expected.html", "w") as f:
-                f.write(expected.content.decode("utf-8"))
-
-        assert response.content == expected.content
-        assert response.status_code == expected.status_code
-
-        content = response.content.decode("utf-8")
-
-        if optional_scopes:
-            assert content.count("Optional permissions") == 1
-        else:
-            assert content.count("Optional permissions") == 0
-
-        if required_scopes:
-            assert content.count("Required permissions") == 1
-        else:
-            assert content.count("Required permissions") == 0
-
-        if optional_scopes and required_scopes:
-            assert content.count("checked") == 6
-        else:
-            assert content.count("checked") == 3
-
-        assert content.count("New</span>") == 0
-
-    @pytest.mark.asyncio
-    @pytest.mark.django_db(reset_sequences=True)
-    async def test_agreement_message_with_some_new_scopes(self, fake, setup, database):
-
-        view = authorize_view()
-        scopes = 4
-        model = await setup(
-            user=1,
-            app=1,
-            scopes=4,
-            optional_scopes=2,
-            required_scopes=2,
-            app_user_agreement={"agreed_at": timezone.now() - timedelta(days=1)},
-            optional_scope_set={"optional_scopes": [1]},
-        )
-
-        request = HttpRequest()
-        request.method = "GET"
-        request.user = model.user
-        request.path = fake.url()
-
-        request_factory = APIRequestFactory()
-        request = request_factory.get(fake.url())
-
-        force_authenticate(request, user=model.user)
-
-        response = await view(request, app_slug=model.app.slug)
-
-        if scopes:
-            scopes = model.scope
-
-        required_scopes_list = model.scope[2:4]
-        optional_scopes_list = model.scope[:2]
-
-        expected = render(
-            request,
-            "authorize.html",
-            {
-                "app": model.app,
-                "required_scopes": required_scopes_list,
-                "optional_scopes": optional_scopes_list,
-                "selected_scopes": [model.scope[0].slug],
-                "new_scopes": [x.slug for x in model.scope],
-                "reject_url": model.app.redirect_url + "?app=breathecode&status=rejected",
-            },
-        )
-
-        if response.content != expected.content or True:
-            with open("content.html", "w") as f:
-                f.write(response.content.decode("utf-8"))
-
-            with open("expected.html", "w") as f:
-                f.write(expected.content.decode("utf-8"))
-
-        assert response.content == expected.content
-        assert response.status_code == expected.status_code
-
-        content = response.content.decode("utf-8")
-
-        assert content.count("Optional permissions") == 1
-        assert content.count("Required permissions") == 1
-        assert content.count("checked") == 3
-        assert content.count("New</span>") == 4
-
-
-class TestPost:
-
-    @pytest.mark.asyncio
-    @pytest.mark.django_db(reset_sequences=True)
-    @pytest.mark.parametrize("value", [None, "https://www.google.com"])
-    async def test_no_auth(self, fake, value):
-        view = authorize_view(login_url=value)
-        request = HttpRequest()
-        request.method = "POST"
-        request.path = fake.url()
-
-        response = await view(request, app_slug=fake.slug())
-        assert response.status_code == 302
-        assert response.content == b""
-
-        if value is None:
-            value = os.getenv("LOGIN_URL")
-
-        assert response.url == value + "?url=" + urllib.parse.quote(encode(request.get_full_path()))
-
-    @pytest.mark.asyncio
-    @pytest.mark.django_db(reset_sequences=True)
-    @pytest.mark.parametrize(
-        "value, get_language, translations",
-        [
-            (
-                None,
-                None,
-                {
-                    "title": "Not found",
-                    "description": "The app was not found",
-                    "btn": "Go back",
-                },
-            ),
-            (
-                "https://www.google.com",
-                get_es_translations,
-                {
-                    "title": "No encontrado",
-                    "description": "La app no fue encontrada",
-                    "btn": "Volver",
-                },
-            ),
-            (
-                "https://manageyourpig.com",
-                get_en_translations,
-                {
-                    "title": "Not found",
-                    "description": "The app was not found",
-                    "btn": "Go back",
-                },
-            ),
-        ],
-    )
-    async def test_app_not_found(self, fake, setup, value, get_language, translations):
-
-        view = authorize_view(app_url=value, get_language=get_language)
-        request = HttpRequest()
-        request.method = "POST"
-        model = await setup(user=1)
-        request.user = model.user
-        request.path = fake.url()
-
-        request_factory = APIRequestFactory()
-        request = request_factory.post(fake.url())  # Specify the path you need
-
-        force_authenticate(request, user=model.user)
-
-        response = await view(request, app_slug=fake.slug())
-
-        if value is None:
-            value = os.getenv("APP_URL")
-
-        expected = render(
-            request,
-            "app-not-found.html",
-            {
-                "app_url": value,
-                **translations,
-            },
-            status=404,
-        )
-
-        assert response.content == expected.content
-        assert response.status_code == expected.status_code
-
-    @pytest.mark.asyncio
-    @pytest.mark.django_db(reset_sequences=True)
-    async def test_agreement_message_without_any_scope(self, fake, database, setup):
-
-        view = authorize_view()
-        request = HttpRequest()
-        request.method = "POST"
-        model = await setup(user=1, app=1)
-        request.user = model.user
-        request.path = fake.url()
-
-        request_factory = APIRequestFactory()
-        request = request_factory.post(fake.url())  # Specify the path you need
-
-        force_authenticate(request, user=model.user)
-
-        response = await view(request, app_slug=model.app.slug)
-        expected = b""
-
-        if response.content != expected or True:
-            with open("content.html", "w") as f:
-                f.write(response.content.decode("utf-8"))
-
-            with open("expected.html", "w") as f:
-                f.write(expected.decode("utf-8"))
-
-        assert response.content == expected
-        assert response.status_code == 302
-        assert response.url == model.app.redirect_url + "?app=breathecode&status=authorized"
-
-    @pytest.mark.asyncio
-    @pytest.mark.django_db(reset_sequences=True)
-    @pytest.mark.parametrize("agreement, optional_scopes, required_scopes", [(True, 3, 3), (False, 0, 3), (True, 3, 0)])
-    async def test_agreement_message_with_some_scopes(self, fake, setup, agreement, optional_scopes, required_scopes):
-        extra = {}
-
-        if agreement:
-            extra = {"app_user_agreement": {"agreed_at": timezone.now() + timedelta(days=1)}}
-
-        view = authorize_view()
-        scopes = optional_scopes + required_scopes
-        model = await setup(
-            user=1, app=1, scopes=scopes, optional_scopes=optional_scopes, required_scopes=required_scopes, **extra
-        )
-
-        request = HttpRequest()
-        request.method = "POST"
-        request.user = model.user
-        request.path = fake.url()
-
-        request_factory = APIRequestFactory()
-        request = request_factory.post(fake.url())  # Specify the path you need
-
-        force_authenticate(request, user=model.user)
-
-        response = await view(request, app_slug=model.app.slug)
-        expected = b""
-
-        if response.content != expected or True:
-            with open("content.html", "w") as f:
-                f.write(response.content.decode("utf-8"))
-
-            with open("expected.html", "w") as f:
-                f.write(expected.decode("utf-8"))
-
-        assert response.content == expected
-        assert response.status_code == 302
-        assert response.url == model.app.redirect_url + "?app=breathecode&status=authorized"
-
-    @pytest.mark.asyncio
-    @pytest.mark.django_db(reset_sequences=True)
-    async def test_agreement_message_with_some_new_scopes(self, fake, setup, database):
-
-        view = authorize_view()
-        model = await setup(
-            user=1,
-            app=1,
-            scopes=4,
-            optional_scopes=2,
-            required_scopes=2,
-            app_user_agreement={"agreed_at": timezone.now() - timedelta(days=1)},
-            optional_scope_set={"optional_scopes": [1]},
-        )
-
-        request = HttpRequest()
-        request.method = "POST"
-        request.user = model.user
-        request.path = fake.url()
-
-        request_factory = APIRequestFactory()
-        request = request_factory.post(fake.url())
-
-        force_authenticate(request, user=model.user)
-
-        response = await view(request, app_slug=model.app.slug)
-        expected = b""
-
-        if response.content != expected or True:
-            with open("content.html", "w") as f:
-                f.write(response.content.decode("utf-8"))
-
-            with open("expected.html", "w") as f:
-                f.write(expected.decode("utf-8"))
-
-        assert response.content == expected
-        assert response.status_code == 302
-        assert response.url == model.app.redirect_url + "?app=breathecode&status=authorized"
+import base64
+import os
+import random
+import urllib.parse
+from datetime import timedelta
+from unittest.mock import MagicMock, patch
+
+import pytest
+from django.http import HttpRequest
+from django.shortcuts import redirect, render
+from django.test import RequestFactory
+from django.utils import timezone
+from rest_framework.test import APIRequestFactory, force_authenticate
+
+from linked_services.core.settings import set_settings
+from linked_services.rest_framework.views import authorize_view
+
+
+async def fix_data(apps=[], scopes=[]):
+
+    def fixer(s):
+        for word in ["permissions", "required", "optional", "checked", "New", "new"]:
+            s = s.replace(word, "x")
+
+        return s
+
+    for app in apps:
+        app.name = fixer(app.name)
+        app.slug = fixer(app.slug)
+        app.description = fixer(app.description)
+        await app.asave()
+
+    for scope in scopes:
+        scope.name = fixer(scope.name)
+        scope.slug = fixer(scope.slug)
+        scope.description = fixer(scope.description)
+        await scope.asave()
+
+
+@pytest.fixture(autouse=True)
+def setup(db: None, database, set_env, fake, monkeypatch: pytest.MonkeyPatch):
+    set_settings(app_name="breathecode")
+    set_env(LOGIN_URL=fake.url(), APP_URL=fake.url())
+
+    def get_scopes(n=0):
+        for n in range(n):
+            slug = fake.slug().replace("-", "_")[:7]
+
+            if random.randint(0, 1):
+                slug += ":" + fake.slug().replace("-", "_")[:7]
+
+            yield {"slug": slug}
+        ...
+
+    async def fn(
+        user=0, app=0, optional_scope_set=0, app_user_agreement=0, scopes=0, optional_scopes=0, required_scopes=0
+    ):
+        # app = {'require_an_agreement': True}
+        # optional_scope_set = {"optional_scopes": []}
+        # import timezone from django
+
+        now = timezone.now()
+        # app_user_agreement = {"agreed_at": now - timedelta(days=1)}
+
+        scopes = [*get_scopes(scopes)]
+
+        if app and isinstance(optional_scopes, list) and isinstance(required_scopes, list):
+            app_required_scopes = required_scopes
+            app_optional_scopes = optional_scopes
+
+        elif app and len(scopes) >= optional_scopes + required_scopes:
+            app_optional_scopes = [
+                {
+                    "app_id": 1,
+                    "scope_id": n + 1,
+                    "agreed_at": now,
+                }
+                for n in range(optional_scopes)
+            ]
+
+            app_required_scopes = [
+                {
+                    "app_id": 1,
+                    "scope_id": optional_scopes + n + 1,
+                    "agreed_at": now,
+                }
+                for n in range(required_scopes)
+            ]
+
+        elif app and optional_scopes + required_scopes != 0:
+            raise Exception("Invalid number of scopes")
+
+        else:
+            app_required_scopes = []
+            app_optional_scopes = []
+
+        model = await database.acreate(
+            user=user,
+            app=app,
+            scope=scopes,
+            app_user_agreement=app_user_agreement,
+            optional_scope_set=optional_scope_set,
+            app_required_scope=app_required_scopes,
+            app_optional_scope=app_optional_scopes,
+        )
+
+        apps = []
+        scopes = []
+
+        if "app" in model:
+            if isinstance(model.app, list):
+                apps = model.app
+            else:
+                apps = [model.app]
+
+        if "scope" in model:
+            if isinstance(model.scope, list):
+                scopes = model.scope
+            else:
+                scopes = [model.scope]
+
+        await fix_data(apps=apps, scopes=scopes)
+        return model
+
+    with patch("django.template.context_processors.get_token", MagicMock(return_value="predicabletoken")):
+        yield fn
+
+
+# class AnonymousUser:
+#     def __init__(self):
+#         self.is_authenticated = False
+
+
+# class RequestMock:
+#     def __init__(self, method="GET", user=AnonymousUser()):
+#         self.method = method
+#         self.user = user
+
+#     async def auser(self):
+#         return self.user
+
+
+def encode(s):
+    return str(base64.b64encode(s.encode("utf-8")), "utf-8")
+
+
+def get_es_translations(request):
+    return "es"
+
+
+def get_en_translations(request):
+    return "en"
+
+
+class TestGet:
+
+    @pytest.mark.asyncio
+    @pytest.mark.django_db(reset_sequences=True)
+    @pytest.mark.parametrize("value", [None, "https://www.google.com"])
+    async def test_no_auth(self, fake, value):
+        view = authorize_view(login_url=value)
+        request = HttpRequest()
+        request.method = "GET"
+        request.path = fake.url()
+
+        response = await view(request, app_slug=fake.slug())
+        assert response.status_code == 302
+        assert response.content == b""
+
+        if value is None:
+            value = os.getenv("LOGIN_URL")
+
+        assert response.url == value + "?url=" + urllib.parse.quote(encode(request.get_full_path()))
+
+    @pytest.mark.asyncio
+    @pytest.mark.django_db(reset_sequences=True)
+    @pytest.mark.parametrize(
+        "value, get_language, translations",
+        [
+            (
+                None,
+                None,
+                {
+                    "title": "Not found",
+                    "description": "The app was not found",
+                    "btn": "Go back",
+                },
+            ),
+            (
+                "https://www.google.com",
+                get_es_translations,
+                {
+                    "title": "No encontrado",
+                    "description": "La app no fue encontrada",
+                    "btn": "Volver",
+                },
+            ),
+            (
+                "https://manageyourpig.com",
+                get_en_translations,
+                {
+                    "title": "Not found",
+                    "description": "The app was not found",
+                    "btn": "Go back",
+                },
+            ),
+        ],
+    )
+    async def test_app_not_found(self, fake, setup, value, get_language, translations):
+
+        view = authorize_view(app_url=value, get_language=get_language)
+        request = HttpRequest()
+        request.method = "GET"
+        model = await setup(user=1)
+        request.user = model.user
+        request.path = fake.url()
+
+        request_factory = APIRequestFactory()
+        request = request_factory.get(fake.url())  # Specify the path you need
+
+        force_authenticate(request, user=model.user)
+
+        response = await view(request, app_slug=fake.slug())
+
+        if value is None:
+            value = os.getenv("APP_URL")
+
+        expected = render(
+            request,
+            "app-not-found.html",
+            {
+                "app_url": value,
+                **translations,
+            },
+            status=404,
+        )
+
+        assert response.content == expected.content
+        assert response.status_code == expected.status_code
+
+    @pytest.mark.asyncio
+    @pytest.mark.django_db(reset_sequences=True)
+    async def test_agreement_message_without_any_scope(self, fake, database, setup):
+
+        view = authorize_view()
+        request = HttpRequest()
+        request.method = "GET"
+        model = await setup(user=1, app=1)
+        request.user = model.user
+        request.path = fake.url()
+
+        request_factory = APIRequestFactory()
+        request = request_factory.get(fake.url())  # Specify the path you need
+
+        force_authenticate(request, user=model.user)
+
+        response = await view(request, app_slug=model.app.slug)
+
+        expected = render(
+            request,
+            "authorize.html",
+            {
+                "app": model.app,
+                "required_scopes": [],
+                "optional_scopes": [],
+                "selected_scopes": [],
+                "new_scopes": [],
+                "reject_url": model.app.redirect_url + "?app=breathecode&status=rejected",
+            },
+        )
+
+        assert response.content == expected.content
+        assert response.status_code == expected.status_code
+
+    @pytest.mark.asyncio
+    @pytest.mark.django_db(reset_sequences=True)
+    @pytest.mark.parametrize("agreement, optional_scopes, required_scopes", [(True, 3, 3), (False, 0, 3), (True, 3, 0)])
+    async def test_agreement_message_with_some_scopes(self, fake, setup, agreement, optional_scopes, required_scopes):
+        extra = {}
+
+        if agreement:
+            extra = {"app_user_agreement": {"agreed_at": timezone.now() + timedelta(days=1)}}
+
+        view = authorize_view()
+        scopes = optional_scopes + required_scopes
+        model = await setup(
+            user=1, app=1, scopes=scopes, optional_scopes=optional_scopes, required_scopes=required_scopes, **extra
+        )
+
+        request = HttpRequest()
+        request.method = "GET"
+        request.user = model.user
+        request.path = fake.url()
+
+        request_factory = APIRequestFactory()
+        request = request_factory.get(fake.url())  # Specify the path you need
+
+        force_authenticate(request, user=model.user)
+
+        response = await view(request, app_slug=model.app.slug)
+
+        if scopes:
+            scopes = model.scope
+
+        required_scopes_list = []
+        optional_scopes_list = []
+
+        if required_scopes:
+            required_scopes_list = model.scope[optional_scopes : optional_scopes + required_scopes]
+
+        if optional_scopes:
+            optional_scopes_list = model.scope[:optional_scopes]
+
+        expected = render(
+            request,
+            "authorize.html",
+            {
+                "app": model.app,
+                "required_scopes": required_scopes_list,
+                "optional_scopes": optional_scopes_list,
+                "selected_scopes": [],
+                "new_scopes": [],
+                "reject_url": model.app.redirect_url + "?app=breathecode&status=rejected",
+            },
+        )
+
+        if response.content != expected.content or True:
+            with open("content.html", "w") as f:
+                f.write(response.content.decode("utf-8"))
+
+            with open("expected.html", "w") as f:
+                f.write(expected.content.decode("utf-8"))
+
+        assert response.content == expected.content
+        assert response.status_code == expected.status_code
+
+        content = response.content.decode("utf-8")
+
+        if optional_scopes:
+            assert content.count("Optional permissions") == 1
+        else:
+            assert content.count("Optional permissions") == 0
+
+        if required_scopes:
+            assert content.count("Required permissions") == 1
+        else:
+            assert content.count("Required permissions") == 0
+
+        if optional_scopes and required_scopes:
+            assert content.count("checked") == 6
+        else:
+            assert content.count("checked") == 3
+
+        assert content.count("New</span>") == 0
+
+    @pytest.mark.asyncio
+    @pytest.mark.django_db(reset_sequences=True)
+    async def test_agreement_message_with_some_new_scopes(self, fake, setup, database):
+
+        view = authorize_view()
+        scopes = 4
+        model = await setup(
+            user=1,
+            app=1,
+            scopes=4,
+            optional_scopes=2,
+            required_scopes=2,
+            app_user_agreement={"agreed_at": timezone.now() - timedelta(days=1)},
+            optional_scope_set={"optional_scopes": [1]},
+        )
+
+        request = HttpRequest()
+        request.method = "GET"
+        request.user = model.user
+        request.path = fake.url()
+
+        request_factory = APIRequestFactory()
+        request = request_factory.get(fake.url())
+
+        force_authenticate(request, user=model.user)
+
+        response = await view(request, app_slug=model.app.slug)
+
+        if scopes:
+            scopes = model.scope
+
+        required_scopes_list = model.scope[2:4]
+        optional_scopes_list = model.scope[:2]
+
+        expected = render(
+            request,
+            "authorize.html",
+            {
+                "app": model.app,
+                "required_scopes": required_scopes_list,
+                "optional_scopes": optional_scopes_list,
+                "selected_scopes": [model.scope[0].slug],
+                "new_scopes": [x.slug for x in model.scope],
+                "reject_url": model.app.redirect_url + "?app=breathecode&status=rejected",
+            },
+        )
+
+        if response.content != expected.content or True:
+            with open("content.html", "w") as f:
+                f.write(response.content.decode("utf-8"))
+
+            with open("expected.html", "w") as f:
+                f.write(expected.content.decode("utf-8"))
+
+        assert response.content == expected.content
+        assert response.status_code == expected.status_code
+
+        content = response.content.decode("utf-8")
+
+        assert content.count("Optional permissions") == 1
+        assert content.count("Required permissions") == 1
+        assert content.count("checked") == 3
+        assert content.count("New</span>") == 4
+
+
+class TestPost:
+
+    @pytest.mark.asyncio
+    @pytest.mark.django_db(reset_sequences=True)
+    @pytest.mark.parametrize("value", [None, "https://www.google.com"])
+    async def test_no_auth(self, fake, value):
+        view = authorize_view(login_url=value)
+        request = HttpRequest()
+        request.method = "POST"
+        request.path = fake.url()
+
+        response = await view(request, app_slug=fake.slug())
+        assert response.status_code == 302
+        assert response.content == b""
+
+        if value is None:
+            value = os.getenv("LOGIN_URL")
+
+        assert response.url == value + "?url=" + urllib.parse.quote(encode(request.get_full_path()))
+
+    @pytest.mark.asyncio
+    @pytest.mark.django_db(reset_sequences=True)
+    @pytest.mark.parametrize(
+        "value, get_language, translations",
+        [
+            (
+                None,
+                None,
+                {
+                    "title": "Not found",
+                    "description": "The app was not found",
+                    "btn": "Go back",
+                },
+            ),
+            (
+                "https://www.google.com",
+                get_es_translations,
+                {
+                    "title": "No encontrado",
+                    "description": "La app no fue encontrada",
+                    "btn": "Volver",
+                },
+            ),
+            (
+                "https://manageyourpig.com",
+                get_en_translations,
+                {
+                    "title": "Not found",
+                    "description": "The app was not found",
+                    "btn": "Go back",
+                },
+            ),
+        ],
+    )
+    async def test_app_not_found(self, fake, setup, value, get_language, translations):
+
+        view = authorize_view(app_url=value, get_language=get_language)
+        request = HttpRequest()
+        request.method = "POST"
+        model = await setup(user=1)
+        request.user = model.user
+        request.path = fake.url()
+
+        request_factory = APIRequestFactory()
+        request = request_factory.post(fake.url())  # Specify the path you need
+
+        force_authenticate(request, user=model.user)
+
+        response = await view(request, app_slug=fake.slug())
+
+        if value is None:
+            value = os.getenv("APP_URL")
+
+        expected = render(
+            request,
+            "app-not-found.html",
+            {
+                "app_url": value,
+                **translations,
+            },
+            status=404,
+        )
+
+        assert response.content == expected.content
+        assert response.status_code == expected.status_code
+
+    @pytest.mark.asyncio
+    @pytest.mark.django_db(reset_sequences=True)
+    async def test_agreement_message_without_any_scope(self, fake, database, setup):
+
+        view = authorize_view()
+        request = HttpRequest()
+        request.method = "POST"
+        model = await setup(user=1, app=1)
+        request.user = model.user
+        request.path = fake.url()
+
+        request_factory = APIRequestFactory()
+        request = request_factory.post(fake.url())  # Specify the path you need
+
+        force_authenticate(request, user=model.user)
+
+        response = await view(request, app_slug=model.app.slug)
+        expected = b""
+
+        if response.content != expected or True:
+            with open("content.html", "w") as f:
+                f.write(response.content.decode("utf-8"))
+
+            with open("expected.html", "w") as f:
+                f.write(expected.decode("utf-8"))
+
+        assert response.content == expected
+        assert response.status_code == 302
+        assert response.url == model.app.redirect_url + "?app=breathecode&status=authorized"
+
+    @pytest.mark.asyncio
+    @pytest.mark.django_db(reset_sequences=True)
+    @pytest.mark.parametrize("agreement, optional_scopes, required_scopes", [(True, 3, 3), (False, 0, 3), (True, 3, 0)])
+    async def test_agreement_message_with_some_scopes(self, fake, setup, agreement, optional_scopes, required_scopes):
+        extra = {}
+
+        if agreement:
+            extra = {"app_user_agreement": {"agreed_at": timezone.now() + timedelta(days=1)}}
+
+        view = authorize_view()
+        scopes = optional_scopes + required_scopes
+        model = await setup(
+            user=1, app=1, scopes=scopes, optional_scopes=optional_scopes, required_scopes=required_scopes, **extra
+        )
+
+        request = HttpRequest()
+        request.method = "POST"
+        request.user = model.user
+        request.path = fake.url()
+
+        request_factory = APIRequestFactory()
+        request = request_factory.post(fake.url())  # Specify the path you need
+
+        force_authenticate(request, user=model.user)
+
+        response = await view(request, app_slug=model.app.slug)
+        expected = b""
+
+        if response.content != expected or True:
+            with open("content.html", "w") as f:
+                f.write(response.content.decode("utf-8"))
+
+            with open("expected.html", "w") as f:
+                f.write(expected.decode("utf-8"))
+
+        assert response.content == expected
+        assert response.status_code == 302
+        assert response.url == model.app.redirect_url + "?app=breathecode&status=authorized"
+
+    @pytest.mark.asyncio
+    @pytest.mark.django_db(reset_sequences=True)
+    async def test_agreement_message_with_some_new_scopes(self, fake, setup, database):
+
+        view = authorize_view()
+        model = await setup(
+            user=1,
+            app=1,
+            scopes=4,
+            optional_scopes=2,
+            required_scopes=2,
+            app_user_agreement={"agreed_at": timezone.now() - timedelta(days=1)},
+            optional_scope_set={"optional_scopes": [1]},
+        )
+
+        request = HttpRequest()
+        request.method = "POST"
+        request.user = model.user
+        request.path = fake.url()
+
+        request_factory = APIRequestFactory()
+        request = request_factory.post(fake.url())
+
+        force_authenticate(request, user=model.user)
+
+        response = await view(request, app_slug=model.app.slug)
+        expected = b""
+
+        if response.content != expected or True:
+            with open("content.html", "w") as f:
+                f.write(response.content.decode("utf-8"))
+
+            with open("expected.html", "w") as f:
+                f.write(expected.decode("utf-8"))
+
+        assert response.content == expected
+        assert response.status_code == 302
+        assert response.url == model.app.redirect_url + "?app=breathecode&status=authorized"
```

### Comparing `linked_services-1.2.1/LICENSE.txt` & `linked_services-1.2.2/LICENSE.txt`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-# GNU LESSER GENERAL PUBLIC LICENSE
-
-Version 3, 29 June 2007
-
-Copyright (C) 2007 Free Software Foundation, Inc.
-<https://fsf.org/>
-
-Everyone is permitted to copy and distribute verbatim copies of this
-license document, but changing it is not allowed.
-
-This version of the GNU Lesser General Public License incorporates the
-terms and conditions of version 3 of the GNU General Public License,
-supplemented by the additional permissions listed below.
-
-## 0. Additional Definitions.
-
-As used herein, "this License" refers to version 3 of the GNU Lesser
-General Public License, and the "GNU GPL" refers to version 3 of the
-GNU General Public License.
-
-"The Library" refers to a covered work governed by this License, other
-than an Application or a Combined Work as defined below.
-
-An "Application" is any work that makes use of an interface provided
-by the Library, but which is not otherwise based on the Library.
-Defining a subclass of a class defined by the Library is deemed a mode
-of using an interface provided by the Library.
-
-A "Combined Work" is a work produced by combining or linking an
-Application with the Library. The particular version of the Library
-with which the Combined Work was made is also called the "Linked
-Version".
-
-The "Minimal Corresponding Source" for a Combined Work means the
-Corresponding Source for the Combined Work, excluding any source code
-for portions of the Combined Work that, considered in isolation, are
-based on the Application, and not on the Linked Version.
-
-The "Corresponding Application Code" for a Combined Work means the
-object code and/or source code for the Application, including any data
-and utility programs needed for reproducing the Combined Work from the
-Application, but excluding the System Libraries of the Combined Work.
-
-## 1. Exception to Section 3 of the GNU GPL.
-
-You may convey a covered work under sections 3 and 4 of this License
-without being bound by section 3 of the GNU GPL.
-
-## 2. Conveying Modified Versions.
-
-If you modify a copy of the Library, and, in your modifications, a
-facility refers to a function or data to be supplied by an Application
-that uses the facility (other than as an argument passed when the
-facility is invoked), then you may convey a copy of the modified
-version:
-
--   a) under this License, provided that you make a good faith effort
-    to ensure that, in the event an Application does not supply the
-    function or data, the facility still operates, and performs
-    whatever part of its purpose remains meaningful, or
--   b) under the GNU GPL, with none of the additional permissions of
-    this License applicable to that copy.
-
-## 3. Object Code Incorporating Material from Library Header Files.
-
-The object code form of an Application may incorporate material from a
-header file that is part of the Library. You may convey such object
-code under terms of your choice, provided that, if the incorporated
-material is not limited to numerical parameters, data structure
-layouts and accessors, or small macros, inline functions and templates
-(ten or fewer lines in length), you do both of the following:
-
--   a) Give prominent notice with each copy of the object code that
-    the Library is used in it and that the Library and its use are
-    covered by this License.
--   b) Accompany the object code with a copy of the GNU GPL and this
-    license document.
-
-## 4. Combined Works.
-
-You may convey a Combined Work under terms of your choice that, taken
-together, effectively do not restrict modification of the portions of
-the Library contained in the Combined Work and reverse engineering for
-debugging such modifications, if you also do each of the following:
-
--   a) Give prominent notice with each copy of the Combined Work that
-    the Library is used in it and that the Library and its use are
-    covered by this License.
--   b) Accompany the Combined Work with a copy of the GNU GPL and this
-    license document.
--   c) For a Combined Work that displays copyright notices during
-    execution, include the copyright notice for the Library among
-    these notices, as well as a reference directing the user to the
-    copies of the GNU GPL and this license document.
--   d) Do one of the following:
-    -   0) Convey the Minimal Corresponding Source under the terms of
-        this License, and the Corresponding Application Code in a form
-        suitable for, and under terms that permit, the user to
-        recombine or relink the Application with a modified version of
-        the Linked Version to produce a modified Combined Work, in the
-        manner specified by section 6 of the GNU GPL for conveying
-        Corresponding Source.
-    -   1) Use a suitable shared library mechanism for linking with
-        the Library. A suitable mechanism is one that (a) uses at run
-        time a copy of the Library already present on the user's
-        computer system, and (b) will operate properly with a modified
-        version of the Library that is interface-compatible with the
-        Linked Version.
--   e) Provide Installation Information, but only if you would
-    otherwise be required to provide such information under section 6
-    of the GNU GPL, and only to the extent that such information is
-    necessary to install and execute a modified version of the
-    Combined Work produced by recombining or relinking the Application
-    with a modified version of the Linked Version. (If you use option
-    4d0, the Installation Information must accompany the Minimal
-    Corresponding Source and Corresponding Application Code. If you
-    use option 4d1, you must provide the Installation Information in
-    the manner specified by section 6 of the GNU GPL for conveying
-    Corresponding Source.)
-
-## 5. Combined Libraries.
-
-You may place library facilities that are a work based on the Library
-side by side in a single library together with other library
-facilities that are not Applications and are not covered by this
-License, and convey such a combined library under terms of your
-choice, if you do both of the following:
-
--   a) Accompany the combined library with a copy of the same work
-    based on the Library, uncombined with any other library
-    facilities, conveyed under the terms of this License.
--   b) Give prominent notice with the combined library that part of it
-    is a work based on the Library, and explaining where to find the
-    accompanying uncombined form of the same work.
-
-## 6. Revised Versions of the GNU Lesser General Public License.
-
-The Free Software Foundation may publish revised and/or new versions
-of the GNU Lesser General Public License from time to time. Such new
-versions will be similar in spirit to the present version, but may
-differ in detail to address new problems or concerns.
-
-Each version is given a distinguishing version number. If the Library
-as you received it specifies that a certain numbered version of the
-GNU Lesser General Public License "or any later version" applies to
-it, you have the option of following the terms and conditions either
-of that published version or of any later version published by the
-Free Software Foundation. If the Library as you received it does not
-specify a version number of the GNU Lesser General Public License, you
-may choose any version of the GNU Lesser General Public License ever
-published by the Free Software Foundation.
-
-If the Library as you received it specifies that a proxy can decide
-whether future versions of the GNU Lesser General Public License shall
-apply, that proxy's public statement of acceptance of any version is
-permanent authorization for you to choose that version for the
-Library.
+# GNU LESSER GENERAL PUBLIC LICENSE
+
+Version 3, 29 June 2007
+
+Copyright (C) 2007 Free Software Foundation, Inc.
+<https://fsf.org/>
+
+Everyone is permitted to copy and distribute verbatim copies of this
+license document, but changing it is not allowed.
+
+This version of the GNU Lesser General Public License incorporates the
+terms and conditions of version 3 of the GNU General Public License,
+supplemented by the additional permissions listed below.
+
+## 0. Additional Definitions.
+
+As used herein, "this License" refers to version 3 of the GNU Lesser
+General Public License, and the "GNU GPL" refers to version 3 of the
+GNU General Public License.
+
+"The Library" refers to a covered work governed by this License, other
+than an Application or a Combined Work as defined below.
+
+An "Application" is any work that makes use of an interface provided
+by the Library, but which is not otherwise based on the Library.
+Defining a subclass of a class defined by the Library is deemed a mode
+of using an interface provided by the Library.
+
+A "Combined Work" is a work produced by combining or linking an
+Application with the Library. The particular version of the Library
+with which the Combined Work was made is also called the "Linked
+Version".
+
+The "Minimal Corresponding Source" for a Combined Work means the
+Corresponding Source for the Combined Work, excluding any source code
+for portions of the Combined Work that, considered in isolation, are
+based on the Application, and not on the Linked Version.
+
+The "Corresponding Application Code" for a Combined Work means the
+object code and/or source code for the Application, including any data
+and utility programs needed for reproducing the Combined Work from the
+Application, but excluding the System Libraries of the Combined Work.
+
+## 1. Exception to Section 3 of the GNU GPL.
+
+You may convey a covered work under sections 3 and 4 of this License
+without being bound by section 3 of the GNU GPL.
+
+## 2. Conveying Modified Versions.
+
+If you modify a copy of the Library, and, in your modifications, a
+facility refers to a function or data to be supplied by an Application
+that uses the facility (other than as an argument passed when the
+facility is invoked), then you may convey a copy of the modified
+version:
+
+-   a) under this License, provided that you make a good faith effort
+    to ensure that, in the event an Application does not supply the
+    function or data, the facility still operates, and performs
+    whatever part of its purpose remains meaningful, or
+-   b) under the GNU GPL, with none of the additional permissions of
+    this License applicable to that copy.
+
+## 3. Object Code Incorporating Material from Library Header Files.
+
+The object code form of an Application may incorporate material from a
+header file that is part of the Library. You may convey such object
+code under terms of your choice, provided that, if the incorporated
+material is not limited to numerical parameters, data structure
+layouts and accessors, or small macros, inline functions and templates
+(ten or fewer lines in length), you do both of the following:
+
+-   a) Give prominent notice with each copy of the object code that
+    the Library is used in it and that the Library and its use are
+    covered by this License.
+-   b) Accompany the object code with a copy of the GNU GPL and this
+    license document.
+
+## 4. Combined Works.
+
+You may convey a Combined Work under terms of your choice that, taken
+together, effectively do not restrict modification of the portions of
+the Library contained in the Combined Work and reverse engineering for
+debugging such modifications, if you also do each of the following:
+
+-   a) Give prominent notice with each copy of the Combined Work that
+    the Library is used in it and that the Library and its use are
+    covered by this License.
+-   b) Accompany the Combined Work with a copy of the GNU GPL and this
+    license document.
+-   c) For a Combined Work that displays copyright notices during
+    execution, include the copyright notice for the Library among
+    these notices, as well as a reference directing the user to the
+    copies of the GNU GPL and this license document.
+-   d) Do one of the following:
+    -   0) Convey the Minimal Corresponding Source under the terms of
+        this License, and the Corresponding Application Code in a form
+        suitable for, and under terms that permit, the user to
+        recombine or relink the Application with a modified version of
+        the Linked Version to produce a modified Combined Work, in the
+        manner specified by section 6 of the GNU GPL for conveying
+        Corresponding Source.
+    -   1) Use a suitable shared library mechanism for linking with
+        the Library. A suitable mechanism is one that (a) uses at run
+        time a copy of the Library already present on the user's
+        computer system, and (b) will operate properly with a modified
+        version of the Library that is interface-compatible with the
+        Linked Version.
+-   e) Provide Installation Information, but only if you would
+    otherwise be required to provide such information under section 6
+    of the GNU GPL, and only to the extent that such information is
+    necessary to install and execute a modified version of the
+    Combined Work produced by recombining or relinking the Application
+    with a modified version of the Linked Version. (If you use option
+    4d0, the Installation Information must accompany the Minimal
+    Corresponding Source and Corresponding Application Code. If you
+    use option 4d1, you must provide the Installation Information in
+    the manner specified by section 6 of the GNU GPL for conveying
+    Corresponding Source.)
+
+## 5. Combined Libraries.
+
+You may place library facilities that are a work based on the Library
+side by side in a single library together with other library
+facilities that are not Applications and are not covered by this
+License, and convey such a combined library under terms of your
+choice, if you do both of the following:
+
+-   a) Accompany the combined library with a copy of the same work
+    based on the Library, uncombined with any other library
+    facilities, conveyed under the terms of this License.
+-   b) Give prominent notice with the combined library that part of it
+    is a work based on the Library, and explaining where to find the
+    accompanying uncombined form of the same work.
+
+## 6. Revised Versions of the GNU Lesser General Public License.
+
+The Free Software Foundation may publish revised and/or new versions
+of the GNU Lesser General Public License from time to time. Such new
+versions will be similar in spirit to the present version, but may
+differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Library
+as you received it specifies that a certain numbered version of the
+GNU Lesser General Public License "or any later version" applies to
+it, you have the option of following the terms and conditions either
+of that published version or of any later version published by the
+Free Software Foundation. If the Library as you received it does not
+specify a version number of the GNU Lesser General Public License, you
+may choose any version of the GNU Lesser General Public License ever
+published by the Free Software Foundation.
+
+If the Library as you received it specifies that a proxy can decide
+whether future versions of the GNU Lesser General Public License shall
+apply, that proxy's public statement of acceptance of any version is
+permanent authorization for you to choose that version for the
+Library.
```

### Comparing `linked_services-1.2.1/README.md` & `linked_services-1.2.2/README.md`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-# linked-services
-
-[![PyPI - Version](https://img.shields.io/pypi/v/linked-services.svg)](https://pypi.org/project/linked-services)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/linked-services.svg)](https://pypi.org/project/linked-services)
-
----
-
-**Table of Contents**
-
-- [What does this](#what-does-this)
-- [Installation](#installation)
-- [License](#license)
-
-## What does this
-
-Linked Services was made by [4geeks.com](https://4geeks.com) to manage communication between multiple services and microservices, it manages specifically communications between pairwise services, so, if only two services share the same key, a request just could has two emisors, the other service and itself. It was designed to replace the signature algorithms because them are significally slower.
-
-## Installation
-
-You should install linked-services with a few optional dependencies running:
-
-```bash
-pip install linked-services[django,requests,aiohttp]
-```
-
-### Optional dependencies
-
-#### django
-
-- django
-- djangorestframework
-- celery-task-manager[django]
-- adrf
-
-#### requests
-
-- requests
-- brotli
-
-#### httpx
-
-- httpx
-- httpcore
-- h11
-- idna
-- brotli
-
-#### aiohttp
-
-- aiohttp
-- aiodns
-- brotli
-
-## License
-
-`linked-services` is distributed under the terms of the [LGPL 3.0](https://spdx.org/licenses/LGPL-3.0-or-later.html) license.
+# linked-services
+
+[![PyPI - Version](https://img.shields.io/pypi/v/linked-services.svg)](https://pypi.org/project/linked-services)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/linked-services.svg)](https://pypi.org/project/linked-services)
+
+---
+
+**Table of Contents**
+
+- [What does this](#what-does-this)
+- [Installation](#installation)
+- [License](#license)
+
+## What does this
+
+Linked Services was made by [4geeks.com](https://4geeks.com) to manage communication between multiple services and microservices, it manages specifically communications between pairwise services, so, if only two services share the same key, a request just could has two emisors, the other service and itself. It was designed to replace the signature algorithms because them are significally slower.
+
+## Installation
+
+You should install linked-services with a few optional dependencies running:
+
+```bash
+pip install linked-services[django,requests,aiohttp]
+```
+
+### Optional dependencies
+
+#### django
+
+- django
+- djangorestframework
+- celery-task-manager[django]
+- adrf
+
+#### requests
+
+- requests
+- brotli
+
+#### httpx
+
+- httpx
+- httpcore
+- h11
+- idna
+- brotli
+
+#### aiohttp
+
+- aiohttp
+- aiodns
+- brotli
+
+## License
+
+`linked-services` is distributed under the terms of the [LGPL 3.0](https://spdx.org/licenses/LGPL-3.0-or-later.html) license.
```

### Comparing `linked_services-1.2.1/pyproject.toml` & `linked_services-1.2.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,139 +1,140 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "linked-services"
-dynamic = ["version"]
-description = ''
-readme = "README.md"
-requires-python = ">=3.10"
-license = "LGPL-3.0-or-later"
-keywords = []
-authors = [{ name = "jefer94", email = "jdefreitaspinto@gmail.com" }]
-classifiers = [
-  "Development Status :: 5 - Production/Stable",
-  "Programming Language :: Python",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: 3.12",
-  "Programming Language :: Python :: Implementation :: CPython",
-  "Programming Language :: Python :: Implementation :: PyPy",
-  "Framework :: Django :: 4.2",
-  "Framework :: Django :: 5.0",
-  "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
-  "Topic :: Software Development :: Libraries",
-]
-dependencies = [
-  "python-slugify",
-  "asgiref",
-  "pyjwt",
-  "cryptography",
-  "celery-task-manager",
-]
-
-[project.urls]
-Documentation = "https://breatheco-de.github.io/linked-services-django-plugin/"
-Issues = "https://github.com/breatheco-de/linked-services-django-plugin/issues"
-Source = "https://github.com/breatheco-de/linked-services-django-plugin"
-
-
-[tool.hatch.build.targets.wheel]
-packages = ["src/linked_services"]
-
-[tool.hatch.version]
-path = "src/linked_services/__about__.py"
-
-[tool.hatch.envs.default]
-dependencies = [
-  "coverage[toml]>=6.5",
-  "pytest",
-  "pytest-django",
-  "black",
-  "anyio[trio]",
-  "django",
-  "djangorestframework",
-  "requests",
-  "aiohttp",
-  "aiodns",
-  "httpx",
-  "httpcore",
-  "h11",
-  "idna",
-  "brotli",
-  "pyjwt",
-  "mkdocs",
-  "mkdocs-material",
-  "celery",
-  "celery-task-manager[django]>=1.0.0b6",
-  "adrf",
-  "faker",
-  "pytest-celery",
-  "celery[pytest]",
-  "pytest-asyncio",
-]
-[tool.hatch.envs.default.scripts]
-test = "pytest {args:tests} --nomigrations --durations=1 --create-db"
-test-cov = "coverage run -m pytest {args:tests} --nomigrations --durations=1"
-cov-report = ["- coverage combine", "coverage report"]
-cov = ["test-cov", "cov-report"]
-docs = "mkdocs serve --livereload"
-generate_docs = "mkdocs build"
-docs_deploy = "mkdocs gh-deploy -c"
-
-[[tool.hatch.envs.all.matrix]]
-python = ["3.11", "3.12"]
-
-[tool.hatch.envs.types]
-dependencies = ["mypy>=1.0.0"]
-[tool.hatch.envs.types.scripts]
-check = "mypy --install-types --non-interactive {args:src/linked_services tests}"
-
-[tool.coverage.run]
-source_pkgs = ["linked_services", "tests"]
-branch = true
-parallel = true
-omit = ["src/linked_services/__about__.py"]
-
-[tool.coverage.paths]
-linked_services = [
-  "src/linked_services",
-  "*/linked-services/src/linked_services",
-]
-tests = ["tests", "*/linked-services/tests"]
-
-[tool.coverage.report]
-exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
-
-[project.optional-dependencies]
-django = [
-  "django",
-  "djangorestframework",
-  "celery-task-manager[django]",
-  "adrf",
-]
-requests = ["requests", "brotli"]
-aiohttp = ["aiohttp", "aiodns", "brotli"]
-httpx = ["httpx", "httpcore", "h11", "idna", "brotli"]
-
-[tool.black]
-line-length = 120
-
-[tool.flake8]
-max-line-length = 120
-
-[tool.pytest.ini_options]
-django_debug_mode = true
-addopts = ["-p", "no:legacypath", "--tb=short"]
-DJANGO_SETTINGS_MODULE = "linked_services.settings"
-# python_files = ["breathecode/**/*.tests.py", "breathecode/**/*.tests_*.py"]
-
-# [tool.pytest]
-# env =
-#     ENV=test
-
-filterwarnings = [
-  # faker is passing a naive datetime to django
-  "ignore::RuntimeWarning:django.db.models.fields.*",
-  "ignore::DeprecationWarning:pkg_resources.*",
-]
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "linked-services"
+dynamic = ["version"]
+description = ''
+readme = "README.md"
+requires-python = ">=3.10"
+license = "LGPL-3.0-or-later"
+keywords = []
+authors = [{ name = "jefer94", email = "jdefreitaspinto@gmail.com" }]
+classifiers = [
+  "Development Status :: 5 - Production/Stable",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: Implementation :: CPython",
+  "Programming Language :: Python :: Implementation :: PyPy",
+  "Framework :: Django :: 4.2",
+  "Framework :: Django :: 5.0",
+  "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
+  "Topic :: Software Development :: Libraries",
+]
+dependencies = [
+  "python-slugify",
+  "asgiref",
+  "pyjwt",
+  "cryptography",
+  "celery-task-manager",
+]
+
+[project.urls]
+Documentation = "https://breatheco-de.github.io/linked-services-django-plugin/"
+Issues = "https://github.com/breatheco-de/linked-services-django-plugin/issues"
+Source = "https://github.com/breatheco-de/linked-services-django-plugin"
+
+
+[tool.hatch.build.targets.wheel]
+packages = ["src/linked_services"]
+
+[tool.hatch.version]
+path = "src/linked_services/__about__.py"
+
+[tool.hatch.envs.default]
+dependencies = [
+  "pytz",
+  "coverage[toml]>=6.5",
+  "pytest",
+  "pytest-django",
+  "black",
+  "anyio[trio]",
+  "django",
+  "djangorestframework",
+  "requests",
+  "aiohttp",
+  "aiodns",
+  "httpx",
+  "httpcore",
+  "h11",
+  "idna",
+  "brotli",
+  "pyjwt",
+  "mkdocs",
+  "mkdocs-material",
+  "celery",
+  "celery-task-manager[django]>=1.0.0b6",
+  "adrf",
+  "faker",
+  "pytest-celery",
+  "celery[pytest]",
+  "pytest-asyncio",
+]
+[tool.hatch.envs.default.scripts]
+test = "pytest {args:tests} --nomigrations --durations=1 --create-db"
+test-cov = "coverage run -m pytest {args:tests} --nomigrations --durations=1"
+cov-report = ["- coverage combine", "coverage report"]
+cov = ["test-cov", "cov-report"]
+docs = "mkdocs serve --livereload"
+generate_docs = "mkdocs build"
+docs_deploy = "mkdocs gh-deploy -c"
+
+[[tool.hatch.envs.all.matrix]]
+python = ["3.11", "3.12"]
+
+[tool.hatch.envs.types]
+dependencies = ["mypy>=1.0.0"]
+[tool.hatch.envs.types.scripts]
+check = "mypy --install-types --non-interactive {args:src/linked_services tests}"
+
+[tool.coverage.run]
+source_pkgs = ["linked_services", "tests"]
+branch = true
+parallel = true
+omit = ["src/linked_services/__about__.py"]
+
+[tool.coverage.paths]
+linked_services = [
+  "src/linked_services",
+  "*/linked-services/src/linked_services",
+]
+tests = ["tests", "*/linked-services/tests"]
+
+[tool.coverage.report]
+exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
+
+[project.optional-dependencies]
+django = [
+  "django",
+  "djangorestframework",
+  "celery-task-manager[django]",
+  "adrf",
+]
+requests = ["requests", "brotli"]
+aiohttp = ["aiohttp", "aiodns", "brotli"]
+httpx = ["httpx", "httpcore", "h11", "idna", "brotli"]
+
+[tool.black]
+line-length = 120
+
+[tool.flake8]
+max-line-length = 120
+
+[tool.pytest.ini_options]
+django_debug_mode = true
+addopts = ["-p", "no:legacypath", "--tb=short"]
+DJANGO_SETTINGS_MODULE = "linked_services.settings"
+# python_files = ["breathecode/**/*.tests.py", "breathecode/**/*.tests_*.py"]
+
+# [tool.pytest]
+# env =
+#     ENV=test
+
+filterwarnings = [
+  # faker is passing a naive datetime to django
+  "ignore::RuntimeWarning:django.db.models.fields.*",
+  "ignore::DeprecationWarning:pkg_resources.*",
+]
```

### Comparing `linked_services-1.2.1/PKG-INFO` & `linked_services-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: linked-services
-Version: 1.2.1
+Version: 1.2.2
 Project-URL: Documentation, https://breatheco-de.github.io/linked-services-django-plugin/
 Project-URL: Issues, https://github.com/breatheco-de/linked-services-django-plugin/issues
 Project-URL: Source, https://github.com/breatheco-de/linked-services-django-plugin
 Author-email: jefer94 <jdefreitaspinto@gmail.com>
 License-Expression: LGPL-3.0-or-later
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
```

