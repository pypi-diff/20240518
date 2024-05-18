# Comparing `tmp/wagtail_fedit-1.5.6.tar.gz` & `tmp/wagtail_fedit-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.6.tar", last modified: Mon May 13 18:26:52 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.7.tar", last modified: Sat May 18 16:17:52 2024, max compression
```

## Comparing `wagtail_fedit-1.5.6.tar` & `wagtail_fedit-1.5.7.tar`

### file list

```diff
@@ -1,136 +1,137 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.986194 wagtail_fedit-1.5.6/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.6/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.6/MANIFEST.in
--rw-rw-rw-   0        0        0     3010 2024-05-13 18:26:51.986194 wagtail_fedit-1.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     1812 2024-04-28 14:18:11.000000 wagtail_fedit-1.5.6/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.6/pyproject.toml
--rw-rw-rw-   0        0        0     1186 2024-05-13 18:26:51.989485 wagtail_fedit-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.362118 wagtail_fedit-1.5.6/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.6/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.503754 wagtail_fedit-1.5.6/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      532 2024-04-22 21:01:35.000000 wagtail_fedit-1.5.6/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0    14469 2024-04-25 18:57:33.000000 wagtail_fedit-1.5.6/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     6545 2024-04-25 18:29:05.000000 wagtail_fedit-1.5.6/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     8652 2024-04-23 18:12:26.000000 wagtail_fedit-1.5.6/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     2305 2024-04-25 18:28:58.000000 wagtail_fedit-1.5.6/wagtail_fedit/adapters/funcs.py
--rw-rw-rw-   0        0        0     2755 2024-04-25 18:28:49.000000 wagtail_fedit-1.5.6/wagtail_fedit/adapters/misc.py
--rw-rw-rw-   0        0        0     5607 2024-05-07 18:13:59.000000 wagtail_fedit-1.5.6/wagtail_fedit/adapters/models.py
--rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.6/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.6/wagtail_fedit/apps.py
--rw-rw-rw-   0        0        0     1354 2024-04-25 09:55:56.000000 wagtail_fedit-1.5.6/wagtail_fedit/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.516727 wagtail_fedit-1.5.6/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.6/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.6/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.6/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.6/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.186760 wagtail_fedit-1.5.6/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.188424 wagtail_fedit-1.5.6/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.516727 wagtail_fedit-1.5.6/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7262 2024-04-23 15:50:58.000000 wagtail_fedit-1.5.6/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    15296 2024-04-25 14:19:13.000000 wagtail_fedit-1.5.6/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.530705 wagtail_fedit-1.5.6/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.6/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.536185 wagtail_fedit-1.5.6/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.6/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.6/wagtail_fedit/models.py
--rw-rw-rw-   0        0        0     1626 2024-04-25 13:40:59.000000 wagtail_fedit-1.5.6/wagtail_fedit/settings.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.188424 wagtail_fedit-1.5.6/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.188424 wagtail_fedit-1.5.6/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.552164 wagtail_fedit-1.5.6/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     5745 2024-05-08 11:26:45.000000 wagtail_fedit-1.5.6/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.6/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.6/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.560817 wagtail_fedit-1.5.6/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    53927 2024-05-10 17:00:41.000000 wagtail_fedit-1.5.6/wagtail_fedit/static/wagtail_fedit/js/edit.js
--rw-rw-rw-   0        0        0    26914 2024-05-07 17:43:52.000000 wagtail_fedit-1.5.6/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.566799 wagtail_fedit-1.5.6/wagtail_fedit/static/wagtail_fedit/js/licenses/
--rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.6/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.188424 wagtail_fedit-1.5.6/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.572523 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/
--rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.576555 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.590914 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
--rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      571 2024-05-08 11:29:32.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.636022 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
--rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
--rw-rw-rw-   0        0        0      555 2024-04-21 21:13:45.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
--rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
--rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.660159 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.670283 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.677282 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.684898 wagtail_fedit-1.5.6/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.6/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.691889 wagtail_fedit-1.5.6/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.6/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    13140 2024-05-08 09:22:37.000000 wagtail_fedit-1.5.6/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    10310 2024-05-07 21:59:17.000000 wagtail_fedit-1.5.6/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.696893 wagtail_fedit-1.5.6/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.710292 wagtail_fedit-1.5.6/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/core/apps.py
--rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/core/context_processors.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.722200 wagtail_fedit-1.5.6/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.757969 wagtail_fedit-1.5.6/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     8962 2024-04-25 13:24:28.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0    28117 2024-04-25 18:07:06.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/core/tests/test_model_edit.py
--rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.929426 wagtail_fedit-1.5.6/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.6/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.6/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0     1196 2024-04-23 17:25:08.000000 wagtail_fedit-1.5.6/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    18101 2024-04-25 13:15:30.000000 wagtail_fedit-1.5.6/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.947083 wagtail_fedit-1.5.6/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      215 2024-04-23 17:24:50.000000 wagtail_fedit-1.5.6/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     8490 2024-04-25 13:06:47.000000 wagtail_fedit-1.5.6/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17778 2024-04-25 09:19:32.000000 wagtail_fedit-1.5.6/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     2239 2024-04-25 09:52:47.000000 wagtail_fedit-1.5.6/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.981186 wagtail_fedit-1.5.6/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.6/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1907 2024-05-13 18:26:02.000000 wagtail_fedit-1.5.6/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0     2446 2024-05-07 21:59:49.000000 wagtail_fedit-1.5.6/wagtail_fedit/wagtail_hooks/adapter_hooks.py
--rw-rw-rw-   0        0        0      328 2024-04-21 16:44:33.000000 wagtail_fedit-1.5.6/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.6/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     3100 2024-05-07 18:11:10.000000 wagtail_fedit-1.5.6/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.6/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7637 2024-04-23 20:17:24.000000 wagtail_fedit-1.5.6/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:26:51.434588 wagtail_fedit-1.5.6/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     3010 2024-05-13 18:26:51.000000 wagtail_fedit-1.5.6/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4466 2024-05-13 18:26:51.000000 wagtail_fedit-1.5.6/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 18:26:51.000000 wagtail_fedit-1.5.6/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-13 18:26:51.000000 wagtail_fedit-1.5.6/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-13 18:26:51.000000 wagtail_fedit-1.5.6/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.286909 wagtail_fedit-1.5.7/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.7/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     3010 2024-05-18 16:17:52.286909 wagtail_fedit-1.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1812 2024-04-28 14:18:11.000000 wagtail_fedit-1.5.7/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1186 2024-05-18 16:17:52.288414 wagtail_fedit-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.202686 wagtail_fedit-1.5.7/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.7/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.218202 wagtail_fedit-1.5.7/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      621 2024-05-18 12:37:42.000000 wagtail_fedit-1.5.7/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0    15018 2024-05-18 12:35:51.000000 wagtail_fedit-1.5.7/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     6666 2024-05-18 12:36:09.000000 wagtail_fedit-1.5.7/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     8779 2024-05-18 12:37:14.000000 wagtail_fedit-1.5.7/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     2305 2024-04-25 18:28:58.000000 wagtail_fedit-1.5.7/wagtail_fedit/adapters/funcs.py
+-rw-rw-rw-   0        0        0     2755 2024-04-25 18:28:49.000000 wagtail_fedit-1.5.7/wagtail_fedit/adapters/misc.py
+-rw-rw-rw-   0        0        0     5607 2024-05-07 18:13:59.000000 wagtail_fedit-1.5.7/wagtail_fedit/adapters/models.py
+-rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.7/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.7/wagtail_fedit/apps.py
+-rw-rw-rw-   0        0        0     1354 2024-04-25 09:55:56.000000 wagtail_fedit-1.5.7/wagtail_fedit/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.220364 wagtail_fedit-1.5.7/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.7/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.7/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.7/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.7/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.174210 wagtail_fedit-1.5.7/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.174210 wagtail_fedit-1.5.7/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.221365 wagtail_fedit-1.5.7/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7262 2024-04-23 15:50:58.000000 wagtail_fedit-1.5.7/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    15296 2024-04-25 14:19:13.000000 wagtail_fedit-1.5.7/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.222364 wagtail_fedit-1.5.7/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.7/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.223363 wagtail_fedit-1.5.7/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.7/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.7/wagtail_fedit/models.py
+-rw-rw-rw-   0        0        0     1626 2024-04-25 13:40:59.000000 wagtail_fedit-1.5.7/wagtail_fedit/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.176549 wagtail_fedit-1.5.7/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.177549 wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.226364 wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     5818 2024-05-18 12:31:35.000000 wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     5011 2024-05-18 15:36:53.000000 wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1249 2024-05-18 12:55:22.000000 wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.227365 wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    55265 2024-05-18 15:44:13.000000 wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/js/edit.js
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.228366 wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/js/licenses/
+-rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.178548 wagtail_fedit-1.5.7/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.229810 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/
+-rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.232059 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.234060 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
+-rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      601 2024-05-17 08:51:23.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+-rw-rw-rw-   0        0        0      378 2024-05-18 11:23:40.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/content/editable_dom_positioned_adapter.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.242571 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
+-rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
+-rw-rw-rw-   0        0        0      770 2024-05-18 12:22:37.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
+-rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
+-rw-rw-rw-   0        0        0      345 2024-05-18 12:28:53.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0      397 2024-05-18 12:21:43.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe_dom_positioned.html
+-rw-rw-rw-   0        0        0     5537 2024-05-18 12:20:21.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      549 2024-05-18 15:36:09.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.248567 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.249750 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.251749 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.252750 wagtail_fedit-1.5.7/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.7/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.253750 wagtail_fedit-1.5.7/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.7/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13170 2024-05-17 09:10:29.000000 wagtail_fedit-1.5.7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10373 2024-05-17 09:10:26.000000 wagtail_fedit-1.5.7/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.254751 wagtail_fedit-1.5.7/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.259778 wagtail_fedit-1.5.7/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.262784 wagtail_fedit-1.5.7/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.270295 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     8962 2024-04-25 13:24:28.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0    28117 2024-04-25 18:07:06.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_model_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.275295 wagtail_fedit-1.5.7/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3660 2024-05-18 16:08:35.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.7/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0     1196 2024-04-23 17:25:08.000000 wagtail_fedit-1.5.7/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    18093 2024-05-17 08:53:56.000000 wagtail_fedit-1.5.7/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.279809 wagtail_fedit-1.5.7/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      215 2024-04-23 17:24:50.000000 wagtail_fedit-1.5.7/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     8593 2024-05-17 08:17:48.000000 wagtail_fedit-1.5.7/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17778 2024-04-25 09:19:32.000000 wagtail_fedit-1.5.7/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     2239 2024-04-25 09:52:47.000000 wagtail_fedit-1.5.7/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.286909 wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1907 2024-05-13 18:26:02.000000 wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0     2446 2024-05-07 21:59:49.000000 wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/adapter_hooks.py
+-rw-rw-rw-   0        0        0      500 2024-05-18 12:38:10.000000 wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     3100 2024-05-07 18:11:10.000000 wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7637 2024-04-23 20:17:24.000000 wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.208195 wagtail_fedit-1.5.7/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     3010 2024-05-18 16:17:52.000000 wagtail_fedit-1.5.7/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4579 2024-05-18 16:17:52.000000 wagtail_fedit-1.5.7/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 16:17:52.000000 wagtail_fedit-1.5.7/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-18 16:17:52.000000 wagtail_fedit-1.5.7/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-18 16:17:52.000000 wagtail_fedit-1.5.7/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.6/LICENSE` & `wagtail_fedit-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/PKG-INFO` & `wagtail_fedit-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.5.6
+Version: 1.5.7
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail_fedit-1.5.6/README.md` & `wagtail_fedit-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/setup.cfg` & `wagtail_fedit-1.5.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 360d 0a64 6573 6372 6970 7469 6f6e 203d  6..description =
+00000030: 370d 0a64 6573 6372 6970 7469 6f6e 203d  7..description =
 00000040: 2046 726f 6e74 656e 6420 6564 6974 696e   Frontend editin
 00000050: 6720 666f 7220 796f 7572 2057 6167 7461  g for your Wagta
 00000060: 696c 2073 6974 650d 0a6c 6f6e 675f 6465  il site..long_de
 00000070: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
 00000080: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
 00000090: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
 000000a0: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
```

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/adapters/__init__.py` & `wagtail_fedit-1.5.7/wagtail_fedit/adapters/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from .base import (
     Keyword,
     BaseAdapter,
+    DomPositionedMixin,
     AdapterError,
 )
 from .registry import (
     AdapterRegistry,
     RegistryLookUpError,
     DuplicateAdapterError,
     AdapterSubclassError,
     registry as adapter_registry,
 )
 from .block import (
     BlockAdapter,
+    DomPositionedBlockAdapter,
 )
 from .field import (
     FieldAdapter,
+    DomPositionedFieldAdapter,
 )
 from .models import (
     ModelAdapter,
 )
 from .funcs import (
     FuncAdapterMixin,
     BaseFieldFuncAdapter,
```

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.5.7/wagtail_fedit/adapters/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,14 +181,15 @@
     identifier              = None
 
     # If the templatetag required the first argument to be model.field or just model
     field_required          = True
 
     # The template used to render the form.
     template_name           = "wagtail_fedit/editor/adapter_iframe.html"
