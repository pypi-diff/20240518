# Comparing `tmp/aa_ledger-0.3.3.tar.gz` & `tmp/aa_ledger-0.3.4.tar.gz`

## Comparing `aa_ledger-0.3.3.tar` & `aa_ledger-0.3.4.tar`

### file list

```diff
@@ -1,77 +1,76 @@
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/__init__.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/admin.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/app_settings.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/apps.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/auth_hooks.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/decorators.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/errors.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/hooks.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/providers.py
--rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/tasks.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/urls.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/api/__init__.py
--rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/api/helpers.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/api/schema.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/api/character/__init__.py
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/api/character/helpers.py
--rw-r--r--   0        0        0    11141 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/api/character/ledger.py
--rw-r--r--   0        0        0    15533 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/api/character/template.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/api/corporation/__init__.py
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/api/corporation/helpers.py
--rw-r--r--   0        0        0     6985 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/api/corporation/ledger.py
--rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/api/corporation/template.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/managers/charaudit_manager.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/managers/corpaudit_manager.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/managers/general_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/migrations/__init__.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/models/__init__.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/models/characteraudit.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/models/corporationaudit.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/models/events.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/models/general.py
--rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/static/ledger/css/billboards_dark.css
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/static/ledger/css/cards.css
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/static/ledger/css/custom.css
--rw-r--r--   0        0        0   236145 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/static/ledger/guides/ledger-1.png
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/static/ledger/guides/ledger-2.png
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/static/ledger/guides/ledger-3.png
--rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/static/ledger/images/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/static/ledger/images/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0    22102 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/static/ledger/js/charledger.js
--rw-r--r--   0        0        0    18824 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/static/ledger/js/corpledger.js
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/static/ledger/js/img.js
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/task_helpers/__init__.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/task_helpers/char_helpers.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/task_helpers/core_helpers.py
--rw-r--r--   0        0        0     8364 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/task_helpers/corp_helpers.py
--rw-r--r--   0        0        0     8377 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/task_helpers/etag_helpers.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/templates/ledger/base.html
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/templates/ledger/error.html
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/templates/ledger/bundles/ledger-css.html
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/templates/ledger/ledger/base.html
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/templates/ledger/ledger/index.html
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/templates/ledger/ledger/menu.html
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/templates/ledger/ledger/charledger/char_ledger.html
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/templates/ledger/ledger/charledger/month.html
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/templates/ledger/ledger/charledger/year.html
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/templates/ledger/ledger/corpledger/corp_ledger.html
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/templates/ledger/ledger/corpledger/month.html
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/templates/ledger/ledger/corpledger/year.html
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/templates/ledger/modals/modal-full.html
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/templates/ledger/modals/modal-xl.html
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/templates/ledger/modals/modal.html
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/templates/ledger/modals/modal_dialog.html
--rw-r--r--   0        0        0    16817 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/templates/ledger/modals/pve/view_character_content.html
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/view_helpers/__init__.py
--rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/view_helpers/core.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/views/__init__.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/views/pve.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/views/character/char_audit.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/views/corporation/corp_audit.py
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/views/corporation/corp_events.py
--rw-r--r--   0        0        0     8818 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/ledger/views/corporation/corp_tax.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/LICENSE
--rw-r--r--   0        0        0     5288 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/README.md
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     7913 2020-02-02 00:00:00.000000 aa_ledger-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/__init__.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/admin.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/app_settings.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/apps.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/auth_hooks.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/decorators.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/errors.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/hooks.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/providers.py
+-rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/tasks.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/urls.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/api/__init__.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/api/helpers.py
+-rw-r--r--   0        0        0    21609 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/api/ledgermanager.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/api/schema.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/api/character/__init__.py
+-rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/api/character/ledger.py
+-rw-r--r--   0        0        0    15634 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/api/character/template.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/api/corporation/__init__.py
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/api/corporation/ledger.py
+-rw-r--r--   0        0        0     6661 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/api/corporation/template.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/managers/charaudit_manager.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/managers/corpaudit_manager.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/managers/general_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/migrations/__init__.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/models/__init__.py
+-rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/models/characteraudit.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/models/corporationaudit.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/models/events.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/models/general.py
+-rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/css/billboards_dark.css
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/css/cards.css
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/css/custom.css
+-rw-r--r--   0        0        0   236145 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/guides/ledger-1.png
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/guides/ledger-2.png
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/guides/ledger-3.png
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/images/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/images/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0    22084 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/js/charledger.js
+-rw-r--r--   0        0        0    18891 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/js/corpledger.js
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/static/ledger/js/img.js
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/task_helpers/__init__.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/task_helpers/char_helpers.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/task_helpers/core_helpers.py
+-rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/task_helpers/corp_helpers.py
+-rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/task_helpers/etag_helpers.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/base.html
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/error.html
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/bundles/ledger-css.html
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/ledger/base.html
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/ledger/index.html
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/ledger/menu.html
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/ledger/charledger/char_ledger.html
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/ledger/charledger/month.html
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/ledger/charledger/year.html
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/ledger/corpledger/corp_ledger.html
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/ledger/corpledger/month.html
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/ledger/corpledger/year.html
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/modals/modal-full.html
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/modals/modal-xl.html
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/modals/modal.html
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/modals/modal_dialog.html
+-rw-r--r--   0        0        0    16817 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/templates/ledger/modals/pve/view_character_content.html
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/view_helpers/__init__.py
+-rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/view_helpers/core.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/views/__init__.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/views/pve.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/views/character/char_audit.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/views/corporation/corp_audit.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/views/corporation/corp_events.py
+-rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/ledger/views/corporation/corp_tax.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/LICENSE
+-rw-r--r--   0        0        0     5158 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/README.md
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     7913 2020-02-02 00:00:00.000000 aa_ledger-0.3.4/PKG-INFO
```