+    editable_template_name  = "wagtail_fedit/content/editable_adapter.html"
 
     signer: Signer          = Signer()
     
     # Keyword arguments for the adapter
     keywords: tuple[Keyword]     = (
         Keyword(
             "inline",
@@ -261,14 +262,20 @@
         return d
     
     def get_template_names(self) -> list[str]:
         """
         Return the template names for the adapter.
         """
         return [self.template_name]
+    
+    def get_editable_template_names(self) -> list[str]:
+        """
+        Return the template names for the adapter.
+        """
+        return [self.editable_template_name]
 
     @property
     def field_value(self):
         """
         Call the value_from_object method on
         the meta field to get the value from the instance.
         """
@@ -463,7 +470,11 @@
             request=self.request,
             adapter=self,
             context=parent_context,
             run_context_processors=True
         )
         return data
 
+class DomPositionedMixin(BaseAdapter):
+    template_name = "wagtail_fedit/editor/adapter_iframe_dom_positioned.html"
+    editable_template_name  = "wagtail_fedit/content/editable_dom_positioned_adapter.html"
+    js_constructor = "wagtail_fedit.editors.DomPositionedBlockFieldEditor"
```

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.5.7/wagtail_fedit/adapters/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 )
 from wagtail.models import (
     RevisionMixin,
 )
 
 from .base import (
     BlockFieldReplacementAdapter,
+    DomPositionedMixin,
     AdapterError,
     Keyword,
     VARIABLES,
 )
 from ..forms import (
     blocks as block_forms,
 )
@@ -180,8 +181,10 @@
 
     def render_content(self, parent_context: dict = None) -> str:
         parent_context = parent_context or {}
         if hasattr(parent_context, "flatten"):
             parent_context = parent_context.flatten()
 
         return self.block.render(parent_context)
-        
+    
+class DomPositionedBlockAdapter(DomPositionedMixin, BlockAdapter):
+    identifier = "dom-block"
```

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.7/wagtail_fedit/adapters/field.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from wagtail.log_actions import log
 from wagtail.models import RevisionMixin
 from wagtail.fields import StreamField
 from wagtail import hooks
 
 from .base import (
     BlockFieldReplacementAdapter,
+    DomPositionedMixin,
     VARIABLES,
 )
 from ..hooks import (
     FIELD_EDITOR_SIZE,
 )
 from ..utils import (
     use_related_form,
@@ -216,7 +217,11 @@
     def render_content(self, parent_context=None):
         return get_field_content(
             self.request,
             self.original_object,
             self.meta_field,
             parent_context,
         )
+
+
+class DomPositionedFieldAdapter(DomPositionedMixin, FieldAdapter):
+    identifier = "dom-field"
```

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/adapters/funcs.py` & `wagtail_fedit-1.5.7/wagtail_fedit/adapters/funcs.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/adapters/misc.py` & `wagtail_fedit-1.5.7/wagtail_fedit/adapters/misc.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/adapters/models.py` & `wagtail_fedit-1.5.7/wagtail_fedit/adapters/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.5.7/wagtail_fedit/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/errors.py` & `wagtail_fedit-1.5.7/wagtail_fedit/errors.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.7/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.5.7/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.7/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.7/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.7/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/models.py` & `wagtail_fedit-1.5.7/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/settings.py` & `wagtail_fedit-1.5.7/wagtail_fedit/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 html, body {
     margin: 0;
     padding: 0;
 }
 .wagtail-fedit-adapter-wrapper {
     position: relative;
 }
+.wagtail-fedit-adapter-wrapper 
 .wagtail-fedit-buttons {
     display: flex;
 }
 
 .wagtail-fedit-adapter-wrapper:has(> .wagtail-fedit-buttons:only-child) {
     min-height: 24px;
 }
@@ -176,15 +177,16 @@
 @media (max-width: 768px) {
     .wagtail-fedit-modal-wrapper .wagtail-fedit-modal {
         margin: 0;
         max-width: 100%;
         max-height: 100%;
     }
 }
-.wagtail-fedit-modal-wrapper iframe {
+.wagtail-fedit-modal-wrapper iframe,
+.wagtail-fedit-adapter-wrapper iframe {
     width: 100%;
     height: 100%;
     border: none;
     flex: 1;
 }
 .wagtail-fedit-modal-wrapper .wagtail-fedit-close-button {
     position: absolute;
```

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files 3% similar despite different names*

```diff
@@ -74,18 +74,14 @@
 .fedit-sidebar .wagtail-fedit-cancel-button:hover {
     color: var(--w-color-critical-200);
 }
 main > div.nice-padding {
     overflow-x: hidden;
     overflow-y: auto;
 }
-.wagtail-fedit-form-wrapper {
-    padding-top: 0.5em;
-    padding-bottom: 0.5em;
-}
 main > div.nice-padding::-webkit-scrollbar {
   width: 0.8em;
   background-color: var(--w-color-surface-page);
   border-left: 1px dotted var(--w-color-surface-menus);
 }
 main > div.nice-padding::-webkit-scrollbar-thumb {
     background: var(--w-color-surface-menus);
```

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     fill: var(--w-color-positive-100);
     opacity: 1;
 }
 [name="action-unpublish"]:hover svg {
     fill: var(--w-color-critical-200);
     opacity: 1;
 }
-.wagtail-fedit-userbar-button.initially-hidden {
+.wagtail-fedit-userbar-button {
     display: none;
 }
 .w-userbar__item a.wagtail-fedit-userbar-button {
     background-color: initial;
     padding-bottom: unset;
     padding-top: unset;
     outline: none;
```

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/static/wagtail_fedit/js/edit.js` & `wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/js/edit.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,250 +1,250 @@
 (() => {
     "use strict";
-    var t = {
-            2: (t, e, n) => {
-                n.d(e, {
+    var e = {
+            2: (e, t, n) => {
+                n.d(t, {
                     A: () => s
                 });
                 var i = n(601),
                     r = n.n(i),
                     o = n(314),
                     a = n.n(o)()(r());
-                a.push([t.id, '.tippy-box[data-animation=fade][data-state=hidden]{opacity:0}[data-tippy-root]{max-width:calc(100vw - 10px)}.tippy-box{position:relative;background-color:#333;color:#fff;border-radius:4px;font-size:14px;line-height:1.4;white-space:normal;outline:0;transition-property:transform,visibility,opacity}.tippy-box[data-placement^=top]>.tippy-arrow{bottom:0}.tippy-box[data-placement^=top]>.tippy-arrow:before{bottom:-7px;left:0;border-width:8px 8px 0;border-top-color:initial;transform-origin:center top}.tippy-box[data-placement^=bottom]>.tippy-arrow{top:0}.tippy-box[data-placement^=bottom]>.tippy-arrow:before{top:-7px;left:0;border-width:0 8px 8px;border-bottom-color:initial;transform-origin:center bottom}.tippy-box[data-placement^=left]>.tippy-arrow{right:0}.tippy-box[data-placement^=left]>.tippy-arrow:before{border-width:8px 0 8px 8px;border-left-color:initial;right:-7px;transform-origin:center left}.tippy-box[data-placement^=right]>.tippy-arrow{left:0}.tippy-box[data-placement^=right]>.tippy-arrow:before{left:-7px;border-width:8px 8px 8px 0;border-right-color:initial;transform-origin:center right}.tippy-box[data-inertia][data-state=visible]{transition-timing-function:cubic-bezier(.54,1.5,.38,1.11)}.tippy-arrow{width:16px;height:16px;color:#333}.tippy-arrow:before{content:"";position:absolute;border-color:transparent;border-style:solid}.tippy-content{position:relative;padding:5px 9px;z-index:1}', ""]);
+                a.push([e.id, '.tippy-box[data-animation=fade][data-state=hidden]{opacity:0}[data-tippy-root]{max-width:calc(100vw - 10px)}.tippy-box{position:relative;background-color:#333;color:#fff;border-radius:4px;font-size:14px;line-height:1.4;white-space:normal;outline:0;transition-property:transform,visibility,opacity}.tippy-box[data-placement^=top]>.tippy-arrow{bottom:0}.tippy-box[data-placement^=top]>.tippy-arrow:before{bottom:-7px;left:0;border-width:8px 8px 0;border-top-color:initial;transform-origin:center top}.tippy-box[data-placement^=bottom]>.tippy-arrow{top:0}.tippy-box[data-placement^=bottom]>.tippy-arrow:before{top:-7px;left:0;border-width:0 8px 8px;border-bottom-color:initial;transform-origin:center bottom}.tippy-box[data-placement^=left]>.tippy-arrow{right:0}.tippy-box[data-placement^=left]>.tippy-arrow:before{border-width:8px 0 8px 8px;border-left-color:initial;right:-7px;transform-origin:center left}.tippy-box[data-placement^=right]>.tippy-arrow{left:0}.tippy-box[data-placement^=right]>.tippy-arrow:before{left:-7px;border-width:8px 8px 8px 0;border-right-color:initial;transform-origin:center right}.tippy-box[data-inertia][data-state=visible]{transition-timing-function:cubic-bezier(.54,1.5,.38,1.11)}.tippy-arrow{width:16px;height:16px;color:#333}.tippy-arrow:before{content:"";position:absolute;border-color:transparent;border-style:solid}.tippy-content{position:relative;padding:5px 9px;z-index:1}', ""]);
                 const s = a
             },
-            314: t => {
-                t.exports = function(t) {
-                    var e = [];
-                    return e.toString = function() {
-                        return this.map((function(e) {
+            314: e => {
+                e.exports = function(e) {
+                    var t = [];
+                    return t.toString = function() {
+                        return this.map((function(t) {
                             var n = "",
-                                i = void 0 !== e[5];
-                            return e[4] && (n += "@supports (".concat(e[4], ") {")), e[2] && (n += "@media ".concat(e[2], " {")), i && (n += "@layer".concat(e[5].length > 0 ? " ".concat(e[5]) : "", " {")), n += t(e), i && (n += "}"), e[2] && (n += "}"), e[4] && (n += "}"), n
+                                i = void 0 !== t[5];
+                            return t[4] && (n += "@supports (".concat(t[4], ") {")), t[2] && (n += "@media ".concat(t[2], " {")), i && (n += "@layer".concat(t[5].length > 0 ? " ".concat(t[5]) : "", " {")), n += e(t), i && (n += "}"), t[2] && (n += "}"), t[4] && (n += "}"), n
                         })).join("")
-                    }, e.i = function(t, n, i, r, o) {
-                        "string" == typeof t && (t = [
-                            [null, t, void 0]
+                    }, t.i = function(e, n, i, r, o) {
+                        "string" == typeof e && (e = [
+                            [null, e, void 0]
                         ]);
                         var a = {};
                         if (i)
                             for (var s = 0; s < this.length; s++) {
                                 var c = this[s][0];
                                 null != c && (a[c] = !0)
                             }
-                        for (var l = 0; l < t.length; l++) {
-                            var d = [].concat(t[l]);
-                            i && a[d[0]] || (void 0 !== o && (void 0 === d[5] || (d[1] = "@layer".concat(d[5].length > 0 ? " ".concat(d[5]) : "", " {").concat(d[1], "}")), d[5] = o), n && (d[2] ? (d[1] = "@media ".concat(d[2], " {").concat(d[1], "}"), d[2] = n) : d[2] = n), r && (d[4] ? (d[1] = "@supports (".concat(d[4], ") {").concat(d[1], "}"), d[4] = r) : d[4] = "".concat(r)), e.push(d))
+                        for (var l = 0; l < e.length; l++) {
+                            var d = [].concat(e[l]);
+                            i && a[d[0]] || (void 0 !== o && (void 0 === d[5] || (d[1] = "@layer".concat(d[5].length > 0 ? " ".concat(d[5]) : "", " {").concat(d[1], "}")), d[5] = o), n && (d[2] ? (d[1] = "@media ".concat(d[2], " {").concat(d[1], "}"), d[2] = n) : d[2] = n), r && (d[4] ? (d[1] = "@supports (".concat(d[4], ") {").concat(d[1], "}"), d[4] = r) : d[4] = "".concat(r)), t.push(d))
                         }
-                    }, e
+                    }, t
                 }
             },
-            601: t => {
-                t.exports = function(t) {
-                    return t[1]
+            601: e => {
+                e.exports = function(e) {
+                    return e[1]
                 }
             },
-            72: t => {
-                var e = [];
+            72: e => {
+                var t = [];
 
-                function n(t) {
-                    for (var n = -1, i = 0; i < e.length; i++)
-                        if (e[i].identifier === t) {
+                function n(e) {
+                    for (var n = -1, i = 0; i < t.length; i++)
+                        if (t[i].identifier === e) {
                             n = i;
                             break
                         } return n
                 }
 
-                function i(t, i) {
-                    for (var o = {}, a = [], s = 0; s < t.length; s++) {
-                        var c = t[s],
+                function i(e, i) {
+                    for (var o = {}, a = [], s = 0; s < e.length; s++) {
+                        var c = e[s],
                             l = i.base ? c[0] + i.base : c[0],
                             d = o[l] || 0,
                             p = "".concat(l, " ").concat(d);
                         o[l] = d + 1;
                         var u = n(p),
                             f = {
                                 css: c[1],
                                 media: c[2],
                                 sourceMap: c[3],
                                 supports: c[4],
                                 layer: c[5]
                             };
-                        if (-1 !== u) e[u].references++, e[u].updater(f);
+                        if (-1 !== u) t[u].references++, t[u].updater(f);
                         else {
                             var h = r(f, i);
-                            i.byIndex = s, e.splice(s, 0, {
+                            i.byIndex = s, t.splice(s, 0, {
                                 identifier: p,
                                 updater: h,
                                 references: 1
                             })
                         }
                         a.push(p)
                     }
                     return a
                 }
 
-                function r(t, e) {
-                    var n = e.domAPI(e);
-                    return n.update(t),
-                        function(e) {
-                            if (e) {
-                                if (e.css === t.css && e.media === t.media && e.sourceMap === t.sourceMap && e.supports === t.supports && e.layer === t.layer) return;
-                                n.update(t = e)
+                function r(e, t) {
+                    var n = t.domAPI(t);
+                    return n.update(e),
+                        function(t) {
+                            if (t) {
+                                if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap && t.supports === e.supports && t.layer === e.layer) return;
+                                n.update(e = t)
                             } else n.remove()
                         }
                 }
-                t.exports = function(t, r) {
-                    var o = i(t = t || [], r = r || {});
-                    return function(t) {
-                        t = t || [];
+                e.exports = function(e, r) {
+                    var o = i(e = e || [], r = r || {});
+                    return function(e) {
+                        e = e || [];
                         for (var a = 0; a < o.length; a++) {
                             var s = n(o[a]);
-                            e[s].references--
+                            t[s].references--
                         }
-                        for (var c = i(t, r), l = 0; l < o.length; l++) {
+                        for (var c = i(e, r), l = 0; l < o.length; l++) {
                             var d = n(o[l]);
-                            0 === e[d].references && (e[d].updater(), e.splice(d, 1))
+                            0 === t[d].references && (t[d].updater(), t.splice(d, 1))
                         }
                         o = c
                     }
                 }
             },
-            659: t => {
-                var e = {};
-                t.exports = function(t, n) {
-                    var i = function(t) {
-                        if (void 0 === e[t]) {
-                            var n = document.querySelector(t);
+            659: e => {
+                var t = {};
+                e.exports = function(e, n) {
+                    var i = function(e) {
+                        if (void 0 === t[e]) {
+                            var n = document.querySelector(e);
                             if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
                                 n = n.contentDocument.head
-                            } catch (t) {
+                            } catch (e) {
                                 n = null
                             }
-                            e[t] = n
+                            t[e] = n
                         }
-                        return e[t]
-                    }(t);
+                        return t[e]
+                    }(e);
                     if (!i) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
                     i.appendChild(n)
                 }
             },
-            540: t => {
-                t.exports = function(t) {
-                    var e = document.createElement("style");
-                    return t.setAttributes(e, t.attributes), t.insert(e, t.options), e
+            540: e => {
+                e.exports = function(e) {
+                    var t = document.createElement("style");
+                    return e.setAttributes(t, e.attributes), e.insert(t, e.options), t
                 }
             },
-            56: (t, e, n) => {
-                t.exports = function(t) {
-                    var e = n.nc;
-                    e && t.setAttribute("nonce", e)
+            56: (e, t, n) => {
+                e.exports = function(e) {
+                    var t = n.nc;
+                    t && e.setAttribute("nonce", t)
                 }
             },
-            825: t => {
-                t.exports = function(t) {
+            825: e => {
+                e.exports = function(e) {
                     if ("undefined" == typeof document) return {
                         update: function() {},
                         remove: function() {}
                     };
-                    var e = t.insertStyleElement(t);
+                    var t = e.insertStyleElement(e);
                     return {
                         update: function(n) {
-                            ! function(t, e, n) {
+                            ! function(e, t, n) {
                                 var i = "";
                                 n.supports && (i += "@supports (".concat(n.supports, ") {")), n.media && (i += "@media ".concat(n.media, " {"));
                                 var r = void 0 !== n.layer;
                                 r && (i += "@layer".concat(n.layer.length > 0 ? " ".concat(n.layer) : "", " {")), i += n.css, r && (i += "}"), n.media && (i += "}"), n.supports && (i += "}");
                                 var o = n.sourceMap;
-                                o && "undefined" != typeof btoa && (i += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(o)))), " */")), e.styleTagTransform(i, t, e.options)
-                            }(e, t, n)
+                                o && "undefined" != typeof btoa && (i += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(o)))), " */")), t.styleTagTransform(i, e, t.options)
+                            }(t, e, n)
                         },
                         remove: function() {
-                            ! function(t) {
-                                if (null === t.parentNode) return !1;
-                                t.parentNode.removeChild(t)
-                            }(e)
+                            ! function(e) {
+                                if (null === e.parentNode) return !1;
+                                e.parentNode.removeChild(e)
+                            }(t)
                         }
                     }
                 }
             },
-            113: t => {
-                t.exports = function(t, e) {
-                    if (e.styleSheet) e.styleSheet.cssText = t;
+            113: e => {
+                e.exports = function(e, t) {
+                    if (t.styleSheet) t.styleSheet.cssText = e;
                     else {
-                        for (; e.firstChild;) e.removeChild(e.firstChild);
-                        e.appendChild(document.createTextNode(t))
+                        for (; t.firstChild;) t.removeChild(t.firstChild);
+                        t.appendChild(document.createTextNode(e))
                     }
                 }
             }
         },
-        e = {};
+        t = {};
 
     function n(i) {
-        var r = e[i];
+        var r = t[i];
         if (void 0 !== r) return r.exports;
-        var o = e[i] = {
+        var o = t[i] = {
             id: i,
             exports: {}
         };
-        return t[i](o, o.exports, n), o.exports
+        return e[i](o, o.exports, n), o.exports
     }
-    n.n = t => {
-        var e = t && t.__esModule ? () => t.default : () => t;
-        return n.d(e, {
-            a: e
-        }), e
-    }, n.d = (t, e) => {
-        for (var i in e) n.o(e, i) && !n.o(t, i) && Object.defineProperty(t, i, {
+    n.n = e => {
+        var t = e && e.__esModule ? () => e.default : () => e;
+        return n.d(t, {
+            a: t
+        }), t
+    }, n.d = (e, t) => {
+        for (var i in t) n.o(t, i) && !n.o(e, i) && Object.defineProperty(e, i, {
             enumerable: !0,
-            get: e[i]
+            get: t[i]
         })
-    }, n.o = (t, e) => Object.prototype.hasOwnProperty.call(t, e), n.nc = void 0, (() => {
-        function t(t) {
-            if (null == t) return window;
-            if ("[object Window]" !== t.toString()) {
-                var e = t.ownerDocument;
-                return e && e.defaultView || window
+    }, n.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), n.nc = void 0, (() => {
+        function e(e) {
+            if (null == e) return window;
+            if ("[object Window]" !== e.toString()) {
+                var t = e.ownerDocument;
+                return t && t.defaultView || window
             }
-            return t
+            return e
         }
 
-        function e(e) {
-            return e instanceof t(e).Element || e instanceof Element
+        function t(t) {
+            return t instanceof e(t).Element || t instanceof Element
         }
 
-        function i(e) {
-            return e instanceof t(e).HTMLElement || e instanceof HTMLElement
+        function i(t) {
+            return t instanceof e(t).HTMLElement || t instanceof HTMLElement
         }
 
-        function r(e) {
-            return "undefined" != typeof ShadowRoot && (e instanceof t(e).ShadowRoot || e instanceof ShadowRoot)
+        function r(t) {
+            return "undefined" != typeof ShadowRoot && (t instanceof e(t).ShadowRoot || t instanceof ShadowRoot)
         }
         var o = Math.max,
             a = Math.min,
             s = Math.round;
 
         function c() {
-            var t = navigator.userAgentData;
-            return null != t && t.brands && Array.isArray(t.brands) ? t.brands.map((function(t) {
-                return t.brand + "/" + t.version
+            var e = navigator.userAgentData;
+            return null != e && e.brands && Array.isArray(e.brands) ? e.brands.map((function(e) {
+                return e.brand + "/" + e.version
             })).join(" ") : navigator.userAgent
         }
 
         function l() {
             return !/^((?!chrome|android).)*safari/i.test(c())
         }
 
         function d(n, r, o) {
             void 0 === r && (r = !1), void 0 === o && (o = !1);
             var a = n.getBoundingClientRect(),
                 c = 1,
                 d = 1;
             r && i(n) && (c = n.offsetWidth > 0 && s(a.width) / n.offsetWidth || 1, d = n.offsetHeight > 0 && s(a.height) / n.offsetHeight || 1);
-            var p = (e(n) ? t(n) : window).visualViewport,
+            var p = (t(n) ? e(n) : window).visualViewport,
                 u = !l() && o,
                 f = (a.left + (u && p ? p.offsetLeft : 0)) / c,
                 h = (a.top + (u && p ? p.offsetTop : 0)) / d,
                 m = a.width / c,
                 v = a.height / d;
             return {
                 width: m,
@@ -254,255 +254,255 @@
                 bottom: h + v,
                 left: f,
                 x: f,
                 y: h
             }
         }
 
-        function p(e) {
-            var n = t(e);
+        function p(t) {
+            var n = e(t);
             return {
                 scrollLeft: n.pageXOffset,
                 scrollTop: n.pageYOffset
             }
         }
 
-        function u(t) {
-            return t ? (t.nodeName || "").toLowerCase() : null
+        function u(e) {
+            return e ? (e.nodeName || "").toLowerCase() : null
         }
 
-        function f(t) {
-            return ((e(t) ? t.ownerDocument : t.document) || window.document).documentElement
+        function f(e) {
+            return ((t(e) ? e.ownerDocument : e.document) || window.document).documentElement
         }
 
-        function h(t) {
-            return d(f(t)).left + p(t).scrollLeft
+        function h(e) {
+            return d(f(e)).left + p(e).scrollLeft
         }
 
-        function m(e) {
-            return t(e).getComputedStyle(e)
+        function m(t) {
+            return e(t).getComputedStyle(t)
         }
 
-        function v(t) {
-            var e = m(t),
-                n = e.overflow,
-                i = e.overflowX,
-                r = e.overflowY;
+        function v(e) {
+            var t = m(e),
+                n = t.overflow,
+                i = t.overflowX,
+                r = t.overflowY;
             return /auto|scroll|overlay|hidden/.test(n + r + i)
         }
 
-        function g(e, n, r) {
+        function g(t, n, r) {
             void 0 === r && (r = !1);
             var o, a, c = i(n),
-                l = i(n) && function(t) {
-                    var e = t.getBoundingClientRect(),
-                        n = s(e.width) / t.offsetWidth || 1,
-                        i = s(e.height) / t.offsetHeight || 1;
+                l = i(n) && function(e) {
+                    var t = e.getBoundingClientRect(),
+                        n = s(t.width) / e.offsetWidth || 1,
+                        i = s(t.height) / e.offsetHeight || 1;
                     return 1 !== n || 1 !== i
                 }(n),
                 m = f(n),
-                g = d(e, l, r),
+                g = d(t, l, r),
                 w = {
                     scrollLeft: 0,
                     scrollTop: 0
                 },
                 y = {
                     x: 0,
                     y: 0
                 };
-            return (c || !c && !r) && (("body" !== u(n) || v(m)) && (w = (o = n) !== t(o) && i(o) ? {
+            return (c || !c && !r) && (("body" !== u(n) || v(m)) && (w = (o = n) !== e(o) && i(o) ? {
                 scrollLeft: (a = o).scrollLeft,
                 scrollTop: a.scrollTop
             } : p(o)), i(n) ? ((y = d(n, !0)).x += n.clientLeft, y.y += n.clientTop) : m && (y.x = h(m))), {
                 x: g.left + w.scrollLeft - y.x,
                 y: g.top + w.scrollTop - y.y,
                 width: g.width,
                 height: g.height
             }
         }
 
-        function w(t) {
-            var e = d(t),
-                n = t.offsetWidth,
-                i = t.offsetHeight;
-            return Math.abs(e.width - n) <= 1 && (n = e.width), Math.abs(e.height - i) <= 1 && (i = e.height), {
-                x: t.offsetLeft,
-                y: t.offsetTop,
+        function w(e) {
+            var t = d(e),
+                n = e.offsetWidth,
+                i = e.offsetHeight;
+            return Math.abs(t.width - n) <= 1 && (n = t.width), Math.abs(t.height - i) <= 1 && (i = t.height), {
+                x: e.offsetLeft,
+                y: e.offsetTop,
                 width: n,
                 height: i
             }
         }
 
-        function y(t) {
-            return "html" === u(t) ? t : t.assignedSlot || t.parentNode || (r(t) ? t.host : null) || f(t)
+        function y(e) {
+            return "html" === u(e) ? e : e.assignedSlot || e.parentNode || (r(e) ? e.host : null) || f(e)
         }
 
-        function b(t) {
-            return ["html", "body", "#document"].indexOf(u(t)) >= 0 ? t.ownerDocument.body : i(t) && v(t) ? t : b(y(t))
+        function b(e) {
+            return ["html", "body", "#document"].indexOf(u(e)) >= 0 ? e.ownerDocument.body : i(e) && v(e) ? e : b(y(e))
         }
 
-        function x(e, n) {
+        function E(t, n) {
             var i;
             void 0 === n && (n = []);
-            var r = b(e),
-                o = r === (null == (i = e.ownerDocument) ? void 0 : i.body),
-                a = t(r),
+            var r = b(t),
+                o = r === (null == (i = t.ownerDocument) ? void 0 : i.body),
+                a = e(r),
                 s = o ? [a].concat(a.visualViewport || [], v(r) ? r : []) : r,
                 c = n.concat(s);
-            return o ? c : c.concat(x(y(s)))
+            return o ? c : c.concat(E(y(s)))
         }
 
-        function E(t) {
-            return ["table", "td", "th"].indexOf(u(t)) >= 0
+        function x(e) {
+            return ["table", "td", "th"].indexOf(u(e)) >= 0
         }
 
-        function O(t) {
-            return i(t) && "fixed" !== m(t).position ? t.offsetParent : null
+        function O(e) {
+            return i(e) && "fixed" !== m(e).position ? e.offsetParent : null
         }
 
-        function L(e) {
-            for (var n = t(e), o = O(e); o && E(o) && "static" === m(o).position;) o = O(o);
-            return o && ("html" === u(o) || "body" === u(o) && "static" === m(o).position) ? n : o || function(t) {
-                var e = /firefox/i.test(c());
-                if (/Trident/i.test(c()) && i(t) && "fixed" === m(t).position) return null;
-                var n = y(t);
+        function L(t) {
+            for (var n = e(t), o = O(t); o && x(o) && "static" === m(o).position;) o = O(o);
+            return o && ("html" === u(o) || "body" === u(o) && "static" === m(o).position) ? n : o || function(e) {
+                var t = /firefox/i.test(c());
+                if (/Trident/i.test(c()) && i(e) && "fixed" === m(e).position) return null;
+                var n = y(e);
                 for (r(n) && (n = n.host); i(n) && ["html", "body"].indexOf(u(n)) < 0;) {
                     var o = m(n);
-                    if ("none" !== o.transform || "none" !== o.perspective || "paint" === o.contain || -1 !== ["transform", "perspective"].indexOf(o.willChange) || e && "filter" === o.willChange || e && o.filter && "none" !== o.filter) return n;
+                    if ("none" !== o.transform || "none" !== o.perspective || "paint" === o.contain || -1 !== ["transform", "perspective"].indexOf(o.willChange) || t && "filter" === o.willChange || t && o.filter && "none" !== o.filter) return n;
                     n = n.parentNode
                 }
                 return null
-            }(e) || n
+            }(t) || n
         }
-        var A = "top",
-            T = "bottom",
+        var T = "top",
+            A = "bottom",
             C = "right",
-            M = "left",
-            S = "auto",
-            D = [A, T, C, M],
-            k = "start",
+            S = "left",
+            D = "auto",
+            M = [T, A, C, S],
+            R = "start",
             j = "end",
-            P = "viewport",
-            N = "popper",
-            H = D.reduce((function(t, e) {
-                return t.concat([e + "-" + k, e + "-" + j])
+            I = "viewport",
+            k = "popper",
+            P = M.reduce((function(e, t) {
+                return e.concat([t + "-" + R, t + "-" + j])
             }), []),
-            R = [].concat(D, [S]).reduce((function(t, e) {
-                return t.concat([e, e + "-" + k, e + "-" + j])
+            H = [].concat(M, [D]).reduce((function(e, t) {
+                return e.concat([t, t + "-" + R, t + "-" + j])
             }), []),
-            W = ["beforeRead", "read", "afterRead", "beforeMain", "main", "afterMain", "beforeWrite", "write", "afterWrite"];
+            N = ["beforeRead", "read", "afterRead", "beforeMain", "main", "afterMain", "beforeWrite", "write", "afterWrite"];
 
-        function B(t) {
-            var e = new Map,
+        function W(e) {
+            var t = new Map,
                 n = new Set,
                 i = [];
 
-            function r(t) {
-                n.add(t.name), [].concat(t.requires || [], t.requiresIfExists || []).forEach((function(t) {
-                    if (!n.has(t)) {
-                        var i = e.get(t);
+            function r(e) {
+                n.add(e.name), [].concat(e.requires || [], e.requiresIfExists || []).forEach((function(e) {
+                    if (!n.has(e)) {
+                        var i = t.get(e);
                         i && r(i)
                     }
-                })), i.push(t)
+                })), i.push(e)
             }
-            return t.forEach((function(t) {
-                e.set(t.name, t)
-            })), t.forEach((function(t) {
-                n.has(t.name) || r(t)
+            return e.forEach((function(e) {
+                t.set(e.name, e)
+            })), e.forEach((function(e) {
+                n.has(e.name) || r(e)
             })), i
         }
-        var I = {
+        var B = {
             placement: "bottom",
             modifiers: [],
             strategy: "absolute"
         };
 
         function _() {
-            for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
-            return !e.some((function(t) {
-                return !(t && "function" == typeof t.getBoundingClientRect)
+            for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
+            return !t.some((function(e) {
+                return !(e && "function" == typeof e.getBoundingClientRect)
             }))
         }
 
-        function F(t) {
-            void 0 === t && (t = {});
-            var n = t,
+        function F(e) {
+            void 0 === e && (e = {});
+            var n = e,
                 i = n.defaultModifiers,
                 r = void 0 === i ? [] : i,
                 o = n.defaultOptions,
-                a = void 0 === o ? I : o;
-            return function(t, n, i) {
+                a = void 0 === o ? B : o;
+            return function(e, n, i) {
                 void 0 === i && (i = a);
                 var o, s, c = {
                         placement: "bottom",
                         orderedModifiers: [],
-                        options: Object.assign({}, I, a),
+                        options: Object.assign({}, B, a),
                         modifiersData: {},
                         elements: {
-                            reference: t,
+                            reference: e,
                             popper: n
                         },
                         attributes: {},
                         styles: {}
                     },
                     l = [],
                     d = !1,
                     p = {
                         state: c,
                         setOptions: function(i) {
                             var o = "function" == typeof i ? i(c.options) : i;
                             u(), c.options = Object.assign({}, a, c.options, o), c.scrollParents = {
-                                reference: e(t) ? x(t) : t.contextElement ? x(t.contextElement) : [],
-                                popper: x(n)
+                                reference: t(e) ? E(e) : e.contextElement ? E(e.contextElement) : [],
+                                popper: E(n)
                             };
-                            var s, d, f = function(t) {
-                                var e = B(t);
-                                return W.reduce((function(t, n) {
-                                    return t.concat(e.filter((function(t) {
-                                        return t.phase === n
+                            var s, d, f = function(e) {
+                                var t = W(e);
+                                return N.reduce((function(e, n) {
+                                    return e.concat(t.filter((function(e) {
+                                        return e.phase === n
                                     })))
                                 }), [])
-                            }((s = [].concat(r, c.options.modifiers), d = s.reduce((function(t, e) {
-                                var n = t[e.name];
-                                return t[e.name] = n ? Object.assign({}, n, e, {
-                                    options: Object.assign({}, n.options, e.options),
-                                    data: Object.assign({}, n.data, e.data)
-                                }) : e, t
-                            }), {}), Object.keys(d).map((function(t) {
-                                return d[t]
+                            }((s = [].concat(r, c.options.modifiers), d = s.reduce((function(e, t) {
+                                var n = e[t.name];
+                                return e[t.name] = n ? Object.assign({}, n, t, {
+                                    options: Object.assign({}, n.options, t.options),
+                                    data: Object.assign({}, n.data, t.data)
+                                }) : t, e
+                            }), {}), Object.keys(d).map((function(e) {
+                                return d[e]
                             }))));
-                            return c.orderedModifiers = f.filter((function(t) {
-                                return t.enabled
-                            })), c.orderedModifiers.forEach((function(t) {
-                                var e = t.name,
-                                    n = t.options,
+                            return c.orderedModifiers = f.filter((function(e) {
+                                return e.enabled
+                            })), c.orderedModifiers.forEach((function(e) {
+                                var t = e.name,
+                                    n = e.options,
                                     i = void 0 === n ? {} : n,
-                                    r = t.effect;
+                                    r = e.effect;
                                 if ("function" == typeof r) {
                                     var o = r({
                                         state: c,
-                                        name: e,
+                                        name: t,
                                         instance: p,
                                         options: i
                                     });
                                     l.push(o || function() {})
                                 }
                             })), p.update()
                         },
                         forceUpdate: function() {
                             if (!d) {
-                                var t = c.elements,
-                                    e = t.reference,
-                                    n = t.popper;
-                                if (_(e, n)) {
+                                var e = c.elements,
+                                    t = e.reference,
+                                    n = e.popper;
+                                if (_(t, n)) {
                                     c.rects = {
-                                        reference: g(e, L(n), "fixed" === c.options.strategy),
+                                        reference: g(t, L(n), "fixed" === c.options.strategy),
                                         popper: w(n)
-                                    }, c.reset = !1, c.placement = c.options.placement, c.orderedModifiers.forEach((function(t) {
-                                        return c.modifiersData[t.name] = Object.assign({}, t.data)
+                                    }, c.reset = !1, c.placement = c.options.placement, c.orderedModifiers.forEach((function(e) {
+                                        return c.modifiersData[e.name] = Object.assign({}, e.data)
                                     }));
                                     for (var i = 0; i < c.orderedModifiers.length; i++)
                                         if (!0 !== c.reset) {
                                             var r = c.orderedModifiers[i],
                                                 o = r.fn,
                                                 a = r.options,
                                                 s = void 0 === a ? {} : a,
@@ -514,907 +514,907 @@
                                                 instance: p
                                             }) || c)
                                         } else c.reset = !1, i = -1
                                 }
                             }
                         },
                         update: (o = function() {
-                            return new Promise((function(t) {
-                                p.forceUpdate(), t(c)
+                            return new Promise((function(e) {
+                                p.forceUpdate(), e(c)
                             }))
                         }, function() {
-                            return s || (s = new Promise((function(t) {
+                            return s || (s = new Promise((function(e) {
                                 Promise.resolve().then((function() {
-                                    s = void 0, t(o())
+                                    s = void 0, e(o())
                                 }))
                             }))), s
                         }),
                         destroy: function() {
                             u(), d = !0
                         }
                     };
-                if (!_(t, n)) return p;
+                if (!_(e, n)) return p;
 
                 function u() {
-                    l.forEach((function(t) {
-                        return t()
+                    l.forEach((function(e) {
+                        return e()
                     })), l = []
                 }
-                return p.setOptions(i).then((function(t) {
-                    !d && i.onFirstUpdate && i.onFirstUpdate(t)
+                return p.setOptions(i).then((function(e) {
+                    !d && i.onFirstUpdate && i.onFirstUpdate(e)
                 })), p
             }
         }
         var q = {
             passive: !0
         };
         const V = {
             name: "eventListeners",
             enabled: !0,
             phase: "write",
             fn: function() {},
-            effect: function(e) {
-                var n = e.state,
-                    i = e.instance,
-                    r = e.options,
+            effect: function(t) {
+                var n = t.state,
+                    i = t.instance,
+                    r = t.options,
                     o = r.scroll,
                     a = void 0 === o || o,
                     s = r.resize,
                     c = void 0 === s || s,
-                    l = t(n.elements.popper),
+                    l = e(n.elements.popper),
                     d = [].concat(n.scrollParents.reference, n.scrollParents.popper);
-                return a && d.forEach((function(t) {
-                        t.addEventListener("scroll", i.update, q)
+                return a && d.forEach((function(e) {
+                        e.addEventListener("scroll", i.update, q)
                     })), c && l.addEventListener("resize", i.update, q),
                     function() {
-                        a && d.forEach((function(t) {
-                            t.removeEventListener("scroll", i.update, q)
+                        a && d.forEach((function(e) {
+                            e.removeEventListener("scroll", i.update, q)
                         })), c && l.removeEventListener("resize", i.update, q)
                     }
             },
             data: {}
         };
 
-        function U(t) {
-            return t.split("-")[0]
+        function U(e) {
+            return e.split("-")[0]
         }
 
-        function $(t) {
-            return t.split("-")[1]
+        function $(e) {
+            return e.split("-")[1]
         }
 
-        function z(t) {
-            return ["top", "bottom"].indexOf(t) >= 0 ? "x" : "y"
+        function z(e) {
+            return ["top", "bottom"].indexOf(e) >= 0 ? "x" : "y"
         }
 
-        function X(t) {
-            var e, n = t.reference,
-                i = t.element,
-                r = t.placement,
+        function X(e) {
+            var t, n = e.reference,
+                i = e.element,
+                r = e.placement,
                 o = r ? U(r) : null,
                 a = r ? $(r) : null,
                 s = n.x + n.width / 2 - i.width / 2,
                 c = n.y + n.height / 2 - i.height / 2;
             switch (o) {
-                case A:
-                    e = {
+                case T:
+                    t = {
                         x: s,
                         y: n.y - i.height
                     };
                     break;
-                case T:
-                    e = {
+                case A:
+                    t = {
                         x: s,
                         y: n.y + n.height
                     };
                     break;
                 case C:
-                    e = {
+                    t = {
                         x: n.x + n.width,
                         y: c
                     };
                     break;
-                case M:
-                    e = {
+                case S:
+                    t = {
                         x: n.x - i.width,
                         y: c
                     };
                     break;
                 default:
-                    e = {
+                    t = {
                         x: n.x,
                         y: n.y
                     }
             }
             var l = o ? z(o) : null;
             if (null != l) {
                 var d = "y" === l ? "height" : "width";
                 switch (a) {
-                    case k:
-                        e[l] = e[l] - (n[d] / 2 - i[d] / 2);
+                    case R:
+                        t[l] = t[l] - (n[d] / 2 - i[d] / 2);
                         break;
                     case j:
-                        e[l] = e[l] + (n[d] / 2 - i[d] / 2)
+                        t[l] = t[l] + (n[d] / 2 - i[d] / 2)
                 }
             }
-            return e
+            return t
         }
         var Y = {
             top: "auto",
             right: "auto",
             bottom: "auto",
             left: "auto"
         };
 
-        function G(e) {
-            var n, i = e.popper,
-                r = e.popperRect,
-                o = e.placement,
-                a = e.variation,
-                c = e.offsets,
-                l = e.position,
-                d = e.gpuAcceleration,
-                p = e.adaptive,
-                u = e.roundOffsets,
-                h = e.isFixed,
+        function G(t) {
+            var n, i = t.popper,
+                r = t.popperRect,
+                o = t.placement,
+                a = t.variation,
+                c = t.offsets,
+                l = t.position,
+                d = t.gpuAcceleration,
+                p = t.adaptive,
+                u = t.roundOffsets,
+                h = t.isFixed,
                 v = c.x,
                 g = void 0 === v ? 0 : v,
                 w = c.y,
                 y = void 0 === w ? 0 : w,
                 b = "function" == typeof u ? u({
                     x: g,
                     y
                 }) : {
                     x: g,
                     y
                 };
             g = b.x, y = b.y;
-            var x = c.hasOwnProperty("x"),
-                E = c.hasOwnProperty("y"),
-                O = M,
-                S = A,
-                D = window;
+            var E = c.hasOwnProperty("x"),
+                x = c.hasOwnProperty("y"),
+                O = S,
+                D = T,
+                M = window;
             if (p) {
-                var k = L(i),
-                    P = "clientHeight",
-                    N = "clientWidth";
-                k === t(i) && "static" !== m(k = f(i)).position && "absolute" === l && (P = "scrollHeight", N = "scrollWidth"), (o === A || (o === M || o === C) && a === j) && (S = T, y -= (h && k === D && D.visualViewport ? D.visualViewport.height : k[P]) - r.height, y *= d ? 1 : -1), o !== M && (o !== A && o !== T || a !== j) || (O = C, g -= (h && k === D && D.visualViewport ? D.visualViewport.width : k[N]) - r.width, g *= d ? 1 : -1)
+                var R = L(i),
+                    I = "clientHeight",
+                    k = "clientWidth";
+                R === e(i) && "static" !== m(R = f(i)).position && "absolute" === l && (I = "scrollHeight", k = "scrollWidth"), (o === T || (o === S || o === C) && a === j) && (D = A, y -= (h && R === M && M.visualViewport ? M.visualViewport.height : R[I]) - r.height, y *= d ? 1 : -1), o !== S && (o !== T && o !== A || a !== j) || (O = C, g -= (h && R === M && M.visualViewport ? M.visualViewport.width : R[k]) - r.width, g *= d ? 1 : -1)
             }
-            var H, R = Object.assign({
+            var P, H = Object.assign({
                     position: l
                 }, p && Y),
-                W = !0 === u ? function(t, e) {
-                    var n = t.x,
-                        i = t.y,
-                        r = e.devicePixelRatio || 1;
+                N = !0 === u ? function(e, t) {
+                    var n = e.x,
+                        i = e.y,
+                        r = t.devicePixelRatio || 1;
                     return {
                         x: s(n * r) / r || 0,
                         y: s(i * r) / r || 0
                     }
                 }({
                     x: g,
                     y
-                }, t(i)) : {
+                }, e(i)) : {
                     x: g,
                     y
                 };
-            return g = W.x, y = W.y, d ? Object.assign({}, R, ((H = {})[S] = E ? "0" : "", H[O] = x ? "0" : "", H.transform = (D.devicePixelRatio || 1) <= 1 ? "translate(" + g + "px, " + y + "px)" : "translate3d(" + g + "px, " + y + "px, 0)", H)) : Object.assign({}, R, ((n = {})[S] = E ? y + "px" : "", n[O] = x ? g + "px" : "", n.transform = "", n))
+            return g = N.x, y = N.y, d ? Object.assign({}, H, ((P = {})[D] = x ? "0" : "", P[O] = E ? "0" : "", P.transform = (M.devicePixelRatio || 1) <= 1 ? "translate(" + g + "px, " + y + "px)" : "translate3d(" + g + "px, " + y + "px, 0)", P)) : Object.assign({}, H, ((n = {})[D] = x ? y + "px" : "", n[O] = E ? g + "px" : "", n.transform = "", n))
         }
         const J = {
                 name: "computeStyles",
                 enabled: !0,
                 phase: "beforeWrite",
-                fn: function(t) {
-                    var e = t.state,
-                        n = t.options,
+                fn: function(e) {
+                    var t = e.state,
+                        n = e.options,
                         i = n.gpuAcceleration,
                         r = void 0 === i || i,
                         o = n.adaptive,
                         a = void 0 === o || o,
                         s = n.roundOffsets,
                         c = void 0 === s || s,
                         l = {
-                            placement: U(e.placement),
-                            variation: $(e.placement),
-                            popper: e.elements.popper,
-                            popperRect: e.rects.popper,
+                            placement: U(t.placement),
+                            variation: $(t.placement),
+                            popper: t.elements.popper,
+                            popperRect: t.rects.popper,
                             gpuAcceleration: r,
-                            isFixed: "fixed" === e.options.strategy
+                            isFixed: "fixed" === t.options.strategy
                         };
-                    null != e.modifiersData.popperOffsets && (e.styles.popper = Object.assign({}, e.styles.popper, G(Object.assign({}, l, {
-                        offsets: e.modifiersData.popperOffsets,
-                        position: e.options.strategy,
+                    null != t.modifiersData.popperOffsets && (t.styles.popper = Object.assign({}, t.styles.popper, G(Object.assign({}, l, {
+                        offsets: t.modifiersData.popperOffsets,
+                        position: t.options.strategy,
                         adaptive: a,
                         roundOffsets: c
-                    })))), null != e.modifiersData.arrow && (e.styles.arrow = Object.assign({}, e.styles.arrow, G(Object.assign({}, l, {
-                        offsets: e.modifiersData.arrow,
+                    })))), null != t.modifiersData.arrow && (t.styles.arrow = Object.assign({}, t.styles.arrow, G(Object.assign({}, l, {
+                        offsets: t.modifiersData.arrow,
                         position: "absolute",
                         adaptive: !1,
                         roundOffsets: c
-                    })))), e.attributes.popper = Object.assign({}, e.attributes.popper, {
-                        "data-popper-placement": e.placement
+                    })))), t.attributes.popper = Object.assign({}, t.attributes.popper, {
+                        "data-popper-placement": t.placement
                     })
                 },
                 data: {}
             },
             K = {
                 name: "applyStyles",
                 enabled: !0,
                 phase: "write",
-                fn: function(t) {
-                    var e = t.state;
-                    Object.keys(e.elements).forEach((function(t) {
-                        var n = e.styles[t] || {},
-                            r = e.attributes[t] || {},
-                            o = e.elements[t];
-                        i(o) && u(o) && (Object.assign(o.style, n), Object.keys(r).forEach((function(t) {
-                            var e = r[t];
-                            !1 === e ? o.removeAttribute(t) : o.setAttribute(t, !0 === e ? "" : e)
+                fn: function(e) {
+                    var t = e.state;
+                    Object.keys(t.elements).forEach((function(e) {
+                        var n = t.styles[e] || {},
+                            r = t.attributes[e] || {},
+                            o = t.elements[e];
+                        i(o) && u(o) && (Object.assign(o.style, n), Object.keys(r).forEach((function(e) {
+                            var t = r[e];
+                            !1 === t ? o.removeAttribute(e) : o.setAttribute(e, !0 === t ? "" : t)
                         })))
                     }))
                 },
-                effect: function(t) {
-                    var e = t.state,
+                effect: function(e) {
+                    var t = e.state,
                         n = {
                             popper: {
-                                position: e.options.strategy,
+                                position: t.options.strategy,
                                 left: "0",
                                 top: "0",
                                 margin: "0"
                             },
                             arrow: {
                                 position: "absolute"
                             },
                             reference: {}
                         };
-                    return Object.assign(e.elements.popper.style, n.popper), e.styles = n, e.elements.arrow && Object.assign(e.elements.arrow.style, n.arrow),
+                    return Object.assign(t.elements.popper.style, n.popper), t.styles = n, t.elements.arrow && Object.assign(t.elements.arrow.style, n.arrow),
                         function() {
-                            Object.keys(e.elements).forEach((function(t) {
-                                var r = e.elements[t],
-                                    o = e.attributes[t] || {},
-                                    a = Object.keys(e.styles.hasOwnProperty(t) ? e.styles[t] : n[t]).reduce((function(t, e) {
-                                        return t[e] = "", t
+                            Object.keys(t.elements).forEach((function(e) {
+                                var r = t.elements[e],
+                                    o = t.attributes[e] || {},
+                                    a = Object.keys(t.styles.hasOwnProperty(e) ? t.styles[e] : n[e]).reduce((function(e, t) {
+                                        return e[t] = "", e
                                     }), {});
-                                i(r) && u(r) && (Object.assign(r.style, a), Object.keys(o).forEach((function(t) {
-                                    r.removeAttribute(t)
+                                i(r) && u(r) && (Object.assign(r.style, a), Object.keys(o).forEach((function(e) {
+                                    r.removeAttribute(e)
                                 })))
                             }))
                         }
                 },
                 requires: ["computeStyles"]
             },
             Q = {
                 name: "offset",
                 enabled: !0,
                 phase: "main",
                 requires: ["popperOffsets"],
-                fn: function(t) {
-                    var e = t.state,
-                        n = t.options,
-                        i = t.name,
+                fn: function(e) {
+                    var t = e.state,
+                        n = e.options,
+                        i = e.name,
                         r = n.offset,
                         o = void 0 === r ? [0, 0] : r,
-                        a = R.reduce((function(t, n) {
-                            return t[n] = function(t, e, n) {
-                                var i = U(t),
-                                    r = [M, A].indexOf(i) >= 0 ? -1 : 1,
-                                    o = "function" == typeof n ? n(Object.assign({}, e, {
-                                        placement: t
+                        a = H.reduce((function(e, n) {
+                            return e[n] = function(e, t, n) {
+                                var i = U(e),
+                                    r = [S, T].indexOf(i) >= 0 ? -1 : 1,
+                                    o = "function" == typeof n ? n(Object.assign({}, t, {
+                                        placement: e
                                     })) : n,
                                     a = o[0],
                                     s = o[1];
-                                return a = a || 0, s = (s || 0) * r, [M, C].indexOf(i) >= 0 ? {
+                                return a = a || 0, s = (s || 0) * r, [S, C].indexOf(i) >= 0 ? {
                                     x: s,
                                     y: a
                                 } : {
                                     x: a,
                                     y: s
                                 }
-                            }(n, e.rects, o), t
+                            }(n, t.rects, o), e
                         }), {}),
-                        s = a[e.placement],
+                        s = a[t.placement],
                         c = s.x,
                         l = s.y;
-                    null != e.modifiersData.popperOffsets && (e.modifiersData.popperOffsets.x += c, e.modifiersData.popperOffsets.y += l), e.modifiersData[i] = a
+                    null != t.modifiersData.popperOffsets && (t.modifiersData.popperOffsets.x += c, t.modifiersData.popperOffsets.y += l), t.modifiersData[i] = a
                 }
             };
         var Z = {
             left: "right",
             right: "left",
             bottom: "top",
             top: "bottom"
         };
 
-        function tt(t) {
-            return t.replace(/left|right|bottom|top/g, (function(t) {
-                return Z[t]
+        function ee(e) {
+            return e.replace(/left|right|bottom|top/g, (function(e) {
+                return Z[e]
             }))
         }
-        var et = {
+        var te = {
             start: "end",
             end: "start"
         };
 
-        function nt(t) {
-            return t.replace(/start|end/g, (function(t) {
-                return et[t]
+        function ne(e) {
+            return e.replace(/start|end/g, (function(e) {
+                return te[e]
             }))
         }
 
-        function it(t, e) {
-            var n = e.getRootNode && e.getRootNode();
-            if (t.contains(e)) return !0;
+        function ie(e, t) {
+            var n = t.getRootNode && t.getRootNode();
+            if (e.contains(t)) return !0;
             if (n && r(n)) {
-                var i = e;
+                var i = t;
                 do {
-                    if (i && t.isSameNode(i)) return !0;
+                    if (i && e.isSameNode(i)) return !0;
                     i = i.parentNode || i.host
                 } while (i)
             }
             return !1
         }
 
-        function rt(t) {
-            return Object.assign({}, t, {
-                left: t.x,
-                top: t.y,
-                right: t.x + t.width,
-                bottom: t.y + t.height
+        function re(e) {
+            return Object.assign({}, e, {
+                left: e.x,
+                top: e.y,
+                right: e.x + e.width,
+                bottom: e.y + e.height
             })
         }
 
-        function ot(n, i, r) {
-            return i === P ? rt(function(e, n) {
-                var i = t(e),
-                    r = f(e),
+        function oe(n, i, r) {
+            return i === I ? re(function(t, n) {
+                var i = e(t),
+                    r = f(t),
                     o = i.visualViewport,
                     a = r.clientWidth,
                     s = r.clientHeight,
                     c = 0,
                     d = 0;
                 if (o) {
                     a = o.width, s = o.height;
                     var p = l();
                     (p || !p && "fixed" === n) && (c = o.offsetLeft, d = o.offsetTop)
                 }
                 return {
                     width: a,
                     height: s,
-                    x: c + h(e),
+                    x: c + h(t),
                     y: d
                 }
-            }(n, r)) : e(i) ? function(t, e) {
-                var n = d(t, !1, "fixed" === e);
-                return n.top = n.top + t.clientTop, n.left = n.left + t.clientLeft, n.bottom = n.top + t.clientHeight, n.right = n.left + t.clientWidth, n.width = t.clientWidth, n.height = t.clientHeight, n.x = n.left, n.y = n.top, n
-            }(i, r) : rt(function(t) {
-                var e, n = f(t),
-                    i = p(t),
-                    r = null == (e = t.ownerDocument) ? void 0 : e.body,
+            }(n, r)) : t(i) ? function(e, t) {
+                var n = d(e, !1, "fixed" === t);
+                return n.top = n.top + e.clientTop, n.left = n.left + e.clientLeft, n.bottom = n.top + e.clientHeight, n.right = n.left + e.clientWidth, n.width = e.clientWidth, n.height = e.clientHeight, n.x = n.left, n.y = n.top, n
+            }(i, r) : re(function(e) {
+                var t, n = f(e),
+                    i = p(e),
+                    r = null == (t = e.ownerDocument) ? void 0 : t.body,
                     a = o(n.scrollWidth, n.clientWidth, r ? r.scrollWidth : 0, r ? r.clientWidth : 0),
                     s = o(n.scrollHeight, n.clientHeight, r ? r.scrollHeight : 0, r ? r.clientHeight : 0),
-                    c = -i.scrollLeft + h(t),
+                    c = -i.scrollLeft + h(e),
                     l = -i.scrollTop;
                 return "rtl" === m(r || n).direction && (c += o(n.clientWidth, r ? r.clientWidth : 0) - a), {
                     width: a,
                     height: s,
                     x: c,
                     y: l
                 }
             }(f(n)))
         }
 
-        function at(t) {
+        function ae(e) {
             return Object.assign({}, {
                 top: 0,
                 right: 0,
                 bottom: 0,
                 left: 0
-            }, t)
+            }, e)
         }
 
-        function st(t, e) {
-            return e.reduce((function(e, n) {
-                return e[n] = t, e
+        function se(e, t) {
+            return t.reduce((function(t, n) {
+                return t[n] = e, t
             }), {})
         }
 
-        function ct(t, n) {
+        function ce(e, n) {
             void 0 === n && (n = {});
             var r = n,
                 s = r.placement,
-                c = void 0 === s ? t.placement : s,
+                c = void 0 === s ? e.placement : s,
                 l = r.strategy,
-                p = void 0 === l ? t.strategy : l,
+                p = void 0 === l ? e.strategy : l,
                 h = r.boundary,
                 v = void 0 === h ? "clippingParents" : h,
                 g = r.rootBoundary,
-                w = void 0 === g ? P : g,
+                w = void 0 === g ? I : g,
                 b = r.elementContext,
-                E = void 0 === b ? N : b,
+                x = void 0 === b ? k : b,
                 O = r.altBoundary,
-                M = void 0 !== O && O,
-                S = r.padding,
-                k = void 0 === S ? 0 : S,
-                j = at("number" != typeof k ? k : st(k, D)),
-                H = E === N ? "reference" : N,
-                R = t.rects.popper,
-                W = t.elements[M ? H : E],
-                B = function(t, n, r, s) {
-                    var c = "clippingParents" === n ? function(t) {
-                            var n = x(y(t)),
-                                r = ["absolute", "fixed"].indexOf(m(t).position) >= 0 && i(t) ? L(t) : t;
-                            return e(r) ? n.filter((function(t) {
-                                return e(t) && it(t, r) && "body" !== u(t)
+                S = void 0 !== O && O,
+                D = r.padding,
+                R = void 0 === D ? 0 : D,
+                j = ae("number" != typeof R ? R : se(R, M)),
+                P = x === k ? "reference" : k,
+                H = e.rects.popper,
+                N = e.elements[S ? P : x],
+                W = function(e, n, r, s) {
+                    var c = "clippingParents" === n ? function(e) {
+                            var n = E(y(e)),
+                                r = ["absolute", "fixed"].indexOf(m(e).position) >= 0 && i(e) ? L(e) : e;
+                            return t(r) ? n.filter((function(e) {
+                                return t(e) && ie(e, r) && "body" !== u(e)
                             })) : []
-                        }(t) : [].concat(n),
+                        }(e) : [].concat(n),
                         l = [].concat(c, [r]),
                         d = l[0],
-                        p = l.reduce((function(e, n) {
-                            var i = ot(t, n, s);
-                            return e.top = o(i.top, e.top), e.right = a(i.right, e.right), e.bottom = a(i.bottom, e.bottom), e.left = o(i.left, e.left), e
-                        }), ot(t, d, s));
+                        p = l.reduce((function(t, n) {
+                            var i = oe(e, n, s);
+                            return t.top = o(i.top, t.top), t.right = a(i.right, t.right), t.bottom = a(i.bottom, t.bottom), t.left = o(i.left, t.left), t
+                        }), oe(e, d, s));
                     return p.width = p.right - p.left, p.height = p.bottom - p.top, p.x = p.left, p.y = p.top, p
-                }(e(W) ? W : W.contextElement || f(t.elements.popper), v, w, p),
-                I = d(t.elements.reference),
+                }(t(N) ? N : N.contextElement || f(e.elements.popper), v, w, p),
+                B = d(e.elements.reference),
                 _ = X({
-                    reference: I,
-                    element: R,
+                    reference: B,
+                    element: H,
                     strategy: "absolute",
                     placement: c
                 }),
-                F = rt(Object.assign({}, R, _)),
-                q = E === N ? F : I,
+                F = re(Object.assign({}, H, _)),
+                q = x === k ? F : B,
                 V = {
-                    top: B.top - q.top + j.top,
-                    bottom: q.bottom - B.bottom + j.bottom,
-                    left: B.left - q.left + j.left,
-                    right: q.right - B.right + j.right
+                    top: W.top - q.top + j.top,
+                    bottom: q.bottom - W.bottom + j.bottom,
+                    left: W.left - q.left + j.left,
+                    right: q.right - W.right + j.right
                 },
-                U = t.modifiersData.offset;
-            if (E === N && U) {
+                U = e.modifiersData.offset;
+            if (x === k && U) {
                 var $ = U[c];
-                Object.keys(V).forEach((function(t) {
-                    var e = [C, T].indexOf(t) >= 0 ? 1 : -1,
-                        n = [A, T].indexOf(t) >= 0 ? "y" : "x";
-                    V[t] += $[n] * e
+                Object.keys(V).forEach((function(e) {
+                    var t = [C, A].indexOf(e) >= 0 ? 1 : -1,
+                        n = [T, A].indexOf(e) >= 0 ? "y" : "x";
+                    V[e] += $[n] * t
                 }))
             }
             return V
         }
-        const lt = {
+        const le = {
             name: "flip",
             enabled: !0,
             phase: "main",
-            fn: function(t) {
-                var e = t.state,
-                    n = t.options,
-                    i = t.name;
-                if (!e.modifiersData[i]._skip) {
-                    for (var r = n.mainAxis, o = void 0 === r || r, a = n.altAxis, s = void 0 === a || a, c = n.fallbackPlacements, l = n.padding, d = n.boundary, p = n.rootBoundary, u = n.altBoundary, f = n.flipVariations, h = void 0 === f || f, m = n.allowedAutoPlacements, v = e.options.placement, g = U(v), w = c || (g !== v && h ? function(t) {
-                            if (U(t) === S) return [];
-                            var e = tt(t);
-                            return [nt(t), e, nt(e)]
-                        }(v) : [tt(v)]), y = [v].concat(w).reduce((function(t, n) {
-                            return t.concat(U(n) === S ? function(t, e) {
-                                void 0 === e && (e = {});
-                                var n = e,
+            fn: function(e) {
+                var t = e.state,
+                    n = e.options,
+                    i = e.name;
+                if (!t.modifiersData[i]._skip) {
+                    for (var r = n.mainAxis, o = void 0 === r || r, a = n.altAxis, s = void 0 === a || a, c = n.fallbackPlacements, l = n.padding, d = n.boundary, p = n.rootBoundary, u = n.altBoundary, f = n.flipVariations, h = void 0 === f || f, m = n.allowedAutoPlacements, v = t.options.placement, g = U(v), w = c || (g !== v && h ? function(e) {
+                            if (U(e) === D) return [];
+                            var t = ee(e);
+                            return [ne(e), t, ne(t)]
+                        }(v) : [ee(v)]), y = [v].concat(w).reduce((function(e, n) {
+                            return e.concat(U(n) === D ? function(e, t) {
+                                void 0 === t && (t = {});
+                                var n = t,
                                     i = n.placement,
                                     r = n.boundary,
                                     o = n.rootBoundary,
                                     a = n.padding,
                                     s = n.flipVariations,
                                     c = n.allowedAutoPlacements,
-                                    l = void 0 === c ? R : c,
+                                    l = void 0 === c ? H : c,
                                     d = $(i),
-                                    p = d ? s ? H : H.filter((function(t) {
-                                        return $(t) === d
-                                    })) : D,
-                                    u = p.filter((function(t) {
-                                        return l.indexOf(t) >= 0
+                                    p = d ? s ? P : P.filter((function(e) {
+                                        return $(e) === d
+                                    })) : M,
+                                    u = p.filter((function(e) {
+                                        return l.indexOf(e) >= 0
                                     }));
                                 0 === u.length && (u = p);
-                                var f = u.reduce((function(e, n) {
-                                    return e[n] = ct(t, {
+                                var f = u.reduce((function(t, n) {
+                                    return t[n] = ce(e, {
                                         placement: n,
                                         boundary: r,
                                         rootBoundary: o,
                                         padding: a
-                                    })[U(n)], e
+                                    })[U(n)], t
                                 }), {});
-                                return Object.keys(f).sort((function(t, e) {
-                                    return f[t] - f[e]
+                                return Object.keys(f).sort((function(e, t) {
+                                    return f[e] - f[t]
                                 }))
-                            }(e, {
+                            }(t, {
                                 placement: n,
                                 boundary: d,
                                 rootBoundary: p,
                                 padding: l,
                                 flipVariations: h,
                                 allowedAutoPlacements: m
                             }) : n)
-                        }), []), b = e.rects.reference, x = e.rects.popper, E = new Map, O = !0, L = y[0], j = 0; j < y.length; j++) {
-                        var P = y[j],
-                            N = U(P),
-                            W = $(P) === k,
-                            B = [A, T].indexOf(N) >= 0,
-                            I = B ? "width" : "height",
-                            _ = ct(e, {
-                                placement: P,
+                        }), []), b = t.rects.reference, E = t.rects.popper, x = new Map, O = !0, L = y[0], j = 0; j < y.length; j++) {
+                        var I = y[j],
+                            k = U(I),
+                            N = $(I) === R,
+                            W = [T, A].indexOf(k) >= 0,
+                            B = W ? "width" : "height",
+                            _ = ce(t, {
+                                placement: I,
                                 boundary: d,
                                 rootBoundary: p,
                                 altBoundary: u,
                                 padding: l
                             }),
-                            F = B ? W ? C : M : W ? T : A;
-                        b[I] > x[I] && (F = tt(F));
-                        var q = tt(F),
+                            F = W ? N ? C : S : N ? A : T;
+                        b[B] > E[B] && (F = ee(F));
+                        var q = ee(F),
                             V = [];
-                        if (o && V.push(_[N] <= 0), s && V.push(_[F] <= 0, _[q] <= 0), V.every((function(t) {
-                                return t
+                        if (o && V.push(_[k] <= 0), s && V.push(_[F] <= 0, _[q] <= 0), V.every((function(e) {
+                                return e
                             }))) {
-                            L = P, O = !1;
+                            L = I, O = !1;
                             break
                         }
-                        E.set(P, V)
+                        x.set(I, V)
                     }
                     if (O)
-                        for (var z = function(t) {
-                                var e = y.find((function(e) {
-                                    var n = E.get(e);
-                                    if (n) return n.slice(0, t).every((function(t) {
-                                        return t
+                        for (var z = function(e) {
+                                var t = y.find((function(t) {
+                                    var n = x.get(t);
+                                    if (n) return n.slice(0, e).every((function(e) {
+                                        return e
                                     }))
                                 }));
-                                if (e) return L = e, "break"
+                                if (t) return L = t, "break"
                             }, X = h ? 3 : 1; X > 0 && "break" !== z(X); X--);
-                    e.placement !== L && (e.modifiersData[i]._skip = !0, e.placement = L, e.reset = !0)
+                    t.placement !== L && (t.modifiersData[i]._skip = !0, t.placement = L, t.reset = !0)
                 }
             },
             requiresIfExists: ["offset"],
             data: {
                 _skip: !1
             }
         };
 
-        function dt(t, e, n) {
-            return o(t, a(e, n))
+        function de(e, t, n) {
+            return o(e, a(t, n))
         }
-        const pt = {
+        const pe = {
                 name: "preventOverflow",
                 enabled: !0,
                 phase: "main",
-                fn: function(t) {
-                    var e = t.state,
-                        n = t.options,
-                        i = t.name,
+                fn: function(e) {
+                    var t = e.state,
+                        n = e.options,
+                        i = e.name,
                         r = n.mainAxis,
                         s = void 0 === r || r,
                         c = n.altAxis,
                         l = void 0 !== c && c,
                         d = n.boundary,
                         p = n.rootBoundary,
                         u = n.altBoundary,
                         f = n.padding,
                         h = n.tether,
                         m = void 0 === h || h,
                         v = n.tetherOffset,
                         g = void 0 === v ? 0 : v,
-                        y = ct(e, {
+                        y = ce(t, {
                             boundary: d,
                             rootBoundary: p,
                             padding: f,
                             altBoundary: u
                         }),
-                        b = U(e.placement),
-                        x = $(e.placement),
-                        E = !x,
+                        b = U(t.placement),
+                        E = $(t.placement),
+                        x = !E,
                         O = z(b),
-                        S = "x" === O ? "y" : "x",
-                        D = e.modifiersData.popperOffsets,
-                        j = e.rects.reference,
-                        P = e.rects.popper,
-                        N = "function" == typeof g ? g(Object.assign({}, e.rects, {
-                            placement: e.placement
+                        D = "x" === O ? "y" : "x",
+                        M = t.modifiersData.popperOffsets,
+                        j = t.rects.reference,
+                        I = t.rects.popper,
+                        k = "function" == typeof g ? g(Object.assign({}, t.rects, {
+                            placement: t.placement
                         })) : g,
-                        H = "number" == typeof N ? {
-                            mainAxis: N,
-                            altAxis: N
+                        P = "number" == typeof k ? {
+                            mainAxis: k,
+                            altAxis: k
                         } : Object.assign({
                             mainAxis: 0,
                             altAxis: 0
-                        }, N),
-                        R = e.modifiersData.offset ? e.modifiersData.offset[e.placement] : null,
-                        W = {
+                        }, k),
+                        H = t.modifiersData.offset ? t.modifiersData.offset[t.placement] : null,
+                        N = {
                             x: 0,
                             y: 0
                         };
-                    if (D) {
+                    if (M) {
                         if (s) {
-                            var B, I = "y" === O ? A : M,
-                                _ = "y" === O ? T : C,
+                            var W, B = "y" === O ? T : S,
+                                _ = "y" === O ? A : C,
                                 F = "y" === O ? "height" : "width",
-                                q = D[O],
-                                V = q + y[I],
+                                q = M[O],
+                                V = q + y[B],
                                 X = q - y[_],
-                                Y = m ? -P[F] / 2 : 0,
-                                G = x === k ? j[F] : P[F],
-                                J = x === k ? -P[F] : -j[F],
-                                K = e.elements.arrow,
+                                Y = m ? -I[F] / 2 : 0,
+                                G = E === R ? j[F] : I[F],
+                                J = E === R ? -I[F] : -j[F],
+                                K = t.elements.arrow,
                                 Q = m && K ? w(K) : {
                                     width: 0,
                                     height: 0
                                 },
-                                Z = e.modifiersData["arrow#persistent"] ? e.modifiersData["arrow#persistent"].padding : {
+                                Z = t.modifiersData["arrow#persistent"] ? t.modifiersData["arrow#persistent"].padding : {
                                     top: 0,
                                     right: 0,
                                     bottom: 0,
                                     left: 0
                                 },
-                                tt = Z[I],
-                                et = Z[_],
-                                nt = dt(0, j[F], Q[F]),
-                                it = E ? j[F] / 2 - Y - nt - tt - H.mainAxis : G - nt - tt - H.mainAxis,
-                                rt = E ? -j[F] / 2 + Y + nt + et + H.mainAxis : J + nt + et + H.mainAxis,
-                                ot = e.elements.arrow && L(e.elements.arrow),
-                                at = ot ? "y" === O ? ot.clientTop || 0 : ot.clientLeft || 0 : 0,
-                                st = null != (B = null == R ? void 0 : R[O]) ? B : 0,
-                                lt = q + rt - st,
-                                pt = dt(m ? a(V, q + it - st - at) : V, q, m ? o(X, lt) : X);
-                            D[O] = pt, W[O] = pt - q
+                                ee = Z[B],
+                                te = Z[_],
+                                ne = de(0, j[F], Q[F]),
+                                ie = x ? j[F] / 2 - Y - ne - ee - P.mainAxis : G - ne - ee - P.mainAxis,
+                                re = x ? -j[F] / 2 + Y + ne + te + P.mainAxis : J + ne + te + P.mainAxis,
+                                oe = t.elements.arrow && L(t.elements.arrow),
+                                ae = oe ? "y" === O ? oe.clientTop || 0 : oe.clientLeft || 0 : 0,
+                                se = null != (W = null == H ? void 0 : H[O]) ? W : 0,
+                                le = q + re - se,
+                                pe = de(m ? a(V, q + ie - se - ae) : V, q, m ? o(X, le) : X);
+                            M[O] = pe, N[O] = pe - q
                         }
                         if (l) {
-                            var ut, ft = "x" === O ? A : M,
-                                ht = "x" === O ? T : C,
-                                mt = D[S],
-                                vt = "y" === S ? "height" : "width",
-                                gt = mt + y[ft],
-                                wt = mt - y[ht],
-                                yt = -1 !== [A, M].indexOf(b),
-                                bt = null != (ut = null == R ? void 0 : R[S]) ? ut : 0,
-                                xt = yt ? gt : mt - j[vt] - P[vt] - bt + H.altAxis,
-                                Et = yt ? mt + j[vt] + P[vt] - bt - H.altAxis : wt,
-                                Ot = m && yt ? function(t, e, n) {
-                                    var i = dt(t, e, n);
+                            var ue, fe = "x" === O ? T : S,
+                                he = "x" === O ? A : C,
+                                me = M[D],
+                                ve = "y" === D ? "height" : "width",
+                                ge = me + y[fe],
+                                we = me - y[he],
+                                ye = -1 !== [T, S].indexOf(b),
+                                be = null != (ue = null == H ? void 0 : H[D]) ? ue : 0,
+                                Ee = ye ? ge : me - j[ve] - I[ve] - be + P.altAxis,
+                                xe = ye ? me + j[ve] + I[ve] - be - P.altAxis : we,
+                                Oe = m && ye ? function(e, t, n) {
+                                    var i = de(e, t, n);
                                     return i > n ? n : i
-                                }(xt, mt, Et) : dt(m ? xt : gt, mt, m ? Et : wt);
-                            D[S] = Ot, W[S] = Ot - mt
+                                }(Ee, me, xe) : de(m ? Ee : ge, me, m ? xe : we);
+                            M[D] = Oe, N[D] = Oe - me
                         }
-                        e.modifiersData[i] = W
+                        t.modifiersData[i] = N
                     }
                 },
                 requiresIfExists: ["offset"]
             },
-            ut = {
+            ue = {
                 name: "arrow",
                 enabled: !0,
                 phase: "main",
-                fn: function(t) {
-                    var e, n = t.state,
-                        i = t.name,
-                        r = t.options,
+                fn: function(e) {
+                    var t, n = e.state,
+                        i = e.name,
+                        r = e.options,
                         o = n.elements.arrow,
                         a = n.modifiersData.popperOffsets,
                         s = U(n.placement),
                         c = z(s),
-                        l = [M, C].indexOf(s) >= 0 ? "height" : "width";
+                        l = [S, C].indexOf(s) >= 0 ? "height" : "width";
                     if (o && a) {
-                        var d = function(t, e) {
-                                return at("number" != typeof(t = "function" == typeof t ? t(Object.assign({}, e.rects, {
-                                    placement: e.placement
-                                })) : t) ? t : st(t, D))
+                        var d = function(e, t) {
+                                return ae("number" != typeof(e = "function" == typeof e ? e(Object.assign({}, t.rects, {
+                                    placement: t.placement
+                                })) : e) ? e : se(e, M))
                             }(r.padding, n),
                             p = w(o),
-                            u = "y" === c ? A : M,
-                            f = "y" === c ? T : C,
+                            u = "y" === c ? T : S,
+                            f = "y" === c ? A : C,
                             h = n.rects.reference[l] + n.rects.reference[c] - a[c] - n.rects.popper[l],
                             m = a[c] - n.rects.reference[c],
                             v = L(o),
                             g = v ? "y" === c ? v.clientHeight || 0 : v.clientWidth || 0 : 0,
                             y = h / 2 - m / 2,
                             b = d[u],
-                            x = g - p[l] - d[f],
-                            E = g / 2 - p[l] / 2 + y,
-                            O = dt(b, E, x),
-                            S = c;
-                        n.modifiersData[i] = ((e = {})[S] = O, e.centerOffset = O - E, e)
+                            E = g - p[l] - d[f],
+                            x = g / 2 - p[l] / 2 + y,
+                            O = de(b, x, E),
+                            D = c;
+                        n.modifiersData[i] = ((t = {})[D] = O, t.centerOffset = O - x, t)
                     }
                 },
-                effect: function(t) {
-                    var e = t.state,
-                        n = t.options.element,
+                effect: function(e) {
+                    var t = e.state,
+                        n = e.options.element,
                         i = void 0 === n ? "[data-popper-arrow]" : n;
-                    null != i && ("string" != typeof i || (i = e.elements.popper.querySelector(i))) && it(e.elements.popper, i) && (e.elements.arrow = i)
+                    null != i && ("string" != typeof i || (i = t.elements.popper.querySelector(i))) && ie(t.elements.popper, i) && (t.elements.arrow = i)
                 },
                 requires: ["popperOffsets"],
                 requiresIfExists: ["preventOverflow"]
             };
 
-        function ft(t, e, n) {
+        function fe(e, t, n) {
             return void 0 === n && (n = {
                 x: 0,
                 y: 0
             }), {
-                top: t.top - e.height - n.y,
-                right: t.right - e.width + n.x,
-                bottom: t.bottom - e.height + n.y,
-                left: t.left - e.width - n.x
+                top: e.top - t.height - n.y,
+                right: e.right - t.width + n.x,
+                bottom: e.bottom - t.height + n.y,
+                left: e.left - t.width - n.x
             }
         }
 
-        function ht(t) {
-            return [A, C, T, M].some((function(e) {
-                return t[e] >= 0
+        function he(e) {
+            return [T, C, A, S].some((function(t) {
+                return e[t] >= 0
             }))
         }
-        var mt = F({
+        var me = F({
                 defaultModifiers: [V, {
                     name: "popperOffsets",
                     enabled: !0,
                     phase: "read",
-                    fn: function(t) {
-                        var e = t.state,
-                            n = t.name;
-                        e.modifiersData[n] = X({
-                            reference: e.rects.reference,
-                            element: e.rects.popper,
+                    fn: function(e) {
+                        var t = e.state,
+                            n = e.name;
+                        t.modifiersData[n] = X({
+                            reference: t.rects.reference,
+                            element: t.rects.popper,
                             strategy: "absolute",
-                            placement: e.placement
+                            placement: t.placement
                         })
                     },
                     data: {}
-                }, J, K, Q, lt, pt, ut, {
+                }, J, K, Q, le, pe, ue, {
                     name: "hide",
                     enabled: !0,
                     phase: "main",
                     requiresIfExists: ["preventOverflow"],
-                    fn: function(t) {
-                        var e = t.state,
-                            n = t.name,
-                            i = e.rects.reference,
-                            r = e.rects.popper,
-                            o = e.modifiersData.preventOverflow,
-                            a = ct(e, {
+                    fn: function(e) {
+                        var t = e.state,
+                            n = e.name,
+                            i = t.rects.reference,
+                            r = t.rects.popper,
+                            o = t.modifiersData.preventOverflow,
+                            a = ce(t, {
                                 elementContext: "reference"
                             }),
-                            s = ct(e, {
+                            s = ce(t, {
                                 altBoundary: !0
                             }),
-                            c = ft(a, i),
-                            l = ft(s, r, o),
-                            d = ht(c),
-                            p = ht(l);
-                        e.modifiersData[n] = {
+                            c = fe(a, i),
+                            l = fe(s, r, o),
+                            d = he(c),
+                            p = he(l);
+                        t.modifiersData[n] = {
                             referenceClippingOffsets: c,
                             popperEscapeOffsets: l,
                             isReferenceHidden: d,
                             hasPopperEscaped: p
-                        }, e.attributes.popper = Object.assign({}, e.attributes.popper, {
+                        }, t.attributes.popper = Object.assign({}, t.attributes.popper, {
                             "data-popper-reference-hidden": d,
                             "data-popper-escaped": p
                         })
                     }
                 }]
             }),
-            vt = "tippy-content",
-            gt = "tippy-backdrop",
-            wt = "tippy-arrow",
-            yt = "tippy-svg-arrow",
-            bt = {
+            ve = "tippy-content",
+            ge = "tippy-backdrop",
+            we = "tippy-arrow",
+            ye = "tippy-svg-arrow",
+            be = {
                 passive: !0,
                 capture: !0
             },
-            xt = function() {
+            Ee = function() {
                 return document.body
             };
 
-        function Et(t, e, n) {
-            if (Array.isArray(t)) {
-                var i = t[e];
-                return null == i ? Array.isArray(n) ? n[e] : n : i
+        function xe(e, t, n) {
+            if (Array.isArray(e)) {
+                var i = e[t];
+                return null == i ? Array.isArray(n) ? n[t] : n : i
             }
-            return t
+            return e
         }
 
-        function Ot(t, e) {
-            var n = {}.toString.call(t);
-            return 0 === n.indexOf("[object") && n.indexOf(e + "]") > -1
+        function Oe(e, t) {
+            var n = {}.toString.call(e);
+            return 0 === n.indexOf("[object") && n.indexOf(t + "]") > -1
         }
 
-        function Lt(t, e) {
-            return "function" == typeof t ? t.apply(void 0, e) : t
+        function Le(e, t) {
+            return "function" == typeof e ? e.apply(void 0, t) : e
         }
 
-        function At(t, e) {
-            return 0 === e ? t : function(i) {
+        function Te(e, t) {
+            return 0 === t ? e : function(i) {
                 clearTimeout(n), n = setTimeout((function() {
-                    t(i)
-                }), e)
+                    e(i)
+                }), t)
             };
             var n
         }
 
-        function Tt(t) {
-            return [].concat(t)
+        function Ae(e) {
+            return [].concat(e)
         }
 
-        function Ct(t, e) {
-            -1 === t.indexOf(e) && t.push(e)
+        function Ce(e, t) {
+            -1 === e.indexOf(t) && e.push(t)
         }
 
-        function Mt(t) {
-            return [].slice.call(t)
+        function Se(e) {
+            return [].slice.call(e)
         }
 
-        function St(t) {
-            return Object.keys(t).reduce((function(e, n) {
-                return void 0 !== t[n] && (e[n] = t[n]), e
+        function De(e) {
+            return Object.keys(e).reduce((function(t, n) {
+                return void 0 !== e[n] && (t[n] = e[n]), t
             }), {})
         }
 
-        function Dt() {
+        function Me() {
             return document.createElement("div")
         }
 
-        function kt(t) {
-            return ["Element", "Fragment"].some((function(e) {
-                return Ot(t, e)
+        function Re(e) {
+            return ["Element", "Fragment"].some((function(t) {
+                return Oe(e, t)
             }))
         }
 
-        function jt(t, e) {
-            t.forEach((function(t) {
-                t && (t.style.transitionDuration = e + "ms")
+        function je(e, t) {
+            e.forEach((function(e) {
+                e && (e.style.transitionDuration = t + "ms")
             }))
         }
 
-        function Pt(t, e) {
-            t.forEach((function(t) {
-                t && t.setAttribute("data-state", e)
+        function Ie(e, t) {
+            e.forEach((function(e) {
+                e && e.setAttribute("data-state", t)
             }))
         }
 
-        function Nt(t, e, n) {
-            var i = e + "EventListener";
-            ["transitionend", "webkitTransitionEnd"].forEach((function(e) {
-                t[i](e, n)
+        function ke(e, t, n) {
+            var i = t + "EventListener";
+            ["transitionend", "webkitTransitionEnd"].forEach((function(t) {
+                e[i](t, n)
             }))
         }
 
-        function Ht(t, e) {
-            for (var n = e; n;) {
+        function Pe(e, t) {
+            for (var n = t; n;) {
                 var i;
-                if (t.contains(n)) return !0;
+                if (e.contains(n)) return !0;
                 n = null == n.getRootNode || null == (i = n.getRootNode()) ? void 0 : i.host
             }
             return !1
         }
-        var Rt = {
+        var He = {
                 isTouch: !1
             },
-            Wt = 0;
+            Ne = 0;
 
-        function Bt() {
-            Rt.isTouch || (Rt.isTouch = !0, window.performance && document.addEventListener("mousemove", It))
+        function We() {
+            He.isTouch || (He.isTouch = !0, window.performance && document.addEventListener("mousemove", Be))
         }
 
-        function It() {
-            var t = performance.now();
-            t - Wt < 20 && (Rt.isTouch = !1, document.removeEventListener("mousemove", It)), Wt = t
+        function Be() {
+            var e = performance.now();
+            e - Ne < 20 && (He.isTouch = !1, document.removeEventListener("mousemove", Be)), Ne = e
         }
 
-        function _t() {
-            var t, e = document.activeElement;
-            if ((t = e) && t._tippy && t._tippy.reference === t) {
-                var n = e._tippy;
-                e.blur && !n.state.isVisible && e.blur()
+        function _e() {
+            var e, t = document.activeElement;
+            if ((e = t) && e._tippy && e._tippy.reference === e) {
+                var n = t._tippy;
+                t.blur && !n.state.isVisible && t.blur()
             }
         }
-        var Ft = !("undefined" == typeof window || "undefined" == typeof document || !window.msCrypto),
-            qt = Object.assign({
-                appendTo: xt,
+        var Fe = !("undefined" == typeof window || "undefined" == typeof document || !window.msCrypto),
+            qe = Object.assign({
+                appendTo: Ee,
                 aria: {
                     content: "auto",
                     expanded: "auto"
                 },
                 delay: 0,
                 duration: [300, 250],
                 getReferenceClientRect: null,
@@ -1457,464 +1457,464 @@
                 content: "",
                 inertia: !1,
                 maxWidth: 350,
                 role: "tooltip",
                 theme: "",
                 zIndex: 9999
             }),
-            Vt = Object.keys(qt);
+            Ve = Object.keys(qe);
 
-        function Ut(t) {
-            var e = (t.plugins || []).reduce((function(e, n) {
+        function Ue(e) {
+            var t = (e.plugins || []).reduce((function(t, n) {
                 var i, r = n.name,
                     o = n.defaultValue;
-                return r && (e[r] = void 0 !== t[r] ? t[r] : null != (i = qt[r]) ? i : o), e
+                return r && (t[r] = void 0 !== e[r] ? e[r] : null != (i = qe[r]) ? i : o), t
             }), {});
-            return Object.assign({}, t, e)
+            return Object.assign({}, e, t)
         }
 
-        function $t(t, e) {
-            var n = Object.assign({}, e, {
-                content: Lt(e.content, [t])
-            }, e.ignoreAttributes ? {} : function(t, e) {
-                return (e ? Object.keys(Ut(Object.assign({}, qt, {
-                    plugins: e
-                }))) : Vt).reduce((function(e, n) {
-                    var i = (t.getAttribute("data-tippy-" + n) || "").trim();
-                    if (!i) return e;
-                    if ("content" === n) e[n] = i;
+        function $e(e, t) {
+            var n = Object.assign({}, t, {
+                content: Le(t.content, [e])
+            }, t.ignoreAttributes ? {} : function(e, t) {
+                return (t ? Object.keys(Ue(Object.assign({}, qe, {
+                    plugins: t
+                }))) : Ve).reduce((function(t, n) {
+                    var i = (e.getAttribute("data-tippy-" + n) || "").trim();
+                    if (!i) return t;
+                    if ("content" === n) t[n] = i;
                     else try {
-                        e[n] = JSON.parse(i)
-                    } catch (t) {
-                        e[n] = i
+                        t[n] = JSON.parse(i)
+                    } catch (e) {
+                        t[n] = i
                     }
-                    return e
+                    return t
                 }), {})
-            }(t, e.plugins));
-            return n.aria = Object.assign({}, qt.aria, n.aria), n.aria = {
-                expanded: "auto" === n.aria.expanded ? e.interactive : n.aria.expanded,
-                content: "auto" === n.aria.content ? e.interactive ? null : "describedby" : n.aria.content
+            }(e, t.plugins));
+            return n.aria = Object.assign({}, qe.aria, n.aria), n.aria = {
+                expanded: "auto" === n.aria.expanded ? t.interactive : n.aria.expanded,
+                content: "auto" === n.aria.content ? t.interactive ? null : "describedby" : n.aria.content
             }, n
         }
-        var zt = function() {
+        var ze = function() {
             return "innerHTML"
         };
 
-        function Xt(t, e) {
-            t[zt()] = e
+        function Xe(e, t) {
+            e[ze()] = t
         }
 
-        function Yt(t) {
-            var e = Dt();
-            return !0 === t ? e.className = wt : (e.className = yt, kt(t) ? e.appendChild(t) : Xt(e, t)), e
+        function Ye(e) {
+            var t = Me();
+            return !0 === e ? t.className = we : (t.className = ye, Re(e) ? t.appendChild(e) : Xe(t, e)), t
         }
 
-        function Gt(t, e) {
-            kt(e.content) ? (Xt(t, ""), t.appendChild(e.content)) : "function" != typeof e.content && (e.allowHTML ? Xt(t, e.content) : t.textContent = e.content)
+        function Ge(e, t) {
+            Re(t.content) ? (Xe(e, ""), e.appendChild(t.content)) : "function" != typeof t.content && (t.allowHTML ? Xe(e, t.content) : e.textContent = t.content)
         }
 
-        function Jt(t) {
-            var e = t.firstElementChild,
-                n = Mt(e.children);
+        function Je(e) {
+            var t = e.firstElementChild,
+                n = Se(t.children);
             return {
-                box: e,
-                content: n.find((function(t) {
-                    return t.classList.contains(vt)
+                box: t,
+                content: n.find((function(e) {
+                    return e.classList.contains(ve)
                 })),
-                arrow: n.find((function(t) {
-                    return t.classList.contains(wt) || t.classList.contains(yt)
+                arrow: n.find((function(e) {
+                    return e.classList.contains(we) || e.classList.contains(ye)
                 })),
-                backdrop: n.find((function(t) {
-                    return t.classList.contains(gt)
+                backdrop: n.find((function(e) {
+                    return e.classList.contains(ge)
                 }))
             }
         }
 
-        function Kt(t) {
-            var e = Dt(),
-                n = Dt();
+        function Ke(e) {
+            var t = Me(),
+                n = Me();
             n.className = "tippy-box", n.setAttribute("data-state", "hidden"), n.setAttribute("tabindex", "-1");
-            var i = Dt();
+            var i = Me();
 
             function r(n, i) {
-                var r = Jt(e),
+                var r = Je(t),
                     o = r.box,
                     a = r.content,
                     s = r.arrow;
-                i.theme ? o.setAttribute("data-theme", i.theme) : o.removeAttribute("data-theme"), "string" == typeof i.animation ? o.setAttribute("data-animation", i.animation) : o.removeAttribute("data-animation"), i.inertia ? o.setAttribute("data-inertia", "") : o.removeAttribute("data-inertia"), o.style.maxWidth = "number" == typeof i.maxWidth ? i.maxWidth + "px" : i.maxWidth, i.role ? o.setAttribute("role", i.role) : o.removeAttribute("role"), n.content === i.content && n.allowHTML === i.allowHTML || Gt(a, t.props), i.arrow ? s ? n.arrow !== i.arrow && (o.removeChild(s), o.appendChild(Yt(i.arrow))) : o.appendChild(Yt(i.arrow)) : s && o.removeChild(s)
+                i.theme ? o.setAttribute("data-theme", i.theme) : o.removeAttribute("data-theme"), "string" == typeof i.animation ? o.setAttribute("data-animation", i.animation) : o.removeAttribute("data-animation"), i.inertia ? o.setAttribute("data-inertia", "") : o.removeAttribute("data-inertia"), o.style.maxWidth = "number" == typeof i.maxWidth ? i.maxWidth + "px" : i.maxWidth, i.role ? o.setAttribute("role", i.role) : o.removeAttribute("role"), n.content === i.content && n.allowHTML === i.allowHTML || Ge(a, e.props), i.arrow ? s ? n.arrow !== i.arrow && (o.removeChild(s), o.appendChild(Ye(i.arrow))) : o.appendChild(Ye(i.arrow)) : s && o.removeChild(s)
             }
-            return i.className = vt, i.setAttribute("data-state", "hidden"), Gt(i, t.props), e.appendChild(n), n.appendChild(i), r(t.props, t.props), {
-                popper: e,
+            return i.className = ve, i.setAttribute("data-state", "hidden"), Ge(i, e.props), t.appendChild(n), n.appendChild(i), r(e.props, e.props), {
+                popper: t,
                 onUpdate: r
             }
         }
-        Kt.$$tippy = !0;
-        var Qt = 1,
-            Zt = [],
-            te = [];
+        Ke.$$tippy = !0;
+        var Qe = 1,
+            Ze = [],
+            et = [];
 
-        function ee(t, e) {
-            var n, i, r, o, a, s, c, l, d = $t(t, Object.assign({}, qt, Ut(St(e)))),
+        function tt(e, t) {
+            var n, i, r, o, a, s, c, l, d = $e(e, Object.assign({}, qe, Ue(De(t)))),
                 p = !1,
                 u = !1,
                 f = !1,
                 h = !1,
                 m = [],
-                v = At(X, d.interactiveDebounce),
-                g = Qt++,
-                w = (l = d.plugins).filter((function(t, e) {
-                    return l.indexOf(t) === e
+                v = Te(X, d.interactiveDebounce),
+                g = Qe++,
+                w = (l = d.plugins).filter((function(e, t) {
+                    return l.indexOf(e) === t
                 })),
                 y = {
                     id: g,
-                    reference: t,
-                    popper: Dt(),
+                    reference: e,
+                    popper: Me(),
                     popperInstance: null,
                     props: d,
                     state: {
                         isEnabled: !0,
                         isVisible: !1,
                         isDestroyed: !1,
                         isMounted: !1,
                         isShown: !1
                     },
                     plugins: w,
                     clearDelayTimeouts: function() {
                         clearTimeout(n), clearTimeout(i), cancelAnimationFrame(r)
                     },
-                    setProps: function(e) {
+                    setProps: function(t) {
                         if (!y.state.isDestroyed) {
-                            P("onBeforeUpdate", [y, e]), $();
+                            I("onBeforeUpdate", [y, t]), $();
                             var n = y.props,
-                                i = $t(t, Object.assign({}, n, St(e), {
+                                i = $e(e, Object.assign({}, n, De(t), {
                                     ignoreAttributes: !0
                                 }));
-                            y.props = i, U(), n.interactiveDebounce !== i.interactiveDebounce && (R(), v = At(X, i.interactiveDebounce)), n.triggerTarget && !i.triggerTarget ? Tt(n.triggerTarget).forEach((function(t) {
-                                t.removeAttribute("aria-expanded")
-                            })) : i.triggerTarget && t.removeAttribute("aria-expanded"), H(), j(), E && E(n, i), y.popperInstance && (K(), Z().forEach((function(t) {
-                                requestAnimationFrame(t._tippy.popperInstance.forceUpdate)
-                            }))), P("onAfterUpdate", [y, e])
+                            y.props = i, U(), n.interactiveDebounce !== i.interactiveDebounce && (H(), v = Te(X, i.interactiveDebounce)), n.triggerTarget && !i.triggerTarget ? Ae(n.triggerTarget).forEach((function(e) {
+                                e.removeAttribute("aria-expanded")
+                            })) : i.triggerTarget && e.removeAttribute("aria-expanded"), P(), j(), x && x(n, i), y.popperInstance && (K(), Z().forEach((function(e) {
+                                requestAnimationFrame(e._tippy.popperInstance.forceUpdate)
+                            }))), I("onAfterUpdate", [y, t])
                         }
                     },
-                    setContent: function(t) {
+                    setContent: function(e) {
                         y.setProps({
-                            content: t
+                            content: e
                         })
                     },
                     show: function() {
-                        var t = y.state.isVisible,
-                            e = y.state.isDestroyed,
+                        var e = y.state.isVisible,
+                            t = y.state.isDestroyed,
                             n = !y.state.isEnabled,
-                            i = Rt.isTouch && !y.props.touch,
-                            r = Et(y.props.duration, 0, qt.duration);
-                        if (!(t || e || n || i || M().hasAttribute("disabled") || (P("onShow", [y], !1), !1 === y.props.onShow(y)))) {
-                            if (y.state.isVisible = !0, C() && (x.style.visibility = "visible"), j(), _(), y.state.isMounted || (x.style.transition = "none"), C()) {
-                                var o = D();
-                                jt([o.box, o.content], 0)
+                            i = He.isTouch && !y.props.touch,
+                            r = xe(y.props.duration, 0, qe.duration);
+                        if (!(e || t || n || i || S().hasAttribute("disabled") || (I("onShow", [y], !1), !1 === y.props.onShow(y)))) {
+                            if (y.state.isVisible = !0, C() && (E.style.visibility = "visible"), j(), _(), y.state.isMounted || (E.style.transition = "none"), C()) {
+                                var o = M();
+                                je([o.box, o.content], 0)
                             }
                             var a, c, l;
                             s = function() {
-                                var t;
+                                var e;
                                 if (y.state.isVisible && !h) {
-                                    if (h = !0, x.offsetHeight, x.style.transition = y.props.moveTransition, C() && y.props.animation) {
-                                        var e = D(),
-                                            n = e.box,
-                                            i = e.content;
-                                        jt([n, i], r), Pt([n, i], "visible")
+                                    if (h = !0, E.offsetHeight, E.style.transition = y.props.moveTransition, C() && y.props.animation) {
+                                        var t = M(),
+                                            n = t.box,
+                                            i = t.content;
+                                        je([n, i], r), Ie([n, i], "visible")
                                     }
-                                    N(), H(), Ct(te, y), null == (t = y.popperInstance) || t.forceUpdate(), P("onMount", [y]), y.props.animation && C() && function(t, e) {
-                                        q(t, (function() {
-                                            y.state.isShown = !0, P("onShown", [y])
+                                    k(), P(), Ce(et, y), null == (e = y.popperInstance) || e.forceUpdate(), I("onMount", [y]), y.props.animation && C() && function(e, t) {
+                                        q(e, (function() {
+                                            y.state.isShown = !0, I("onShown", [y])
                                         }))
                                     }(r)
                                 }
-                            }, c = y.props.appendTo, l = M(), (a = y.props.interactive && c === xt || "parent" === c ? l.parentNode : Lt(c, [l])).contains(x) || a.appendChild(x), y.state.isMounted = !0, K()
+                            }, c = y.props.appendTo, l = S(), (a = y.props.interactive && c === Ee || "parent" === c ? l.parentNode : Le(c, [l])).contains(E) || a.appendChild(E), y.state.isMounted = !0, K()
                         }
                     },
                     hide: function() {
-                        var t = !y.state.isVisible,
-                            e = y.state.isDestroyed,
+                        var e = !y.state.isVisible,
+                            t = y.state.isDestroyed,
                             n = !y.state.isEnabled,
-                            i = Et(y.props.duration, 1, qt.duration);
-                        if (!(t || e || n) && (P("onHide", [y], !1), !1 !== y.props.onHide(y))) {
-                            if (y.state.isVisible = !1, y.state.isShown = !1, h = !1, p = !1, C() && (x.style.visibility = "hidden"), R(), F(), j(!0), C()) {
-                                var r = D(),
+                            i = xe(y.props.duration, 1, qe.duration);
+                        if (!(e || t || n) && (I("onHide", [y], !1), !1 !== y.props.onHide(y))) {
+                            if (y.state.isVisible = !1, y.state.isShown = !1, h = !1, p = !1, C() && (E.style.visibility = "hidden"), H(), F(), j(!0), C()) {
+                                var r = M(),
                                     o = r.box,
                                     a = r.content;
-                                y.props.animation && (jt([o, a], i), Pt([o, a], "hidden"))
+                                y.props.animation && (je([o, a], i), Ie([o, a], "hidden"))
                             }
-                            N(), H(), y.props.animation ? C() && function(t, e) {
-                                q(t, (function() {
-                                    !y.state.isVisible && x.parentNode && x.parentNode.contains(x) && e()
+                            k(), P(), y.props.animation ? C() && function(e, t) {
+                                q(e, (function() {
+                                    !y.state.isVisible && E.parentNode && E.parentNode.contains(E) && t()
                                 }))
                             }(i, y.unmount) : y.unmount()
                         }
                     },
-                    hideWithInteractivity: function(t) {
-                        S().addEventListener("mousemove", v), Ct(Zt, v), v(t)
+                    hideWithInteractivity: function(e) {
+                        D().addEventListener("mousemove", v), Ce(Ze, v), v(e)
                     },
                     enable: function() {
                         y.state.isEnabled = !0
                     },
                     disable: function() {
                         y.hide(), y.state.isEnabled = !1
                     },
                     unmount: function() {
-                        y.state.isVisible && y.hide(), y.state.isMounted && (Q(), Z().forEach((function(t) {
-                            t._tippy.unmount()
-                        })), x.parentNode && x.parentNode.removeChild(x), te = te.filter((function(t) {
-                            return t !== y
-                        })), y.state.isMounted = !1, P("onHidden", [y]))
+                        y.state.isVisible && y.hide(), y.state.isMounted && (Q(), Z().forEach((function(e) {
+                            e._tippy.unmount()
+                        })), E.parentNode && E.parentNode.removeChild(E), et = et.filter((function(e) {
+                            return e !== y
+                        })), y.state.isMounted = !1, I("onHidden", [y]))
                     },
                     destroy: function() {
-                        y.state.isDestroyed || (y.clearDelayTimeouts(), y.unmount(), $(), delete t._tippy, y.state.isDestroyed = !0, P("onDestroy", [y]))
+                        y.state.isDestroyed || (y.clearDelayTimeouts(), y.unmount(), $(), delete e._tippy, y.state.isDestroyed = !0, I("onDestroy", [y]))
                     }
                 };
             if (!d.render) return y;
             var b = d.render(y),
-                x = b.popper,
-                E = b.onUpdate;
-            x.setAttribute("data-tippy-root", ""), x.id = "tippy-" + y.id, y.popper = x, t._tippy = y, x._tippy = y;
-            var O = w.map((function(t) {
-                    return t.fn(y)
+                E = b.popper,
+                x = b.onUpdate;
+            E.setAttribute("data-tippy-root", ""), E.id = "tippy-" + y.id, y.popper = E, e._tippy = y, E._tippy = y;
+            var O = w.map((function(e) {
+                    return e.fn(y)
                 })),
-                L = t.hasAttribute("aria-expanded");
-            return U(), H(), j(), P("onCreate", [y]), d.showOnCreate && tt(), x.addEventListener("mouseenter", (function() {
+                L = e.hasAttribute("aria-expanded");
+            return U(), P(), j(), I("onCreate", [y]), d.showOnCreate && ee(), E.addEventListener("mouseenter", (function() {
                 y.props.interactive && y.state.isVisible && y.clearDelayTimeouts()
-            })), x.addEventListener("mouseleave", (function() {
-                y.props.interactive && y.props.trigger.indexOf("mouseenter") >= 0 && S().addEventListener("mousemove", v)
+            })), E.addEventListener("mouseleave", (function() {
+                y.props.interactive && y.props.trigger.indexOf("mouseenter") >= 0 && D().addEventListener("mousemove", v)
             })), y;
 
-            function A() {
-                var t = y.props.touch;
-                return Array.isArray(t) ? t : [t, 0]
-            }
-
             function T() {
-                return "hold" === A()[0]
+                var e = y.props.touch;
+                return Array.isArray(e) ? e : [e, 0]
             }
 
-            function C() {
-                var t;
-                return !(null == (t = y.props.render) || !t.$$tippy)
+            function A() {
+                return "hold" === T()[0]
             }
 
-            function M() {
-                return c || t
+            function C() {
+                var e;
+                return !(null == (e = y.props.render) || !e.$$tippy)
             }
 
             function S() {
-                var t, e, n = M().parentNode;
-                return n ? null != (e = Tt(n)[0]) && null != (t = e.ownerDocument) && t.body ? e.ownerDocument : document : document
+                return c || e
             }
 
             function D() {
-                return Jt(x)
+                var e, t, n = S().parentNode;
+                return n ? null != (t = Ae(n)[0]) && null != (e = t.ownerDocument) && e.body ? t.ownerDocument : document : document
+            }
+
+            function M() {
+                return Je(E)
             }
 
-            function k(t) {
-                return y.state.isMounted && !y.state.isVisible || Rt.isTouch || o && "focus" === o.type ? 0 : Et(y.props.delay, t ? 0 : 1, qt.delay)
+            function R(e) {
+                return y.state.isMounted && !y.state.isVisible || He.isTouch || o && "focus" === o.type ? 0 : xe(y.props.delay, e ? 0 : 1, qe.delay)
             }
 
-            function j(t) {
-                void 0 === t && (t = !1), x.style.pointerEvents = y.props.interactive && !t ? "" : "none", x.style.zIndex = "" + y.props.zIndex
+            function j(e) {
+                void 0 === e && (e = !1), E.style.pointerEvents = y.props.interactive && !e ? "" : "none", E.style.zIndex = "" + y.props.zIndex
             }
 
-            function P(t, e, n) {
+            function I(e, t, n) {
                 var i;
                 void 0 === n && (n = !0), O.forEach((function(n) {
-                    n[t] && n[t].apply(n, e)
-                })), n && (i = y.props)[t].apply(i, e)
+                    n[e] && n[e].apply(n, t)
+                })), n && (i = y.props)[e].apply(i, t)
             }
 
-            function N() {
-                var e = y.props.aria;
-                if (e.content) {
-                    var n = "aria-" + e.content,
-                        i = x.id;
-                    Tt(y.props.triggerTarget || t).forEach((function(t) {
-                        var e = t.getAttribute(n);
-                        if (y.state.isVisible) t.setAttribute(n, e ? e + " " + i : i);
+            function k() {
+                var t = y.props.aria;
+                if (t.content) {
+                    var n = "aria-" + t.content,
+                        i = E.id;
+                    Ae(y.props.triggerTarget || e).forEach((function(e) {
+                        var t = e.getAttribute(n);
+                        if (y.state.isVisible) e.setAttribute(n, t ? t + " " + i : i);
                         else {
-                            var r = e && e.replace(i, "").trim();
-                            r ? t.setAttribute(n, r) : t.removeAttribute(n)
+                            var r = t && t.replace(i, "").trim();
+                            r ? e.setAttribute(n, r) : e.removeAttribute(n)
                         }
                     }))
                 }
             }
 
-            function H() {
-                !L && y.props.aria.expanded && Tt(y.props.triggerTarget || t).forEach((function(t) {
-                    y.props.interactive ? t.setAttribute("aria-expanded", y.state.isVisible && t === M() ? "true" : "false") : t.removeAttribute("aria-expanded")
+            function P() {
+                !L && y.props.aria.expanded && Ae(y.props.triggerTarget || e).forEach((function(e) {
+                    y.props.interactive ? e.setAttribute("aria-expanded", y.state.isVisible && e === S() ? "true" : "false") : e.removeAttribute("aria-expanded")
                 }))
             }
 
-            function R() {
-                S().removeEventListener("mousemove", v), Zt = Zt.filter((function(t) {
-                    return t !== v
+            function H() {
+                D().removeEventListener("mousemove", v), Ze = Ze.filter((function(e) {
+                    return e !== v
                 }))
             }
 
-            function W(e) {
-                if (!Rt.isTouch || !f && "mousedown" !== e.type) {
-                    var n = e.composedPath && e.composedPath()[0] || e.target;
-                    if (!y.props.interactive || !Ht(x, n)) {
-                        if (Tt(y.props.triggerTarget || t).some((function(t) {
-                                return Ht(t, n)
+            function N(t) {
+                if (!He.isTouch || !f && "mousedown" !== t.type) {
+                    var n = t.composedPath && t.composedPath()[0] || t.target;
+                    if (!y.props.interactive || !Pe(E, n)) {
+                        if (Ae(y.props.triggerTarget || e).some((function(e) {
+                                return Pe(e, n)
                             }))) {
-                            if (Rt.isTouch) return;
+                            if (He.isTouch) return;
                             if (y.state.isVisible && y.props.trigger.indexOf("click") >= 0) return
-                        } else P("onClickOutside", [y, e]);
+                        } else I("onClickOutside", [y, t]);
                         !0 === y.props.hideOnClick && (y.clearDelayTimeouts(), y.hide(), u = !0, setTimeout((function() {
                             u = !1
                         })), y.state.isMounted || F())
                     }
                 }
             }
 
-            function B() {
+            function W() {
                 f = !0
             }
 
-            function I() {
+            function B() {
                 f = !1
             }
 
             function _() {
-                var t = S();
-                t.addEventListener("mousedown", W, !0), t.addEventListener("touchend", W, bt), t.addEventListener("touchstart", I, bt), t.addEventListener("touchmove", B, bt)
+                var e = D();
+                e.addEventListener("mousedown", N, !0), e.addEventListener("touchend", N, be), e.addEventListener("touchstart", B, be), e.addEventListener("touchmove", W, be)
             }
 
             function F() {
-                var t = S();
-                t.removeEventListener("mousedown", W, !0), t.removeEventListener("touchend", W, bt), t.removeEventListener("touchstart", I, bt), t.removeEventListener("touchmove", B, bt)
+                var e = D();
+                e.removeEventListener("mousedown", N, !0), e.removeEventListener("touchend", N, be), e.removeEventListener("touchstart", B, be), e.removeEventListener("touchmove", W, be)
             }
 
-            function q(t, e) {
-                var n = D().box;
+            function q(e, t) {
+                var n = M().box;
 
-                function i(t) {
-                    t.target === n && (Nt(n, "remove", i), e())
+                function i(e) {
+                    e.target === n && (ke(n, "remove", i), t())
                 }
-                if (0 === t) return e();
-                Nt(n, "remove", a), Nt(n, "add", i), a = i
+                if (0 === e) return t();
+                ke(n, "remove", a), ke(n, "add", i), a = i
             }
 
-            function V(e, n, i) {
-                void 0 === i && (i = !1), Tt(y.props.triggerTarget || t).forEach((function(t) {
-                    t.addEventListener(e, n, i), m.push({
-                        node: t,
-                        eventType: e,
+            function V(t, n, i) {
+                void 0 === i && (i = !1), Ae(y.props.triggerTarget || e).forEach((function(e) {
+                    e.addEventListener(t, n, i), m.push({
+                        node: e,
+                        eventType: t,
                         handler: n,
                         options: i
                     })
                 }))
             }
 
             function U() {
-                var t;
-                T() && (V("touchstart", z, {
+                var e;
+                A() && (V("touchstart", z, {
                     passive: !0
                 }), V("touchend", Y, {
                     passive: !0
-                })), (t = y.props.trigger, t.split(/\s+/).filter(Boolean)).forEach((function(t) {
-                    if ("manual" !== t) switch (V(t, z), t) {
+                })), (e = y.props.trigger, e.split(/\s+/).filter(Boolean)).forEach((function(e) {
+                    if ("manual" !== e) switch (V(e, z), e) {
                         case "mouseenter":
                             V("mouseleave", Y);
                             break;
                         case "focus":
-                            V(Ft ? "focusout" : "blur", G);
+                            V(Fe ? "focusout" : "blur", G);
                             break;
                         case "focusin":
                             V("focusout", G)
                     }
                 }))
             }
 
             function $() {
-                m.forEach((function(t) {
-                    var e = t.node,
-                        n = t.eventType,
-                        i = t.handler,
-                        r = t.options;
-                    e.removeEventListener(n, i, r)
+                m.forEach((function(e) {
+                    var t = e.node,
+                        n = e.eventType,
+                        i = e.handler,
+                        r = e.options;
+                    t.removeEventListener(n, i, r)
                 })), m = []
             }
 
-            function z(t) {
-                var e, n = !1;
-                if (y.state.isEnabled && !J(t) && !u) {
-                    var i = "focus" === (null == (e = o) ? void 0 : e.type);
-                    o = t, c = t.currentTarget, H(), !y.state.isVisible && Ot(t, "MouseEvent") && Zt.forEach((function(e) {
-                        return e(t)
-                    })), "click" === t.type && (y.props.trigger.indexOf("mouseenter") < 0 || p) && !1 !== y.props.hideOnClick && y.state.isVisible ? n = !0 : tt(t), "click" === t.type && (p = !n), n && !i && et(t)
+            function z(e) {
+                var t, n = !1;
+                if (y.state.isEnabled && !J(e) && !u) {
+                    var i = "focus" === (null == (t = o) ? void 0 : t.type);
+                    o = e, c = e.currentTarget, P(), !y.state.isVisible && Oe(e, "MouseEvent") && Ze.forEach((function(t) {
+                        return t(e)
+                    })), "click" === e.type && (y.props.trigger.indexOf("mouseenter") < 0 || p) && !1 !== y.props.hideOnClick && y.state.isVisible ? n = !0 : ee(e), "click" === e.type && (p = !n), n && !i && te(e)
                 }
             }
 
-            function X(t) {
-                var e = t.target,
-                    n = M().contains(e) || x.contains(e);
-                if ("mousemove" !== t.type || !n) {
-                    var i = Z().concat(x).map((function(t) {
-                        var e, n = null == (e = t._tippy.popperInstance) ? void 0 : e.state;
+            function X(e) {
+                var t = e.target,
+                    n = S().contains(t) || E.contains(t);
+                if ("mousemove" !== e.type || !n) {
+                    var i = Z().concat(E).map((function(e) {
+                        var t, n = null == (t = e._tippy.popperInstance) ? void 0 : t.state;
                         return n ? {
-                            popperRect: t.getBoundingClientRect(),
+                            popperRect: e.getBoundingClientRect(),
                             popperState: n,
                             props: d
                         } : null
                     })).filter(Boolean);
-                    (function(t, e) {
-                        var n = e.clientX,
-                            i = e.clientY;
-                        return t.every((function(t) {
-                            var e = t.popperRect,
-                                r = t.popperState,
-                                o = t.props.interactiveBorder,
+                    (function(e, t) {
+                        var n = t.clientX,
+                            i = t.clientY;
+                        return e.every((function(e) {
+                            var t = e.popperRect,
+                                r = e.popperState,
+                                o = e.props.interactiveBorder,
                                 a = r.placement.split("-")[0],
                                 s = r.modifiersData.offset;
                             if (!s) return !0;
                             var c = "bottom" === a ? s.top.y : 0,
                                 l = "top" === a ? s.bottom.y : 0,
                                 d = "right" === a ? s.left.x : 0,
                                 p = "left" === a ? s.right.x : 0,
-                                u = e.top - i + c > o,
-                                f = i - e.bottom - l > o,
-                                h = e.left - n + d > o,
-                                m = n - e.right - p > o;
+                                u = t.top - i + c > o,
+                                f = i - t.bottom - l > o,
+                                h = t.left - n + d > o,
+                                m = n - t.right - p > o;
                             return u || f || h || m
                         }))
-                    })(i, t) && (R(), et(t))
+                    })(i, e) && (H(), te(e))
                 }
             }
 
-            function Y(t) {
-                J(t) || y.props.trigger.indexOf("click") >= 0 && p || (y.props.interactive ? y.hideWithInteractivity(t) : et(t))
+            function Y(e) {
+                J(e) || y.props.trigger.indexOf("click") >= 0 && p || (y.props.interactive ? y.hideWithInteractivity(e) : te(e))
             }
 
-            function G(t) {
-                y.props.trigger.indexOf("focusin") < 0 && t.target !== M() || y.props.interactive && t.relatedTarget && x.contains(t.relatedTarget) || et(t)
+            function G(e) {
+                y.props.trigger.indexOf("focusin") < 0 && e.target !== S() || y.props.interactive && e.relatedTarget && E.contains(e.relatedTarget) || te(e)
             }
 
-            function J(t) {
-                return !!Rt.isTouch && T() !== t.type.indexOf("touch") >= 0
+            function J(e) {
+                return !!He.isTouch && A() !== e.type.indexOf("touch") >= 0
             }
 
             function K() {
                 Q();
-                var e = y.props,
-                    n = e.popperOptions,
-                    i = e.placement,
-                    r = e.offset,
-                    o = e.getReferenceClientRect,
-                    a = e.moveTransition,
-                    c = C() ? Jt(x).arrow : null,
+                var t = y.props,
+                    n = t.popperOptions,
+                    i = t.placement,
+                    r = t.offset,
+                    o = t.getReferenceClientRect,
+                    a = t.moveTransition,
+                    c = C() ? Je(E).arrow : null,
                     l = o ? {
                         getBoundingClientRect: o,
-                        contextElement: o.contextElement || M()
-                    } : t,
+                        contextElement: o.contextElement || S()
+                    } : e,
                     d = [{
                         name: "offset",
                         options: {
                             offset: r
                         }
                     }, {
                         name: "preventOverflow",
@@ -1937,646 +1937,686 @@
                             adaptive: !a
                         }
                     }, {
                         name: "$$tippy",
                         enabled: !0,
                         phase: "beforeWrite",
                         requires: ["computeStyles"],
-                        fn: function(t) {
-                            var e = t.state;
+                        fn: function(e) {
+                            var t = e.state;
                             if (C()) {
-                                var n = D().box;
-                                ["placement", "reference-hidden", "escaped"].forEach((function(t) {
-                                    "placement" === t ? n.setAttribute("data-placement", e.placement) : e.attributes.popper["data-popper-" + t] ? n.setAttribute("data-" + t, "") : n.removeAttribute("data-" + t)
-                                })), e.attributes.popper = {}
+                                var n = M().box;
+                                ["placement", "reference-hidden", "escaped"].forEach((function(e) {
+                                    "placement" === e ? n.setAttribute("data-placement", t.placement) : t.attributes.popper["data-popper-" + e] ? n.setAttribute("data-" + e, "") : n.removeAttribute("data-" + e)
+                                })), t.attributes.popper = {}
                             }
                         }
                     }];
                 C() && c && d.push({
                     name: "arrow",
                     options: {
                         element: c,
                         padding: 3
                     }
-                }), d.push.apply(d, (null == n ? void 0 : n.modifiers) || []), y.popperInstance = mt(l, x, Object.assign({}, n, {
+                }), d.push.apply(d, (null == n ? void 0 : n.modifiers) || []), y.popperInstance = me(l, E, Object.assign({}, n, {
                     placement: i,
                     onFirstUpdate: s,
                     modifiers: d
                 }))
             }
 
             function Q() {
                 y.popperInstance && (y.popperInstance.destroy(), y.popperInstance = null)
             }
 
             function Z() {
-                return Mt(x.querySelectorAll("[data-tippy-root]"))
+                return Se(E.querySelectorAll("[data-tippy-root]"))
             }
 
-            function tt(t) {
-                y.clearDelayTimeouts(), t && P("onTrigger", [y, t]), _();
-                var e = k(!0),
-                    i = A(),
+            function ee(e) {
+                y.clearDelayTimeouts(), e && I("onTrigger", [y, e]), _();
+                var t = R(!0),
+                    i = T(),
                     r = i[0],
                     o = i[1];
-                Rt.isTouch && "hold" === r && o && (e = o), e ? n = setTimeout((function() {
+                He.isTouch && "hold" === r && o && (t = o), t ? n = setTimeout((function() {
                     y.show()
-                }), e) : y.show()
+                }), t) : y.show()
             }
 
-            function et(t) {
-                if (y.clearDelayTimeouts(), P("onUntrigger", [y, t]), y.state.isVisible) {
-                    if (!(y.props.trigger.indexOf("mouseenter") >= 0 && y.props.trigger.indexOf("click") >= 0 && ["mouseleave", "mousemove"].indexOf(t.type) >= 0 && p)) {
-                        var e = k(!1);
-                        e ? i = setTimeout((function() {
+            function te(e) {
+                if (y.clearDelayTimeouts(), I("onUntrigger", [y, e]), y.state.isVisible) {
+                    if (!(y.props.trigger.indexOf("mouseenter") >= 0 && y.props.trigger.indexOf("click") >= 0 && ["mouseleave", "mousemove"].indexOf(e.type) >= 0 && p)) {
+                        var t = R(!1);
+                        t ? i = setTimeout((function() {
                             y.state.isVisible && y.hide()
-                        }), e) : r = requestAnimationFrame((function() {
+                        }), t) : r = requestAnimationFrame((function() {
                             y.hide()
                         }))
                     }
                 } else F()
             }
         }
 
-        function ne(t, e) {
-            void 0 === e && (e = {});
-            var n = qt.plugins.concat(e.plugins || []);
-            document.addEventListener("touchstart", Bt, bt), window.addEventListener("blur", _t);
-            var i, r = Object.assign({}, e, {
+        function nt(e, t) {
+            void 0 === t && (t = {});
+            var n = qe.plugins.concat(t.plugins || []);
+            document.addEventListener("touchstart", We, be), window.addEventListener("blur", _e);
+            var i, r = Object.assign({}, t, {
                     plugins: n
                 }),
-                o = (i = t, kt(i) ? [i] : function(t) {
-                    return Ot(t, "NodeList")
-                }(i) ? Mt(i) : Array.isArray(i) ? i : Mt(document.querySelectorAll(i))).reduce((function(t, e) {
-                    var n = e && ee(e, r);
-                    return n && t.push(n), t
+                o = (i = e, Re(i) ? [i] : function(e) {
+                    return Oe(e, "NodeList")
+                }(i) ? Se(i) : Array.isArray(i) ? i : Se(document.querySelectorAll(i))).reduce((function(e, t) {
+                    var n = t && tt(t, r);
+                    return n && e.push(n), e
                 }), []);
-            return kt(t) ? o[0] : o
+            return Re(e) ? o[0] : o
         }
-        ne.defaultProps = qt, ne.setDefaultProps = function(t) {
-            Object.keys(t).forEach((function(e) {
-                qt[e] = t[e]
+        nt.defaultProps = qe, nt.setDefaultProps = function(e) {
+            Object.keys(e).forEach((function(t) {
+                qe[t] = e[t]
             }))
-        }, ne.currentInput = Rt, Object.assign({}, K, {
-            effect: function(t) {
-                var e = t.state,
+        }, nt.currentInput = He, Object.assign({}, K, {
+            effect: function(e) {
+                var t = e.state,
                     n = {
                         popper: {
-                            position: e.options.strategy,
+                            position: t.options.strategy,
                             left: "0",
                             top: "0",
                             margin: "0"
                         },
                         arrow: {
                             position: "absolute"
                         },
                         reference: {}
                     };
-                Object.assign(e.elements.popper.style, n.popper), e.styles = n, e.elements.arrow && Object.assign(e.elements.arrow.style, n.arrow)
+                Object.assign(t.elements.popper.style, n.popper), t.styles = n, t.elements.arrow && Object.assign(t.elements.arrow.style, n.arrow)
             }
-        }), ne.setDefaultProps({
-            render: Kt
+        }), nt.setDefaultProps({
+            render: Ke
         });
-        const ie = ne;
-        var re = n(72),
-            oe = n.n(re),
-            ae = n(825),
-            se = n.n(ae),
-            ce = n(659),
-            le = n.n(ce),
-            de = n(56),
-            pe = n.n(de),
-            ue = n(540),
-            fe = n.n(ue),
-            he = n(113),
-            me = n.n(he),
-            ve = n(2),
-            ge = {};
-        ge.styleTagTransform = me(), ge.setAttributes = pe(), ge.insert = le().bind(null, "head"), ge.domAPI = se(), ge.insertStyleElement = fe(), oe()(ve.A, ge), ve.A && ve.A.locals && ve.A.locals;
-        class we {
-            constructor(t) {
-                this.element = t, this.tooltipConfig = this.makeConfig(), this.init()
+        const it = nt;
+        var rt = n(72),
+            ot = n.n(rt),
+            at = n(825),
+            st = n.n(at),
+            ct = n(659),
+            lt = n.n(ct),
+            dt = n(56),
+            pt = n.n(dt),
+            ut = n(540),
+            ft = n.n(ut),
+            ht = n(113),
+            mt = n.n(ht),
+            vt = n(2),
+            gt = {};
+        gt.styleTagTransform = mt(), gt.setAttributes = pt(), gt.insert = lt().bind(null, "head"), gt.domAPI = st(), gt.insertStyleElement = ft(), ot()(vt.A, gt), vt.A && vt.A.locals && vt.A.locals;
+        class wt {
+            constructor(e) {
+                this.element = e, this.tooltipConfig = this.makeConfig(), this.init()
             }
             init() {
-                ie(this.element, this.tooltipConfig)
+                it(this.element, this.tooltipConfig)
             }
             makeConfig() {
-                const t = {
+                const e = {
                     content: this.element.getAttribute("title")
                 };
-                for (let e = 0; e < this.element.attributes.length; e++) {
-                    const n = this.element.attributes[e];
-                    n.name.startsWith("data-tooltip-") && (t[n.name.replace("data-tooltip-", "")] = n.value)
+                for (let t = 0; t < this.element.attributes.length; t++) {
+                    const n = this.element.attributes[t];
+                    n.name.startsWith("data-tooltip-") && (e[n.name.replace("data-tooltip-", "")] = n.value)
                 }
-                return this.tooltipConfig = t, t
+                return this.tooltipConfig = e, e
             }
         }
 
-        function ye(t) {
-            const e = t.dataset.feditConstructor;
-            if (e) return window.wagtailFedit.editors[e];
+        function yt(e) {
+            const t = e.dataset.feditConstructor;
+            if (t) return window.wagtailFedit.editors[t];
             throw new Error("No editor class found for element")
         }
 
-        function be(t = document) {
-            let e;
-            e = t instanceof HTMLElement && t.classList.contains("wagtail-fedit-adapter-wrapper") && !t.classList.contains("wagtail-fedit-initialized") ? [t] : t.querySelectorAll(".wagtail-fedit-adapter-wrapper");
-            for (let n = 0; n < e.length; n++) {
-                const i = e[n];
+        function bt(e = document) {
+            let t;
+            t = e instanceof HTMLElement && e.classList.contains("wagtail-fedit-adapter-wrapper") && !e.classList.contains("wagtail-fedit-initialized") ? [e] : e.querySelectorAll(".wagtail-fedit-adapter-wrapper");
+            for (let n = 0; n < t.length; n++) {
+                const i = t[n];
                 if (!i.classList.contains("wagtail-fedit-initialized")) {
                     i.classList.add("wagtail-fedit-initialized");
-                    const t = ye(i);
-                    t ? new t(i) : console.error("No editor class found for element", i)
+                    const e = yt(i);
+                    e ? new e(i) : console.error("No editor class found for element", i)
                 }
-                const r = t.querySelectorAll("[data-tooltip='true']");
-                for (let t = 0; t < r.length; t++) {
-                    const e = r[t];
-                    "true" == e.dataset.tooltip && (new we(e), delete e.dataset.tooltip)
+                const r = e.querySelectorAll("[data-tooltip='true']");
+                for (let e = 0; e < r.length; e++) {
+                    const t = r[e];
+                    "true" == t.dataset.tooltip && (new wt(t), delete t.dataset.tooltip)
                 }
             }
         }
 
-        function xe(t) {
-            if (!t) return;
-            const e = new URL(t.href);
-            window.scrollY > 100 && e.searchParams.set("scrollY", `${window.scrollY}`), window.scrollX > 100 && e.searchParams.set("scrollX", `${window.scrollX}`), t.href = e.toString()
+        function Et(e) {
+            if (!e) return;
+            const t = new URL(e.href);
+            window.scrollY > 100 && t.searchParams.set("scrollY", `${window.scrollY}`), window.scrollX > 100 && t.searchParams.set("scrollX", `${window.scrollX}`), e.href = t.toString()
         }
-        class Ee {
-            constructor(t) {
-                this.editor = t
+        class xt {
+            constructor(e) {
+                this.editor = e
             }
-            openModal() {
-                this.editor.makeModal()
+            openEditor() {
+                this.editor.openEditor()
             }
-            closeModal() {
-                this.editor.modal.closeModal()
+            closeEditor() {
+                this.editor.closeEditor()
             }
-            executeEvent(t, e) {
-                this.editor.executeEvent(t, e)
+            executeEvent(e, t) {
+                this.editor.executeEvent(e, t)
             }
-            addEventListener(t, e) {
-                this.editor.addEventListener(t, e)
+            addEventListener(e, t) {
+                this.editor.addEventListener(e, t)
             }
-            removeEventListener(t, e, n) {
-                this.editor.removeEventListener(t, e, n)
+            removeEventListener(e, t, n) {
+                this.editor.removeEventListener(e, t, n)
             }
-            updateHtml(t) {
-                return new Promise(((e, n) => {
-                    const i = t => {
+            updateHtml(e) {
+                return new Promise(((t, n) => {
+                    const i = e => {
                         const n = this.editor.wrapperElement,
                             i = document.createElement("div");
-                        i.innerHTML = t;
+                        i.innerHTML = e;
                         const r = i.firstElementChild;
-                        return r.classList.add("wagtail-fedit-initialized"), n.parentNode.insertBefore(r, n), n.parentNode.removeChild(n), this.editor.wrapperElement = r, this.editor.initNewEditors(), this.editor.init(), e(r), n
+                        return r.classList.add("wagtail-fedit-initialized"), n.parentNode.insertBefore(r, n), n.parentNode.removeChild(n), this.editor.wrapperElement = r, this.editor.initNewEditors(), this.editor.init(), t(r), n
                     };
-                    if ("string" != typeof t) return "function" == typeof t ? (this.editor.wrapperElement.editorAPI = this, void t(i)) : void 0;
-                    i(t)
+                    if ("string" != typeof e) return "function" == typeof e ? (this.editor.wrapperElement.editorAPI = this, void e(i)) : void 0;
+                    i(e)
                 }))
             }
             refetch() {
                 return this.editor.refetch()
             }
-            execRelated(t) {
-                for (const e of this.editor.relatedWrappers) t(e.editorAPI)
+            execRelated(e) {
+                for (const t of this.editor.relatedWrappers) e(t.editorAPI)
             }
         }
-        const Oe = "wagtail-fedit-modal",
-            Le = `\n<div class="${Oe}-wrapper">\n    <div class="${Oe}" id="${Oe}-__ID__-modal">\n    </div>\n</div>`;
-        class Ae {
-            constructor(t) {
-                this.options = t, this.modalHtml = Le.replace("__ID__", this.options.modalId)
+        const Ot = "wagtail-fedit-modal",
+            Lt = `\n<div class="${Ot}-wrapper">\n    <div class="${Ot}" id="${Ot}-__ID__-modal">\n    </div>\n</div>`;
+        class Tt {
+            constructor(e) {
+                this.options = e, this.modalHtml = Lt.replace("__ID__", this.options.modalId)
             }
             static get modalWrapper() {
-                var t = document.querySelector(`#${Oe}-wrapper`);
-                return t || ((t = document.createElement("div")).id = `${Oe}-wrapper`, t.classList.add(`${Oe}-wrapper`), document.body.appendChild(t), t)
+                var e = document.querySelector(`#${Ot}-wrapper`);
+                return e || ((e = document.createElement("div")).id = `${Ot}-wrapper`, e.classList.add(`${Ot}-wrapper`), document.body.appendChild(e), e)
             }
             get wrapper() {
                 return this.constructor.modalWrapper
             }
             get modal() {
-                var t = this.wrapper.querySelector(`.${Oe}`);
-                t && t.id !== `${Oe}-${this.options.modalId}-modal` && (t.remove(), t = null), t || (t = this.buildModal());
-                var e = t;
-                return e.modal = this, e
+                var e = this.wrapper.querySelector(`.${Ot}`);
+                e && e.id !== `${Ot}-${this.options.modalId}-modal` && (e.remove(), e = null), e || (e = this.buildModal());
+                var t = e;
+                return t.modal = this, t
             }
             get innerHTML() {
                 return this.modal.innerHTML
             }
-            set innerHTML(t) {
-                this.modal.innerHTML = t
+            set innerHTML(e) {
+                this.modal.innerHTML = e
             }
             get style() {
                 return this.modal.style
             }
             get classList() {
                 return this.modal.classList
             }
             get children() {
                 return this.modal.children
             }
             buildModal() {
-                var t = this.wrapper,
-                    e = t.querySelector(`.${Oe}`);
-                return e || (t.innerHTML = this.modalHtml, e = t.querySelector(`.${Oe}`)), e.modal || (e.modal = this), e
+                var e = this.wrapper,
+                    t = e.querySelector(`.${Ot}`);
+                return t || (e.innerHTML = this.modalHtml, t = e.querySelector(`.${Ot}`)), t.modal || (t.modal = this), t
             }
-            addClass(t) {
-                this.modal.classList.add(t)
+            addClass(e) {
+                this.modal.classList.add(e)
             }
-            removeClass(t) {
-                this.modal.classList.remove(t)
+            removeClass(e) {
+                this.modal.classList.remove(e)
             }
             openModal() {
                 this.wrapper.classList.add("open"), this.options.onOpen && this.options.onOpen()
             }
             closeModal() {
                 this.wrapper.classList.remove("open"), this.wrapper.innerHTML = "", this.options.onClose && this.options.onClose()
             }
             destroy() {
                 this.wrapper.remove(), this.options.onDestroy && this.options.onDestroy()
             }
-            appendChild(...t) {
-                if (0 !== t.length)
-                    for (let e = 0; e < t.length; e++) this.modal.appendChild(t[e])
-            }
-            removeChild(t) {
-                this.modal.removeChild(t)
-            }
-            dispatchEvent(t, e) {
-                e || (e = {}), e.modal = this.modal;
-                const n = new CustomEvent(t, {
-                    detail: e
+            appendChild(...e) {
+                if (0 !== e.length)
+                    for (let t = 0; t < e.length; t++) this.modal.appendChild(e[t])
+            }
+            removeChild(e) {
+                this.modal.removeChild(e)
+            }
+            dispatchEvent(e, t) {
+                t || (t = {}), t.modal = this.modal;
+                const n = new CustomEvent(e, {
+                    detail: t
                 });
                 this.modal.dispatchEvent(n)
             }
-            addEventListener(t, e) {
-                this.modal.addEventListener(t, e)
+            addEventListener(e, t) {
+                this.modal.addEventListener(e, t)
             }
-            removeEventListener(t, e) {
-                this.modal.removeEventListener(t, e)
+            removeEventListener(e, t) {
+                this.modal.removeEventListener(e, t)
             }
         }
-        class Te {
-            constructor(t) {
+        class At {
+            constructor(e) {
+                this.executeOnloadImmediately = !1;
                 const {
-                    id: e,
+                    id: t,
                     className: n,
                     srcdoc: i = null,
                     url: r = null,
                     onLoad: o = (() => {}),
                     onError: a = (() => {}),
-                    onCancel: s = (() => {})
-                } = t;
-                this.url = r, this.srcdoc = i, this.iframe = null, this.id = e, this.className = n, this.onLoad = o, this.onError = a, this.onCancel = s, this.render()
+                    onCancel: s = (() => {}),
+                    onResize: c = (() => {}),
+                    executeOnloadImmediately: l = !1
+                } = e;
+                this.url = r, this.srcdoc = i, this.iframe = null, this.id = t, this.className = n, this.onResize = c, this.executeOnloadImmediately = l, this.onLoad = o, this.onError = a, this.onCancel = s, this.render()
             }
             get element() {
                 return this.iframe || (this.iframe = this._renderFrame(this.url, this.srcdoc, this.onLoad)), this.iframe
             }
             get document() {
-                return this.element.contentWindow.document
+                return this.window ? this.window.document : null
             }
             get window() {
                 return this.element.contentWindow
             }
             get mainElement() {
-                return this.document.querySelector("#main")
+                var e;
+                return null === (e = this.document) || void 0 === e ? void 0 : e.querySelector("#main")
             }
             get formElement() {
-                return this.document.querySelector("#wagtail-fedit-form")
+                var e;
+                return null === (e = this.document) || void 0 === e ? void 0 : e.querySelector("#wagtail-fedit-form")
             }
             get formWrapper() {
-                return this.document.querySelector(".wagtail-fedit-form-wrapper")
+                var e;
+                return null === (e = this.document) || void 0 === e ? void 0 : e.querySelector(".wagtail-fedit-form-wrapper")
             }
-            update(t, e) {
-                this.srcdoc = e, this.url = t, this._renderFrame(this.url, this.srcdoc, (({
-                    newFrame: t
+            destroy() {
+                this.iframe.remove()
+            }
+            update(e, t) {
+                this.srcdoc = t, this.url = e, this._renderFrame(this.url, this.srcdoc, (({
+                    newFrame: e
                 }) => {
-                    this.iframe.remove(), this.iframe = t, this.onLoad({
-                        newFrame: t
+                    this.iframe.remove(), this.iframe = e, this.onLoad({
+                        newFrame: e
                     })
                 }), this.onError)
             }
             render() {
                 return this.iframe || (this.iframe = this._renderFrame(this.url, this.srcdoc, this.onLoad)), this.iframe
             }
-            _renderFrame(t, e, n, i = (() => {})) {
+            _renderFrame(e, t, n, i = (() => {})) {
                 const r = document.createElement("iframe");
-                return e ? r.srcdoc = e : r.src = t, r.id = this.id, r.className = this.className, r.onload = () => {
-                    const t = this.document.querySelector(".wagtail-fedit-cancel-button");
-                    t && t.addEventListener("click", this.onCancel), n({
+                return t ? r.srcdoc = t : r.src = e, r.id = this.id, r.className = this.className, r.onload = () => {
+                    if (!this.formElement) return void i();
+                    let e, t = this.formElement,
+                        o = t.scrollHeight;
+                    this.onResize && this.onResize(0, o), this.onResize && (e = setInterval((() => {
+                        t ? o !== t.scrollHeight && (this.onResize(o, t.scrollHeight), o = t.scrollHeight) : clearInterval(e)
+                    }), 25));
+                    const a = this.document.querySelector(".wagtail-fedit-cancel-button");
+                    a && a.addEventListener("click", (() => {
+                        clearInterval(e), this.onCancel()
+                    })), "complete" === this.document.readyState || this.executeOnloadImmediately ? n({
                         newFrame: r
-                    })
+                    }) : r.contentWindow.addEventListener("DOMContentLoaded", (() => {
+                        n({
+                            newFrame: r
+                        })
+                    }))
                 }, r.onerror = () => {
                     i()
                 }, r
             }
         }
-        var Ce = function(t, e, n, i) {
-            return new(n || (n = Promise))((function(r, o) {
-                function a(t) {
-                    try {
-                        c(i.next(t))
-                    } catch (t) {
-                        o(t)
-                    }
-                }
-
-                function s(t) {
-                    try {
-                        c(i.throw(t))
-                    } catch (t) {
-                        o(t)
-                    }
-                }
-
-                function c(t) {
-                    var e;
-                    t.done ? r(t.value) : (e = t.value, e instanceof n ? e : new n((function(t) {
-                        t(e)
-                    }))).then(a, s)
-                }
-                c((i = i.apply(t, e || [])).next())
-            }))
-        };
-        class Me extends EventTarget {
-            constructor(t) {
-                super(), this.api = new Ee(this), this.initialTitle = document.title, this.wrapperElement = t, this.sharedContext = null, this.editBtn = null, this.iframe = null, this.init(), this.modal = new Ae({
-                    modalId: this.wrapperElement.id,
-                    onClose: () => {
-                        window.history.pushState(null, this.initialTitle, window.location.href.split("#")[0]), document.title = this.initialTitle, this.executeEvent(window.wagtailFedit.EVENTS.MODAL_CLOSE)
-                    }
-                }), window.location.hash === `#${this.wrapperElement.id}` && (this.makeModal(), this.focus())
+        class Ct extends EventTarget {
+            constructor(e) {
+                super(), this.api = new xt(this), this.initialTitle = document.title, this.wrapperElement = e, this.sharedContext = null, this.editBtn = null, this.iframe = null, this.init(), window.location.hash === `#${this.wrapperElement.id}` && (this.openEditor(), this.focus())
             }
             get editUrl() {
                 return this.wrapperElement.dataset.editUrl
             }
             get refetchUrl() {
                 return this.wrapperElement.dataset.refetchUrl
             }
             get relatedWrappers() {
-                const t = this.wrapperElement.dataset.wrapperId,
-                    e = document.querySelectorAll(`[data-wrapper-id="${t}"]`);
-                return Array.from(e).filter((t => t !== this.wrapperElement))
+                const e = this.wrapperElement.dataset.wrapperId,
+                    t = document.querySelectorAll(`[data-wrapper-id="${e}"]`);
+                return Array.from(t).filter((e => e !== this.wrapperElement))
             }
             init() {
-                this.sharedContext = this.wrapperElement.dataset.sharedContext, this.wrapperElement.editorAPI = this.api, this.editBtn = this.wrapperElement.querySelector(".wagtail-fedit-edit-button"), this.editBtn.addEventListener("click", (t => Ce(this, void 0, void 0, (function*() {
-                    t.preventDefault(), t.stopPropagation(), yield this.makeModal()
-                }))))
+                this.sharedContext = this.wrapperElement.dataset.sharedContext, this.wrapperElement.editorAPI = this.api, this.editBtn = this.wrapperElement.querySelector(".wagtail-fedit-edit-button"), this.editBtn.addEventListener("click", (e => {
+                    return t = this, n = void 0, r = function*() {
+                        e.preventDefault(), e.stopPropagation(), this.opened || this.openEditor()
+                    }, new((i = void 0) || (i = Promise))((function(e, o) {
+                        function a(e) {
+                            try {
+                                c(r.next(e))
+                            } catch (e) {
+                                o(e)
+                            }
+                        }
+
+                        function s(e) {
+                            try {
+                                c(r.throw(e))
+                            } catch (e) {
+                                o(e)
+                            }
+                        }
+
+                        function c(t) {
+                            var n;
+                            t.done ? e(t.value) : (n = t.value, n instanceof i ? n : new i((function(e) {
+                                e(n)
+                            }))).then(a, s)
+                        }
+                        c((r = r.apply(t, n || [])).next())
+                    }));
+                    var t, n, i, r
+                }))
             }
             initNewEditors() {
-                be(this.wrapperElement)
+                bt(this.wrapperElement)
             }
             focus() {
                 this.wrapperElement.focus()
             }
             refetch() {
-                return new Promise(((t, e) => {
-                    fetch(this.getRefetchUrl()).then((t => t.json())).then((e => {
-                        e.success ? (this.onResponse(e), t(e)) : console.error("Errors rendering response, failed to refetch", e)
-                    })).catch((t => {
-                        console.error("Failed to refetch", t), e(t)
+                return new Promise(((e, t) => {
+                    fetch(this.getRefetchUrl()).then((e => e.json())).then((t => {
+                        t.success ? (this.onResponse(t), e(t)) : console.error("Errors rendering response, failed to refetch", t)
+                    })).catch((e => {
+                        console.error("Failed to refetch", e), t(e)
                     }))
                 }))
             }
-            onResponse(t) {
+            onResponse(e) {
                 throw new Error("onResponse not implemented, cannot call super")
             }
             getEditUrl() {
-                const t = new URL(window.location.href);
-                return t.pathname = this.editUrl, this.sharedContext && t.searchParams.set("shared_context", this.sharedContext), t.toString()
+                const e = new URL(window.location.href);
+                return e.pathname = this.editUrl, this.sharedContext && e.searchParams.set("shared_context", this.sharedContext), e.toString()
             }
             getRefetchUrl() {
-                const t = new URL(window.location.href);
-                return t.pathname = this.refetchUrl, this.sharedContext && t.searchParams.set("shared_context", this.sharedContext), t.toString()
+                const e = new URL(window.location.href);
+                return e.pathname = this.refetchUrl, this.sharedContext && e.searchParams.set("shared_context", this.sharedContext), e.toString()
+            }
+            get frameOptions() {
+                return {}
             }
-            makeModal() {
-                return Ce(this, void 0, void 0, (function*() {
-                    this.iframe = new Te({
-                        url: this.getEditUrl(),
-                        id: "wagtail-fedit-iframe",
-                        className: null,
-                        onLoad: () => {
-                            const t = e => {
-                                e.preventDefault();
-                                const n = new FormData(this.iframe.formElement);
-                                this.executeEvent(window.wagtailFedit.EVENTS.SUBMIT, {
-                                    element: this.wrapperElement,
-                                    formData: n
-                                }), fetch(this.getEditUrl(), {
-                                    method: "POST",
-                                    body: n
-                                }).then((t => t.json())).then((e => {
-                                    if (!e.success) {
-                                        console.error("Errors rendering response", e);
-                                        let n = document.createElement("div");
-                                        n.innerHTML = e.html, this.iframe.mainElement.innerHTML = n.querySelector("#main").innerHTML, this.iframe.formElement.onsubmit = t;
-                                        const i = this.iframe.mainElement.querySelector("#value[data-block]");
-                                        i && this.iframe.window.initBlockWidget(i.id);
-                                        const r = this.iframe.document.querySelector(".wagtail-fedit-cancel-button"),
-                                            o = this.modal.closeModal.bind(this.modal);
-                                        return r.addEventListener("click", o), this.iframe.onCancel = o, void this.executeEvent(window.wagtailFedit.EVENTS.SUBMIT_ERROR, {
-                                            element: this.wrapperElement,
-                                            response: e
+            openIframe(e, t) {
+                this.iframe || (this.iframe = new At(Object.assign(Object.assign({
+                    url: this.getEditUrl(),
+                    id: "wagtail-fedit-iframe",
+                    className: null,
+                    executeOnloadImmediately: !0
+                }, this.frameOptions), {
+                    onLoad: () => {
+                        const t = e => {
+                            e.preventDefault();
+                            const n = new FormData(this.iframe.formElement);
+                            this.executeEvent(window.wagtailFedit.EVENTS.SUBMIT, {
+                                element: this.wrapperElement,
+                                formData: n
+                            }), fetch(this.getEditUrl(), {
+                                method: "POST",
+                                body: n
+                            }).then((e => e.json())).then((e => {
+                                if (!e.success) {
+                                    console.error("Errors rendering response", e);
+                                    let n = document.createElement("div");
+                                    n.innerHTML = e.html, this.iframe.mainElement.innerHTML = n.querySelector("#main").innerHTML, this.iframe.formElement.onsubmit = t;
+                                    const i = this.iframe.mainElement.querySelector("#value[data-block]");
+                                    i && this.iframe.window.initBlockWidget(i.id);
+                                    const r = this.iframe.document.querySelector(".wagtail-fedit-cancel-button"),
+                                        o = this.closeEditor.bind(this);
+                                    return r.addEventListener("click", o), this.iframe.onCancel = o, void this.executeEvent(window.wagtailFedit.EVENTS.SUBMIT_ERROR, {
+                                        element: this.wrapperElement,
+                                        response: e
+                                    })
+                                }
+                                const n = this.onResponse(e),
+                                    i = () => {
+                                        this.closeEditor(), this.executeEvent(window.wagtailFedit.EVENTS.CHANGE, {
+                                            element: this.wrapperElement
                                         })
-                                    }
-                                    const n = this.onResponse(e),
-                                        i = () => {
-                                            this.modal.closeModal(), this.executeEvent(window.wagtailFedit.EVENTS.CHANGE, {
-                                                element: this.wrapperElement
-                                            })
-                                        };
-                                    n instanceof Promise ? n.then(i) : i()
-                                }))
-                            };
-                            this.iframe.formElement.onsubmit = t, this.iframe.onCancel = this.modal.closeModal.bind(this.modal);
-                            const e = this.iframe.formWrapper,
-                                n = ["large", "full"];
-                            for (const t of n)
-                                if (e && (e.classList.contains(`fedit-${t}`) || (this.iframe.formElement.dataset.editorSize || "").toLowerCase() === t)) {
-                                    this.modal.addClass(`fedit-${t}`);
-                                    break
-                                } const i = window.location.href.split("#")[0];
-                            window.history.pushState(null, this.iframe.document.title, i + `#${this.wrapperElement.id}`), document.title = this.iframe.document.title, this.executeEvent(window.wagtailFedit.EVENTS.MODAL_LOAD, {
-                                iframe: this.iframe,
-                                modal: this.modal
-                            })
-                        },
-                        onError: () => {
-                            this.modal.closeModal()
-                        },
-                        onCancel: () => {
-                            this.modal.closeModal()
-                        }
-                    }), this.modal.appendChild(this.iframe.element);
+                                    };
+                                n instanceof Promise ? n.then(i) : i()
+                            }))
+                        };
+                        this.iframe.formElement.onsubmit = t, this.iframe.onCancel = this.closeEditor.bind(this);
+                        const n = this.iframe.formWrapper,
+                            i = ["large", "full"];
+                        for (const t of i)
+                            if (n && (n.classList.contains(`fedit-${t}`) || (this.iframe.formElement.dataset.editorSize || "").toLowerCase() === t)) {
+                                e.classList.add(`fedit-${t}`);
+                                break
+                            } const r = window.location.href.split("#")[0];
+                        window.history.pushState(null, this.iframe.document.title, r + `#${this.wrapperElement.id}`), document.title = this.iframe.document.title, this.executeEvent(window.wagtailFedit.EVENTS.EDITOR_LOAD, {
+                            iframe: this.iframe
+                        })
+                    },
+                    onError: () => {
+                        this.closeEditor()
+                    },
+                    onCancel: () => {
+                        this.closeEditor()
+                    }
+                })), e.appendChild(this.iframe.element)), t(this.iframe)
+            }
+            openEditor() {
+                this.modal || (this.modal = new Tt({
+                    modalId: this.wrapperElement.id
+                })), this.opened = !0, this.openIframe(this.modal, (e => {
                     const t = document.createElement("button");
-                    t.innerHTML = "&times;", t.classList.add("wagtail-fedit-close-button"), t.addEventListener("click", this.modal.closeModal.bind(this.modal)), this.modal.appendChild(t), this.executeEvent(window.wagtailFedit.EVENTS.MODAL_OPEN, {
+                    t.innerHTML = "&times;", t.classList.add("wagtail-fedit-close-button"), t.addEventListener("click", this.closeEditor.bind(this)), this.modal.appendChild(t), this.executeEvent(window.wagtailFedit.EVENTS.EDITOR_OPEN, {
                         iframe: this.iframe,
                         modal: this.modal
                     }), this.modal.openModal()
                 }))
             }
-            executeEvent(t, e) {
-                e || (e = {
+            closeEditor() {
+                this.opened = !1, window.history.pushState(null, this.initialTitle, window.location.href.split("#")[0]), document.title = this.initialTitle, this.executeEvent(window.wagtailFedit.EVENTS.EDITOR_CLOSE), this.modal.closeModal()
+            }
+            executeEvent(e, t) {
+                t || (t = {
                     element: this.wrapperElement
-                }), e.editor = this, e.api = this.api;
-                let n = t.toLowerCase();
-                t.startsWith(`${window.wagtailFedit.NAMESPACE}:`) || (n = `${window.wagtailFedit.NAMESPACE}:${t}`);
-                const i = new CustomEvent(n, {
-                    detail: e
+                }), t.editor = this, t.api = this.api, e.startsWith(`${window.wagtailFedit.NAMESPACE}:`) || (e = `${window.wagtailFedit.NAMESPACE}:${e}`);
+                const n = new CustomEvent(e, {
+                    detail: t
                 });
-                super.dispatchEvent(i), this.wrapperElement.dispatchEvent(i), document.dispatchEvent(i)
+                super.dispatchEvent(n), this.wrapperElement.dispatchEvent(n), document.dispatchEvent(n)
             }
         }
-        class Se {
-            constructor(t) {
-                this.publishButton = t, this.publishButtonsWrapper = t.parentElement.querySelector(".wagtail-fedit-form-buttons");
-                const e = this.publishButtonsWrapper.querySelectorAll(".wagtail-fedit-userbar-button");
-                let n = !1;
-                for (let t = 0; t < e.length; t++)
-                    if (e[t].classList.contains("initially-hidden")) {
-                        n = !0;
-                        break
-                    } n && document.addEventListener(window.wagtailFedit.EVENTS.CHANGE, (() => {
-                    for (let t = 0; t < e.length; t++) {
-                        const n = e[t];
-                        n.classList.contains("initially-hidden") && n.classList.remove("initially-hidden")
-                    }
-                })), this.init()
+        class St {
+            constructor(e) {
+                this.publishButton = e, this.publishButtonsWrapper = e.parentElement.querySelector(".wagtail-fedit-form-buttons"), this.publishButtonsWrapper.querySelectorAll(".wagtail-fedit-userbar-button"), this.init()
             }
             init() {
-                this.publishButton.addEventListener("click", (t => {
+                this.publishButton.addEventListener("click", (e => {
                     this.publishButtonsWrapper.classList.contains("open") ? this.publishButtonsWrapper.animate([{
                         opacity: 1,
                         height: `${this.publishButtonsWrapper.scrollHeight}px`
                     }, {
                         opacity: 0,
                         height: "0px"
                     }], {
                         duration: 500,
                         easing: "ease-in-out"
                     }).onfinish = () => {
                         this.publishButtonsWrapper.classList.remove("open")
-                    } : (t.preventDefault(), t.stopPropagation(), this.publishButtonsWrapper.animate([{
+                    } : (e.preventDefault(), e.stopPropagation(), this.publishButtonsWrapper.animate([{
                         opacity: 0,
                         height: "0px"
                     }, {
                         opacity: 1,
                         height: `${this.publishButtonsWrapper.scrollHeight}px`
                     }], {
                         duration: 500,
                         easing: "ease-in-out"
                     }).onfinish = () => {
                         this.publishButtonsWrapper.classList.add("open")
                     })
                 }))
             }
         }
-        class De extends Me {
+        class Dt extends Ct {
             static get funcMap() {
                 return window
             }
-            onResponse(t) {
-                const e = t.func.name,
-                    n = t.func.target;
-                if (!e || !n) return void console.error("Invalid response", t);
+            onResponse(e) {
+                const t = e.func.name,
+                    n = e.func.target;
+                if (!t || !n) return void console.error("Invalid response", e);
                 const i = document.querySelector(n);
                 if (!i) return void console.error("Target element not found", n);
-                const r = this.constructor.funcMap[e];
-                if (r) return r(i, t);
-                console.error("Function not found", e)
+                const r = this.constructor.funcMap[t];
+                if (r) return r(i, e);
+                console.error("Function not found", t)
+            }
+        }
+        class Mt extends Ct {
+            onResponse(e) {
+                return this.api.updateHtml((t => {
+                    this.wrapperElement.animate([{
+                        opacity: 1
+                    }, {
+                        opacity: 0
+                    }], {
+                        duration: 350,
+                        easing: "ease-in-out"
+                    }).onfinish = () => {
+                        const n = t(e.html);
+                        e.refetch || this.api.execRelated((e => {
+                            e.refetch()
+                        })), n.animate([{
+                            opacity: 0
+                        }, {
+                            opacity: 1
+                        }], {
+                            duration: 350,
+                            easing: "ease-in-out"
+                        }).onfinish = () => {
+                            n.style.opacity = "1"
+                        }
+                    }
+                }))
             }
         }
 
-        function ke() {
-            be(), new MutationObserver((t => {
-                for (const e of t)
-                    for (let t = 0; t < e.addedNodes.length; t++) {
-                        const n = e.addedNodes[t];
-                        1 === n.nodeType && be(n)
+        function Rt() {
+            bt(), new MutationObserver((e => {
+                for (const t of e)
+                    for (let e = 0; e < t.addedNodes.length; e++) {
+                        const n = t.addedNodes[e];
+                        1 === n.nodeType && bt(n)
                     }
             })).observe(document.body, {
                 childList: !0,
                 subtree: !0
             });
-            const t = new URL(window.location.href),
-                e = t.searchParams.get("scrollY") || 0,
-                n = t.searchParams.get("scrollX") || 0;
-            (e > 0 || n > 0) && window.scrollTo(n, e);
+            const e = new URL(window.location.href),
+                t = e.searchParams.get("scrollY") || 0,
+                n = e.searchParams.get("scrollX") || 0;
+            (t > 0 || n > 0) && window.scrollTo(n, t);
             const i = document.querySelector("wagtail-userbar");
             if (i) {
-                const t = i.shadowRoot.querySelector("#wagtail-fedit-editor-button"),
-                    e = i.shadowRoot.querySelector("#wagtail-fedit-live-button"),
+                const e = i.shadowRoot.querySelector("#wagtail-fedit-editor-button"),
+                    t = i.shadowRoot.querySelector("#wagtail-fedit-live-button"),
                     n = i.shadowRoot.querySelector("#wagtail-fedit-publish-menu");
-                if (t || e) {
+                if (e || t) {
                     let n;
                     window.addEventListener("scroll", (() => {
                         n && clearTimeout(n), n = setTimeout((() => {
-                            xe(t), xe(e);
+                            Et(e), Et(t);
                             const n = new URL(window.location.href);
                             n.searchParams.set("scrollY", `${window.scrollY}`), n.searchParams.set("scrollX", `${window.scrollX}`), window.history.replaceState(null, "", n.toString())
                         }), 50)
                     }))
                 }
-                n && new Se(n)
+                n && new St(n)
             }
         }
         window.wagtailFedit = {
             NAMESPACE: "wagtail-fedit",
             EVENTS: {
                 SUBMIT: "wagtail-fedit:submit",
                 CHANGE: "wagtail-fedit:change",
-                MODAL_OPEN: "wagtail-fedit:modalOpen",
-                MODAL_LOAD: "wagtail-fedit:modalLoad",
-                MODAL_CLOSE: "wagtail-fedit:modalClose",
+                EDITOR_OPEN: "wagtail-fedit:editorOpen",
+                EDITOR_LOAD: "wagtail-fedit:editorLoad",
+                EDITOR_CLOSE: "wagtail-fedit:editorClose",
                 SUBMIT_ERROR: "wagtail-fedit:submitError"
             },
             editors: {
-                "wagtail_fedit.editors.BaseFuncEditor": De,
-                "wagtail_fedit.editors.BlockFieldEditor": class extends Me {
-                    onResponse(t) {
-                        return this.api.updateHtml((e => {
-                            this.wrapperElement.animate([{
-                                opacity: 1
-                            }, {
-                                opacity: 0
-                            }], {
-                                duration: 350,
-                                easing: "ease-in-out"
-                            }).onfinish = () => {
-                                const n = e(t.html);
-                                t.refetch || this.api.execRelated((t => {
-                                    t.refetch()
-                                })), n.animate([{
-                                    opacity: 0
-                                }, {
-                                    opacity: 1
-                                }], {
-                                    duration: 350,
-                                    easing: "ease-in-out"
-                                }).onfinish = () => {
-                                    n.style.opacity = "1"
-                                }
+                "wagtail_fedit.editors.BaseFuncEditor": Dt,
+                "wagtail_fedit.editors.BlockFieldEditor": Mt,
+                "wagtail_fedit.editors.DomPositionedBlockFieldEditor": class extends Mt {
+                    get buttonsElement() {
+                        return this.wrapperElement.querySelector(".wagtail-fedit-buttons")
+                    }
+                    get formElement() {
+                        return this.wrapperElement.querySelector(".wagtail-fedit-adapter-form")
+                    }
+                    get contentElement() {
+                        return this.wrapperElement.querySelector(".wagtail-fedit-adapter-content")
+                    }
+                    get frameOptions() {
+                        return {
+                            onResize: (e, t) => {
+                                this.iframe.element.style.height = `${t}px`
                             }
+                        }
+                    }
+                    openEditor() {
+                        this.openIframe(this.formElement, (e => {
+                            this.contentElement.style.display = "none"
                         }))
                     }
+                    closeEditor() {
+                        this.opened = !1, window.history.pushState(null, this.initialTitle, window.location.href.split("#")[0]), document.title = this.initialTitle, this.contentElement.style.display = "block", this.iframe.destroy(), delete this.iframe, this.executeEvent(window.wagtailFedit.EVENTS.EDITOR_CLOSE)
+                    }
                 },
-                "wagtail_fedit.editors.WagtailFeditFuncEditor": class extends De {
+                "wagtail_fedit.editors.WagtailFeditFuncEditor": class extends Dt {
                     static get funcMap() {
                         return window.wagtailFedit.funcs
                     }
                 }
             },
             funcs: {
-                "wagtail_fedit.funcs.backgroundImageFunc": function(t, e) {
-                    const n = e.url,
-                        i = e.css_variable_name;
-                    i ? (i.startsWith("--"), t.style.setProperty(i, `url(${n})`)) : t.style.backgroundImage = `url(${n})`
+                "wagtail_fedit.funcs.backgroundImageFunc": function(e, t) {
+                    const n = t.url,
+                        i = t.css_variable_name;
+                    i ? (i.startsWith("--"), e.style.setProperty(i, `url(${n})`)) : e.style.backgroundImage = `url(${n})`
                 }
             },
-            register: function(t, e) {
-                this.editors[t] = e
+            register: function(e, t) {
+                this.editors[e] = t
             },
-            registerFunc: function(t, e) {
-                this.funcs[t] = e
+            registerFunc: function(e, t) {
+                this.funcs[e] = t
             }
-        }, "loading" === document.readyState ? document.addEventListener("DOMContentLoaded", ke) : ke()
+        }, "loading" === document.readyState ? document.addEventListener("DOMContentLoaded", Rt) : Rt()
     })()
 })();
```

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE` & `wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html` & `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html` & `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 {% load fedit %}<div id="{{ unique_id }}" data-wrapper-id="{{ unique_id }}" class="wagtail-fedit-adapter-wrapper{% if shared_context.inline or adapter.inline %} wagtail-fedit-inline{%endif%} wagtail-fedit-{{ identifier }}" data-fedit-constructor="{{ js_constructor }}" {% if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{{ edit_url }}" data-refetch-url="{{ refetch_url }}">
-    <div class="wagtail-fedit-buttons">
+    {% block root %}<div class="wagtail-fedit-buttons">
         {% for button in buttons %}
             {{ button }}
         {% endfor %}
-    </div>{% render_adapter adapter %}
+    </div>{% render_adapter adapter %}{% endblock %}
 </div>
```

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files 9% similar despite different names*

```diff
@@ -16,19 +16,21 @@
 {{ block.super }}
 {{ form.media.js }}
 {% endblock %}
 
 {% block furniture %}
 
     <main class="content-wrapper w-overflow-x-hidden" id="main">
+
         {% block header %}
             <header id="modal-header">
                 <h1 id="modal-title">{{ view.get_header_title }}</h1>
             </header>
         {% endblock %}
+
         <div class="messages" role="status">
             {# Always show messages div so it can be appended to by JS #}
             {% if messages or form.non_field_errors %}
                 <ul>
                     {% if form.non_field_errors %}
                         {% for error in form.non_field_errors %}
                             <li class="error">{{ error }}</li>
@@ -37,51 +39,55 @@
                     {% for message in messages %}
                         <li class="{{ message.tags }}">{{ message }}</li>
                     {% endfor %}
                 </ul>
             {% endif %}
         </div>
 
-        <div class="nice-padding">
-    
-            {% if help_text %}
-                {% panel id="wagtail-fedit-help-text" icon="help" heading=help_text.heading %}
-                    {% help_block status=help_text.status %}
-                        <p><strong>{{ help_text.title }}</strong></p>
-                        <p>{{ help_text.text }}</p>
-                    {% endhelp_block %}
-                {% endpanel %}
-            {% endif %}
+        {% block padded %}
+            <div class="nice-padding">
+            
+                {% block info %}
+                    {% if help_text %}
+                        {% panel id="wagtail-fedit-help-text" icon="help" heading=help_text.heading %}
+                            {% help_block status=help_text.status %}
+                                <p><strong>{{ help_text.title }}</strong></p>
+                                <p>{{ help_text.text }}</p>
+                            {% endhelp_block %}
+                        {% endpanel %}
+                    {% endif %}
 
-            {% translate "Locked" as locked_heading %}
-            {% if locked and not locked_for_user %}
-                {% panel id="wagtail-fedit-lock-text" icon="help" heading=locked_heading %}
-                    {% help_block status="info" %}
-                        <p>{% translate "This object is locked" %}</p>
-                        <p>{% translate "You are still able to edit this object." %}</p>
-                    {% endhelp_block %}
-                {% endpanel %}
-            {% endif %}
+                    {% translate "Locked" as locked_heading %}
+                    {% if locked and not locked_for_user %}
+                        {% panel id="wagtail-fedit-lock-text" icon="help" heading=locked_heading %}
+                            {% help_block status="info" %}
+                                <p>{% translate "This object is locked" %}</p>
+                                <p>{% translate "You are still able to edit this object." %}</p>
+                            {% endhelp_block %}
+                        {% endpanel %}
+                    {% endif %}
+                {% endblock %}
 
-            {% if locked_for_user %}
-                {% panel id="wagtail-fedit-lock-text" icon="help" heading=locked_heading %}
-                    {% help_block status="info" %}
-                        <p>{% translate "This object is locked and cannot be edited." %}</p>
-                    {% endhelp_block %}
-                {% endpanel %}
-            {% else %}
-            
-                {% block content %}
+                {% if locked_for_user %}
+                    {% panel id="wagtail-fedit-lock-text" icon="help" heading=locked_heading %}
+                        {% help_block status="info" %}
+                            <p>{% translate "This object is locked and cannot be edited." %}</p>
+                        {% endhelp_block %}
+                    {% endpanel %}
+                {% else %}
 
-                    
+                    {% block content %}
 
-                {% endblock %}
-                
-            {% endif %}
-        </div>
+
+
+                    {% endblock %}
+
+                {% endif %}
+            </div>
+        {% endblock %}
     </main>
     {% block sidebar_root %}
         <aside>
             <div class="fedit-sidebar-logo">
                 {% block sidebar_logo %}{% endblock %}
             </div>
             <div class="fedit-sidebar">
```

#### html2text {}

```diff
@@ -11,31 +11,33 @@
 form.non_field_errors %}
     * {% if form.non_field_errors %} {% for error in form.non_field_errors %}
     * {{ error }}
     * {% endfor %} {% endif %} {% for message in messages %}
     * {{ message }}
     * {% endfor %}
 {% endif %}
-{% if help_text %} {% panel id="wagtail-fedit-help-text" icon="help"
-heading=help_text.heading %} {% help_block status=help_text.status %}
+{% block padded %}
+{% block info %} {% if help_text %} {% panel id="wagtail-fedit-help-text"
+icon="help" heading=help_text.heading %} {% help_block status=help_text.status
+%}
 {{{{ hheellpp__tteexxtt..ttiittllee }}}}
 {{ help_text.text }}
 {% endhelp_block %} {% endpanel %} {% endif %} {% translate "Locked" as
 locked_heading %} {% if locked and not locked_for_user %} {% panel id="wagtail-
 fedit-lock-text" icon="help" heading=locked_heading %} {% help_block
 status="info" %}
 {% translate "This object is locked" %}
 {% translate "You are still able to edit this object." %}
-{% endhelp_block %} {% endpanel %} {% endif %} {% if locked_for_user %} {%
-panel id="wagtail-fedit-lock-text" icon="help" heading=locked_heading %} {%
-help_block status="info" %}
+{% endhelp_block %} {% endpanel %} {% endif %} {% endblock %} {% if
+locked_for_user %} {% panel id="wagtail-fedit-lock-text" icon="help"
+heading=locked_heading %} {% help_block status="info" %}
 {% translate "This object is locked and cannot be edited." %}
 {% endhelp_block %} {% endpanel %} {% else %} {% block content %} {% endblock
 %} {% endif %}
-{% block sidebar_root %}
+{% endblock %} {% block sidebar_root %}
 {% block sidebar_logo %}{% endblock %}
 {% block sidebar %} {% if admin_edit_url %}
 }" target="_blank"> {% icon name="link-external" %}
 {% endif %}
 }">
 }" viewBox="0 0 16 16">
 }">
```

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x35a43a66 (Tue May  7 21:59:17 2024 UTC)
-files sz: 10310
+moddate:  0x021f4766 (Fri May 17 09:10:26 2024 UTC)
+files sz: 10373
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a046d
@@ -241,78 +241,78 @@
                458 MAKE_FUNCTION            4 (annotations)
    
    230         460 PRECALL                  0
                464 CALL                     0
    
    231         474 STORE_NAME              54 (render_adapter)
    
-   252         476 LOAD_NAME               45 (register)
+   257         476 LOAD_NAME               45 (register)
                478 LOAD_METHOD             55 (inclusion_tag)
                500 LOAD_CONST              33 ('wagtail_fedit/_hook_output.html')
                502 LOAD_CONST              34 ('fedit_scripts')
                504 LOAD_CONST              29 (True)
                506 KW_NAMES                35
                508 PRECALL                  3
                512 CALL                     3
    
-   253         522 LOAD_CONST              21 ('return')
+   258         522 LOAD_CONST              21 ('return')
                524 LOAD_NAME               56 (dict)
                526 BUILD_TUPLE              2
-               528 LOAD_CONST              36 (<code object static_hook_output, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 252>)
+               528 LOAD_CONST              36 (<code object static_hook_output, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 257>)
                530 MAKE_FUNCTION            4 (annotations)
    
-   252         532 PRECALL                  0
+   257         532 PRECALL                  0
                536 CALL                     0
    
-   253         546 STORE_NAME              57 (static_hook_output)
+   258         546 STORE_NAME              57 (static_hook_output)
    
-   282         548 LOAD_NAME               45 (register)
+   287         548 LOAD_NAME               45 (register)
                550 LOAD_METHOD             53 (simple_tag)
                572 LOAD_CONST              37 (False)
                574 LOAD_CONST              38 ('tooltip')
                576 KW_NAMES                39
                578 PRECALL                  2
                582 CALL                     2
    
-   283         592 LOAD_CONST              49 ((None,))
+   288         592 LOAD_CONST              49 ((None,))
                594 LOAD_CONST              40 ('wrapping')
                596 LOAD_NAME               48 (str)
                598 LOAD_CONST              21 ('return')
                600 LOAD_NAME               48 (str)
                602 BUILD_TUPLE              4
-               604 LOAD_CONST              41 (<code object tooltip, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 282>)
+               604 LOAD_CONST              41 (<code object tooltip, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 287>)
                606 MAKE_FUNCTION            5 (defaults, annotations)
    
-   282         608 PRECALL                  0
+   287         608 PRECALL                  0
                612 CALL                     0
    
-   283         622 STORE_NAME              58 (tooltip)
+   288         622 STORE_NAME              58 (tooltip)
    
-   301         624 LOAD_NAME               45 (register)
+   306         624 LOAD_NAME               45 (register)
                626 LOAD_METHOD             53 (simple_tag)
                648 LOAD_CONST              29 (True)
                650 LOAD_CONST              42 ('fedit_userbar')
                652 KW_NAMES                39
                654 PRECALL                  2
                658 CALL                     2
    
-   302         668 LOAD_CONST              43 ('model')
+   307         668 LOAD_CONST              43 ('model')
                670 LOAD_NAME                2 (Any)
                672 LOAD_CONST              21 ('return')
                674 LOAD_NAME               48 (str)
                676 BUILD_TUPLE              4
-               678 LOAD_CONST              44 (<code object do_with_userbar_model, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 301>)
+               678 LOAD_CONST              44 (<code object do_with_userbar_model, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 306>)
                680 MAKE_FUNCTION            4 (annotations)
    
-   301         682 PRECALL                  0
+   306         682 PRECALL                  0
                686 CALL                     0
    
-   302         696 STORE_NAME              59 (do_with_userbar_model)
+   307         696 STORE_NAME              59 (do_with_userbar_model)
    
-   309         698 LOAD_CONST              50 ((None, None))
+   314         698 LOAD_CONST              50 ((None, None))
                700 LOAD_CONST              26 ('parser')
                702 LOAD_NAME               10 (Parser)
                704 LOAD_CONST              45 ('tokens')
                706 LOAD_NAME               60 (list)
                708 LOAD_NAME               48 (str)
                710 BINARY_SUBSCR
                720 LOAD_CONST              46 ('kwarg_list')
@@ -322,15 +322,15 @@
                736 LOAD_CONST              47 ('absolute_tokens')
                738 LOAD_NAME               60 (list)
                740 LOAD_NAME               48 (str)
                742 BINARY_SUBSCR
                752 LOAD_CONST              21 ('return')
                754 LOAD_NAME               56 (dict)
                756 BUILD_TUPLE             10
-               758 LOAD_CONST              48 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 309>)
+               758 LOAD_CONST              48 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 314>)
                760 MAKE_FUNCTION            5 (defaults, annotations)
                762 STORE_NAME              61 (get_kwargs)
                764 LOAD_CONST              10 (None)
                766 RETURN_VALUE
    consts
       0
       ('Type', 'Any')
@@ -1250,82 +1250,91 @@
       'adapter'
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 3
          flags     : 3
          code
-            0x970069007d0264017c007600720b7c006401190000000000000000007d
-            027c0064013d007401000000000000000000007c00a6010000ab01000000
-            00000000007d007401000000000000000000007c02a6010000ab01000000
-            00000000007d027c00a00100000000000000000000000000000000000000
-            007c02a6010000ab01000000000000000001007c01a00200000000000000
-            000000000000000000000000007c00a6010000ab01000000000000000053
-            00
+            0x970069007d0264017c00760072087c006401190000000000000000007d
+            027401000000000000000000007c00a6010000ab0100000000000000007d
+            007401000000000000000000007c02a6010000ab0100000000000000007d
+            0264017c00760072037c0064013d007c00a0010000000000000000000000
+            0000000000000000007c02a6010000ab01000000000000000001007c01a0
+            0200000000000000000000000000000000000000007c00a6010000ab0100
+            000000000000005300
          230           0 RESUME                   0
          
          232           2 BUILD_MAP                0
                        4 STORE_FAST               2 (adapter_context)
          
-         234           6 LOAD_CONST               1 ('adapter_context')
+         235           6 LOAD_CONST               1 ('adapter_context')
                        8 LOAD_FAST                0 (context)
                       10 CONTAINS_OP              0
-                      12 POP_JUMP_FORWARD_IF_FALSE    11 (to 36)
+                      12 POP_JUMP_FORWARD_IF_FALSE     8 (to 30)
          
-         235          14 LOAD_FAST                0 (context)
+         236          14 LOAD_FAST                0 (context)
                       16 LOAD_CONST               1 ('adapter_context')
                       18 BINARY_SUBSCR
                       28 STORE_FAST               2 (adapter_context)
          
-         236          30 LOAD_FAST                0 (context)
-                      32 LOAD_CONST               1 ('adapter_context')
-                      34 DELETE_SUBSCR
+         238     >>   30 LOAD_GLOBAL              1 (NULL + _flatten_context)
          
-         238     >>   36 LOAD_GLOBAL              1 (NULL + _flatten_context)
+         239          42 LOAD_FAST                0 (context)
          
-         239          48 LOAD_FAST                0 (context)
+         238          44 PRECALL                  1
+                      48 CALL                     1
+                      58 STORE_FAST               0 (context)
          
-         238          50 PRECALL                  1
-                      54 CALL                     1
-                      64 STORE_FAST               0 (context)
+         241          60 LOAD_GLOBAL              1 (NULL + _flatten_context)
          
-         241          66 LOAD_GLOBAL              1 (NULL + _flatten_context)
+         242          72 LOAD_FAST                2 (adapter_context)
          
-         242          78 LOAD_FAST                2 (adapter_context)
+         241          74 PRECALL                  1
+                      78 CALL                     1
+                      88 STORE_FAST               2 (adapter_context)
          
-         241          80 PRECALL                  1
-                      84 CALL                     1
-                      94 STORE_FAST               2 (adapter_context)
+         245          90 LOAD_CONST               1 ('adapter_context')
+                      92 LOAD_FAST                0 (context)
+                      94 CONTAINS_OP              0
+                      96 POP_JUMP_FORWARD_IF_FALSE     3 (to 104)
          
-         245          96 LOAD_FAST                0 (context)
-                      98 LOAD_METHOD              1 (update)
-                     120 LOAD_FAST                2 (adapter_context)
-                     122 PRECALL                  1
-                     126 CALL                     1
-                     136 POP_TOP
+         246          98 LOAD_FAST                0 (context)
+                     100 LOAD_CONST               1 ('adapter_context')
+                     102 DELETE_SUBSCR
          
-         247         138 LOAD_FAST                1 (adapter)
-                     140 LOAD_METHOD              2 (render_content)
+         248     >>  104 LOAD_FAST                0 (context)
+                     106 LOAD_METHOD              1 (update)
          
-         248         162 LOAD_FAST                0 (context)
+         249         128 LOAD_FAST                2 (adapter_context)
          
-         247         164 PRECALL                  1
-                     168 CALL                     1
-                     178 RETURN_VALUE
+         248         130 PRECALL                  1
+                     134 CALL                     1
+                     144 POP_TOP
+         
+         252         146 LOAD_FAST                1 (adapter)
+                     148 LOAD_METHOD              2 (render_content)
+         
+         253         170 LOAD_FAST                0 (context)
+         
+         252         172 PRECALL                  1
+                     176 CALL                     1
+                     186 RETURN_VALUE
          consts
             None
             'adapter_context'
          names      ('_flatten_context', 'update', 'render_content')
          varnames   ('context', 'adapter', 'adapter_context')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'render_adapter'
          firstlineno 230
-         lnotab 0x020204020801100106020c0102ff10030c0102ff10042a02180102ff
+         lnotab
+            0x02020403080110020c0102ff10030c0102ff100408010602180102ff10
+            04180102ff
       'wagtail_fedit/_hook_output.html'
       'fedit_scripts'
       ('name', 'takes_context')
       code
          argcount  : 2
          nlocals   : 7
          stacksize : 6
@@ -1341,107 +1350,107 @@
             00530067007d04740f000000000000000000006a0800000000000000007c
             03a6010000ab01000000000000000044005d417d0502007c057c02a60100
             00ab0100000000000000007d067413000000000000000000007c06741400
             0000000000000000007416000000000000000000006602a6020000ab0200
             0000000000000073037c0667017d067c04a00c0000000000000000000000
             0000000000000000007c06a6010000ab01000000000000000001008c4264
             067c0469015300
-         252           0 RESUME                   0
+         257           0 RESUME                   0
          
-         254           2 LOAD_FAST                1 (css_or_js)
+         259           2 LOAD_FAST                1 (css_or_js)
                        4 LOAD_METHOD              0 (lower)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               1 (css_or_js)
          
-         256          42 LOAD_FAST                1 (css_or_js)
+         261          42 LOAD_FAST                1 (css_or_js)
                       44 LOAD_CONST               1 (('css', 'js'))
                       46 CONTAINS_OP              1
                       48 POP_JUMP_FORWARD_IF_FALSE    15 (to 80)
          
-         257          50 LOAD_GLOBAL              3 (NULL + ValueError)
+         262          50 LOAD_GLOBAL              3 (NULL + ValueError)
                       62 LOAD_CONST               2 ("Invalid argument, must be 'css' or 'js'")
                       64 PRECALL                  1
                       68 CALL                     1
                       78 RAISE_VARARGS            1
          
-         259     >>   80 LOAD_FAST                0 (context)
+         264     >>   80 LOAD_FAST                0 (context)
                       82 LOAD_METHOD              2 (get)
                      104 LOAD_CONST               3 ('request')
                      106 PRECALL                  1
                      110 CALL                     1
                      120 STORE_FAST               2 (request)
          
-         261         122 LOAD_FAST                1 (css_or_js)
+         266         122 LOAD_FAST                1 (css_or_js)
                      124 LOAD_CONST               4 ('css')
                      126 COMPARE_OP               2 (==)
                      132 POP_JUMP_FORWARD_IF_FALSE     8 (to 150)
          
-         262         134 LOAD_GLOBAL              6 (REGISTER_CSS)
+         267         134 LOAD_GLOBAL              6 (REGISTER_CSS)
                      146 STORE_FAST               3 (hook_name)
                      148 JUMP_FORWARD             7 (to 164)
          
-         264     >>  150 LOAD_GLOBAL              8 (REGISTER_JS)
+         269     >>  150 LOAD_GLOBAL              8 (REGISTER_JS)
                      162 STORE_FAST               3 (hook_name)
          
-         266     >>  164 LOAD_GLOBAL             11 (NULL + getattr)
+         271     >>  164 LOAD_GLOBAL             11 (NULL + getattr)
                      176 LOAD_FAST                2 (request)
                      178 LOAD_GLOBAL             12 (FEDIT_PREVIEW_VAR)
                      190 LOAD_CONST               5 (False)
                      192 PRECALL                  3
                      196 CALL                     3
                      206 POP_JUMP_FORWARD_IF_TRUE     2 (to 212)
          
-         267         208 BUILD_MAP                0
+         272         208 BUILD_MAP                0
                      210 RETURN_VALUE
          
-         269     >>  212 BUILD_LIST               0
+         274     >>  212 BUILD_LIST               0
                      214 STORE_FAST               4 (files)
          
-         270         216 LOAD_GLOBAL             15 (NULL + hooks)
+         275         216 LOAD_GLOBAL             15 (NULL + hooks)
                      228 LOAD_ATTR                8 (get_hooks)
                      238 LOAD_FAST                3 (hook_name)
                      240 PRECALL                  1
                      244 CALL                     1
                      254 GET_ITER
                  >>  256 FOR_ITER                65 (to 388)
                      258 STORE_FAST               5 (hook)
          
-         271         260 PUSH_NULL
+         276         260 PUSH_NULL
                      262 LOAD_FAST                5 (hook)
                      264 LOAD_FAST                2 (request)
                      266 PRECALL                  1
                      270 CALL                     1
                      280 STORE_FAST               6 (ret)
          
-         273         282 LOAD_GLOBAL             19 (NULL + isinstance)
+         278         282 LOAD_GLOBAL             19 (NULL + isinstance)
                      294 LOAD_FAST                6 (ret)
                      296 LOAD_GLOBAL             20 (list)
                      308 LOAD_GLOBAL             22 (tuple)
                      320 BUILD_TUPLE              2
                      322 PRECALL                  2
                      326 CALL                     2
                      336 POP_JUMP_FORWARD_IF_TRUE     3 (to 344)
          
-         274         338 LOAD_FAST                6 (ret)
+         279         338 LOAD_FAST                6 (ret)
                      340 BUILD_LIST               1
                      342 STORE_FAST               6 (ret)
          
-         276     >>  344 LOAD_FAST                4 (files)
+         281     >>  344 LOAD_FAST                4 (files)
                      346 LOAD_METHOD             12 (extend)
                      368 LOAD_FAST                6 (ret)
                      370 PRECALL                  1
                      374 CALL                     1
                      384 POP_TOP
                      386 JUMP_BACKWARD           66 (to 256)
          
-         279     >>  388 LOAD_CONST               6 ('hook_output')
+         284     >>  388 LOAD_CONST               6 ('hook_output')
                      390 LOAD_FAST                4 (files)
          
-         278         392 BUILD_MAP                1
+         283         392 BUILD_MAP                1
                      394 RETURN_VALUE
          consts
             None
             ('css', 'js')
             "Invalid argument, must be 'css' or 'js'"
             'request'
             'css'
@@ -1449,15 +1458,15 @@
             'hook_output'
          names      ('lower', 'ValueError', 'get', 'REGISTER_CSS', 'REGISTER_JS', 'getattr', 'FEDIT_PREVIEW_VAR', 'hooks', 'get_hooks', 'isinstance', 'list', 'tuple', 'extend')
          varnames   ('context', 'css_or_js', 'request', 'hook_name', 'files', 'hook', 'ret')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'static_hook_output'
-         firstlineno 252
+         firstlineno 257
          lnotab
             0x0202280208011e022a020c0110020e022c01040204012c011602380106
             022c0304ff
       False
       'tooltip'
       ('takes_context', 'name')
       'wrapping'
@@ -1473,43 +1482,43 @@
             02000000000000000000000000000000000000000064047c049b00640574
             07000000000000000000007c05a6010000ab0100000000000000009b0064
             069d05a6010000ab01000000000000000001008c2f6407a0040000000000
             0000000000000000000000000000007c03a6010000ab0100000000000000
             007d067c01730f740b000000000000000000007c06a6010000ab01000000
             00000000005300740b0000000000000000000064087c069b0064097c019b
             00640a9d05a6010000ab0100000000000000005300
-         282           0 RESUME                   0
+         287           0 RESUME                   0
          
-         285           2 LOAD_GLOBAL              0 (TIPPY_ENABLED)
+         290           2 LOAD_GLOBAL              0 (TIPPY_ENABLED)
                       14 POP_JUMP_FORWARD_IF_TRUE     2 (to 20)
          
-         286          16 LOAD_CONST               1 ('')
+         291          16 LOAD_CONST               1 ('')
                       18 RETURN_VALUE
          
-         288     >>   20 LOAD_FAST                0 (content)
+         293     >>   20 LOAD_FAST                0 (content)
                       22 LOAD_FAST                2 (kwargs)
                       24 LOAD_CONST               2 ('content')
                       26 STORE_SUBSCR
          
-         290          30 LOAD_CONST               3 ("data-tooltip='true'")
+         295          30 LOAD_CONST               3 ("data-tooltip='true'")
          
-         289          32 BUILD_LIST               1
+         294          32 BUILD_LIST               1
                       34 STORE_FAST               3 (s)
          
-         292          36 LOAD_FAST                2 (kwargs)
+         297          36 LOAD_FAST                2 (kwargs)
                       38 LOAD_METHOD              1 (items)
                       60 PRECALL                  0
                       64 CALL                     0
                       74 GET_ITER
                  >>   76 FOR_ITER                46 (to 170)
                       78 UNPACK_SEQUENCE          2
                       82 STORE_FAST               4 (key)
                       84 STORE_FAST               5 (value)
          
-         293          86 LOAD_FAST                3 (s)
+         298          86 LOAD_FAST                3 (s)
                       88 LOAD_METHOD              2 (append)
                      110 LOAD_CONST               4 ('data-tooltip-')
                      112 LOAD_FAST                4 (key)
                      114 FORMAT_VALUE             0
                      116 LOAD_CONST               5 ("='")
                      118 LOAD_GLOBAL              7 (NULL + escape)
                      130 LOAD_FAST                5 (value)
@@ -1519,31 +1528,31 @@
                      148 LOAD_CONST               6 ("'")
                      150 BUILD_STRING             5
                      152 PRECALL                  1
                      156 CALL                     1
                      166 POP_TOP
                      168 JUMP_BACKWARD           47 (to 76)
          
-         294     >>  170 LOAD_CONST               7 (' ')
+         299     >>  170 LOAD_CONST               7 (' ')
                      172 LOAD_METHOD              4 (join)
                      194 LOAD_FAST                3 (s)
                      196 PRECALL                  1
                      200 CALL                     1
                      210 STORE_FAST               6 (attrs)
          
-         296         212 LOAD_FAST                1 (wrapping)
+         301         212 LOAD_FAST                1 (wrapping)
                      214 POP_JUMP_FORWARD_IF_TRUE    15 (to 246)
          
-         297         216 LOAD_GLOBAL             11 (NULL + mark_safe)
+         302         216 LOAD_GLOBAL             11 (NULL + mark_safe)
                      228 LOAD_FAST                6 (attrs)
                      230 PRECALL                  1
                      234 CALL                     1
                      244 RETURN_VALUE
          
-         299     >>  246 LOAD_GLOBAL             11 (NULL + mark_safe)
+         304     >>  246 LOAD_GLOBAL             11 (NULL + mark_safe)
                      258 LOAD_CONST               8 ('<span ')
                      260 LOAD_FAST                6 (attrs)
                      262 FORMAT_VALUE             0
                      264 LOAD_CONST               9 ('>')
                      266 LOAD_FAST                1 (wrapping)
                      268 FORMAT_VALUE             0
                      270 LOAD_CONST              10 ('</span>')
@@ -1565,76 +1574,76 @@
             '</span>'
          names      ('TIPPY_ENABLED', 'items', 'append', 'escape', 'join', 'mark_safe')
          varnames   ('content', 'wrapping', 'kwargs', 's', 'key', 'value', 'attrs')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'tooltip'
-         firstlineno 282
+         firstlineno 287
          lnotab 0x02030e0104020a0202ff0403320154012a0204011e02
       'fedit_userbar'
       'model'
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x970064017c00760072197401000000000000000000007c006401190000
             000000000000007c01a6020000ab0200000000000000007c0064013c0000
             007402000000000000000000007c007600721b7c00740200000000000000
             000000190000000000000000007c016b0300000000720a7c017c00740200
             0000000000000000003c00000064025300
-         301           0 RESUME                   0
+         306           0 RESUME                   0
          
-         303           2 LOAD_CONST               1 ('request')
+         308           2 LOAD_CONST               1 ('request')
                        4 LOAD_FAST                0 (context)
                        6 CONTAINS_OP              0
                        8 POP_JUMP_FORWARD_IF_FALSE    25 (to 60)
          
-         304          10 LOAD_GLOBAL              1 (NULL + with_userbar_model)
+         309          10 LOAD_GLOBAL              1 (NULL + with_userbar_model)
                       22 LOAD_FAST                0 (context)
                       24 LOAD_CONST               1 ('request')
                       26 BINARY_SUBSCR
                       36 LOAD_FAST                1 (model)
                       38 PRECALL                  2
                       42 CALL                     2
                       52 LOAD_FAST                0 (context)
                       54 LOAD_CONST               1 ('request')
                       56 STORE_SUBSCR
          
-         305     >>   60 LOAD_GLOBAL              2 (PAGE_TEMPLATE_VAR)
+         310     >>   60 LOAD_GLOBAL              2 (PAGE_TEMPLATE_VAR)
                       72 LOAD_FAST                0 (context)
                       74 CONTAINS_OP              0
                       76 POP_JUMP_FORWARD_IF_FALSE    27 (to 132)
                       78 LOAD_FAST                0 (context)
                       80 LOAD_GLOBAL              2 (PAGE_TEMPLATE_VAR)
                       92 BINARY_SUBSCR
                      102 LOAD_FAST                1 (model)
                      104 COMPARE_OP               3 (!=)
                      110 POP_JUMP_FORWARD_IF_FALSE    10 (to 132)
          
-         306         112 LOAD_FAST                1 (model)
+         311         112 LOAD_FAST                1 (model)
                      114 LOAD_FAST                0 (context)
                      116 LOAD_GLOBAL              2 (PAGE_TEMPLATE_VAR)
                      128 STORE_SUBSCR
          
-         307     >>  132 LOAD_CONST               2 ('')
+         312     >>  132 LOAD_CONST               2 ('')
                      134 RETURN_VALUE
          consts
             None
             'request'
             ''
          names      ('with_userbar_model', 'PAGE_TEMPLATE_VAR')
          varnames   ('context', 'model')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_with_userbar_model'
-         firstlineno 301
+         firstlineno 306
          lnotab 0x02020801320134011401
       'tokens'
       'kwarg_list'
       'absolute_tokens'
       code
          argcount  : 4
          nlocals   : 11
@@ -1661,212 +1670,212 @@
             0000007d0a7c0a7c057c093c0000008cd37c086404190000000000000000
             007d097c097c0376007213740d0000000000000000000064077c099b0064
             089d03a6010000ab01000000000000000082017c00a00500000000000000
             000000000000000000000000007c08640319000000000000000000a60100
             00ab0100000000000000007c057c093c00000064057d0490018c147c0244
             005d187d097c097c0576017212740d0000000000000000000064097c099b
             009d02a6010000ab01000000000000000082018c197c055300
-         309           0 RESUME                   0
+         314           0 RESUME                   0
          
-         310           2 LOAD_CONST               1 (False)
+         315           2 LOAD_CONST               1 (False)
                        4 STORE_FAST               4 (had_kwargs)
          
-         311           6 BUILD_MAP                0
+         316           6 BUILD_MAP                0
                        8 STORE_FAST               5 (kwargs)
          
-         313          10 LOAD_FAST                2 (kwarg_list)
+         318          10 LOAD_FAST                2 (kwarg_list)
                       12 POP_JUMP_FORWARD_IF_TRUE    14 (to 42)
          
-         314          14 LOAD_GLOBAL              1 (NULL + tuple)
+         319          14 LOAD_GLOBAL              1 (NULL + tuple)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (kwarg_list)
          
-         316     >>   42 LOAD_FAST                3 (absolute_tokens)
+         321     >>   42 LOAD_FAST                3 (absolute_tokens)
                       44 POP_JUMP_FORWARD_IF_TRUE    14 (to 74)
          
-         317          46 LOAD_GLOBAL              1 (NULL + tuple)
+         322          46 LOAD_GLOBAL              1 (NULL + tuple)
                       58 PRECALL                  0
                       62 CALL                     0
                       72 STORE_FAST               3 (absolute_tokens)
          
-         319     >>   74 LOAD_GLOBAL              3 (NULL + enumerate)
+         324     >>   74 LOAD_GLOBAL              3 (NULL + enumerate)
                       86 LOAD_FAST                1 (tokens)
                       88 PRECALL                  1
                       92 CALL                     1
                      102 GET_ITER
                  >>  104 EXTENDED_ARG             1
                      106 FOR_ITER               274 (to 656)
                      108 UNPACK_SEQUENCE          2
                      112 STORE_FAST               6 (i)
                      114 STORE_FAST               7 (token)
          
-         320         116 LOAD_FAST                7 (token)
+         325         116 LOAD_FAST                7 (token)
                      118 LOAD_METHOD              2 (split)
                      140 LOAD_CONST               2 ('=')
                      142 PRECALL                  1
                      146 CALL                     1
                      156 STORE_FAST               8 (split)
          
-         321         158 LOAD_GLOBAL              7 (NULL + len)
+         326         158 LOAD_GLOBAL              7 (NULL + len)
                      170 LOAD_FAST                8 (split)
                      172 PRECALL                  1
                      176 CALL                     1
                      186 LOAD_CONST               3 (1)
                      188 COMPARE_OP               2 (==)
                      194 POP_JUMP_FORWARD_IF_FALSE    89 (to 374)
                      196 LOAD_GLOBAL              7 (NULL + len)
                      208 LOAD_FAST                2 (kwarg_list)
                      210 PRECALL                  1
                      214 CALL                     1
                      224 LOAD_FAST                6 (i)
                      226 COMPARE_OP               4 (>)
                      232 POP_JUMP_FORWARD_IF_FALSE    70 (to 374)
          
-         322         234 LOAD_FAST                8 (split)
+         327         234 LOAD_FAST                8 (split)
                      236 LOAD_CONST               4 (0)
                      238 BINARY_SUBSCR
                      248 LOAD_FAST                3 (absolute_tokens)
                      250 CONTAINS_OP              0
                      252 POP_JUMP_FORWARD_IF_FALSE    12 (to 278)
          
-         323         254 LOAD_CONST               5 (True)
+         328         254 LOAD_CONST               5 (True)
                      256 LOAD_FAST                5 (kwargs)
                      258 LOAD_FAST                8 (split)
                      260 LOAD_CONST               4 (0)
                      262 BINARY_SUBSCR
                      272 STORE_SUBSCR
          
-         324         276 JUMP_BACKWARD           87 (to 104)
+         329         276 JUMP_BACKWARD           87 (to 104)
          
-         326     >>  278 LOAD_FAST                4 (had_kwargs)
+         331     >>  278 LOAD_FAST                4 (had_kwargs)
                      280 POP_JUMP_FORWARD_IF_FALSE    15 (to 312)
          
-         327         282 LOAD_GLOBAL              9 (NULL + ValueError)
+         332         282 LOAD_GLOBAL              9 (NULL + ValueError)
                      294 LOAD_CONST               6 ('Unexpected positional argument after keyword argument')
                      296 PRECALL                  1
                      300 CALL                     1
                      310 RAISE_VARARGS            1
          
-         329     >>  312 LOAD_FAST                0 (parser)
+         334     >>  312 LOAD_FAST                0 (parser)
                      314 LOAD_METHOD              5 (compile_filter)
                      336 LOAD_FAST                7 (token)
                      338 PRECALL                  1
                      342 CALL                     1
                      352 LOAD_FAST                5 (kwargs)
                      354 LOAD_FAST                2 (kwarg_list)
                      356 LOAD_FAST                6 (i)
                      358 BINARY_SUBSCR
                      368 STORE_SUBSCR
                      372 JUMP_BACKWARD          135 (to 104)
          
-         330     >>  374 LOAD_GLOBAL              7 (NULL + len)
+         335     >>  374 LOAD_GLOBAL              7 (NULL + len)
                      386 LOAD_FAST                8 (split)
                      388 PRECALL                  1
                      392 CALL                     1
                      402 LOAD_CONST               3 (1)
                      404 COMPARE_OP               2 (==)
                      410 POP_JUMP_FORWARD_IF_FALSE    57 (to 526)
          
-         331         412 LOAD_FAST                8 (split)
+         336         412 LOAD_FAST                8 (split)
                      414 LOAD_CONST               4 (0)
                      416 BINARY_SUBSCR
                      426 LOAD_FAST                3 (absolute_tokens)
                      428 CONTAINS_OP              0
                      430 POP_JUMP_FORWARD_IF_FALSE    12 (to 456)
          
-         332         432 LOAD_CONST               5 (True)
+         337         432 LOAD_CONST               5 (True)
                      434 LOAD_FAST                5 (kwargs)
                      436 LOAD_FAST                8 (split)
                      438 LOAD_CONST               4 (0)
                      440 BINARY_SUBSCR
                      450 STORE_SUBSCR
          
-         333         454 JUMP_BACKWARD          176 (to 104)
+         338         454 JUMP_BACKWARD          176 (to 104)
          
-         335     >>  456 LOAD_FAST                8 (split)
+         340     >>  456 LOAD_FAST                8 (split)
                      458 LOAD_CONST               4 (0)
                      460 BINARY_SUBSCR
                      470 STORE_FAST               9 (key)
          
-         336         472 LOAD_FAST                0 (parser)
+         341         472 LOAD_FAST                0 (parser)
                      474 LOAD_METHOD              5 (compile_filter)
                      496 LOAD_FAST                9 (key)
                      498 PRECALL                  1
                      502 CALL                     1
                      512 STORE_FAST              10 (value)
          
-         337         514 LOAD_FAST               10 (value)
+         342         514 LOAD_FAST               10 (value)
                      516 LOAD_FAST                5 (kwargs)
                      518 LOAD_FAST                9 (key)
                      520 STORE_SUBSCR
                      524 JUMP_BACKWARD          211 (to 104)
          
-         339     >>  526 LOAD_FAST                8 (split)
+         344     >>  526 LOAD_FAST                8 (split)
                      528 LOAD_CONST               4 (0)
                      530 BINARY_SUBSCR
                      540 STORE_FAST               9 (key)
          
-         342         542 LOAD_FAST                9 (key)
+         347         542 LOAD_FAST                9 (key)
                      544 LOAD_FAST                3 (absolute_tokens)
                      546 CONTAINS_OP              0
                      548 POP_JUMP_FORWARD_IF_FALSE    19 (to 588)
          
-         343         550 LOAD_GLOBAL             13 (NULL + TemplateSyntaxError)
+         348         550 LOAD_GLOBAL             13 (NULL + TemplateSyntaxError)
          
-         344         562 LOAD_CONST               7 ('Keyword argument ')
+         349         562 LOAD_CONST               7 ('Keyword argument ')
                      564 LOAD_FAST                9 (key)
                      566 FORMAT_VALUE             0
                      568 LOAD_CONST               8 (' cannot be resolved; it can only be used as an absolute argument.')
                      570 BUILD_STRING             3
          
-         343         572 PRECALL                  1
+         348         572 PRECALL                  1
                      576 CALL                     1
                      586 RAISE_VARARGS            1
          
-         348     >>  588 LOAD_FAST                0 (parser)
+         353     >>  588 LOAD_FAST                0 (parser)
                      590 LOAD_METHOD              5 (compile_filter)
                      612 LOAD_FAST                8 (split)
                      614 LOAD_CONST               3 (1)
                      616 BINARY_SUBSCR
                      626 PRECALL                  1
                      630 CALL                     1
                      640 LOAD_FAST                5 (kwargs)
                      642 LOAD_FAST                9 (key)
                      644 STORE_SUBSCR
          
-         349         648 LOAD_CONST               5 (True)
+         354         648 LOAD_CONST               5 (True)
                      650 STORE_FAST               4 (had_kwargs)
                      652 EXTENDED_ARG             1
                      654 JUMP_BACKWARD          276 (to 104)
          
-         351     >>  656 LOAD_FAST                2 (kwarg_list)
+         356     >>  656 LOAD_FAST                2 (kwarg_list)
                      658 GET_ITER
                  >>  660 FOR_ITER                24 (to 710)
                      662 STORE_FAST               9 (key)
          
-         352         664 LOAD_FAST                9 (key)
+         357         664 LOAD_FAST                9 (key)
                      666 LOAD_FAST                5 (kwargs)
                      668 CONTAINS_OP              1
                      670 POP_JUMP_FORWARD_IF_FALSE    18 (to 708)
          
-         353         672 LOAD_GLOBAL             13 (NULL + TemplateSyntaxError)
+         358         672 LOAD_GLOBAL             13 (NULL + TemplateSyntaxError)
          
-         354         684 LOAD_CONST               9 ('Missing required keyword argument ')
+         359         684 LOAD_CONST               9 ('Missing required keyword argument ')
                      686 LOAD_FAST                9 (key)
                      688 FORMAT_VALUE             0
                      690 BUILD_STRING             2
          
-         353         692 PRECALL                  1
+         358         692 PRECALL                  1
                      696 CALL                     1
                      706 RAISE_VARARGS            1
          
-         352     >>  708 JUMP_BACKWARD           25 (to 660)
+         357     >>  708 JUMP_BACKWARD           25 (to 660)
          
-         357     >>  710 LOAD_FAST                5 (kwargs)
+         362     >>  710 LOAD_FAST                5 (kwargs)
                      712 RETURN_VALUE
          consts
             None
             False
             '='
             1
             0
@@ -1877,15 +1886,15 @@
             'Missing required keyword argument '
          names      ('tuple', 'enumerate', 'split', 'len', 'ValueError', 'compile_filter', 'TemplateSyntaxError')
          varnames   ('parser', 'tokens', 'kwarg_list', 'absolute_tokens', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key', 'value')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'get_kwargs'
-         firstlineno 309
+         firstlineno 314
          lnotab
             0x02010401040204011c0204011c022a012a014c0114011601020204011e
             023e01260114011601020210012a010c02100308010c010aff10053c0108
             02080108010c0108ff10ff0205
       (None,)
       (None, None)
    names      ('typing', 'Type', 'Any', 'django.template', 'library', 'Node', 'TemplateSyntaxError', 'django.template.context', 'Context', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.utils.html', 'escape', 'django.utils.safestring', 'mark_safe', 'django.core', 'signing', 'wagtail', 'hooks', 'wagtail.models', 'Page', 'PAGE_TEMPLATE_VAR', 'warnings', 'settings', 'TIPPY_ENABLED', 'adapters', 'adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError', 'utils', 'wrap_adapter', 'with_userbar_model', 'base_adapter_context', '_flatten_context', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME', 'FIELD_TEMPLATE_VAR', 'INSTANCE_TEMPLATE_VAR', 'REGISTER_CSS', 'REGISTER_JS', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'str', 'as_var', 'AdapterNode', 'tag', 'do_render_fedit', 'simple_tag', 'render_adapter', 'inclusion_tag', 'dict', 'static_hook_output', 'tooltip', 'do_with_userbar_model', 'list', 'get_kwargs')
@@ -1893,9 +1902,9 @@
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201100114030c0314040c010c010c020c01100508020c0318062c
-      0c10061e030401040318071c6d2a010eff0e0102372a0112ff0e0102152e
+      0c10061e030401040318071c6d2a010eff0e0102372a0112ff0e01021a2e
       010aff0e01021d2c0110ff0e0102122c010eff0e010207
```

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.7/wagtail_fedit/templatetags/fedit.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,26 +227,31 @@
     )
 
 
 @register.simple_tag(takes_context=True)
 def render_adapter(context: Context, adapter: BaseAdapter) -> str:
     adapter_context = {}
     
+    
     if "adapter_context" in context:
         adapter_context = context["adapter_context"]
-        del context["adapter_context"]
 
     context = _flatten_context(
         context,
     )
     adapter_context = _flatten_context(
         adapter_context,
     )
 
-    context.update(adapter_context)
+    if "adapter_context" in context:
+        del context["adapter_context"]
+
+    context.update(
+        adapter_context,
+    )
 
     return adapter.render_content(
         context,
     )
 
 
 @register.inclusion_tag("wagtail_fedit/_hook_output.html", name="fedit_scripts", takes_context=True)
```

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.5.7/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.7/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/test/core/tests/test_model_edit.py` & `wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_model_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.7/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.7/wagtail_fedit/test/testapp/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 """
 
 from pathlib import Path
 
 # Build paths inside the project like this: BASE_DIR / 'subdir'.
 BASE_DIR = Path(__file__).resolve().parent.parent
 
+WAGTAILADMIN_BASE_URL = '/admin/'
 
 # Quick-start development settings - unsuitable for production
 # See https://docs.djangoproject.com/en/5.0/howto/deployment/checklist/
 
 # SECURITY WARNING: keep the secret key used in production secret!
 SECRET_KEY = 'test_key_wagtail_fedit'
```

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.7/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.7/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.7/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.7/wagtail_fedit/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -519,15 +519,15 @@
     if adapter.field_name is not None:
         reverse_kwargs["field_name"] = adapter.field_name
 
     shared = adapter.encode_shared_context()
     js_constructor = adapter.get_js_constructor()
     
     return render_to_string(
-        "wagtail_fedit/content/editable_adapter.html",
+        adapter.get_editable_template_names(),
         {
             "identifier": adapter.identifier,
             "adapter": adapter,
             "buttons": items,
             "shared": shared,
             "unique_id": adapter.get_element_id(),
             "js_constructor": js_constructor,
```

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.5.7/wagtail_fedit/views/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,26 +108,26 @@
             return HttpResponseBadRequest(
                 INVALID.format(
                     _("field name"),
                     self.instance,
                 )
             )
 
-        shared_context = request.GET.get("shared_context")
-        if shared_context:
+        shared_context_str: dict = request.GET.get("shared_context")
+        if shared_context_str:
             self.shared_context = self.adapter_class.decode_shared_context(
                 request,
                 self.instance,
                 field_name,
-                shared_context,
+                shared_context_str,
             )
         else:
             self.shared_context = {}
 
-        self.adapter = self.adapter_class(
+        self.adapter: BaseAdapter = self.adapter_class(
             request=request,
             object=self.instance,
             field_name=field_name,
             **self.shared_context,
         )
 
         if not self.adapter.check_permissions():
@@ -179,17 +179,17 @@
     def get_header_title(self):
         return self.adapter.get_header_title()
 
     def get_help_text(self):
         return self.adapter.get_help_text()
     
     def get_context_data(self, **kwargs):
-        shared_context = None
+        shared_context_str = None
         if self.shared_context:
-            shared_context =\
+            shared_context_str =\
                 self.request.GET["shared_context"]
 
         verbose_name = self.model._meta.verbose_name
         if self.adapter.field_required:
             verbose_name = self.adapter.meta_field.verbose_name
 
         extra = {}
@@ -200,15 +200,16 @@
             extra[PAGE_TEMPLATE_VAR] = self.instance
 
         # Form context; used for rendering the modal.
         if "form" in kwargs:
             extra.update({
                 "verbose_name": verbose_name,
                 "locked_for_user": self.locked_for_user,
-                "shared_context": shared_context,
+                "shared_context": self.shared_context,
+                "shared_context_str": shared_context_str,
                 "form_attrs": self.adapter.get_form_attrs(),
                 "locked": self.lock is not None,
                 **self.adapter.get_form_context(
                     **kwargs,
                 ),
             })
         # Add adapter context instead of form context
```

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.7/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.7/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/wagtail_hooks/adapter_hooks.py` & `wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/adapter_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.5.7/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.5.6
+Version: 1.5.7
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail_fedit-1.5.6/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.7/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,27 +33,28 @@
 wagtail_fedit/locale/nl/LC_MESSAGES/django.po
 wagtail_fedit/migrations/__init__.py
 wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
 wagtail_fedit/static/wagtail_fedit/css/frontend.css
 wagtail_fedit/static/wagtail_fedit/css/furniture.css
 wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
 wagtail_fedit/static/wagtail_fedit/js/edit.js
-wagtail_fedit/static/wagtail_fedit/js/frontend.js
 wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE
 wagtail_fedit/templates/wagtail_fedit/_hook_output.html
 wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+wagtail_fedit/templates/wagtail_fedit/content/editable_dom_positioned_adapter.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe_dom_positioned.html
 wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/field.html
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
```