### Comparing `aa_ledger-0.3.3/ledger/admin.py` & `aa_ledger-0.3.4/ledger/admin.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/app_settings.py` & `aa_ledger-0.3.4/ledger/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/auth_hooks.py` & `aa_ledger-0.3.4/ledger/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/decorators.py` & `aa_ledger-0.3.4/ledger/decorators.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/hooks.py` & `aa_ledger-0.3.4/ledger/hooks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/tasks.py` & `aa_ledger-0.3.4/ledger/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/urls.py` & `aa_ledger-0.3.4/ledger/urls.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/api/__init__.py` & `aa_ledger-0.3.4/ledger/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/api/helpers.py` & `aa_ledger-0.3.4/ledger/api/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
     - `List`: Character IDS
     """
 
     # TODO users profile filter corporation über main char und alt chars corp ids
 
     mains = {}
 
+    # pylint: disable=no-member
     users = (
         UserProfile.objects.select_related("main_character")
         .all()
         .order_by("main_character_id")
     )
 
     for char in users:
```

### Comparing `aa_ledger-0.3.3/ledger/api/schema.py` & `aa_ledger-0.3.4/ledger/api/schema.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/api/character/helpers.py` & `aa_ledger-0.3.4/ledger/api/corporation/template.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,193 +1,182 @@
-import math
 from datetime import datetime
+from typing import List
 
-from django.db.models import F, Q, Sum
+from ninja import NinjaAPI
 
-from ledger import app_settings
+from django.db.models import Q
+from django.shortcuts import render
+
+from ledger.api import schema
+from ledger.api.helpers import get_corporations, get_main_and_alts_all
 from ledger.hooks import get_extension_logger
+from ledger.models.corporationaudit import CorporationWalletJournalEntry
+from ledger.view_helpers.core import (
+    calculate_days_year,
+    calculate_ess_stolen,
+    calculate_journal,
+)
 
 logger = get_extension_logger(__name__)
 
 
-def _billboard_char_ledger(models: list, mining_data, monthly, year: int, month: int):
-    """
-    Billboard System for Char Ledger
-    """
-
-    current_date = datetime.now()
-    billboard_dict = {"walletcharts": [], "rattingbar": [], "workflowgauge": []}
-
-    # Ratting Amount from Character Journal
-    sum_amount = [
-        "Ratting",
-    ]
-    sum_amount_ess = [
-        "ESS Payout",
-    ]
-    sum_amount_misc = [
-        "Miscellaneous",
-    ]
-    sum_amount_mining = [
-        "Mining",
-    ]
-    date_billboard = [
-        "x",
-    ]
-
-    entries, ess_entries = models
-
-    # total amounts
-    total_isk = 0
-    total_cost = 0
-
-    # costs
-    total_production_cost = 0
-    total_market = 0
-
-    # Month, Days
-    range_data = 12 if monthly else 31
-    # Vorbedingungen festlegen
-    day_checks = list(range(1, range_data + 1))
-
-    # Rückwärts durch die Tage iterieren
-    for range_ in day_checks:  # pylint: disable=duplicate-code
-        try:
-            date = current_date
-
-            total_bounty = 0
-            total_ess_payout = 0
-            total_miscellaneous = 0
-
-            if monthly:
-                date = date.replace(day=1)
-
-            filter_date = (
-                Q(date__year=year, date__month=range_)
-                if monthly
-                else Q(date__year=year, date__month=month, date__day=range_)
-            )
-            my_filter_mining = filter_date
-
-            mining_query = mining_data.filter(my_filter_mining).values("total", "date")
-            mining_aggregated = mining_query.aggregate(total_amount=Sum(F("total")))
-            total_amount_mining = mining_aggregated["total_amount"] or 0
-
-            # Char Journal
-            for w in entries:
-                if w.date.year == year and (
-                    w.date.month == range_
-                    if monthly
-                    else w.date.month == month and w.date.day == range_
-                ):
-                    if w.ref_type == "bounty_prizes" and w.amount > 0:
-                        total_bounty += w.amount
-                    if (
-                        w.ref_type
-                        in [
-                            "market_escrow",
-                            "transaction_tax",
-                            "market_provider_tax",
-                            "brokers_fee",
-                        ]
-                        and w.amount < 0
-                    ):
-                        total_market += w.amount
-                    if (
-                        w.ref_type in ["industry_job_tax", "manufacturing"]
-                        and w.amount < 0
-                    ):
-                        total_production_cost += w.amount
-                    if (
-                        w.ref_type
-                        in [
-                            "market_transaction",
-                            "contract_price_payment_corp",
-                            "contract_reward",
-                            "contract_price",
-                        ]
-                        and w.amount > 0
-                    ):
-                        total_miscellaneous += w.amount
-                    if w.amount > 0:
-                        total_isk += w.amount
-                    else:
-                        total_cost += w.amount
-
-            # Corp Journal
-            for w in ess_entries:
-                if w.date.year == year and (
-                    w.date.month == range_
-                    if monthly
-                    else w.date.month == month and w.date.day == range_
-                ):
-                    if w.ref_type == "ess_escrow_transfer":
-                        total_ess_payout += (
-                            w.amount / app_settings.LEDGER_CORP_TAX
-                        ) * (100 - app_settings.LEDGER_CORP_TAX)
-
-            date_billboard.append(  # pylint disable:duplicate-code
-                date.replace(day=range_).strftime("%Y-%m-%d")
-                if not monthly
-                else date.replace(month=range_).strftime("%Y-%m")
-            )
-
-            sum_amount.append(int(total_bounty))
-            sum_amount_ess.append(int(total_ess_payout))
-            sum_amount_misc.append(int(total_miscellaneous))
-            sum_amount_mining.append(int(total_amount_mining))
-        except ValueError:
-            continue
-
-    # Misc Costs
-    misc_cost = abs(total_cost - total_production_cost - total_market)
-
-    # Gesamtbetrag berechnen
-    total_sum = sum(
-        sum(filter(lambda x: isinstance(x, int), lst))
-        for lst in [sum_amount, sum_amount_ess, sum_amount_misc, sum_amount_mining]
-    )
-
-    # Prozentuale Anteile berechnen
-    percentages = [
-        (
-            (sum(filter(lambda x: isinstance(x, int), lst)) / total_sum * 100)
-            if total_sum > 0
-            else 0
+# TODO Refactor this class
+# pylint: disable=too-many-locals, too-many-branches, too-many-statements
+class LedgerTemplateApiEndpoints:
+    tags = ["CorporationLedgerTemplate"]
+
+    def __init__(self, api: NinjaAPI):
+
+        @api.get(
+            "corporation/{main_id}/ledger/template/year/{year}/month/{month}",
+            response={200: List[schema.CharacterLedgerTemplate], 403: str},
+            tags=self.tags,
         )
-        for lst in [sum_amount, sum_amount_ess, sum_amount_misc, sum_amount_mining]
-    ]
+        def get_corporation_ledger_template(
+            request, main_id: int, year: int, month: int
+        ):
+            overall_mode = False
+
+            perms = request.user.has_perm("ledger.basic_access")
+
+            if main_id == 0:
+                overall_mode = True
+
+            if not perms:
+                logger.error(
+                    "Permission Denied for %s to view corporation ledger template!",
+                    request.user,
+                )
+                return 403, "Permission Denied!"
+
+            current_date = datetime.now()
+
+            total_amount = 0
+            total_amount_day = 0
+            total_amount_hour = 0
+            # ESS
+            total_amount_ess = 0
+            total_amount_day_ess = 0
+            total_amount_hour_ess = 0
+
+            current_date = current_date.replace(year=year)
+            if not month == 0:
+                current_date = current_date.replace(month=month)
+
+            current_day = calculate_days_year() if month == 0 else current_date.day
+
+            character_id = request.user.profile.main_character.character_id
+            corporations = get_corporations(request, character_id)
+
+            mains, chars = get_main_and_alts_all(corporations, char_ids=True)
+
+            filters = Q(second_party_id__in=chars)
+            filter_date = Q(date__year=current_date.year)
+            if not month == 0:
+                filter_date &= Q(date__month=current_date.month)
+
+            wallet_journal = (
+                CorporationWalletJournalEntry.objects.filter(filters, filter_date)
+                .select_related("first_party", "second_party", "division")
+                .values("amount", "date", "second_party_id", "ref_type")
+                .order_by("-date")
+            )
 
-    rounded_percentages = [math.floor(perc * 10) / 10 for perc in percentages]
+            if overall_mode:
+                mains_data = mains
+            else:
+                mains_data = {main_id: mains.get(main_id, None)}
+
+            for _, mains_data in mains_data.items():
+                main = mains_data["main"]
+                alts = mains_data["alts"]
+
+                # Each Chars from a Main Character
+                chars = [alt.character_id for alt in alts] + [main.character_id]
+
+                char_name = main.character_name if not main_id == 0 else "Summary"
+                char_id = main.character_id if not main_id == 0 else 0
+
+                my_filter = Q(second_party_id__in=chars)
+                my_filter_bounty = my_filter & Q(ref_type="bounty_prizes")
+                my_filter_ess_payout = my_filter & Q(ref_type="ess_escrow_transfer")
+
+                amount_ess = calculate_journal(wallet_journal, my_filter_ess_payout)
+
+                amount_bounty = calculate_journal(
+                    wallet_journal,
+                    my_filter_bounty,
+                )
+
+                # Berechne die Gesamtsumme für alle Charaktere
+                total_amount += amount_bounty["total_amount"]
+                total_amount_day += amount_bounty["total_amount_day"]
+                total_amount_hour += amount_bounty["total_amount_hour"]
+
+                # ESS
+                total_amount_ess += amount_ess["total_amount"]
+                total_amount_day_ess += amount_ess["total_amount_day"]
+                total_amount_hour_ess += amount_ess["total_amount_hour"]
+
+            stolen = 0
+            gain = 0
+
+            # If not 0 then add to Rattingledger
+            if total_amount > 0:
+                stolen, gain = calculate_ess_stolen(total_amount, total_amount_ess)
+
+            day_avg_isk = round(total_amount / current_day)
+            day_avg_ess = round(total_amount_ess / current_day)
+
+            hourly_avg_isk = round((total_amount / current_day) / 24)
+            hourly_avg_ess = round((total_amount_ess / current_day) / 24)
+
+            total_summary = total_amount + total_amount_ess
+            total_summary_day = total_amount_day + total_amount_day_ess
+            total_summary_hour = total_amount_hour + total_amount_hour_ess
+
+            # pylint: disable=duplicate-code
+            summary = {
+                "main_name": char_name,
+                "main_id": char_id,
+                "date": (
+                    str(current_date.year)
+                    if month == 0
+                    else current_date.strftime("%B")
+                ),
+                "summary_isk": total_amount,
+                "summary_ess": total_amount_ess,
+                "summary": total_summary,
+                "day_avg_isk": day_avg_isk,
+                "day_avg_ess": day_avg_ess,
+                "summary_day": total_summary_day,
+                "hourly_avg_isk": hourly_avg_isk,
+                "hourly_avg_ess": hourly_avg_ess,
+                "summary_hour": total_summary_hour,
+            }
+            if not overall_mode:
+                summary.update(
+                    {
+                        "day_isk": total_amount_day,
+                        "day_ess": total_amount_day_ess,
+                        "hourly_isk": total_amount_hour,
+                        "hourly_ess": total_amount_hour_ess,
+                    }
+                )
+            if stolen:
+                day_stolen = round(stolen / current_date.day)
+                hourly_stolen = round((stolen / current_date.day) / 24)
+
+                summary.update(
+                    {
+                        "gain": gain,
+                        "stolen": stolen,
+                        "day_stolen": day_stolen,
+                        "hourly_stolen": hourly_stolen,
+                    }
+                )
 
-    # Daten für die Gauge vorbereiten
-    billboard_dict["workflowgauge"] = (
-        [
-            ["Ratting", rounded_percentages[0]],
-            ["ESS Payout", rounded_percentages[1]],
-            ["Miscellaneous", rounded_percentages[2]],
-            ["Mining", rounded_percentages[3]],
-        ]
-        if total_sum
-        else None
-    )
-    billboard_dict["rattingbar"] = (
-        [date_billboard, sum_amount, sum_amount_ess, sum_amount_misc, sum_amount_mining]
-        if total_sum
-        else None
-    )
-
-    # Daten für die Wallet-Charts vorbereiten
-    wallet_chart_data = [
-        # Earns
-        ["Earns", int(total_isk)],
-        # ["Ratting", int(total_sum_ratting)],  ["Mining", int(total_sum_mining)], ["Misc.", int(total_sum_misc)],
-        # Costs
-        ["Market Cost", int(abs(total_market))],
-        ["Production Cost", int(abs(total_production_cost))],
-        ["Misc. Costs", int(misc_cost)],
-    ]
-    billboard_dict["walletcharts"] = (
-        wallet_chart_data if any(item[1] != 0 for item in wallet_chart_data) else None
-    )
+            context = {"character": summary}
 
-    return billboard_dict
+            return render(
+                request, "ledger/modals/pve/view_character_content.html", context
+            )
```

### Comparing `aa_ledger-0.3.3/ledger/api/character/ledger.py` & `aa_ledger-0.3.4/ledger/api/character/template.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,295 +1,429 @@
+from datetime import datetime
 from decimal import Decimal
 from typing import List
 
 from ninja import NinjaAPI
-from ninja.pagination import paginate
 
-from django.db.models import DecimalField, F, Q, Sum
-from django.db.models.functions import Coalesce
+from django.db.models import F, Q, Sum
+from django.shortcuts import render
+
+from allianceauth.eveonline.models import EveCharacter
 
 from ledger import app_settings
-from ledger.api import schema
-from ledger.api.character.helpers import _billboard_char_ledger
-from ledger.api.helpers import Paginator, get_alts_queryset, get_main_character
-from ledger.models.corporationaudit import CorporationWalletJournalEntry
-from ledger.view_helpers.core import events_filter
 
 if app_settings.LEDGER_MEMBERAUDIT_USE:
     from memberaudit.models import CharacterMiningLedgerEntry as CharacterMiningLedger
     from memberaudit.models import CharacterWalletJournalEntry
 else:
     from ledger.models.characteraudit import (
         CharacterWalletJournalEntry,
         CharacterMiningLedger,
     )
 
+from ledger.api import schema
+from ledger.api.helpers import get_alts_queryset, get_main_character
+from ledger.app_settings import LEDGER_CORP_TAX
 from ledger.hooks import get_extension_logger
+from ledger.models.corporationaudit import CorporationWalletJournalEntry
+from ledger.view_helpers.core import (
+    calculate_days_year,
+    calculate_ess_stolen,
+    calculate_journal,
+    events_filter,
+)
 
 logger = get_extension_logger(__name__)
 
-SR_CHAR = (
-    "character__eve_character"
-    if app_settings.LEDGER_MEMBERAUDIT_USE
-    else "character__character"
-)
-
 
-class LedgerApiEndpoints:
-    tags = ["CharacerLedger"]
+# TODO Refactor this class
+# pylint: disable=too-many-locals, too-many-branches, too-many-statements
+class LedgerTemplateApiEndpoints:
+    tags = ["CharacerLedgerTemplate"]
 
     def __init__(self, api: NinjaAPI):
 
         @api.get(
-            "account/{character_id}/wallet",
-            response={200: List[schema.CharacterWalletEvent], 403: str},
+            "account/{character_id}/ledger/template/year/{year}/month/{month}",
+            response={200: List[schema.CharacterLedgerTemplate], 403: str},
             tags=self.tags,
         )
-        @paginate(Paginator)
-        def get_character_wallet(request, character_id: int):
+        def get_character_ledger_template(
+            request,
+            character_id: int,
+            year: int,
+            month: int,
+            **kwargs,  # pylint: disable=unused-argument
+        ):
+            overall_mode = False
+
             if character_id == 0:
                 character_id = request.user.profile.main_character.character_id
+                overall_mode = True
             response, main = get_main_character(request, character_id)
 
+            current_date = datetime.now()
+
+            current_date = current_date.replace(year=year)
+            if not month == 0:
+                current_date = current_date.replace(month=month)
+
             if not response:
                 return 403, "Permission Denied"
 
-            characters = get_alts_queryset(main)
+            alts = get_alts_queryset(main)
 
-            wallet_journal = (
-                CharacterWalletJournalEntry.objects.filter(
-                    character__character__in=characters
-                )
-                .select_related("first_party", "second_party", SR_CHAR)
-                .order_by("-date")[:35000]
-            )
-            output = []
+            main = EveCharacter.objects.get(character_id=character_id)
 
-            for w in wallet_journal:
-                output.append(
-                    {
-                        "character": w.character.eve_character,
-                        "id": w.entry_id,
-                        "date": w.date,
-                        "first_party": {
-                            "id": w.first_party_id,
-                            "name": w.first_party.name,
-                            "cat": w.first_party.category,
-                        },
-                        "second_party": {
-                            "id": w.second_party_id,
-                            "name": w.second_party.name,
-                            "cat": w.second_party.category,
-                        },
-                        "ref_type": w.ref_type,
-                        "amount": w.amount,
-                        "balance": w.balance,
-                        "reason": w.reason,
-                    }
-                )
+            current_day = calculate_days_year() if month == 0 else current_date.day
 
-            return output
+            characters = alts if overall_mode else [main]
 
-        @api.get(
-            "account/{character_id}/ledger/year/{year}/month/{month}",
-            response={200: List[schema.CharacterLedger], 403: str},
-            tags=self.tags,
-        )
-        @paginate(Paginator)
-        def get_character_ledger(request, character_id: int, year: int, month: int):
-            if character_id == 0:
-                character_id = request.user.profile.main_character.character_id
-            response, main = get_main_character(request, character_id)
-
-            if not response:
-                return 403, "Permission Denied"
-
-            characters = get_alts_queryset(main)
+            filters = Q(character__eve_character__in=characters)
+            filter_date = Q(date__year=current_date.year)
+            if not month == 0:
+                filter_date &= Q(date__month=current_date.month)
 
-            monthly = True
-            filters = (
-                Q(character__eve_character__in=characters)
-                if app_settings.LEDGER_MEMBERAUDIT_USE
-                else Q(character__character__in=characters)
+            chars = (
+                [char.character_id for char in characters]
+                if overall_mode
+                else [main.character_id]
             )
-            filter_date = Q(date__year=year)
-            if not month == 0:
-                filter_date &= Q(date__month=month)
-                monthly = False
 
-            chars = [char.character_id for char in characters]
+            chars_list = [char.character_id for char in alts]
 
             entries_filter = Q(second_party_id__in=chars) | Q(first_party_id__in=chars)
 
-            # Dictionary zur Speicherung der Zusammenfassung für jede main_character_id
-            summary_dict = {}
-            summary_dict_total = {}
-            billboard_dict = {}
-
-            summary_dict_total["total_amount"] = 0
-            summary_dict_total["total_amount_ess"] = 0
-            summary_dict_total["total_amount_others"] = 0
-            summary_dict_total["total_amount_all"] = 0
-            summary_dict_total["total_amount_mining"] = 0
-
-            wallet_journal = (
+            # pylint: disable=duplicate-code
+            wallet_template_journal = (
                 CharacterWalletJournalEntry.objects.filter(filters, filter_date)
-                .select_related("first_party", "second_party", SR_CHAR)
+                .select_related(
+                    "first_party", "second_party", "character__eve_character"
+                )
                 .order_by("-date")
             )
 
             corporation_journal = (
                 CorporationWalletJournalEntry.objects.filter(
                     entries_filter, filter_date
                 )
                 .select_related("first_party", "second_party")
                 .order_by("-date")
             )
 
             # Exclude Events to avoid wrong stats
             corporation_journal = events_filter(corporation_journal)
+
             mining_entries_data = (
                 CharacterMiningLedger.objects.filter(filters, filter_date)
-                .select_related(SR_CHAR)
+                .select_related("character__eve_character")
                 .order_by("-date")
             )
 
             mining_entries_data = mining_entries_data.annotate_pricing()
 
-            # TODO Field Tax and Amount
-            # Ratting, Others
+            total_amount = {}
+            total_amount_day = {}
+            total_amount_hour = {}
+
+            amount = {}
+
+            total_list = [
+                "total",
+                "ess",
+                "transaction",
+                "contract",
+                "donation",
+                "production_cost",
+                "market_cost",
+                "mining",
+            ]
+
+            for total in total_list:
+                total_amount[total] = 0
+                total_amount_day[total] = 0
+                total_amount_hour[total] = 0
+            stolen = None
+
             for char in characters:
                 char_id = char.character_id
                 char_name = char.character_name
 
-                # Core
-                filter_ledger = Q(second_party_id=char_id)
+                my_filter = Q(second_party_id=char_id) | Q(first_party_id=char_id)
 
-                # Industry
-                filter_market = filter_ledger & Q(ref_type="market_transaction")
-                filter_contracts = filter_ledger & Q(
+                my_filter_market = my_filter & Q(ref_type="market_transaction")
+                my_filter_market_cost = my_filter & Q(
+                    ref_type__in=[
+                        "transaction_tax",
+                        "market_provider_tax",
+                        "brokers_fee",
+                    ]
+                )
+                my_filter_production = my_filter & Q(
+                    ref_type__in=["industry_job_tax", "manufacturing"]
+                )
+                my_filter_contracts = my_filter & Q(
                     ref_type__in=[
                         "contract_price_payment_corp",
                         "contract_reward",
                         "contract_price",
                     ],
                     amount__gt=0,
                 )
-                filter_donations = filter_ledger & Q(ref_type="player_donation")
+                my_filter_donations = my_filter & Q(ref_type="player_donation")
+
+                my_filter_bounty = my_filter & Q(ref_type="bounty_prizes")
+                my_filter_ess = my_filter & Q(ref_type="ess_escrow_transfer")
+                filter_mining = Q(character__eve_character__character_id=char_id)
 
-                # Ratting
-                filter_bounty = filter_ledger & Q(ref_type="bounty_prizes")
-                filter_ess = filter_ledger & Q(ref_type="ess_escrow_transfer")
-                # Mining
-                filter_mining = (
-                    Q(character__eve_character__character_id=char_id)
-                    if app_settings.LEDGER_MEMBERAUDIT_USE
-                    else Q(character__character__character_id=char_id)
+                amount["total"] = calculate_journal(
+                    wallet_template_journal,
+                    my_filter_bounty,
                 )
 
-                amount_bounty = wallet_journal.filter(filter_bounty).aggregate(
-                    total_amount=Coalesce(
-                        Sum(F("amount")), 0, output_field=DecimalField()
-                    )
+                amount["ess"] = calculate_journal(
+                    corporation_journal,
+                    my_filter_ess,
                 )
 
-                amount_ess = corporation_journal.filter(filter_ess).aggregate(
-                    total_amount=Coalesce(
-                        Sum(F("amount")), 0, output_field=DecimalField()
-                    )
+                amount["transaction"] = calculate_journal(
+                    wallet_template_journal,
+                    my_filter_market,
                 )
 
-                amount_contracts = wallet_journal.filter(filter_contracts).aggregate(
-                    total_amount=Coalesce(
-                        Sum(F("amount")), 0, output_field=DecimalField()
-                    )
+                amount["production_cost"] = calculate_journal(
+                    wallet_template_journal,
+                    my_filter_production,
                 )
 
-                amount_transactions = wallet_journal.filter(filter_market).aggregate(
-                    total_amount=Coalesce(
-                        Sum(F("amount")), 0, output_field=DecimalField()
-                    )
+                amount["market_cost"] = calculate_journal(
+                    wallet_template_journal,
+                    my_filter_market_cost,
                 )
 
-                amount_donations = (
-                    wallet_journal.filter(filter_donations)
-                    .exclude(first_party_id__in=chars)
-                    .aggregate(
-                        total_amount=Coalesce(
-                            Sum(F("amount")), 0, output_field=DecimalField()
-                        )
-                    )
+                amount["contract"] = calculate_journal(
+                    wallet_template_journal,
+                    my_filter_contracts,
+                )
+
+                amount["donation"] = calculate_journal(
+                    wallet_template_journal,
+                    my_filter_donations,
+                    exclude=chars_list,
                 )
 
-                amount_mining = (
+                # Mining Ledger
+                amount["mining"] = {}
+                amount["mining"]["total_amount"] = 0
+                amount["mining"]["total_amount_day"] = 0
+                amount["mining"]["total_amount_hour"] = 0
+
+                mining_aggregated = (
                     mining_entries_data.filter(filter_date, filter_mining)
                     .values("total", "date")
                     .aggregate(
-                        total_amount=Coalesce(
-                            Sum(F("total")), 0, output_field=DecimalField()
-                        )
+                        total_amount=Sum(F("total")),
+                        total_amount_day=Sum(
+                            F("total"), filter=Q(date__day=current_date.day)
+                        ),
                     )
                 )
 
-                amount_ess["total_amount"] = Decimal(
-                    (amount_ess["total_amount"] / app_settings.LEDGER_CORP_TAX)
-                    * (100 - app_settings.LEDGER_CORP_TAX)
-                )
-                total_amount_others = (
-                    amount_contracts["total_amount"]
-                    + amount_transactions["total_amount"]
-                    + amount_donations["total_amount"]
-                )
-                combined_amount = (
-                    amount_bounty["total_amount"]
-                    + amount_ess["total_amount"]
-                    + total_amount_others
-                )
-
-                if amount_bounty["total_amount"] > 0 or total_amount_others > 0:
-                    summary_dict[char_id] = {
-                        "main_id": char_id,
-                        "main_name": char_name,
-                        "total_amount": amount_bounty["total_amount"],
-                        "total_amount_ess": amount_ess["total_amount"],
-                        "total_amount_mining": amount_mining["total_amount"],
-                        "total_amount_others": total_amount_others,
-                    }
+                amount["mining"]["total_amount"] += Decimal(
+                    mining_aggregated["total_amount"] or 0
+                )
+                amount["mining"]["total_amount_day"] += Decimal(
+                    mining_aggregated["total_amount_day"] or 0
+                )
+                amount["mining"]["total_amount_hour"] += Decimal(
+                    amount["mining"]["total_amount_day"] / 24
+                )
 
-                # Total Amount
-                summary_dict_total["total_amount"] += amount_bounty["total_amount"]
-                # ESS
-                summary_dict_total["total_amount_ess"] += amount_ess["total_amount"]
-                # Mined
-                summary_dict_total["total_amount_mining"] += amount_mining[
-                    "total_amount"
-                ]
-                # others
-                summary_dict_total["total_amount_others"] += total_amount_others
-                # Combined
-                summary_dict_total["total_amount_all"] += combined_amount
-
-            # Save Dicts & Models for billboard function
-            models = wallet_journal, corporation_journal
-            # dicts = summary_dict, summary_dict_total
-            # Outsource Function to Create Billboard Data
-            billboard_dict = _billboard_char_ledger(
-                models, mining_entries_data, monthly, year, month
-            )
+                # Calculate ESS Payout Char
+                amount["ess"]["total_amount"] = Decimal(
+                    (amount["ess"]["total_amount"] / LEDGER_CORP_TAX)
+                    * (100 - LEDGER_CORP_TAX)
+                )
+                amount["ess"]["total_amount_day"] = Decimal(
+                    (amount["ess"]["total_amount_day"] / LEDGER_CORP_TAX)
+                    * (100 - LEDGER_CORP_TAX)
+                )
+                amount["ess"]["total_amount_hour"] = Decimal(
+                    (amount["ess"]["total_amount_hour"] / LEDGER_CORP_TAX)
+                    * (100 - LEDGER_CORP_TAX)
+                )
 
-            summary_dict_total["total_amount_all"] += Decimal(
-                summary_dict_total["total_amount_mining"]
-            )
+                # Sum Total Amounts
+                for total in total_list:
+                    if amount[total]["total_amount"]:
+                        total_amount[total] += amount[total]["total_amount"]
+                        total_amount_day[total] += amount[total]["total_amount_day"]
+                        total_amount_hour[total] += amount[total]["total_amount_hour"]
+            gain = 0
+            stolen_day = 0
+            # If not 0 then add to Rattingledger
+            if total_amount["total"] > 0:
+                stolen, gain = calculate_ess_stolen(
+                    total_amount["total"], total_amount["ess"]
+                )
+                stolen_day, _ = calculate_ess_stolen(
+                    total_amount_day["total"], total_amount_day["ess"]
+                )
+
+            day_avg_isk = round(total_amount["total"] / current_day)
+            day_avg_ess = round(total_amount["ess"] / current_day)
 
-            output = []
+            hourly_avg_isk = round((total_amount["total"] / current_day) / 24)
+            hourly_avg_ess = round((total_amount["ess"] / current_day) / 24)
 
-            output.append(
-                {
-                    "ratting": sorted(
-                        list(summary_dict.values()), key=lambda x: x["main_name"]
-                    ),
-                    "total": summary_dict_total,
-                    "billboard": billboard_dict,
-                }
+            total_summary = sum(
+                total_amount[key] for key in total_list if key in total_amount
             )
+            total_summary_day = sum(
+                total_amount_day[key] for key in total_list if key in total_amount_day
+            )
+            total_summary_hour = sum(
+                total_amount_hour[key] for key in total_list if key in total_amount_hour
+            )
+
+            main_name = char_name if not overall_mode else "Summary"
+            main_id = char_id if not overall_mode else 0
+
+            summary = {
+                "main_name": main_name,
+                "main_id": main_id,
+                "date": (
+                    str(current_date.year)
+                    if month == 0
+                    else current_date.strftime("%B")
+                ),
+                "summary_isk": total_amount["total"],
+                "summary_ess": total_amount["ess"],
+                "summary": total_summary,
+                "day_avg_isk": day_avg_isk,
+                "day_avg_ess": day_avg_ess,
+                "summary_day": total_summary_day,
+                "hourly_avg_isk": hourly_avg_isk,
+                "hourly_avg_ess": hourly_avg_ess,
+                "summary_hour": total_summary_hour,
+            }
+
+            if not overall_mode:
+                summary.update(
+                    {
+                        "day_isk": total_amount_day["total"],
+                        "day_ess": total_amount_day["ess"],
+                        "hourly_isk": total_amount_hour["total"],
+                        "hourly_ess": total_amount_hour["ess"],
+                    }
+                )
+            if stolen:
+                day_stolen = round(stolen / current_date.day)
+                hourly_stolen = round((stolen / current_date.day) / 24)
 
-            return output
+                summary.update(
+                    {
+                        "gain": gain,
+                        "stolen": stolen,
+                        "day_stolen_ess": stolen_day,
+                        "day_stolen": day_stolen,
+                        "hourly_stolen": hourly_stolen,
+                    }
+                )
+
+            def _calculate_aggregates(
+                total_amount,
+                total_amount_day,
+                total_amount_hour,
+                summary_key,
+                day_key,
+                hour_key,
+                overall_mode,
+            ):  # pylint: disable=too-many-arguments
+                summary.update(
+                    {
+                        summary_key: total_amount,
+                        day_key: total_amount_day,
+                        hour_key: total_amount_hour,
+                        f"day_avg_{summary_key}": round(
+                            total_amount / current_date.day
+                        ),
+                        f"hourly_avg_{summary_key}": round(
+                            total_amount / (current_date.day * 24)
+                        ),
+                    }
+                )
+                if overall_mode or current_date.month != datetime.now().month:
+                    summary.pop(day_key, 0)
+                    summary.pop(hour_key, 0)
+
+            if total_amount["mining"]:
+                _calculate_aggregates(
+                    total_amount["mining"],
+                    total_amount_day["mining"],
+                    total_amount_hour["mining"],
+                    "mining",
+                    "mining_day",
+                    "mining_hour",
+                    overall_mode,
+                )
+
+            if total_amount["transaction"]:
+                _calculate_aggregates(
+                    total_amount["transaction"],
+                    total_amount_day["transaction"],
+                    total_amount_hour["transaction"],
+                    "trading",
+                    "trading_day",
+                    "trading_hour",
+                    overall_mode,
+                )
+
+            if total_amount["contract"]:
+                _calculate_aggregates(
+                    total_amount["contract"],
+                    total_amount_day["contract"],
+                    total_amount_hour["contract"],
+                    "contract",
+                    "contract_day",
+                    "contract_hour",
+                    overall_mode,
+                )
+
+            if total_amount["production_cost"]:
+                _calculate_aggregates(
+                    total_amount["production_cost"],
+                    total_amount_day["production_cost"],
+                    total_amount_hour["production_cost"],
+                    "production_cost",
+                    "production_cost_day",
+                    "production_cost_hour",
+                    overall_mode,
+                )
+
+            if total_amount["market_cost"]:
+                _calculate_aggregates(
+                    total_amount["market_cost"],
+                    total_amount_day["market_cost"],
+                    total_amount_hour["market_cost"],
+                    "trading_cost",
+                    "trading_cost_day",
+                    "trading_cost_hour",
+                    overall_mode,
+                )
+
+            if total_amount["donation"]:
+                _calculate_aggregates(
+                    total_amount["donation"],
+                    total_amount_day["donation"],
+                    total_amount_hour["donation"],
+                    "donation",
+                    "donation_day",
+                    "donation_hour",
+                    overall_mode,
+                )
+
+            context = {"character": summary}
+
+            return render(
+                request, "ledger/modals/pve/view_character_content.html", context
+            )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa_ledger-0.3.3/ledger/managers/charaudit_manager.py` & `aa_ledger-0.3.4/ledger/managers/charaudit_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/managers/corpaudit_manager.py` & `aa_ledger-0.3.4/ledger/managers/corpaudit_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/managers/general_manager.py` & `aa_ledger-0.3.4/ledger/managers/general_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/models/characteraudit.py` & `aa_ledger-0.3.4/ledger/models/characteraudit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/models/corporationaudit.py` & `aa_ledger-0.3.4/ledger/models/corporationaudit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/models/events.py` & `aa_ledger-0.3.4/ledger/models/events.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/models/general.py` & `aa_ledger-0.3.4/ledger/models/general.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/static/ledger/css/billboards_dark.css` & `aa_ledger-0.3.4/ledger/static/ledger/css/billboards_dark.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/static/ledger/css/cards.css` & `aa_ledger-0.3.4/ledger/static/ledger/css/cards.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/static/ledger/css/custom.css` & `aa_ledger-0.3.4/ledger/static/ledger/css/custom.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/static/ledger/guides/ledger-1.png` & `aa_ledger-0.3.4/ledger/static/ledger/guides/ledger-1.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/static/ledger/guides/ledger-2.png` & `aa_ledger-0.3.4/ledger/static/ledger/guides/ledger-2.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/static/ledger/guides/ledger-3.png` & `aa_ledger-0.3.4/ledger/static/ledger/guides/ledger-3.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/static/ledger/images/Spinner-1s-64px-dark.gif` & `aa_ledger-0.3.4/ledger/static/ledger/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/static/ledger/images/Spinner-1s-64px-light.gif` & `aa_ledger-0.3.4/ledger/static/ledger/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/static/ledger/js/charledger.js` & `aa_ledger-0.3.4/ledger/static/ledger/js/charledger.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -17,15 +17,15 @@
         var selectedYear = currentYear; // Hier die Logik zum Auslesen des ausgewählten Jahres implementieren, falls nötig
         var monthText = getMonthName(selectedMonth);
 
         // URL für die Daten der ausgewählten Kombination von Jahr und Monat erstellen
         var url = '/ledger/api/account/0/ledger/year/' + selectedYear + '/month/' + selectedMonth;
 
         // DataTable neu laden mit den Daten des ausgewählten Monats
-        currentMonthTable.ajax.url(url).load();
+        MonthTable.ajax.url(url).load();
         $('#currentMonthLink').text('Month - ' + monthText);
     });
 
     function getMonthName(monthNumber) {
         var months = [
             'January', 'February', 'March', 'April', 'May', 'June',
             'July', 'August', 'September', 'October', 'November', 'December'
@@ -52,15 +52,15 @@
         var color = value >= 0 ? 'chartreuse' : 'red';
 
         // Rückgabe des formatierten Strings mit Farbe und Einheit
         return '<span style="color: ' + color + ';">' + formattedValue + '</span> ISK';
     }
 
     // Initialize DataTable for current_month
-    var currentMonthTable = $('#ratting').DataTable({
+    var MonthTable = $('#ratting').DataTable({
         ajax: {
             url: '/ledger/api/account/0/ledger/year/' + currentYear + '/month/' + selectedMonth + '',
             dataSrc: function(data) {
                 // Zusätzliche Daten im DataTable-Objekt speichern
                 total_amount = data.items[0].total.total_amount;
                 total_amount_ess = data.items[0].total.total_amount_ess;
                 total_amount_others = data.items[0].total.total_amount_others;
@@ -256,15 +256,15 @@
     $('a[data-bs-toggle="tab"]').on('shown.bs.tab', function(e) {
         // Get the id of the tab that was clicked
         var targetTabId = $(e.target).attr('href');
 
         // Check if the clicked tab is the one containing the year DataTable
         if (targetTabId === '#tab-all_month' && !yearTableInitialized) {
             // Initialisiere DataTable für den Hauptinhalt
-            currentMonthTable = $('#ratting_year').DataTable({
+            var YearTable = $('#ratting_year').DataTable({
                 ajax: {
                     url: '/ledger/api/account/0/ledger/year/' + currentYear + '/month/0',
                     dataSrc: function(data) {
                         // Zusätzliche Daten im DataTable-Objekt speichern
                         total_amount = data.items[0].total.total_amount;
                         total_amount_ess = data.items[0].total.total_amount_ess;
                         total_amount_mining = data.items[0].total.total_amount_mining;
```

### Comparing `aa_ledger-0.3.3/ledger/static/ledger/js/corpledger.js` & `aa_ledger-0.3.4/ledger/static/ledger/js/corpledger.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -17,15 +17,15 @@
         var selectedYear = currentYear; // Hier die Logik zum Auslesen des ausgewählten Jahres implementieren, falls nötig
         var monthText = getMonthName(selectedMonth);
 
         // URL für die Daten der ausgewählten Kombination von Jahr und Monat erstellen
         var url = '/ledger/api/corporation/0/ledger/year/' + selectedYear + '/month/' + selectedMonth;
 
         // DataTable neu laden mit den Daten des ausgewählten Monats
-        currentMonthTable.ajax.url(url).load();
+        MonthTable.ajax.url(url).load();
         $('#currentMonthLink').text('Month - ' + monthText);
     });
 
     function getMonthName(monthNumber) {
         var months = [
             'January', 'February', 'March', 'April', 'May', 'June',
             'July', 'August', 'September', 'October', 'November', 'December'
@@ -52,15 +52,15 @@
         var color = value >= 0 ? 'chartreuse' : 'red';
 
         // Rückgabe des formatierten Strings mit Farbe und Einheit
         return '<span style="color: ' + color + ';">' + formattedValue + '</span> ISK';
     }
 
     // Initialize DataTable for current_month
-    var currentMonthTable = $('#ratting').DataTable({
+    var MonthTable = $('#ratting').DataTable({
         ajax: {
             url: '/ledger/api/corporation/0/ledger/year/' + currentYear + '/month/' + selectedMonth + '',
             dataSrc: function(data) {
                 // Zusätzliche Daten im DataTable-Objekt speichern
                 total_amount = data.items[0].total.total_amount;
                 total_amount_ess = data.items[0].total.total_amount_ess;
                 total_amount_combined = data.items[0].total.total_amount_all;
@@ -215,15 +215,16 @@
         // Get the id of the tab that was clicked
         var targetTabId = $(e.target).attr('href');
 
         // Check if the clicked tab is the one containing the year DataTable
         if (targetTabId === '#tab-all_month' && !yearTableInitialized) {
 
             // Initialisiere DataTable für den Hauptinhalt
-            $('#ratting_year').DataTable({
+            // eslint-disable-next-line no-undef
+            YearTable = $('#ratting_year').DataTable({
                 ajax: {
                     url: '/ledger/api/corporation/0/ledger/year/' + currentYear + '/month/0',
                     dataSrc: function(data) {
                         // Zusätzliche Daten im DataTable-Objekt speichern
                         total_amount = data.items[0].total.total_amount;
                         total_amount_ess = data.items[0].total.total_amount_ess;
                         total_amount_combined = data.items[0].total.total_amount_all;
@@ -362,18 +363,18 @@
                     sortable: false,
                     targets: [3]
                 }, ],
                 footerCallback: function(row, data, start, end, display) {
                     var totalAmountAllChars = parseFloat(total_amount);
                     var totalEssAmountAllChars = parseFloat(total_amount_ess);
                     var totalCombinedAmountAllChars = parseFloat(total_amount_combined);
-                    $('#foot .col-total-amount').html('' + formatAndColor(totalAmountAllChars) + '');
-                    $('#foot .col-total-ess').html('' + formatAndColor(totalEssAmountAllChars) + '');
-                    $('#foot .col-total-gesamt').html('' + formatAndColor(totalCombinedAmountAllChars) + '');
-                    $('#foot .col-total-button').html('<button class="btn btn-sm btn-info btn-square" data-bs-toggle="modal" data-bs-target="#modalViewCharacterContainer"' +
+                    $('#foot-year .col-total-amount').html('' + formatAndColor(totalAmountAllChars) + '');
+                    $('#foot-year .col-total-ess').html('' + formatAndColor(totalEssAmountAllChars) + '');
+                    $('#foot-year .col-total-gesamt').html('' + formatAndColor(totalCombinedAmountAllChars) + '');
+                    $('#foot-year .col-total-button').html('<button class="btn btn-sm btn-info btn-square" data-bs-toggle="modal" data-bs-target="#modalViewCharacterContainer"' +
                         'aria-label="{{ data.main_name }}"' +
                         'data-ajax_url="/voicesofwar/api/corporation/0/ledger/template/year/' + currentYear + '/month/' + selectedMonth + '" ' +
                         'title="{{ data.main_name }}"> <span class="fas fa-info"></span></button>');
                 },
             });
 
             yearTableInitialized = true;
```

### Comparing `aa_ledger-0.3.3/ledger/static/ledger/js/img.js` & `aa_ledger-0.3.4/ledger/static/ledger/js/img.js`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/task_helpers/char_helpers.py` & `aa_ledger-0.3.4/ledger/task_helpers/char_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         .first()
     )
     if token:
         return token
     return False
 
 
+# pylint: disable=too-many-locals
 def update_character_wallet(character_id, force_refresh=False):
     audit_char = CharacterAudit.objects.get(character__character_id=character_id)
     logger.debug(
         "Updating wallet transactions for: %s", audit_char.character.character_name
     )
 
     req_scopes = ["esi-wallet.read_character_wallet.v1"]
```

### Comparing `aa_ledger-0.3.3/ledger/task_helpers/core_helpers.py` & `aa_ledger-0.3.4/ledger/task_helpers/core_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/task_helpers/corp_helpers.py` & `aa_ledger-0.3.4/ledger/task_helpers/corp_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,15 @@
 
     audit_corp.last_update_wallet = timezone.now()
     audit_corp.save()
 
     return ("Finished wallet divs for: %s", audit_corp.corporation.corporation_name)
 
 
+# pylint: disable=too-many-locals
 def update_corp_wallet_journal(corp_id, wallet_division, force_refresh=False):
     audit_corp = CorporationAudit.objects.get(corporation__corporation_id=corp_id)
 
     division = CorporationWalletDivision.objects.get(
         corporation=audit_corp, division=wallet_division
     )
```

### Comparing `aa_ledger-0.3.3/ledger/task_helpers/etag_helpers.py` & `aa_ledger-0.3.4/ledger/task_helpers/etag_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 def stringify_params(operation):
     out = []
     for p, v in operation.future.request.params.items():
         out.append(f"{p}: {v}")
     return ", ".join(out)
 
 
+# pylint: disable=too-many-statements, too-many-branches
 def etag_results(operation, token, force_refresh=False):
     _start_tm = time.perf_counter()
     results = []
     # override to always get the raw response for expiry header
     operation.request_config.also_return_response = True
     if token:
         operation.future.request.headers["Authorization"] = (
```

### Comparing `aa_ledger-0.3.3/ledger/templates/ledger/base.html` & `aa_ledger-0.3.4/ledger/templates/ledger/base.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/templates/ledger/error.html` & `aa_ledger-0.3.4/ledger/templates/ledger/error.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/templates/ledger/ledger/base.html` & `aa_ledger-0.3.4/ledger/templates/ledger/ledger/base.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/templates/ledger/ledger/index.html` & `aa_ledger-0.3.4/ledger/templates/ledger/ledger/index.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/templates/ledger/ledger/menu.html` & `aa_ledger-0.3.4/ledger/templates/ledger/ledger/menu.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/templates/ledger/ledger/charledger/char_ledger.html` & `aa_ledger-0.3.4/ledger/templates/ledger/ledger/charledger/char_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/templates/ledger/ledger/charledger/month.html` & `aa_ledger-0.3.4/ledger/templates/ledger/ledger/charledger/month.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/templates/ledger/ledger/charledger/year.html` & `aa_ledger-0.3.4/ledger/templates/ledger/ledger/charledger/year.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/templates/ledger/ledger/corpledger/corp_ledger.html` & `aa_ledger-0.3.4/ledger/templates/ledger/ledger/corpledger/corp_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/templates/ledger/ledger/corpledger/month.html` & `aa_ledger-0.3.4/ledger/templates/ledger/ledger/corpledger/month.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/templates/ledger/ledger/corpledger/year.html` & `aa_ledger-0.3.4/ledger/templates/ledger/ledger/corpledger/year.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/templates/ledger/modals/modal-full.html` & `aa_ledger-0.3.4/ledger/templates/ledger/modals/modal-full.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/templates/ledger/modals/modal-xl.html` & `aa_ledger-0.3.4/ledger/templates/ledger/modals/modal-xl.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/templates/ledger/modals/modal.html` & `aa_ledger-0.3.4/ledger/templates/ledger/modals/modal.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/templates/ledger/modals/modal_dialog.html` & `aa_ledger-0.3.4/ledger/templates/ledger/modals/modal_dialog.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/templates/ledger/modals/pve/view_character_content.html` & `aa_ledger-0.3.4/ledger/templates/ledger/modals/pve/view_character_content.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/view_helpers/core.py` & `aa_ledger-0.3.4/ledger/view_helpers/core.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/views/pve.py` & `aa_ledger-0.3.4/ledger/views/pve.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/views/character/char_audit.py` & `aa_ledger-0.3.4/ledger/views/character/char_audit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/views/corporation/corp_audit.py` & `aa_ledger-0.3.4/ledger/views/corporation/corp_audit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/views/corporation/corp_events.py` & `aa_ledger-0.3.4/ledger/views/corporation/corp_events.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/ledger/views/corporation/corp_tax.py` & `aa_ledger-0.3.4/ledger/views/corporation/corp_tax.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from ledger.hooks import get_extension_logger
 from ledger.models.corporationaudit import CorporationWalletJournalEntry, CorpSteuer
 
 logger = get_extension_logger(__name__)
 now = timezone.now()
 
 
+# TODO refactor this class
+# pylint: disable=too-many-locals, too-many-branches, too-many-statements
 @login_required
 @permission_required("ledger.basic_access")
 def index_steuer(request):
     """
     Index view
     :param request:
     :return:
```

### Comparing `aa_ledger-0.3.3/LICENSE` & `aa_ledger-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/README.md` & `aa_ledger-0.3.4/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-# Ledger module for AllianceAuth.<a name="aa-ledger"></a>
-
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Geuthur/aa-ledger/master.svg)](https://results.pre-commit.ci/latest/github/Geuthur/aa-ledger/master)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Tests](https://github.com/Geuthur/aa-ledger/actions/workflows/autotester.yml/badge.svg)](https://github.com/Geuthur/aa-ledger/actions/workflows/autotester.yml)
-
-- [AA Ledger](#aa-ledger)
-  - [Features](#features)
-  - [Upcoming](#upcoming)
-  - [Installation](#features)
-    - [Step 1 - Install the Package](#step1)
-    - [Step 2 - Configure Alliance Auth](#step2)
-    - [Step 3 - Add the Scheduled Tasks](#step3)
-    - [Step 4 - Migration to AA](#step4)
-    - [Step 5 - Setting up Permissions](#step5)
-    - [Step 6 - (Optional) Setting up Compatibilies](#step6)
-  - [Highlights](#highlights)
-
-## Features<a name="features"></a>
-
-- Graphical Overview
-- Ratting,Mining,Trading
-- Character Ledger
-- Corporation Ledger
-
-## Upcoming<a name="upcoming"></a>
-
-- Corp Tax System (Tracks specific amount that transfer'd to specific division)
-- Events Calender
-
-## Installation<a name="installation"></a>
-
-### Step 1 - Install the Package<a name="step1"></a>
-
-Make sure you're in your virtual environment (venv) of your Alliance Auth then install the pakage.
-
-```shell
-pip install aa-ledger
-```
-
-### Step 2 - Configure Alliance Auth<a name="step2"></a>
-
-Configure your Alliance Auth settings (`local.py`) as follows:
-
-- Add `'allianceauth.corputils',` to `INSTALLED_APPS`
-- Add `'eveuniverse',` to `INSTALLED_APPS`
-- Add `'ledger',` to `INSTALLED_APPS`
-
-### Step 3 - Add the Scheduled Tasks<a name="step3"></a>
-
-To set up the Scheduled Tasks add following code to your `local.py`
-
-```python
-CELERYBEAT_SCHEDULE["ledger_character_audit_update_all"] = {
-    "task": "ledger.tasks.update_all_characters",
-    "schedule": crontab(hour="*/1"),
-}
-CELERYBEAT_SCHEDULE["ledger_corporation_audit_update_all"] = {
-    "task": "ledger.tasks.update_all_corps",
-    "schedule": crontab(hour="*/1"),
-}
-```
-
-### Step 4 - Migration to AA<a name="step4"></a>
-
-```shell
-python manage.py collectstatic
-python manage.py migrate
-```
-
-### Step 5 - Setting up Permissions<a name="step5"></a>
-
-With the Following IDs you can set up the permissions for the Ledger
-
-| ID                        | Description                            |                                                                                         |
-| :------------------------ | :------------------------------------- | :-------------------------------------------------------------------------------------- |
-| `basic_access`            | Can access the Ledger module           | All Members with the Permission can access the Ledger.                                  |
-| `moderator_access`        | Has access to moderation tools         | Not Implemented yet.                                                                    |
-| `admin_access`            | Has access to all Administration tools | Not Implemented yet.                                                                    |
-| `char_audit_admin_access` | Can Manage Character Audit Module      | Can Manage Character Audit Module, Like Add Memeberaudit Chars, View Character Journals |
-| `corp_audit_admin_access` | Can Manage Corporation Audit Module    | Can Manage Corporation Audit Module, Like Add Corp, View Corporation Journals           |
-
-### Step 6 - (Optional) Setting up Compatibilies<a name="step6"></a>
-
-The Following Settings can be setting up in the `local.py`
-
-- LEDGER_LOGGER_USE:        `True / False`
-- LEDGER_MEMBERAUDIT_USE:   `True / False`
-- LEDGER_CORPSTATS_TWO:     `True / False`
-
-If you set up LEDGER_LOGGER_USE to `True` you need to add the following code below:
-
-```python
-LOGGING_LEDGER = {
-    "handlers": {
-        "ledger_file": {
-            "level": "DEBUG",
-            "class": "logging.handlers.RotatingFileHandler",
-            "filename": os.path.join(BASE_DIR, "log/ledger.log"),
-            "formatter": "verbose",
-            "maxBytes": 1024 * 1024 * 5,
-            "backupCount": 5,
-        },
-    },
-    "loggers": {
-        "ledger": {
-            "handlers": ["ledger_file", "console"],
-            "level": "DEBUG",
-        },
-    },
-}
-LOGGING["handlers"].update(LOGGING_LEDGER["handlers"])
-LOGGING["loggers"].update(LOGGING_LEDGER["loggers"])
-```
-
-## Highlights<a name="highlights"></a>
-
-![Screenshot 2024-05-14 121014](https://github.com/Geuthur/aa-ledger/assets/761682/d0604260-b672-4bf5-a16a-d1b90557744d)
-
-![Screenshot 2024-05-14 121025](https://github.com/Geuthur/aa-ledger/assets/761682/f8f20e6a-d37d-4a50-a1aa-8615c0f8e88b)
-
-![Screenshot 2024-05-14 120944](https://github.com/Geuthur/aa-ledger/assets/761682/2d695369-1331-4be9-8adf-9c6dabf80dda)
-
-![Screenshot 2024-05-14 121001](https://github.com/Geuthur/aa-ledger/assets/761682/463b9921-150c-42c1-8c3e-eee0f5cfc2bb)
-
-> \[!NOTE\]
-> Contributing
-> You want to improve the project?
-> Just Make a [Pull Request](https://github.com/Geuthur/aa-ledger/pulls) with the Guidelines.
-> We Using pre-commit
+# Ledger module for AllianceAuth.<a name="aa-ledger"></a>
+
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Geuthur/aa-ledger/master.svg)](https://results.pre-commit.ci/latest/github/Geuthur/aa-ledger/master)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Tests](https://github.com/Geuthur/aa-ledger/actions/workflows/autotester.yml/badge.svg)](https://github.com/Geuthur/aa-ledger/actions/workflows/autotester.yml)
+
+- [AA Ledger](#aa-ledger)
+  - [Features](#features)
+  - [Upcoming](#upcoming)
+  - [Installation](#features)
+    - [Step 1 - Install the Package](#step1)
+    - [Step 2 - Configure Alliance Auth](#step2)
+    - [Step 3 - Add the Scheduled Tasks](#step3)
+    - [Step 4 - Migration to AA](#step4)
+    - [Step 5 - Setting up Permissions](#step5)
+    - [Step 6 - (Optional) Setting up Compatibilies](#step6)
+  - [Highlights](#highlights)
+
+## Features<a name="features"></a>
+
+- Graphical Overview
+- Ratting,Mining,Trading
+- Character Ledger
+- Corporation Ledger
+
+## Upcoming<a name="upcoming"></a>
+
+- Corp Tax System (Tracks specific amount that transfer'd to specific division)
+- Events Calender
+
+## Installation<a name="installation"></a>
+
+### Step 1 - Install the Package<a name="step1"></a>
+
+Make sure you're in your virtual environment (venv) of your Alliance Auth then install the pakage.
+
+```shell
+pip install aa-ledger
+```
+
+### Step 2 - Configure Alliance Auth<a name="step2"></a>
+
+Configure your Alliance Auth settings (`local.py`) as follows:
+
+- Add `'allianceauth.corputils',` to `INSTALLED_APPS`
+- Add `'eveuniverse',` to `INSTALLED_APPS`
+- Add `'ledger',` to `INSTALLED_APPS`
+
+### Step 3 - Add the Scheduled Tasks<a name="step3"></a>
+
+To set up the Scheduled Tasks add following code to your `local.py`
+
+```python
+CELERYBEAT_SCHEDULE["ledger_character_audit_update_all"] = {
+    "task": "ledger.tasks.update_all_characters",
+    "schedule": crontab(hour="*/1"),
+}
+CELERYBEAT_SCHEDULE["ledger_corporation_audit_update_all"] = {
+    "task": "ledger.tasks.update_all_corps",
+    "schedule": crontab(hour="*/1"),
+}
+```
+
+### Step 4 - Migration to AA<a name="step4"></a>
+
+```shell
+python manage.py collectstatic
+python manage.py migrate
+```
+
+### Step 5 - Setting up Permissions<a name="step5"></a>
+
+With the Following IDs you can set up the permissions for the Ledger
+
+| ID                        | Description                            |                                                                                         |
+| :------------------------ | :------------------------------------- | :-------------------------------------------------------------------------------------- |
+| `basic_access`            | Can access the Ledger module           | All Members with the Permission can access the Ledger.                                  |
+| `moderator_access`        | Has access to moderation tools         | Not Implemented yet.                                                                    |
+| `admin_access`            | Has access to all Administration tools | Not Implemented yet.                                                                    |
+| `char_audit_admin_access` | Can Manage Character Audit Module      | Can Manage Character Audit Module, Like Add Memeberaudit Chars, View Character Journals |
+| `corp_audit_admin_access` | Can Manage Corporation Audit Module    | Can Manage Corporation Audit Module, Like Add Corp, View Corporation Journals           |
+
+### Step 6 - (Optional) Setting up Compatibilies<a name="step6"></a>
+
+The Following Settings can be setting up in the `local.py`
+
+- LEDGER_LOGGER_USE:        `True / False`
+- LEDGER_MEMBERAUDIT_USE:   `True / False`
+- LEDGER_CORPSTATS_TWO:     `True / False`
+
+If you set up LEDGER_LOGGER_USE to `True` you need to add the following code below:
+
+```python
+LOGGING_LEDGER = {
+    "handlers": {
+        "ledger_file": {
+            "level": "DEBUG",
+            "class": "logging.handlers.RotatingFileHandler",
+            "filename": os.path.join(BASE_DIR, "log/ledger.log"),
+            "formatter": "verbose",
+            "maxBytes": 1024 * 1024 * 5,
+            "backupCount": 5,
+        },
+    },
+    "loggers": {
+        "ledger": {
+            "handlers": ["ledger_file", "console"],
+            "level": "DEBUG",
+        },
+    },
+}
+LOGGING["handlers"].update(LOGGING_LEDGER["handlers"])
+LOGGING["loggers"].update(LOGGING_LEDGER["loggers"])
+```
+
+## Highlights<a name="highlights"></a>
+
+![Screenshot 2024-05-14 121014](https://github.com/Geuthur/aa-ledger/assets/761682/d0604260-b672-4bf5-a16a-d1b90557744d)
+
+![Screenshot 2024-05-14 121025](https://github.com/Geuthur/aa-ledger/assets/761682/f8f20e6a-d37d-4a50-a1aa-8615c0f8e88b)
+
+![Screenshot 2024-05-14 120944](https://github.com/Geuthur/aa-ledger/assets/761682/2d695369-1331-4be9-8adf-9c6dabf80dda)
+
+![Screenshot 2024-05-14 121001](https://github.com/Geuthur/aa-ledger/assets/761682/463b9921-150c-42c1-8c3e-eee0f5cfc2bb)
+
+> \[!NOTE\]
+> Contributing
+> You want to improve the project?
+> Just Make a [Pull Request](https://github.com/Geuthur/aa-ledger/pulls) with the Guidelines.
+> We Using pre-commit
```

### Comparing `aa_ledger-0.3.3/pyproject.toml` & `aa_ledger-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.3/PKG-INFO` & `aa_ledger-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aa-ledger
-Version: 0.3.3
+Version: 0.3.4
 Dynamic: Summary
 Project-URL: Changelog, https://github.com/Geuthur/aa-ledger/blob/master/CHANGELOG.md
 Project-URL: Homepage, https://github.com/Geuthur/aa-ledger
 Project-URL: Source, https://github.com/Geuthur/aa-ledger
 Project-URL: Tracker, https://github.com/Geuthur/aa-ledger/issues
 Author-email: Geuthur <devgeuthur@gmail.com>
 License: MIT License
```

