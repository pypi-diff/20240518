# Comparing `tmp/coderedcms-3.0.3.tar.gz` & `tmp/coderedcms-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coderedcms-3.0.3.tar", last modified: Thu Jan 11 19:10:44 2024, max compression
+gzip compressed data, was "coderedcms-3.0.4.tar", last modified: Sat May 18 16:38:34 2024, max compression
```

## Comparing `coderedcms-3.0.3.tar` & `coderedcms-3.0.4.tar`

### file list

```diff
@@ -1,567 +1,567 @@
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.892752 coderedcms-3.0.3/
--rw-rw-rw-   0        0        0     1985 2022-08-03 20:24:51.000000 coderedcms-3.0.3/LICENSE
--rw-rw-rw-   0        0        0       94 2022-08-03 20:24:51.000000 coderedcms-3.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6061 2024-01-11 19:10:44.892752 coderedcms-3.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4364 2023-11-03 01:29:15.000000 coderedcms-3.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.499699 coderedcms-3.0.3/coderedcms/
--rw-rw-rw-   0        0        0      827 2024-01-11 19:09:24.000000 coderedcms-3.0.3/coderedcms/__init__.py
--rw-rw-rw-   0        0        0      482 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/admin_urls.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.499699 coderedcms-3.0.3/coderedcms/api/
--rw-rw-rw-   0        0        0     2996 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/api/mailchimp.py
--rw-rw-rw-   0        0        0      331 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/apps.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.499699 coderedcms-3.0.3/coderedcms/bin/
--rw-rw-rw-   0        0        0        0 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/bin/__init__.py
--rw-rw-rw-   0        0        0     5513 2023-11-21 20:09:40.000000 coderedcms-3.0.3/coderedcms/bin/coderedcms.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.515338 coderedcms-3.0.3/coderedcms/blocks/
--rw-rw-rw-   0        0        0     5043 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/blocks/__init__.py
--rw-rw-rw-   0        0        0     9087 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/blocks/base_blocks.py
--rw-rw-rw-   0        0        0     7977 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/blocks/content_blocks.py
--rw-rw-rw-   0        0        0     8169 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/blocks/html_blocks.py
--rw-rw-rw-   0        0        0     2828 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/blocks/layout_blocks.py
--rw-rw-rw-   0        0        0     3856 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/blocks/stream_form_blocks.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.515338 coderedcms-3.0.3/coderedcms/blocks/tests/
--rw-rw-rw-   0        0        0        0 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/blocks/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/blocks/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3201 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/fields.py
--rw-rw-rw-   0        0        0     5856 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/forms.py
--rw-rw-rw-   0        0        0     5656 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/importexport.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.547025 coderedcms-3.0.3/coderedcms/migrations/
--rw-rw-rw-   0        0        0    31791 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1460 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0002_auto_20180829_1538.py
--rw-rw-rw-   0        0        0     1445 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0003_auto_20180912_1632.py
--rw-rw-rw-   0        0        0     1160 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0004_auto_20181119_1507.py
--rw-rw-rw-   0        0        0     2371 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0005_auto_20181214_2214.py
--rw-rw-rw-   0        0        0      945 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0006_mailchimpapisettings.py
--rw-rw-rw-   0        0        0      514 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0007_auto_20190114_1515.py
--rw-rw-rw-   0        0        0     1108 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0008_auto_20190122_1242.py
--rw-rw-rw-   0        0        0      825 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0009_auto_20190201_1546.py
--rw-rw-rw-   0        0        0     1108 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0010_auto_20190320_1231.py
--rw-rw-rw-   0        0        0      618 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0010_generalsettings_email.py
--rw-rw-rw-   0        0        0      340 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0010_remove_generalsettings_robots.py
--rw-rw-rw-   0        0        0      293 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0011_merge_20190322_1309.py
--rw-rw-rw-   0        0        0      280 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0012_merge_20190322_1324.py
--rw-rw-rw-   0        0        0     1328 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0013_pagepreview_templates.py
--rw-rw-rw-   0        0        0     3846 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0014_classifiers.py
--rw-rw-rw-   0        0        0     2799 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0015_coderedsessionformsubmission_coderedsubmissionrevision.py
--rw-rw-rw-   0        0        0     1363 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0016_auto_20191025_1620.py
--rw-rw-rw-   0        0        0      460 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0017_generalsettings_external_new_tab.py
--rw-rw-rw-   0        0        0     1341 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0018_auto_20200805_1702.py
--rw-rw-rw-   0        0        0     1502 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0019_spelling_corrections.py
--rw-rw-rw-   0        0        0      997 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0020_auto_20210527_1030.py
--rw-rw-rw-   0        0        0      838 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0021_auto_20210730_1637.py
--rw-rw-rw-   0        0        0     1561 2023-11-03 22:11:51.000000 coderedcms-3.0.3/coderedcms/migrations/0022_auto_20210731_1853.py
--rw-rw-rw-   0        0        0     1372 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0023_auto_20210908_1702.py
--rw-rw-rw-   0        0        0     1059 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0024_analyticssettings.py
--rw-rw-rw-   0        0        0      311 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0025_delete_socialmediasettings.py
--rw-rw-rw-   0        0        0     1336 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0026_auto_20220513_1627.py
--rw-rw-rw-   0        0        0      608 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0027_auto_20220603_1142.py
--rw-rw-rw-   0        0        0     1915 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0028_auto_20220609_1532.py
--rw-rw-rw-   0        0        0     3522 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0029_multinavs.py
--rw-rw-rw-   0        0        0      587 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0030_alter_coderedtag_tag.py
--rw-rw-rw-   0        0        0     1840 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0031_wagtail3.py
--rw-rw-rw-   0        0        0     1784 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0032_accordion_accordionpanel.py
--rw-rw-rw-   0        0        0     2680 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0033_alter_coderedpage_struct_org_actions_and_more.py
--rw-rw-rw-   0        0        0      488 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0033_remove_carousel_animation_and_more.py
--rw-rw-rw-   0        0        0      319 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0034_delete_adasettings.py
--rw-rw-rw-   0        0        0     3367 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0035_remove_googleapisettings_site_and_more.py
--rw-rw-rw-   0        0        0     3873 2023-11-03 22:11:51.000000 coderedcms-3.0.3/coderedcms/migrations/0036_filmstrip_filmpanel.py
--rw-rw-rw-   0        0        0     1404 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0037_coderedpage_related_classifier_term_and_more.py
--rw-rw-rw-   0        0        0      551 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0038_alter_classifier_slug.py
--rw-rw-rw-   0        0        0      532 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0039_alter_classifierterm_slug.py
--rw-rw-rw-   0        0        0      357 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/0040_remove_analyticssettings_ga_tracking_id.py
--rw-rw-rw-   0        0        0        0 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.547025 coderedcms-3.0.3/coderedcms/models/
--rw-rw-rw-   0        0        0      323 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/models/__init__.py
--rw-rw-rw-   0        0        0     6389 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/models/integration_models.py
--rw-rw-rw-   0        0        0    72483 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/models/page_models.py
--rw-rw-rw-   0        0        0    14702 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/models/snippet_models.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.562664 coderedcms-3.0.3/coderedcms/models/tests/
--rw-rw-rw-   0        0        0        0 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/models/tests/__init__.py
--rw-rw-rw-   0        0        0     4844 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/models/tests/test_navbars_and_footers.py
--rw-rw-rw-   0        0        0     9031 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/models/tests/test_page_models.py
--rw-rw-rw-   0        0        0     1960 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/models/tests/test_wagtailsettings_models.py
--rw-rw-rw-   0        0        0    10348 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/models/wagtailsettings_models.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.467870 coderedcms-3.0.3/coderedcms/project_template/
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.562664 coderedcms-3.0.3/coderedcms/project_template/basic/
--rw-rw-rw-   0        0        0      722 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/project_template/basic/.editorconfig
--rw-rw-rw-   0        0        0      364 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/project_template/basic/.gitattributes
--rw-rw-rw-   0        0        0     5735 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/basic/.gitignore
--rw-rw-rw-   0        0        0      932 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/project_template/basic/README.md
--rw-rw-rw-   0        0        0      289 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/basic/manage.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.562664 coderedcms-3.0.3/coderedcms/project_template/basic/project_name/
--rw-rw-rw-   0        0        0        0 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/project_template/basic/project_name/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.562664 coderedcms-3.0.3/coderedcms/project_template/basic/project_name/settings/
--rw-rw-rw-   0        0        0        0 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/project_template/basic/project_name/settings/__init__.py
--rw-rw-rw-   0        0        0     4834 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/project_template/basic/project_name/settings/base.py
--rw-rw-rw-   0        0        0      388 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/project_template/basic/project_name/settings/dev.py
--rw-rw-rw-   0        0        0     1294 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/basic/project_name/settings/prod.py
--rw-rw-rw-   0        0        0     1266 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/basic/project_name/urls.py
--rw-rw-rw-   0        0        0      444 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/basic/project_name/wsgi.py
--rw-rw-rw-   0        0        0      656 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/basic/pyproject.toml
--rw-rw-rw-   0        0        0      119 2023-03-30 17:43:55.000000 coderedcms-3.0.3/coderedcms/project_template/basic/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.562664 coderedcms-3.0.3/coderedcms/project_template/basic/website/
--rw-rw-rw-   0        0        0        0 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/project_template/basic/website/__init__.py
--rw-rw-rw-   0        0        0       89 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/project_template/basic/website/apps.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.578289 coderedcms-3.0.3/coderedcms/project_template/basic/website/migrations/
--rw-rw-rw-   0        0        0  5770141 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/basic/website/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1440 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/basic/website/migrations/0002_initial_data.py
--rw-rw-rw-   0        0        0        0 2023-10-31 21:37:52.000000 coderedcms-3.0.3/coderedcms/project_template/basic/website/migrations/__init__.py
--rw-rw-rw-   0        0        0     3879 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/basic/website/models.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.467870 coderedcms-3.0.3/coderedcms/project_template/basic/website/static/
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.467870 coderedcms-3.0.3/coderedcms/project_template/basic/website/static/website/
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.578289 coderedcms-3.0.3/coderedcms/project_template/basic/website/static/website/css/
--rw-rw-rw-   0        0        0      219 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/project_template/basic/website/static/website/css/custom.css
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.578289 coderedcms-3.0.3/coderedcms/project_template/basic/website/static/website/js/
--rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/project_template/basic/website/static/website/js/custom.js
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.467870 coderedcms-3.0.3/coderedcms/project_template/basic/website/templates/
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.467870 coderedcms-3.0.3/coderedcms/project_template/basic/website/templates/coderedcms/
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.578289 coderedcms-3.0.3/coderedcms/project_template/basic/website/templates/coderedcms/pages/
--rw-rw-rw-   0        0        0      392 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/project_template/basic/website/templates/coderedcms/pages/base.html
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.578289 coderedcms-3.0.3/coderedcms/project_template/pro/
--rw-rw-rw-   0        0        0      216 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/.cr.ini
--rw-rw-rw-   0        0        0      722 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/.editorconfig
--rw-rw-rw-   0        0        0      364 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/.gitattributes
--rw-rw-rw-   0        0        0     5735 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/.gitignore
--rw-rw-rw-   0        0        0     1695 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/README.md
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.594560 coderedcms-3.0.3/coderedcms/project_template/pro/custom_media/
--rw-rw-rw-   0        0        0        0 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/custom_media/__init__.py
--rw-rw-rw-   0        0        0      172 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/custom_media/admin.py
--rw-rw-rw-   0        0        0      155 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/custom_media/apps.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.594560 coderedcms-3.0.3/coderedcms/project_template/pro/custom_media/migrations/
--rw-rw-rw-   0        0        0     9744 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/custom_media/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/custom_media/migrations/__init__.py
--rw-rw-rw-   0        0        0     1785 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/custom_media/models.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.594560 coderedcms-3.0.3/coderedcms/project_template/pro/custom_user/
--rw-rw-rw-   0        0        0        0 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/custom_user/__init__.py
--rw-rw-rw-   0        0        0     1414 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/custom_user/admin.py
--rw-rw-rw-   0        0        0      153 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/custom_user/apps.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.594560 coderedcms-3.0.3/coderedcms/project_template/pro/custom_user/migrations/
--rw-rw-rw-   0        0        0     4389 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/custom_user/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/custom_user/migrations/__init__.py
--rw-rw-rw-   0        0        0     1918 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/custom_user/models.py
--rw-rw-rw-   0        0        0      289 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/manage.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.594560 coderedcms-3.0.3/coderedcms/project_template/pro/project_name/
--rw-rw-rw-   0        0        0        0 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/project_name/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.594560 coderedcms-3.0.3/coderedcms/project_template/pro/project_name/settings/
--rw-rw-rw-   0        0        0        0 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/project_name/settings/__init__.py
--rw-rw-rw-   0        0        0     5026 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/project_template/pro/project_name/settings/base.py
--rw-rw-rw-   0        0        0      438 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/project_name/settings/dev.py
--rw-rw-rw-   0        0        0     1294 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/project_name/settings/prod.py
--rw-rw-rw-   0        0        0     1266 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/project_name/urls.py
--rw-rw-rw-   0        0        0      444 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/project_name/wsgi.py
--rw-rw-rw-   0        0        0      656 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/pyproject.toml
--rw-rw-rw-   0        0        0      150 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/requirements-dev.txt
--rw-rw-rw-   0        0        0      251 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.594560 coderedcms-3.0.3/coderedcms/project_template/pro/website/
--rw-rw-rw-   0        0        0        0 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/website/__init__.py
--rw-rw-rw-   0        0        0       89 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/website/apps.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.609757 coderedcms-3.0.3/coderedcms/project_template/pro/website/migrations/
--rw-rw-rw-   0        0        0  5770141 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/website/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1440 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/website/migrations/0002_initial_data.py
--rw-rw-rw-   0        0        0        0 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/website/migrations/__init__.py
--rw-rw-rw-   0        0        0     3879 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/website/models.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.467870 coderedcms-3.0.3/coderedcms/project_template/pro/website/static/
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.467870 coderedcms-3.0.3/coderedcms/project_template/pro/website/static/website/
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.609757 coderedcms-3.0.3/coderedcms/project_template/pro/website/static/website/js/
--rw-rw-rw-   0        0        0        0 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/website/static/website/js/custom.js
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.609757 coderedcms-3.0.3/coderedcms/project_template/pro/website/static/website/src/
--rw-rw-rw-   0        0        0     1974 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/website/static/website/src/_variables.scss
--rw-rw-rw-   0        0        0     1001 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/website/static/website/src/custom.scss
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.467870 coderedcms-3.0.3/coderedcms/project_template/pro/website/templates/
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.467870 coderedcms-3.0.3/coderedcms/project_template/pro/website/templates/coderedcms/
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.609757 coderedcms-3.0.3/coderedcms/project_template/pro/website/templates/coderedcms/pages/
--rw-rw-rw-   0        0        0      913 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/project_template/pro/website/templates/coderedcms/pages/base.html
--rw-rw-rw-   0        0        0      125 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/search_urls.py
--rw-rw-rw-   0        0        0     9433 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/settings.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.467870 coderedcms-3.0.3/coderedcms/static/
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.467870 coderedcms-3.0.3/coderedcms/static/coderedcms/
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.609757 coderedcms-3.0.3/coderedcms/static/coderedcms/css/
--rw-rw-rw-   0        0        0     1705 2023-11-21 20:09:40.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/css/crx-admin.css
--rw-rw-rw-   0        0        0     5642 2023-11-01 21:37:22.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/css/crx-front.css
--rw-rw-rw-   0        0        0     5628 2023-04-21 16:47:29.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/css/crx-front.css.map
--rw-rw-rw-   0        0        0     4620 2023-11-01 21:37:22.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/css/crx-front.min.css
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.625400 coderedcms-3.0.3/coderedcms/static/coderedcms/js/
--rw-rw-rw-   0        0        0      717 2023-11-01 21:37:22.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/js/crx-editor.js
--rw-rw-rw-   0        0        0     1488 2023-11-01 21:37:22.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/js/crx-events.js
--rw-rw-rw-   0        0        0     5742 2023-11-01 21:37:22.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/js/crx-front.js
--rw-rw-rw-   0        0        0     5256 2023-11-01 21:37:22.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/js/crx-maps.js
--rw-rw-rw-   0        0        0     1805 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/js/crx-streamforms.js
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.631905 coderedcms-3.0.3/coderedcms/static/coderedcms/scss/
--rw-rw-rw-   0        0        0      205 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/scss/_crx-article.scss
--rw-rw-rw-   0        0        0      367 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/scss/_crx-bs-overrides.scss
--rw-rw-rw-   0        0        0      330 2023-04-21 16:47:29.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/scss/_crx-filmstrip.scss
--rw-rw-rw-   0        0        0      152 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/scss/_crx-gallery.scss
--rw-rw-rw-   0        0        0      318 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/scss/_crx-hero.scss
--rw-rw-rw-   0        0        0     1749 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/scss/_crx-location.scss
--rw-rw-rw-   0        0        0     1988 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/scss/_crx-navbar.scss
--rw-rw-rw-   0        0        0      818 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/scss/_crx-pricelist.scss
--rw-rw-rw-   0        0        0      222 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/scss/_crx-richtext.scss
--rw-rw-rw-   0        0        0      429 2023-11-01 21:37:22.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/scss/crx-front.scss
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.467870 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.631905 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/
--rw-rw-rw-   0        0        0     1093 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/LICENSE
--rw-rw-rw-   0        0        0      130 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/README.txt
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.484031 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.672702 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/
--rw-rw-rw-   0        0        0    70329 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css
--rw-rw-rw-   0        0        0   203178 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css.map
--rw-rw-rw-   0        0        0    51795 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css
--rw-rw-rw-   0        0        0   115987 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css.map
--rw-rw-rw-   0        0        0    70403 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.css
--rw-rw-rw-   0        0        0   203182 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.css.map
--rw-rw-rw-   0        0        0    51870 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.min.css
--rw-rw-rw-   0        0        0   116064 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map
--rw-rw-rw-   0        0        0    12065 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css
--rw-rw-rw-   0        0        0   129327 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css.map
--rw-rw-rw-   0        0        0    10126 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css
--rw-rw-rw-   0        0        0    51369 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css.map
--rw-rw-rw-   0        0        0    12058 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.css
--rw-rw-rw-   0        0        0   129342 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.css.map
--rw-rw-rw-   0        0        0    10198 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.min.css
--rw-rw-rw-   0        0        0    63943 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map
--rw-rw-rw-   0        0        0   107823 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.css
--rw-rw-rw-   0        0        0   267491 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.css.map
--rw-rw-rw-   0        0        0    85352 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.min.css
--rw-rw-rw-   0        0        0   180381 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.min.css.map
--rw-rw-rw-   0        0        0   107691 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.css
--rw-rw-rw-   0        0        0   267432 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.css.map
--rw-rw-rw-   0        0        0    85281 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.min.css
--rw-rw-rw-   0        0        0   180217 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map
--rw-rw-rw-   0        0        0   280813 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css
--rw-rw-rw-   0        0        0   679011 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css.map
--rw-rw-rw-   0        0        0   232948 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css
--rw-rw-rw-   0        0        0   589161 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css.map
--rw-rw-rw-   0        0        0   280392 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.css
--rw-rw-rw-   0        0        0   678856 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.css.map
--rw-rw-rw-   0        0        0   233055 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.min.css
--rw-rw-rw-   0        0        0   588695 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.min.css.map
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.688347 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/
--rw-rw-rw-   0        0        0   207731 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js
--rw-rw-rw-   0        0        0   444286 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js.map
--rw-rw-rw-   0        0        0    80663 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   331886 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0        0        0   135747 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.js
--rw-rw-rw-   0        0        0   305152 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.js.map
--rw-rw-rw-   0        0        0    74154 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.min.js
--rw-rw-rw-   0        0        0   222462 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.min.js.map
--rw-rw-rw-   0        0        0   145313 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js
--rw-rw-rw-   0        0        0   306320 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js.map
--rw-rw-rw-   0        0        0    60577 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js
--rw-rw-rw-   0        0        0   220350 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js.map
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.484031 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.688347 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/
--rw-rw-rw-   0        0        0     1903 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/alert.js
--rw-rw-rw-   0        0        0     1932 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/base-component.js
--rw-rw-rw-   0        0        0     1625 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/button.js
--rw-rw-rw-   0        0        0    11817 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/carousel.js
--rw-rw-rw-   0        0        0     7594 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/collapse.js
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.703953 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dom/
--rw-rw-rw-   0        0        0     1395 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dom/data.js
--rw-rw-rw-   0        0        0     8351 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dom/event-handler.js
--rw-rw-rw-   0        0        0     1658 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dom/manipulator.js
--rw-rw-rw-   0        0        0     3381 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dom/selector-engine.js
--rw-rw-rw-   0        0        0    13205 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dropdown.js
--rw-rw-rw-   0        0        0     9581 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/modal.js
--rw-rw-rw-   0        0        0     6806 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/offcanvas.js
--rw-rw-rw-   0        0        0     1870 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/popover.js
--rw-rw-rw-   0        0        0     8472 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/scrollspy.js
--rw-rw-rw-   0        0        0     9068 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tab.js
--rw-rw-rw-   0        0        0     5039 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/toast.js
--rw-rw-rw-   0        0        0    16029 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tooltip.js
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.703953 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/
--rw-rw-rw-   0        0        0     3125 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/backdrop.js
--rw-rw-rw-   0        0        0     1114 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/component-functions.js
--rw-rw-rw-   0        0        0     1784 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/config.js
--rw-rw-rw-   0        0        0     2518 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/focustrap.js
--rw-rw-rw-   0        0        0     7640 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/index.js
--rw-rw-rw-   0        0        0     2933 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/sanitizer.js
--rw-rw-rw-   0        0        0     3754 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/scrollbar.js
--rw-rw-rw-   0        0        0     3409 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/swipe.js
--rw-rw-rw-   0        0        0     3612 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/template-factory.js
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.735646 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/
--rw-rw-rw-   0        0        0     5066 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_accordion.scss
--rw-rw-rw-   0        0        0     2073 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_alert.scss
--rw-rw-rw-   0        0        0     1118 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_badge.scss
--rw-rw-rw-   0        0        0     1751 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_breadcrumb.scss
--rw-rw-rw-   0        0        0     3201 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_button-group.scss
--rw-rw-rw-   0        0        0     6746 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_buttons.scss
--rw-rw-rw-   0        0        0     6979 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_card.scss
--rw-rw-rw-   0        0        0     5879 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_carousel.scss
--rw-rw-rw-   0        0        0     2018 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_close.scss
--rw-rw-rw-   0        0        0     1201 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_containers.scss
--rw-rw-rw-   0        0        0     8093 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_dropdown.scss
--rw-rw-rw-   0        0        0      256 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_forms.scss
--rw-rw-rw-   0        0        0    10554 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_functions.scss
--rw-rw-rw-   0        0        0      683 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_grid.scss
--rw-rw-rw-   0        0        0      353 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_helpers.scss
--rw-rw-rw-   0        0        0     1158 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_images.scss
--rw-rw-rw-   0        0        0     6852 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_list-group.scss
--rw-rw-rw-   0        0        0     6005 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_maps.scss
--rw-rw-rw-   0        0        0      875 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_mixins.scss
--rw-rw-rw-   0        0        0     7762 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_modal.scss
--rw-rw-rw-   0        0        0     5211 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_nav.scss
--rw-rw-rw-   0        0        0     9155 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_navbar.scss
--rw-rw-rw-   0        0        0     4725 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_offcanvas.scss
--rw-rw-rw-   0        0        0     3947 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_pagination.scss
--rw-rw-rw-   0        0        0      859 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_placeholders.scss
--rw-rw-rw-   0        0        0     6907 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_popover.scss
--rw-rw-rw-   0        0        0     2016 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_progress.scss
--rw-rw-rw-   0        0        0    12438 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_reboot.scss
--rw-rw-rw-   0        0        0     6924 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_root.scss
--rw-rw-rw-   0        0        0     2429 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_spinners.scss
--rw-rw-rw-   0        0        0     4945 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_tables.scss
--rw-rw-rw-   0        0        0     2490 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_toasts.scss
--rw-rw-rw-   0        0        0     4281 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_tooltip.scss
--rw-rw-rw-   0        0        0      425 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_transitions.scss
--rw-rw-rw-   0        0        0     1420 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_type.scss
--rw-rw-rw-   0        0        0    19235 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_utilities.scss
--rw-rw-rw-   0        0        0     5057 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_variables-dark.scss
--rw-rw-rw-   0        0        0    76286 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_variables.scss
--rw-rw-rw-   0        0        0     1183 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap-grid.scss
--rw-rw-rw-   0        0        0      189 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap-reboot.scss
--rw-rw-rw-   0        0        0      306 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap-utilities.scss
--rw-rw-rw-   0        0        0      938 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap.scss
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.751320 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/
--rw-rw-rw-   0        0        0     2688 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_floating-labels.scss
--rw-rw-rw-   0        0        0     4851 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-check.scss
--rw-rw-rw-   0        0        0     6590 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-control.scss
--rw-rw-rw-   0        0        0     2796 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-range.scss
--rw-rw-rw-   0        0        0     2488 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-select.scss
--rw-rw-rw-   0        0        0      219 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-text.scss
--rw-rw-rw-   0        0        0     3899 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_input-group.scss
--rw-rw-rw-   0        0        0     1142 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_labels.scss
--rw-rw-rw-   0        0        0      478 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_validation.scss
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.751320 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/
--rw-rw-rw-   0        0        0       37 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_clearfix.scss
--rw-rw-rw-   0        0        0      403 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_color-bg.scss
--rw-rw-rw-   0        0        0     1755 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_colored-links.scss
--rw-rw-rw-   0        0        0      385 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_focus-ring.scss
--rw-rw-rw-   0        0        0      605 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_icon-link.scss
--rw-rw-rw-   0        0        0      621 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_position.scss
--rw-rw-rw-   0        0        0      399 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_ratio.scss
--rw-rw-rw-   0        0        0      245 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_stacks.scss
--rw-rw-rw-   0        0        0      223 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_stretched-link.scss
--rw-rw-rw-   0        0        0       73 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_text-truncation.scss
--rw-rw-rw-   0        0        0      136 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_visually-hidden.scss
--rw-rw-rw-   0        0        0      160 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_vr.scss
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.782542 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/
--rw-rw-rw-   0        0        0      525 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_alert.scss
--rw-rw-rw-   0        0        0      328 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_backdrop.scss
--rw-rw-rw-   0        0        0      223 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_banner.scss
--rw-rw-rw-   0        0        0     2031 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_border-radius.scss
--rw-rw-rw-   0        0        0      398 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_box-shadow.scss
--rw-rw-rw-   0        0        0     4580 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_breakpoints.scss
--rw-rw-rw-   0        0        0     3220 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_buttons.scss
--rw-rw-rw-   0        0        0     1587 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_caret.scss
--rw-rw-rw-   0        0        0      147 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_clearfix.scss
--rw-rw-rw-   0        0        0      447 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_color-mode.scss
--rw-rw-rw-   0        0        0      167 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_color-scheme.scss
--rw-rw-rw-   0        0        0      410 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_container.scss
--rw-rw-rw-   0        0        0      613 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_deprecate.scss
--rw-rw-rw-   0        0        0     4164 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_forms.scss
--rw-rw-rw-   0        0        0     1956 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_gradients.scss
--rw-rw-rw-   0        0        0     4735 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_grid.scss
--rw-rw-rw-   0        0        0      395 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_image.scss
--rw-rw-rw-   0        0        0      581 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_list-group.scss
--rw-rw-rw-   0        0        0      168 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_lists.scss
--rw-rw-rw-   0        0        0      387 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_pagination.scss
--rw-rw-rw-   0        0        0      495 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_reset-text.scss
--rw-rw-rw-   0        0        0      202 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_resize.scss
--rw-rw-rw-   0        0        0     1101 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_table-variants.scss
--rw-rw-rw-   0        0        0      168 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_text-truncate.scss
--rw-rw-rw-   0        0        0      661 2023-10-31 18:32:58.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_transition.scss
--rw-rw-rw-   0        0        0     3384 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_utilities.scss
--rw-rw-rw-   0        0        0     1110 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_visually-hidden.scss
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.782542 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/
--rw-rw-rw-   0        0        0      449 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/jasmine.js
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.782542 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/mixins/
--rw-rw-rw-   0        0        0     1859 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/mixins/_color-modes.test.scss
--rw-rw-rw-   0        0        0      246 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/mixins/_media-query-color-mode-full.test.scss
--rw-rw-rw-   0        0        0     8772 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/mixins/_utilities.test.scss
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.782542 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/sass-true/
--rw-rw-rw-   0        0        0      377 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/sass-true/register.js
--rw-rw-rw-   0        0        0      450 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/sass-true/runner.js
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.782542 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/utilities/
--rw-rw-rw-   0        0        0     1462 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/utilities/_api.test.scss
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.782542 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/utilities/
--rw-rw-rw-   0        0        0     1737 2023-10-31 18:32:59.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/utilities/_api.scss
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.782542 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/vendor/
--rw-rw-rw-   0        0        0    10012 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/vendor/_rfs.scss
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.782542 coderedcms-3.0.3/coderedcms/templates/
--rw-rw-rw-   0        0        0      280 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/404.html
--rw-rw-rw-   0        0        0      725 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/templates/500.html
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.484031 coderedcms-3.0.3/coderedcms/templates/coderedcms/
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.829438 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/
--rw-rw-rw-   0        0        0     1129 2023-02-17 20:46:38.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/accordion_block.html
--rw-rw-rw-   0        0        0      791 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/article_block_card.html
--rw-rw-rw-   0        0        0      173 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/base_block.html
--rw-rw-rw-   0        0        0     1789 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/base_link_block.html
--rw-rw-rw-   0        0        0      617 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/button_block.html
--rw-rw-rw-   0        0        0      734 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/card_block.html
--rw-rw-rw-   0        0        0      840 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/card_blurb.html
--rw-rw-rw-   0        0        0      771 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/card_foot.html
--rw-rw-rw-   0        0        0      720 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/card_head.html
--rw-rw-rw-   0        0        0      757 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/card_head_foot.html
--rw-rw-rw-   0        0        0      775 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/card_img.html
--rw-rw-rw-   0        0        0      368 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/cardgrid_columns.html
--rw-rw-rw-   0        0        0      278 2023-02-17 20:46:38.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/cardgrid_deck.html
--rw-rw-rw-   0        0        0      262 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/cardgrid_group.html
--rw-rw-rw-   0        0        0     2154 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/carousel_block.html
--rw-rw-rw-   0        0        0      389 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/column_block.html
--rw-rw-rw-   0        0        0      833 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/content_wall_block.html
--rw-rw-rw-   0        0        0      141 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/document_link_block.html
--rw-rw-rw-   0        0        0      732 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/download_block.html
--rw-rw-rw-   0        0        0      105 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/embed_video_block.html
--rw-rw-rw-   0        0        0       99 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/external_link_block.html
--rw-rw-rw-   0        0        0     1453 2023-07-12 20:31:45.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/film_strip_block.html
--rw-rw-rw-   0        0        0      582 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/google_map.html
--rw-rw-rw-   0        0        0      374 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/grid_block.html
--rw-rw-rw-   0        0        0      198 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/h1_block.html
--rw-rw-rw-   0        0        0      198 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/h2_block.html
--rw-rw-rw-   0        0        0      198 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/h3_block.html
--rw-rw-rw-   0        0        0      846 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/hero_block.html
--rw-rw-rw-   0        0        0      299 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/image_block.html
--rw-rw-rw-   0        0        0     1196 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/image_gallery_block.html
--rw-rw-rw-   0        0        0      631 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/image_link_block.html
--rw-rw-rw-   0        0        0      992 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/modal_block.html
--rw-rw-rw-   0        0        0      167 2023-02-09 20:20:28.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/page_link_block.html
--rw-rw-rw-   0        0        0      444 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/pagelist_article_card_columns.html
--rw-rw-rw-   0        0        0      392 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/pagelist_article_card_deck.html
--rw-rw-rw-   0        0        0      324 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/pagelist_article_card_group.html
--rw-rw-rw-   0        0        0      916 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/pagelist_article_media.html
--rw-rw-rw-   0        0        0      320 2023-04-21 16:47:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/pagelist_block.html
--rw-rw-rw-   0        0        0      561 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/pagelist_list_group.html
--rw-rw-rw-   0        0        0      204 2023-04-21 16:47:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/pagepreview_block.html
--rw-rw-rw-   0        0        0      803 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/pagepreview_card.html
--rw-rw-rw-   0        0        0     1009 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/pagepreview_form.html
--rw-rw-rw-   0        0        0      227 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/pricelist_block.html
--rw-rw-rw-   0        0        0      533 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/pricelistitem_block.html
--rw-rw-rw-   0        0        0      347 2023-07-12 20:31:45.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/quote_block.html
--rw-rw-rw-   0        0        0      258 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/reusable_content_block.html
--rw-rw-rw-   0        0        0       86 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/rich_text_block.html
--rw-rw-rw-   0        0        0      877 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/table_block.html
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.831972 coderedcms-3.0.3/coderedcms/templates/coderedcms/formfields/
--rw-rw-rw-   0        0        0      266 2023-10-31 19:00:50.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/formfields/date.html
--rw-rw-rw-   0        0        0      411 2023-11-21 20:09:40.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/formfields/datetime.html
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.831972 coderedcms-3.0.3/coderedcms/templates/coderedcms/formfields/mailchimp/
--rw-rw-rw-   0        0        0     6685 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/formfields/mailchimp/subscriber_integration_js.html
--rw-rw-rw-   0        0        0      793 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/formfields/mailchimp/subscriber_integration_widget.html
--rw-rw-rw-   0        0        0      263 2023-10-31 19:00:50.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/formfields/time.html
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.847455 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/
--rw-rw-rw-   0        0        0      465 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-align-left.svg
--rw-rw-rw-   0        0        0      573 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-check-square-o.svg
--rw-rw-rw-   0        0        0      277 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-columns.svg
--rw-rw-rw-   0        0        0      359 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-desktop.svg
--rw-rw-rw-   0        0        0      571 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-font.svg
--rw-rw-rw-   0        0        0      292 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-google.svg
--rw-rw-rw-   0        0        0      813 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-hand-pointer-o.svg
--rw-rw-rw-   0        0        0      666 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-hashtag.svg
--rw-rw-rw-   0        0        0      840 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-header.svg
--rw-rw-rw-   0        0        0      835 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-list-alt.svg
--rw-rw-rw-   0        0        0      459 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-map.svg
--rw-rw-rw-   0        0        0      448 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-newspaper-o.svg
--rw-rw-rw-   0        0        0      721 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-puzzle-piece.svg
--rw-rw-rw-   0        0        0      635 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-recycle.svg
--rw-rw-rw-   0        0        0      174 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-stop.svg
--rw-rw-rw-   0        0        0      505 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-th-large.svg
--rw-rw-rw-   0        0        0      762 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-universal-access.svg
--rw-rw-rw-   0        0        0      548 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-usd.svg
--rw-rw-rw-   0        0        0      225 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-window-maximize.svg
--rw-rw-rw-   0        0        0      199 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-window-minimize.svg
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.847455 coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/
--rw-rw-rw-   0        0        0      714 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/classifier_dropdowns.html
--rw-rw-rw-   0        0        0      534 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/classifier_nav.html
--rw-rw-rw-   0        0        0      296 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/crx_banner.html
--rw-rw-rw-   0        0        0      262 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/form_honeypot.html
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.847455 coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/ical/
--rw-rw-rw-   0        0        0      531 2023-10-31 19:00:50.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/ical/calendar.html
--rw-rw-rw-   0        0        0      365 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/ical/calendar_ical_button.html
--rw-rw-rw-   0        0        0      406 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/ical/recurring_ical_button.html
--rw-rw-rw-   0        0        0      565 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/ical/single_ical_button.html
--rw-rw-rw-   0        0        0      261 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/iframe_gmap.html
--rw-rw-rw-   0        0        0      320 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/map_list_description.html
--rw-rw-rw-   0        0        0      107 2022-08-04 15:54:45.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/map_pin_description.html
--rw-rw-rw-   0        0        0      983 2023-03-30 19:10:04.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/pagination.html
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.847455 coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/stream_forms/
--rw-rw-rw-   0        0        0      533 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/stream_forms/render_field.html
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.861484 coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/
--rw-rw-rw-   0        0        0     1526 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/article_index_page.html
--rw-rw-rw-   0        0        0     1332 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/article_page.html
--rw-rw-rw-   0        0        0     1094 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/article_page.search.html
--rw-rw-rw-   0        0        0     7594 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/base.html
--rw-rw-rw-   0        0        0     1929 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/event_index_page.html
--rw-rw-rw-   0        0        0     1846 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/event_page.html
--rw-rw-rw-   0        0        0     1001 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/form_page.html
--rw-rw-rw-   0        0        0      921 2023-04-21 16:47:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/form_page.mini.html
--rw-rw-rw-   0        0        0      244 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/form_page_landing.html
--rw-rw-rw-   0        0        0       55 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/home_page.html
--rw-rw-rw-   0        0        0     1580 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/location_index_page.html
--rw-rw-rw-   0        0        0      858 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/location_page.html
--rw-rw-rw-   0        0        0      505 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/page.mini.html
--rw-rw-rw-   0        0        0     2605 2023-11-27 22:26:53.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/search.html
--rw-rw-rw-   0        0        0      417 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/search_result.html
--rw-rw-rw-   0        0        0     2525 2023-11-01 21:37:22.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/stream_form_page.html
--rw-rw-rw-   0        0        0      528 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/web_page.html
--rw-rw-rw-   0        0        0      209 2023-04-21 16:47:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/web_page_notitle.html
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.861484 coderedcms-3.0.3/coderedcms/templates/coderedcms/snippets/
--rw-rw-rw-   0        0        0      471 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/snippets/footer.html
--rw-rw-rw-   0        0        0     2424 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/snippets/navbar.html
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.861484 coderedcms-3.0.3/coderedcms/templates/coderedcms/widgets/
--rw-rw-rw-   0        0        0     1245 2023-11-01 21:37:22.000000 coderedcms-3.0.3/coderedcms/templates/coderedcms/widgets/checkbox_classifiers.html
--rw-rw-rw-   0        0        0      118 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/robots.txt
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.861484 coderedcms-3.0.3/coderedcms/templates/wagtailadmin/
--rw-rw-rw-   0        0        0      728 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/templates/wagtailadmin/base.html
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.877156 coderedcms-3.0.3/coderedcms/templates/wagtailadmin/block_forms/
--rw-rw-rw-   0        0        0      716 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html
--rw-rw-rw-   0        0        0       95 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/wagtailadmin/home.html
--rw-rw-rw-   0        0        0      177 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/wagtailadmin/login.html
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.877156 coderedcms-3.0.3/coderedcms/templates/wagtailcore/
--rw-rw-rw-   0        0        0      692 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/wagtailcore/password_required.html
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.877156 coderedcms-3.0.3/coderedcms/templates/wagtailembeds/
--rw-rw-rw-   0        0        0      522 2023-02-09 20:20:29.000000 coderedcms-3.0.3/coderedcms/templates/wagtailembeds/embed_frontend.html
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.877156 coderedcms-3.0.3/coderedcms/templates/wagtailforms/
--rw-rw-rw-   0        0        0     1528 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/wagtailforms/list_submissions.html
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.877156 coderedcms-3.0.3/coderedcms/templates/wagtailimportexport/
--rw-rw-rw-   0        0        0     1396 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/wagtailimportexport/import_from_csv.html
--rw-rw-rw-   0        0        0      470 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/templates/wagtailimportexport/index.html
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.877156 coderedcms-3.0.3/coderedcms/templatetags/
--rw-rw-rw-   0        0        0     5877 2023-10-31 21:37:54.000000 coderedcms-3.0.3/coderedcms/templatetags/coderedcms_tags.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.877156 coderedcms-3.0.3/coderedcms/tests/
--rw-rw-rw-   0        0        0     5157 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/tests/settings.py
--rw-rw-rw-   0        0        0     2805 2023-11-13 16:26:32.000000 coderedcms-3.0.3/coderedcms/tests/test_bin.py
--rw-rw-rw-   0        0        0     1593 2023-10-31 21:37:54.000000 coderedcms-3.0.3/coderedcms/tests/test_templates.py
--rw-rw-rw-   0        0        0      821 2023-10-31 21:37:54.000000 coderedcms-3.0.3/coderedcms/tests/test_templatetags.py
--rw-rw-rw-   0        0        0    12176 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/tests/test_urls.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.877156 coderedcms-3.0.3/coderedcms/tests/testapp/
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.892752 coderedcms-3.0.3/coderedcms/tests/testapp/migrations/
--rw-rw-rw-   0        0        0   257599 2023-11-01 18:36:21.000000 coderedcms-3.0.3/coderedcms/tests/testapp/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1481 2023-10-31 21:37:54.000000 coderedcms-3.0.3/coderedcms/tests/testapp/migrations/0002_initial.py
--rw-rw-rw-   0        0        0   250426 2023-10-31 21:37:54.000000 coderedcms-3.0.3/coderedcms/tests/testapp/migrations/0003_eventindexpage_eventoccurrence_eventpage_locationindexpage_locationpage.py
--rw-rw-rw-   0        0        0   101517 2023-10-31 21:37:54.000000 coderedcms-3.0.3/coderedcms/tests/testapp/migrations/0004_streamformconfirmemail_streamformpage.py
--rw-rw-rw-   0        0        0   346621 2023-10-31 21:37:54.000000 coderedcms-3.0.3/coderedcms/tests/testapp/migrations/0005_auto_20210908_1741.py
--rw-rw-rw-   0        0        0      770 2023-10-31 21:37:54.000000 coderedcms-3.0.3/coderedcms/tests/testapp/migrations/0006_indextestpage.py
--rw-rw-rw-   0        0        0     1011 2023-10-31 21:37:54.000000 coderedcms-3.0.3/coderedcms/tests/testapp/migrations/0007_auto_20210910_1614.py
--rw-rw-rw-   0        0        0        0 2023-10-31 21:37:54.000000 coderedcms-3.0.3/coderedcms/tests/testapp/migrations/__init__.py
--rw-rw-rw-   0        0        0     3991 2023-10-31 21:37:54.000000 coderedcms-3.0.3/coderedcms/tests/testapp/models.py
--rw-rw-rw-   0        0        0      519 2023-10-31 21:37:54.000000 coderedcms-3.0.3/coderedcms/tests/urls.py
--rw-rw-rw-   0        0        0     1470 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/urls.py
--rw-rw-rw-   0        0        0     1390 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/utils.py
--rw-rw-rw-   0        0        0    11286 2024-01-11 19:08:54.000000 coderedcms-3.0.3/coderedcms/views.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.892752 coderedcms-3.0.3/coderedcms/wagtail_flexible_forms/
--rw-rw-rw-   0        0        0     1506 2022-08-03 20:24:51.000000 coderedcms-3.0.3/coderedcms/wagtail_flexible_forms/LICENSE
--rw-rw-rw-   0        0        0     7670 2023-10-31 21:37:54.000000 coderedcms-3.0.3/coderedcms/wagtail_flexible_forms/blocks.py
--rw-rw-rw-   0        0        0     1191 2023-10-31 21:37:54.000000 coderedcms-3.0.3/coderedcms/wagtail_flexible_forms/edit_handlers.py
--rw-rw-rw-   0        0        0    30401 2023-10-31 21:37:54.000000 coderedcms-3.0.3/coderedcms/wagtail_flexible_forms/models.py
--rw-rw-rw-   0        0        0     4763 2023-11-21 20:09:40.000000 coderedcms-3.0.3/coderedcms/wagtail_hooks.py
--rw-rw-rw-   0        0        0     1473 2023-10-31 21:37:51.000000 coderedcms-3.0.3/coderedcms/widgets.py
-drwxrwxrwx   0        0        0        0 2024-01-11 19:10:44.892752 coderedcms-3.0.3/coderedcms.egg-info/
--rw-rw-rw-   0        0        0     6061 2024-01-11 19:10:44.000000 coderedcms-3.0.3/coderedcms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    28416 2024-01-11 19:10:44.000000 coderedcms-3.0.3/coderedcms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-11 19:10:44.000000 coderedcms-3.0.3/coderedcms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-01-11 19:10:44.000000 coderedcms-3.0.3/coderedcms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-08-04 17:39:55.000000 coderedcms-3.0.3/coderedcms.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      186 2024-01-11 19:10:44.000000 coderedcms-3.0.3/coderedcms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-01-11 19:10:44.000000 coderedcms-3.0.3/coderedcms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      299 2023-02-09 20:20:29.000000 coderedcms-3.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      384 2024-01-11 19:10:44.892752 coderedcms-3.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2180 2024-01-11 19:08:54.000000 coderedcms-3.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.181795 coderedcms-3.0.4/
+-rw-rw-rw-   0        0        0     1985 2022-08-03 20:24:51.000000 coderedcms-3.0.4/LICENSE
+-rw-rw-rw-   0        0        0       94 2022-08-03 20:24:51.000000 coderedcms-3.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6061 2024-05-18 16:38:34.181795 coderedcms-3.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4364 2023-11-03 01:29:15.000000 coderedcms-3.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.916163 coderedcms-3.0.4/coderedcms/
+-rw-rw-rw-   0        0        0      827 2024-05-18 16:34:32.000000 coderedcms-3.0.4/coderedcms/__init__.py
+-rw-rw-rw-   0        0        0      482 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/admin_urls.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.916163 coderedcms-3.0.4/coderedcms/api/
+-rw-rw-rw-   0        0        0     2996 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/api/mailchimp.py
+-rw-rw-rw-   0        0        0      331 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.916163 coderedcms-3.0.4/coderedcms/bin/
+-rw-rw-rw-   0        0        0        0 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/bin/__init__.py
+-rw-rw-rw-   0        0        0     5513 2023-11-21 20:09:40.000000 coderedcms-3.0.4/coderedcms/bin/coderedcms.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.931808 coderedcms-3.0.4/coderedcms/blocks/
+-rw-rw-rw-   0        0        0     5043 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/blocks/__init__.py
+-rw-rw-rw-   0        0        0     9087 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/blocks/base_blocks.py
+-rw-rw-rw-   0        0        0     7977 2024-05-18 16:33:43.000000 coderedcms-3.0.4/coderedcms/blocks/content_blocks.py
+-rw-rw-rw-   0        0        0     8169 2024-05-18 16:33:43.000000 coderedcms-3.0.4/coderedcms/blocks/html_blocks.py
+-rw-rw-rw-   0        0        0     2828 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/blocks/layout_blocks.py
+-rw-rw-rw-   0        0        0     3856 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/blocks/stream_form_blocks.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.931808 coderedcms-3.0.4/coderedcms/blocks/tests/
+-rw-rw-rw-   0        0        0        0 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/blocks/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/blocks/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3201 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/fields.py
+-rw-rw-rw-   0        0        0     5856 2024-05-18 16:33:43.000000 coderedcms-3.0.4/coderedcms/forms.py
+-rw-rw-rw-   0        0        0     5656 2024-05-18 16:33:43.000000 coderedcms-3.0.4/coderedcms/importexport.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.947428 coderedcms-3.0.4/coderedcms/migrations/
+-rw-rw-rw-   0        0        0    31791 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1460 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0002_auto_20180829_1538.py
+-rw-rw-rw-   0        0        0     1445 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0003_auto_20180912_1632.py
+-rw-rw-rw-   0        0        0     1160 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0004_auto_20181119_1507.py
+-rw-rw-rw-   0        0        0     2371 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0005_auto_20181214_2214.py
+-rw-rw-rw-   0        0        0      945 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0006_mailchimpapisettings.py
+-rw-rw-rw-   0        0        0      514 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0007_auto_20190114_1515.py
+-rw-rw-rw-   0        0        0     1108 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0008_auto_20190122_1242.py
+-rw-rw-rw-   0        0        0      825 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0009_auto_20190201_1546.py
+-rw-rw-rw-   0        0        0     1108 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0010_auto_20190320_1231.py
+-rw-rw-rw-   0        0        0      618 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0010_generalsettings_email.py
+-rw-rw-rw-   0        0        0      340 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0010_remove_generalsettings_robots.py
+-rw-rw-rw-   0        0        0      293 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0011_merge_20190322_1309.py
+-rw-rw-rw-   0        0        0      280 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0012_merge_20190322_1324.py
+-rw-rw-rw-   0        0        0     1328 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0013_pagepreview_templates.py
+-rw-rw-rw-   0        0        0     3846 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0014_classifiers.py
+-rw-rw-rw-   0        0        0     2799 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0015_coderedsessionformsubmission_coderedsubmissionrevision.py
+-rw-rw-rw-   0        0        0     1363 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0016_auto_20191025_1620.py
+-rw-rw-rw-   0        0        0      460 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0017_generalsettings_external_new_tab.py
+-rw-rw-rw-   0        0        0     1341 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0018_auto_20200805_1702.py
+-rw-rw-rw-   0        0        0     1502 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0019_spelling_corrections.py
+-rw-rw-rw-   0        0        0      997 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0020_auto_20210527_1030.py
+-rw-rw-rw-   0        0        0      838 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0021_auto_20210730_1637.py
+-rw-rw-rw-   0        0        0     1561 2023-11-03 22:11:51.000000 coderedcms-3.0.4/coderedcms/migrations/0022_auto_20210731_1853.py
+-rw-rw-rw-   0        0        0     1372 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0023_auto_20210908_1702.py
+-rw-rw-rw-   0        0        0     1059 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0024_analyticssettings.py
+-rw-rw-rw-   0        0        0      311 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0025_delete_socialmediasettings.py
+-rw-rw-rw-   0        0        0     1336 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0026_auto_20220513_1627.py
+-rw-rw-rw-   0        0        0      608 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0027_auto_20220603_1142.py
+-rw-rw-rw-   0        0        0     1915 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0028_auto_20220609_1532.py
+-rw-rw-rw-   0        0        0     3522 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0029_multinavs.py
+-rw-rw-rw-   0        0        0      587 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0030_alter_coderedtag_tag.py
+-rw-rw-rw-   0        0        0     1840 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0031_wagtail3.py
+-rw-rw-rw-   0        0        0     1784 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0032_accordion_accordionpanel.py
+-rw-rw-rw-   0        0        0     2680 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0033_alter_coderedpage_struct_org_actions_and_more.py
+-rw-rw-rw-   0        0        0      488 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0033_remove_carousel_animation_and_more.py
+-rw-rw-rw-   0        0        0      319 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0034_delete_adasettings.py
+-rw-rw-rw-   0        0        0     3367 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0035_remove_googleapisettings_site_and_more.py
+-rw-rw-rw-   0        0        0     3873 2023-11-03 22:11:51.000000 coderedcms-3.0.4/coderedcms/migrations/0036_filmstrip_filmpanel.py
+-rw-rw-rw-   0        0        0     1404 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0037_coderedpage_related_classifier_term_and_more.py
+-rw-rw-rw-   0        0        0      551 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0038_alter_classifier_slug.py
+-rw-rw-rw-   0        0        0      532 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0039_alter_classifierterm_slug.py
+-rw-rw-rw-   0        0        0      357 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/0040_remove_analyticssettings_ga_tracking_id.py
+-rw-rw-rw-   0        0        0        0 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.947428 coderedcms-3.0.4/coderedcms/models/
+-rw-rw-rw-   0        0        0      323 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/models/__init__.py
+-rw-rw-rw-   0        0        0     6389 2024-05-18 16:33:43.000000 coderedcms-3.0.4/coderedcms/models/integration_models.py
+-rw-rw-rw-   0        0        0    72483 2024-05-18 16:33:43.000000 coderedcms-3.0.4/coderedcms/models/page_models.py
+-rw-rw-rw-   0        0        0    14702 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/models/snippet_models.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.963042 coderedcms-3.0.4/coderedcms/models/tests/
+-rw-rw-rw-   0        0        0        0 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/models/tests/__init__.py
+-rw-rw-rw-   0        0        0     4844 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/models/tests/test_navbars_and_footers.py
+-rw-rw-rw-   0        0        0     9031 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/models/tests/test_page_models.py
+-rw-rw-rw-   0        0        0     1960 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/models/tests/test_wagtailsettings_models.py
+-rw-rw-rw-   0        0        0    10348 2024-05-18 16:33:43.000000 coderedcms-3.0.4/coderedcms/models/wagtailsettings_models.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.900422 coderedcms-3.0.4/coderedcms/project_template/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.963042 coderedcms-3.0.4/coderedcms/project_template/basic/
+-rw-rw-rw-   0        0        0      722 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/project_template/basic/.editorconfig
+-rw-rw-rw-   0        0        0      364 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/project_template/basic/.gitattributes
+-rw-rw-rw-   0        0        0     5735 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/basic/.gitignore
+-rw-rw-rw-   0        0        0      932 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/project_template/basic/README.md
+-rw-rw-rw-   0        0        0      289 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/basic/manage.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.963042 coderedcms-3.0.4/coderedcms/project_template/basic/project_name/
+-rw-rw-rw-   0        0        0        0 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/project_template/basic/project_name/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.963042 coderedcms-3.0.4/coderedcms/project_template/basic/project_name/settings/
+-rw-rw-rw-   0        0        0        0 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/project_template/basic/project_name/settings/__init__.py
+-rw-rw-rw-   0        0        0     4834 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/project_template/basic/project_name/settings/base.py
+-rw-rw-rw-   0        0        0      388 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/project_template/basic/project_name/settings/dev.py
+-rw-rw-rw-   0        0        0     1294 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/basic/project_name/settings/prod.py
+-rw-rw-rw-   0        0        0     1266 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/basic/project_name/urls.py
+-rw-rw-rw-   0        0        0      444 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/basic/project_name/wsgi.py
+-rw-rw-rw-   0        0        0      656 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/basic/pyproject.toml
+-rw-rw-rw-   0        0        0      119 2023-03-30 17:43:55.000000 coderedcms-3.0.4/coderedcms/project_template/basic/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.963042 coderedcms-3.0.4/coderedcms/project_template/basic/website/
+-rw-rw-rw-   0        0        0        0 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/project_template/basic/website/__init__.py
+-rw-rw-rw-   0        0        0       89 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/project_template/basic/website/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.978670 coderedcms-3.0.4/coderedcms/project_template/basic/website/migrations/
+-rw-rw-rw-   0        0        0  5770141 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/basic/website/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1440 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/basic/website/migrations/0002_initial_data.py
+-rw-rw-rw-   0        0        0        0 2023-10-31 21:37:52.000000 coderedcms-3.0.4/coderedcms/project_template/basic/website/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3879 2024-05-18 16:33:43.000000 coderedcms-3.0.4/coderedcms/project_template/basic/website/models.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.900422 coderedcms-3.0.4/coderedcms/project_template/basic/website/static/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.900422 coderedcms-3.0.4/coderedcms/project_template/basic/website/static/website/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.978670 coderedcms-3.0.4/coderedcms/project_template/basic/website/static/website/css/
+-rw-rw-rw-   0        0        0      219 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/project_template/basic/website/static/website/css/custom.css
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.978670 coderedcms-3.0.4/coderedcms/project_template/basic/website/static/website/js/
+-rw-rw-rw-   0        0        0        0 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/project_template/basic/website/static/website/js/custom.js
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.900422 coderedcms-3.0.4/coderedcms/project_template/basic/website/templates/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.900422 coderedcms-3.0.4/coderedcms/project_template/basic/website/templates/coderedcms/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.978670 coderedcms-3.0.4/coderedcms/project_template/basic/website/templates/coderedcms/pages/
+-rw-rw-rw-   0        0        0      392 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/project_template/basic/website/templates/coderedcms/pages/base.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.978670 coderedcms-3.0.4/coderedcms/project_template/pro/
+-rw-rw-rw-   0        0        0      216 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/.cr.ini
+-rw-rw-rw-   0        0        0      722 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/.editorconfig
+-rw-rw-rw-   0        0        0      364 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/.gitattributes
+-rw-rw-rw-   0        0        0     5735 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/.gitignore
+-rw-rw-rw-   0        0        0     1695 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.978670 coderedcms-3.0.4/coderedcms/project_template/pro/custom_media/
+-rw-rw-rw-   0        0        0        0 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/custom_media/__init__.py
+-rw-rw-rw-   0        0        0      172 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/custom_media/admin.py
+-rw-rw-rw-   0        0        0      155 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/custom_media/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.978670 coderedcms-3.0.4/coderedcms/project_template/pro/custom_media/migrations/
+-rw-rw-rw-   0        0        0     9744 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/custom_media/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/custom_media/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1785 2024-05-18 16:33:43.000000 coderedcms-3.0.4/coderedcms/project_template/pro/custom_media/models.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.978670 coderedcms-3.0.4/coderedcms/project_template/pro/custom_user/
+-rw-rw-rw-   0        0        0        0 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/custom_user/__init__.py
+-rw-rw-rw-   0        0        0     1414 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/custom_user/admin.py
+-rw-rw-rw-   0        0        0      153 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/custom_user/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.978670 coderedcms-3.0.4/coderedcms/project_template/pro/custom_user/migrations/
+-rw-rw-rw-   0        0        0     4389 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/custom_user/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/custom_user/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1918 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/custom_user/models.py
+-rw-rw-rw-   0        0        0      289 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/manage.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.978670 coderedcms-3.0.4/coderedcms/project_template/pro/project_name/
+-rw-rw-rw-   0        0        0        0 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/project_name/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.994293 coderedcms-3.0.4/coderedcms/project_template/pro/project_name/settings/
+-rw-rw-rw-   0        0        0        0 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/project_name/settings/__init__.py
+-rw-rw-rw-   0        0        0     5026 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/project_template/pro/project_name/settings/base.py
+-rw-rw-rw-   0        0        0      438 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/project_name/settings/dev.py
+-rw-rw-rw-   0        0        0     1294 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/project_name/settings/prod.py
+-rw-rw-rw-   0        0        0     1266 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/project_name/urls.py
+-rw-rw-rw-   0        0        0      444 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/project_name/wsgi.py
+-rw-rw-rw-   0        0        0      656 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/pyproject.toml
+-rw-rw-rw-   0        0        0      150 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/requirements-dev.txt
+-rw-rw-rw-   0        0        0      251 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.994293 coderedcms-3.0.4/coderedcms/project_template/pro/website/
+-rw-rw-rw-   0        0        0        0 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/website/__init__.py
+-rw-rw-rw-   0        0        0       89 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/website/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.994293 coderedcms-3.0.4/coderedcms/project_template/pro/website/migrations/
+-rw-rw-rw-   0        0        0  5770141 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/website/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1440 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/website/migrations/0002_initial_data.py
+-rw-rw-rw-   0        0        0        0 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/website/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3879 2024-05-18 16:33:43.000000 coderedcms-3.0.4/coderedcms/project_template/pro/website/models.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.900422 coderedcms-3.0.4/coderedcms/project_template/pro/website/static/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.900422 coderedcms-3.0.4/coderedcms/project_template/pro/website/static/website/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.994293 coderedcms-3.0.4/coderedcms/project_template/pro/website/static/website/js/
+-rw-rw-rw-   0        0        0        0 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/website/static/website/js/custom.js
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.994293 coderedcms-3.0.4/coderedcms/project_template/pro/website/static/website/src/
+-rw-rw-rw-   0        0        0     1974 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/website/static/website/src/_variables.scss
+-rw-rw-rw-   0        0        0     1001 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/website/static/website/src/custom.scss
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.900422 coderedcms-3.0.4/coderedcms/project_template/pro/website/templates/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.900422 coderedcms-3.0.4/coderedcms/project_template/pro/website/templates/coderedcms/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.994293 coderedcms-3.0.4/coderedcms/project_template/pro/website/templates/coderedcms/pages/
+-rw-rw-rw-   0        0        0      913 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/project_template/pro/website/templates/coderedcms/pages/base.html
+-rw-rw-rw-   0        0        0      125 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/search_urls.py
+-rw-rw-rw-   0        0        0     9433 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.900422 coderedcms-3.0.4/coderedcms/static/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.900422 coderedcms-3.0.4/coderedcms/static/coderedcms/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.994293 coderedcms-3.0.4/coderedcms/static/coderedcms/css/
+-rw-rw-rw-   0        0        0     1705 2023-11-21 20:09:40.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/css/crx-admin.css
+-rw-rw-rw-   0        0        0     5642 2023-11-01 21:37:22.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/css/crx-front.css
+-rw-rw-rw-   0        0        0     5628 2023-04-21 16:47:29.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/css/crx-front.css.map
+-rw-rw-rw-   0        0        0     4620 2023-11-01 21:37:22.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/css/crx-front.min.css
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.994293 coderedcms-3.0.4/coderedcms/static/coderedcms/js/
+-rw-rw-rw-   0        0        0      717 2023-11-01 21:37:22.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/js/crx-editor.js
+-rw-rw-rw-   0        0        0     1488 2023-11-01 21:37:22.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/js/crx-events.js
+-rw-rw-rw-   0        0        0     5742 2023-11-01 21:37:22.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/js/crx-front.js
+-rw-rw-rw-   0        0        0     5256 2023-11-01 21:37:22.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/js/crx-maps.js
+-rw-rw-rw-   0        0        0     1805 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/js/crx-streamforms.js
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.009910 coderedcms-3.0.4/coderedcms/static/coderedcms/scss/
+-rw-rw-rw-   0        0        0      205 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/scss/_crx-article.scss
+-rw-rw-rw-   0        0        0      367 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/scss/_crx-bs-overrides.scss
+-rw-rw-rw-   0        0        0      330 2023-04-21 16:47:29.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/scss/_crx-filmstrip.scss
+-rw-rw-rw-   0        0        0      152 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/scss/_crx-gallery.scss
+-rw-rw-rw-   0        0        0      318 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/scss/_crx-hero.scss
+-rw-rw-rw-   0        0        0     1749 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/scss/_crx-location.scss
+-rw-rw-rw-   0        0        0     1988 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/scss/_crx-navbar.scss
+-rw-rw-rw-   0        0        0      818 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/scss/_crx-pricelist.scss
+-rw-rw-rw-   0        0        0      222 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/scss/_crx-richtext.scss
+-rw-rw-rw-   0        0        0      429 2023-11-01 21:37:22.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/scss/crx-front.scss
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.900422 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.009910 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/
+-rw-rw-rw-   0        0        0     1093 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/LICENSE
+-rw-rw-rw-   0        0        0      130 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.900422 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.025436 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/
+-rw-rw-rw-   0        0        0    70329 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css
+-rw-rw-rw-   0        0        0   203178 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css.map
+-rw-rw-rw-   0        0        0    51795 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css
+-rw-rw-rw-   0        0        0   115987 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css.map
+-rw-rw-rw-   0        0        0    70403 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.css
+-rw-rw-rw-   0        0        0   203182 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.css.map
+-rw-rw-rw-   0        0        0    51870 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.min.css
+-rw-rw-rw-   0        0        0   116064 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map
+-rw-rw-rw-   0        0        0    12065 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css
+-rw-rw-rw-   0        0        0   129327 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css.map
+-rw-rw-rw-   0        0        0    10126 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css
+-rw-rw-rw-   0        0        0    51369 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css.map
+-rw-rw-rw-   0        0        0    12058 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.css
+-rw-rw-rw-   0        0        0   129342 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.css.map
+-rw-rw-rw-   0        0        0    10198 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.min.css
+-rw-rw-rw-   0        0        0    63943 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map
+-rw-rw-rw-   0        0        0   107823 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.css
+-rw-rw-rw-   0        0        0   267491 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.css.map
+-rw-rw-rw-   0        0        0    85352 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.min.css
+-rw-rw-rw-   0        0        0   180381 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.min.css.map
+-rw-rw-rw-   0        0        0   107691 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.css
+-rw-rw-rw-   0        0        0   267432 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.css.map
+-rw-rw-rw-   0        0        0    85281 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.min.css
+-rw-rw-rw-   0        0        0   180217 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map
+-rw-rw-rw-   0        0        0   280813 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css
+-rw-rw-rw-   0        0        0   679011 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css.map
+-rw-rw-rw-   0        0        0   232948 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0   589161 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css.map
+-rw-rw-rw-   0        0        0   280392 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.css
+-rw-rw-rw-   0        0        0   678856 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.css.map
+-rw-rw-rw-   0        0        0   233055 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.min.css
+-rw-rw-rw-   0        0        0   588695 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.min.css.map
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.041174 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/
+-rw-rw-rw-   0        0        0   207731 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js
+-rw-rw-rw-   0        0        0   444286 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js.map
+-rw-rw-rw-   0        0        0    80663 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   331886 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0        0        0   135747 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.js
+-rw-rw-rw-   0        0        0   305152 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.js.map
+-rw-rw-rw-   0        0        0    74154 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.min.js
+-rw-rw-rw-   0        0        0   222462 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.min.js.map
+-rw-rw-rw-   0        0        0   145313 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js
+-rw-rw-rw-   0        0        0   306320 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js.map
+-rw-rw-rw-   0        0        0    60577 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0   220350 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js.map
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.900422 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.041174 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/
+-rw-rw-rw-   0        0        0     1903 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/alert.js
+-rw-rw-rw-   0        0        0     1932 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/base-component.js
+-rw-rw-rw-   0        0        0     1625 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/button.js
+-rw-rw-rw-   0        0        0    11817 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/carousel.js
+-rw-rw-rw-   0        0        0     7594 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/collapse.js
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.056792 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dom/
+-rw-rw-rw-   0        0        0     1395 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dom/data.js
+-rw-rw-rw-   0        0        0     8351 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dom/event-handler.js
+-rw-rw-rw-   0        0        0     1658 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dom/manipulator.js
+-rw-rw-rw-   0        0        0     3381 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dom/selector-engine.js
+-rw-rw-rw-   0        0        0    13205 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dropdown.js
+-rw-rw-rw-   0        0        0     9581 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/modal.js
+-rw-rw-rw-   0        0        0     6806 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/offcanvas.js
+-rw-rw-rw-   0        0        0     1870 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/popover.js
+-rw-rw-rw-   0        0        0     8472 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/scrollspy.js
+-rw-rw-rw-   0        0        0     9068 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tab.js
+-rw-rw-rw-   0        0        0     5039 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/toast.js
+-rw-rw-rw-   0        0        0    16029 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tooltip.js
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.056792 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/
+-rw-rw-rw-   0        0        0     3125 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/backdrop.js
+-rw-rw-rw-   0        0        0     1114 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/component-functions.js
+-rw-rw-rw-   0        0        0     1784 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/config.js
+-rw-rw-rw-   0        0        0     2518 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/focustrap.js
+-rw-rw-rw-   0        0        0     7640 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/index.js
+-rw-rw-rw-   0        0        0     2933 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/sanitizer.js
+-rw-rw-rw-   0        0        0     3754 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/scrollbar.js
+-rw-rw-rw-   0        0        0     3409 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/swipe.js
+-rw-rw-rw-   0        0        0     3612 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/template-factory.js
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.072353 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/
+-rw-rw-rw-   0        0        0     5066 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_accordion.scss
+-rw-rw-rw-   0        0        0     2073 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_alert.scss
+-rw-rw-rw-   0        0        0     1118 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_badge.scss
+-rw-rw-rw-   0        0        0     1751 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_breadcrumb.scss
+-rw-rw-rw-   0        0        0     3201 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_button-group.scss
+-rw-rw-rw-   0        0        0     6746 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_buttons.scss
+-rw-rw-rw-   0        0        0     6979 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_card.scss
+-rw-rw-rw-   0        0        0     5879 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_carousel.scss
+-rw-rw-rw-   0        0        0     2018 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_close.scss
+-rw-rw-rw-   0        0        0     1201 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_containers.scss
+-rw-rw-rw-   0        0        0     8093 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_dropdown.scss
+-rw-rw-rw-   0        0        0      256 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_forms.scss
+-rw-rw-rw-   0        0        0    10554 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_functions.scss
+-rw-rw-rw-   0        0        0      683 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_grid.scss
+-rw-rw-rw-   0        0        0      353 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_helpers.scss
+-rw-rw-rw-   0        0        0     1158 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_images.scss
+-rw-rw-rw-   0        0        0     6852 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_list-group.scss
+-rw-rw-rw-   0        0        0     6005 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_maps.scss
+-rw-rw-rw-   0        0        0      875 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_mixins.scss
+-rw-rw-rw-   0        0        0     7762 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_modal.scss
+-rw-rw-rw-   0        0        0     5211 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_nav.scss
+-rw-rw-rw-   0        0        0     9155 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_navbar.scss
+-rw-rw-rw-   0        0        0     4725 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_offcanvas.scss
+-rw-rw-rw-   0        0        0     3947 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_pagination.scss
+-rw-rw-rw-   0        0        0      859 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_placeholders.scss
+-rw-rw-rw-   0        0        0     6907 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_popover.scss
+-rw-rw-rw-   0        0        0     2016 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_progress.scss
+-rw-rw-rw-   0        0        0    12438 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_reboot.scss
+-rw-rw-rw-   0        0        0     6924 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_root.scss
+-rw-rw-rw-   0        0        0     2429 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_spinners.scss
+-rw-rw-rw-   0        0        0     4945 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_tables.scss
+-rw-rw-rw-   0        0        0     2490 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_toasts.scss
+-rw-rw-rw-   0        0        0     4281 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_tooltip.scss
+-rw-rw-rw-   0        0        0      425 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_transitions.scss
+-rw-rw-rw-   0        0        0     1420 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_type.scss
+-rw-rw-rw-   0        0        0    19235 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_utilities.scss
+-rw-rw-rw-   0        0        0     5057 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_variables-dark.scss
+-rw-rw-rw-   0        0        0    76286 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_variables.scss
+-rw-rw-rw-   0        0        0     1183 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap-grid.scss
+-rw-rw-rw-   0        0        0      189 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap-reboot.scss
+-rw-rw-rw-   0        0        0      306 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap-utilities.scss
+-rw-rw-rw-   0        0        0      938 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap.scss
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.088044 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/
+-rw-rw-rw-   0        0        0     2688 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_floating-labels.scss
+-rw-rw-rw-   0        0        0     4851 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-check.scss
+-rw-rw-rw-   0        0        0     6590 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-control.scss
+-rw-rw-rw-   0        0        0     2796 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-range.scss
+-rw-rw-rw-   0        0        0     2488 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-select.scss
+-rw-rw-rw-   0        0        0      219 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-text.scss
+-rw-rw-rw-   0        0        0     3899 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_input-group.scss
+-rw-rw-rw-   0        0        0     1142 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_labels.scss
+-rw-rw-rw-   0        0        0      478 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_validation.scss
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.088044 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/
+-rw-rw-rw-   0        0        0       37 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_clearfix.scss
+-rw-rw-rw-   0        0        0      403 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_color-bg.scss
+-rw-rw-rw-   0        0        0     1755 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_colored-links.scss
+-rw-rw-rw-   0        0        0      385 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_focus-ring.scss
+-rw-rw-rw-   0        0        0      605 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_icon-link.scss
+-rw-rw-rw-   0        0        0      621 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_position.scss
+-rw-rw-rw-   0        0        0      399 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_ratio.scss
+-rw-rw-rw-   0        0        0      245 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_stacks.scss
+-rw-rw-rw-   0        0        0      223 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_stretched-link.scss
+-rw-rw-rw-   0        0        0       73 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_text-truncation.scss
+-rw-rw-rw-   0        0        0      136 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_visually-hidden.scss
+-rw-rw-rw-   0        0        0      160 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_vr.scss
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.103680 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/
+-rw-rw-rw-   0        0        0      525 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_alert.scss
+-rw-rw-rw-   0        0        0      328 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_backdrop.scss
+-rw-rw-rw-   0        0        0      223 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_banner.scss
+-rw-rw-rw-   0        0        0     2031 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_border-radius.scss
+-rw-rw-rw-   0        0        0      398 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_box-shadow.scss
+-rw-rw-rw-   0        0        0     4580 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_breakpoints.scss
+-rw-rw-rw-   0        0        0     3220 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_buttons.scss
+-rw-rw-rw-   0        0        0     1587 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_caret.scss
+-rw-rw-rw-   0        0        0      147 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_clearfix.scss
+-rw-rw-rw-   0        0        0      447 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_color-mode.scss
+-rw-rw-rw-   0        0        0      167 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_color-scheme.scss
+-rw-rw-rw-   0        0        0      410 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_container.scss
+-rw-rw-rw-   0        0        0      613 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_deprecate.scss
+-rw-rw-rw-   0        0        0     4164 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_forms.scss
+-rw-rw-rw-   0        0        0     1956 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_gradients.scss
+-rw-rw-rw-   0        0        0     4735 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_grid.scss
+-rw-rw-rw-   0        0        0      395 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_image.scss
+-rw-rw-rw-   0        0        0      581 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_list-group.scss
+-rw-rw-rw-   0        0        0      168 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_lists.scss
+-rw-rw-rw-   0        0        0      387 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_pagination.scss
+-rw-rw-rw-   0        0        0      495 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_reset-text.scss
+-rw-rw-rw-   0        0        0      202 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_resize.scss
+-rw-rw-rw-   0        0        0     1101 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_table-variants.scss
+-rw-rw-rw-   0        0        0      168 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_text-truncate.scss
+-rw-rw-rw-   0        0        0      661 2023-10-31 18:32:58.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_transition.scss
+-rw-rw-rw-   0        0        0     3384 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_utilities.scss
+-rw-rw-rw-   0        0        0     1110 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_visually-hidden.scss
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.103680 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/
+-rw-rw-rw-   0        0        0      449 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/jasmine.js
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.103680 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/mixins/
+-rw-rw-rw-   0        0        0     1859 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/mixins/_color-modes.test.scss
+-rw-rw-rw-   0        0        0      246 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/mixins/_media-query-color-mode-full.test.scss
+-rw-rw-rw-   0        0        0     8772 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/mixins/_utilities.test.scss
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.103680 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/sass-true/
+-rw-rw-rw-   0        0        0      377 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/sass-true/register.js
+-rw-rw-rw-   0        0        0      450 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/sass-true/runner.js
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.103680 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/utilities/
+-rw-rw-rw-   0        0        0     1462 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/utilities/_api.test.scss
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.103680 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/utilities/
+-rw-rw-rw-   0        0        0     1737 2023-10-31 18:32:59.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/utilities/_api.scss
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.103680 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/vendor/
+-rw-rw-rw-   0        0        0    10012 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/vendor/_rfs.scss
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.119290 coderedcms-3.0.4/coderedcms/templates/
+-rw-rw-rw-   0        0        0      280 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/404.html
+-rw-rw-rw-   0        0        0      725 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/templates/500.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:33.900422 coderedcms-3.0.4/coderedcms/templates/coderedcms/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.134921 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/
+-rw-rw-rw-   0        0        0     1129 2023-02-17 20:46:38.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/accordion_block.html
+-rw-rw-rw-   0        0        0      791 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/article_block_card.html
+-rw-rw-rw-   0        0        0      173 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/base_block.html
+-rw-rw-rw-   0        0        0     1789 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/base_link_block.html
+-rw-rw-rw-   0        0        0      617 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/button_block.html
+-rw-rw-rw-   0        0        0      734 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/card_block.html
+-rw-rw-rw-   0        0        0      840 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/card_blurb.html
+-rw-rw-rw-   0        0        0      771 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/card_foot.html
+-rw-rw-rw-   0        0        0      720 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/card_head.html
+-rw-rw-rw-   0        0        0      757 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/card_head_foot.html
+-rw-rw-rw-   0        0        0      775 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/card_img.html
+-rw-rw-rw-   0        0        0      368 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/cardgrid_columns.html
+-rw-rw-rw-   0        0        0      278 2023-02-17 20:46:38.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/cardgrid_deck.html
+-rw-rw-rw-   0        0        0      262 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/cardgrid_group.html
+-rw-rw-rw-   0        0        0     2154 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/carousel_block.html
+-rw-rw-rw-   0        0        0      389 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/column_block.html
+-rw-rw-rw-   0        0        0      833 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/content_wall_block.html
+-rw-rw-rw-   0        0        0      141 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/document_link_block.html
+-rw-rw-rw-   0        0        0      732 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/download_block.html
+-rw-rw-rw-   0        0        0      105 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/embed_video_block.html
+-rw-rw-rw-   0        0        0       99 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/external_link_block.html
+-rw-rw-rw-   0        0        0     1453 2024-05-18 16:33:43.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/film_strip_block.html
+-rw-rw-rw-   0        0        0      582 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/google_map.html
+-rw-rw-rw-   0        0        0      374 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/grid_block.html
+-rw-rw-rw-   0        0        0      198 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/h1_block.html
+-rw-rw-rw-   0        0        0      198 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/h2_block.html
+-rw-rw-rw-   0        0        0      198 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/h3_block.html
+-rw-rw-rw-   0        0        0      846 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/hero_block.html
+-rw-rw-rw-   0        0        0      299 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/image_block.html
+-rw-rw-rw-   0        0        0     1196 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/image_gallery_block.html
+-rw-rw-rw-   0        0        0      631 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/image_link_block.html
+-rw-rw-rw-   0        0        0      992 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/modal_block.html
+-rw-rw-rw-   0        0        0      167 2023-02-09 20:20:28.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/page_link_block.html
+-rw-rw-rw-   0        0        0      444 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/pagelist_article_card_columns.html
+-rw-rw-rw-   0        0        0      392 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/pagelist_article_card_deck.html
+-rw-rw-rw-   0        0        0      324 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/pagelist_article_card_group.html
+-rw-rw-rw-   0        0        0      916 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/pagelist_article_media.html
+-rw-rw-rw-   0        0        0      320 2023-04-21 16:47:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/pagelist_block.html
+-rw-rw-rw-   0        0        0      561 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/pagelist_list_group.html
+-rw-rw-rw-   0        0        0      204 2023-04-21 16:47:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/pagepreview_block.html
+-rw-rw-rw-   0        0        0      803 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/pagepreview_card.html
+-rw-rw-rw-   0        0        0     1009 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/pagepreview_form.html
+-rw-rw-rw-   0        0        0      227 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/pricelist_block.html
+-rw-rw-rw-   0        0        0      533 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/pricelistitem_block.html
+-rw-rw-rw-   0        0        0      347 2023-07-12 20:31:45.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/quote_block.html
+-rw-rw-rw-   0        0        0      258 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/reusable_content_block.html
+-rw-rw-rw-   0        0        0       86 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/rich_text_block.html
+-rw-rw-rw-   0        0        0      877 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/table_block.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.134921 coderedcms-3.0.4/coderedcms/templates/coderedcms/formfields/
+-rw-rw-rw-   0        0        0      266 2023-10-31 19:00:50.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/formfields/date.html
+-rw-rw-rw-   0        0        0      411 2023-11-21 20:09:40.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/formfields/datetime.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.134921 coderedcms-3.0.4/coderedcms/templates/coderedcms/formfields/mailchimp/
+-rw-rw-rw-   0        0        0     6685 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/formfields/mailchimp/subscriber_integration_js.html
+-rw-rw-rw-   0        0        0      793 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/formfields/mailchimp/subscriber_integration_widget.html
+-rw-rw-rw-   0        0        0      263 2023-10-31 19:00:50.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/formfields/time.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.150436 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/
+-rw-rw-rw-   0        0        0      465 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-align-left.svg
+-rw-rw-rw-   0        0        0      573 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-check-square-o.svg
+-rw-rw-rw-   0        0        0      277 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-columns.svg
+-rw-rw-rw-   0        0        0      359 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-desktop.svg
+-rw-rw-rw-   0        0        0      571 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-font.svg
+-rw-rw-rw-   0        0        0      292 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-google.svg
+-rw-rw-rw-   0        0        0      813 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-hand-pointer-o.svg
+-rw-rw-rw-   0        0        0      666 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-hashtag.svg
+-rw-rw-rw-   0        0        0      840 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-header.svg
+-rw-rw-rw-   0        0        0      835 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-list-alt.svg
+-rw-rw-rw-   0        0        0      459 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-map.svg
+-rw-rw-rw-   0        0        0      448 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-newspaper-o.svg
+-rw-rw-rw-   0        0        0      721 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-puzzle-piece.svg
+-rw-rw-rw-   0        0        0      635 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-recycle.svg
+-rw-rw-rw-   0        0        0      174 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-stop.svg
+-rw-rw-rw-   0        0        0      505 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-th-large.svg
+-rw-rw-rw-   0        0        0      762 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-universal-access.svg
+-rw-rw-rw-   0        0        0      548 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-usd.svg
+-rw-rw-rw-   0        0        0      225 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-window-maximize.svg
+-rw-rw-rw-   0        0        0      199 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-window-minimize.svg
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.150436 coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/
+-rw-rw-rw-   0        0        0      714 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/classifier_dropdowns.html
+-rw-rw-rw-   0        0        0      534 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/classifier_nav.html
+-rw-rw-rw-   0        0        0      296 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/crx_banner.html
+-rw-rw-rw-   0        0        0      262 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/form_honeypot.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.166109 coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/ical/
+-rw-rw-rw-   0        0        0      531 2023-10-31 19:00:50.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/ical/calendar.html
+-rw-rw-rw-   0        0        0      365 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/ical/calendar_ical_button.html
+-rw-rw-rw-   0        0        0      406 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/ical/recurring_ical_button.html
+-rw-rw-rw-   0        0        0      565 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/ical/single_ical_button.html
+-rw-rw-rw-   0        0        0      261 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/iframe_gmap.html
+-rw-rw-rw-   0        0        0      320 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/map_list_description.html
+-rw-rw-rw-   0        0        0      107 2022-08-04 15:54:45.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/map_pin_description.html
+-rw-rw-rw-   0        0        0      983 2023-03-30 19:10:04.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/pagination.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.166109 coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/stream_forms/
+-rw-rw-rw-   0        0        0      533 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/stream_forms/render_field.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.166109 coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/
+-rw-rw-rw-   0        0        0     1526 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/article_index_page.html
+-rw-rw-rw-   0        0        0     1332 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/article_page.html
+-rw-rw-rw-   0        0        0     1094 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/article_page.search.html
+-rw-rw-rw-   0        0        0     7594 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/base.html
+-rw-rw-rw-   0        0        0     1929 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/event_index_page.html
+-rw-rw-rw-   0        0        0     1846 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/event_page.html
+-rw-rw-rw-   0        0        0     1001 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/form_page.html
+-rw-rw-rw-   0        0        0      921 2023-04-21 16:47:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/form_page.mini.html
+-rw-rw-rw-   0        0        0      244 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/form_page_landing.html
+-rw-rw-rw-   0        0        0       55 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/home_page.html
+-rw-rw-rw-   0        0        0     1580 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/location_index_page.html
+-rw-rw-rw-   0        0        0      858 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/location_page.html
+-rw-rw-rw-   0        0        0      505 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/page.mini.html
+-rw-rw-rw-   0        0        0     2605 2023-11-27 22:26:53.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/search.html
+-rw-rw-rw-   0        0        0      417 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/search_result.html
+-rw-rw-rw-   0        0        0     2525 2023-11-01 21:37:22.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/stream_form_page.html
+-rw-rw-rw-   0        0        0      528 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/web_page.html
+-rw-rw-rw-   0        0        0      209 2023-04-21 16:47:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/web_page_notitle.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.166109 coderedcms-3.0.4/coderedcms/templates/coderedcms/snippets/
+-rw-rw-rw-   0        0        0      471 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/snippets/footer.html
+-rw-rw-rw-   0        0        0     2424 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/snippets/navbar.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.166109 coderedcms-3.0.4/coderedcms/templates/coderedcms/widgets/
+-rw-rw-rw-   0        0        0     1245 2023-11-01 21:37:22.000000 coderedcms-3.0.4/coderedcms/templates/coderedcms/widgets/checkbox_classifiers.html
+-rw-rw-rw-   0        0        0      193 2024-05-18 16:33:19.000000 coderedcms-3.0.4/coderedcms/templates/robots.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.166109 coderedcms-3.0.4/coderedcms/templates/wagtailadmin/
+-rw-rw-rw-   0        0        0      728 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/templates/wagtailadmin/base.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.166109 coderedcms-3.0.4/coderedcms/templates/wagtailadmin/block_forms/
+-rw-rw-rw-   0        0        0      716 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html
+-rw-rw-rw-   0        0        0       95 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/wagtailadmin/home.html
+-rw-rw-rw-   0        0        0      177 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/wagtailadmin/login.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.166109 coderedcms-3.0.4/coderedcms/templates/wagtailcore/
+-rw-rw-rw-   0        0        0      692 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/wagtailcore/password_required.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.166109 coderedcms-3.0.4/coderedcms/templates/wagtailembeds/
+-rw-rw-rw-   0        0        0      522 2023-02-09 20:20:29.000000 coderedcms-3.0.4/coderedcms/templates/wagtailembeds/embed_frontend.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.181795 coderedcms-3.0.4/coderedcms/templates/wagtailforms/
+-rw-rw-rw-   0        0        0     1528 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/wagtailforms/list_submissions.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.181795 coderedcms-3.0.4/coderedcms/templates/wagtailimportexport/
+-rw-rw-rw-   0        0        0     1396 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/wagtailimportexport/import_from_csv.html
+-rw-rw-rw-   0        0        0      470 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/templates/wagtailimportexport/index.html
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.181795 coderedcms-3.0.4/coderedcms/templatetags/
+-rw-rw-rw-   0        0        0     5892 2024-05-18 16:33:48.000000 coderedcms-3.0.4/coderedcms/templatetags/coderedcms_tags.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.181795 coderedcms-3.0.4/coderedcms/tests/
+-rw-rw-rw-   0        0        0     5157 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/tests/settings.py
+-rw-rw-rw-   0        0        0     2805 2023-11-13 16:26:32.000000 coderedcms-3.0.4/coderedcms/tests/test_bin.py
+-rw-rw-rw-   0        0        0     1593 2023-10-31 21:37:54.000000 coderedcms-3.0.4/coderedcms/tests/test_templates.py
+-rw-rw-rw-   0        0        0      821 2023-10-31 21:37:54.000000 coderedcms-3.0.4/coderedcms/tests/test_templatetags.py
+-rw-rw-rw-   0        0        0    12176 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/tests/test_urls.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.181795 coderedcms-3.0.4/coderedcms/tests/testapp/
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.181795 coderedcms-3.0.4/coderedcms/tests/testapp/migrations/
+-rw-rw-rw-   0        0        0   257599 2023-11-01 18:36:21.000000 coderedcms-3.0.4/coderedcms/tests/testapp/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1481 2023-10-31 21:37:54.000000 coderedcms-3.0.4/coderedcms/tests/testapp/migrations/0002_initial.py
+-rw-rw-rw-   0        0        0   250426 2023-10-31 21:37:54.000000 coderedcms-3.0.4/coderedcms/tests/testapp/migrations/0003_eventindexpage_eventoccurrence_eventpage_locationindexpage_locationpage.py
+-rw-rw-rw-   0        0        0   101517 2023-10-31 21:37:54.000000 coderedcms-3.0.4/coderedcms/tests/testapp/migrations/0004_streamformconfirmemail_streamformpage.py
+-rw-rw-rw-   0        0        0   346621 2023-10-31 21:37:54.000000 coderedcms-3.0.4/coderedcms/tests/testapp/migrations/0005_auto_20210908_1741.py
+-rw-rw-rw-   0        0        0      770 2023-10-31 21:37:54.000000 coderedcms-3.0.4/coderedcms/tests/testapp/migrations/0006_indextestpage.py
+-rw-rw-rw-   0        0        0     1011 2023-10-31 21:37:54.000000 coderedcms-3.0.4/coderedcms/tests/testapp/migrations/0007_auto_20210910_1614.py
+-rw-rw-rw-   0        0        0        0 2023-10-31 21:37:54.000000 coderedcms-3.0.4/coderedcms/tests/testapp/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3991 2023-10-31 21:37:54.000000 coderedcms-3.0.4/coderedcms/tests/testapp/models.py
+-rw-rw-rw-   0        0        0      519 2023-10-31 21:37:54.000000 coderedcms-3.0.4/coderedcms/tests/urls.py
+-rw-rw-rw-   0        0        0     1470 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/urls.py
+-rw-rw-rw-   0        0        0     1390 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/utils.py
+-rw-rw-rw-   0        0        0    11286 2024-01-11 19:08:54.000000 coderedcms-3.0.4/coderedcms/views.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.181795 coderedcms-3.0.4/coderedcms/wagtail_flexible_forms/
+-rw-rw-rw-   0        0        0     1506 2022-08-03 20:24:51.000000 coderedcms-3.0.4/coderedcms/wagtail_flexible_forms/LICENSE
+-rw-rw-rw-   0        0        0     7670 2023-10-31 21:37:54.000000 coderedcms-3.0.4/coderedcms/wagtail_flexible_forms/blocks.py
+-rw-rw-rw-   0        0        0     1191 2023-10-31 21:37:54.000000 coderedcms-3.0.4/coderedcms/wagtail_flexible_forms/edit_handlers.py
+-rw-rw-rw-   0        0        0    30401 2024-05-18 16:33:43.000000 coderedcms-3.0.4/coderedcms/wagtail_flexible_forms/models.py
+-rw-rw-rw-   0        0        0     4763 2024-05-18 16:33:43.000000 coderedcms-3.0.4/coderedcms/wagtail_hooks.py
+-rw-rw-rw-   0        0        0     1473 2023-10-31 21:37:51.000000 coderedcms-3.0.4/coderedcms/widgets.py
+drwxrwxrwx   0        0        0        0 2024-05-18 16:38:34.181795 coderedcms-3.0.4/coderedcms.egg-info/
+-rw-rw-rw-   0        0        0     6061 2024-05-18 16:38:33.000000 coderedcms-3.0.4/coderedcms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    28416 2024-05-18 16:38:33.000000 coderedcms-3.0.4/coderedcms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 16:38:33.000000 coderedcms-3.0.4/coderedcms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-18 16:38:33.000000 coderedcms-3.0.4/coderedcms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-18 16:38:05.000000 coderedcms-3.0.4/coderedcms.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      186 2024-05-18 16:38:33.000000 coderedcms-3.0.4/coderedcms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-18 16:38:33.000000 coderedcms-3.0.4/coderedcms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      299 2023-02-09 20:20:29.000000 coderedcms-3.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      384 2024-05-18 16:38:34.197412 coderedcms-3.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2180 2024-05-18 16:33:43.000000 coderedcms-3.0.4/setup.py
```

### Comparing `coderedcms-3.0.3/LICENSE` & `coderedcms-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/PKG-INFO` & `coderedcms-3.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coderedcms
-Version: 3.0.3
+Version: 3.0.4
 Summary: Wagtail-based CMS by CodeRed for building marketing websites.
 Home-page: https://github.com/coderedcorp/coderedcms
 Author: CodeRed LLC
 Author-email: info@coderedcorp.com
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `coderedcms-3.0.3/README.md` & `coderedcms-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/__init__.py` & `coderedcms-3.0.4/coderedcms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 5th element is for dev/post releases. Leave blank for stable releases.
 
     X.Y.Z.devN   # Development release
     X.Y.Z.postN  # Post release (e.g. docs changes but no actual code changes)
 
 See: https://www.python.org/dev/peps/pep-0440/
 """
-release = ["3", "0", "3", "", ""]
+release = ["3", "0", "4", "", ""]
 
 
 def _get_version() -> str:
     v = "{0}.{1}.{2}".format(release[0], release[1], release[2])
     if release[3]:
         v = "{0}{1}".format(v, release[3])
     if release[4]:
```

### Comparing `coderedcms-3.0.3/coderedcms/api/mailchimp.py` & `coderedcms-3.0.4/coderedcms/api/mailchimp.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/bin/coderedcms.py` & `coderedcms-3.0.4/coderedcms/bin/coderedcms.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/blocks/__init__.py` & `coderedcms-3.0.4/coderedcms/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/blocks/base_blocks.py` & `coderedcms-3.0.4/coderedcms/blocks/base_blocks.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/blocks/content_blocks.py` & `coderedcms-3.0.4/coderedcms/blocks/content_blocks.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/blocks/html_blocks.py` & `coderedcms-3.0.4/coderedcms/blocks/html_blocks.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/blocks/layout_blocks.py` & `coderedcms-3.0.4/coderedcms/blocks/layout_blocks.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/blocks/stream_form_blocks.py` & `coderedcms-3.0.4/coderedcms/blocks/stream_form_blocks.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/fields.py` & `coderedcms-3.0.4/coderedcms/fields.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/forms.py` & `coderedcms-3.0.4/coderedcms/forms.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/importexport.py` & `coderedcms-3.0.4/coderedcms/importexport.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0001_initial.py` & `coderedcms-3.0.4/coderedcms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0002_auto_20180829_1538.py` & `coderedcms-3.0.4/coderedcms/migrations/0002_auto_20180829_1538.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0003_auto_20180912_1632.py` & `coderedcms-3.0.4/coderedcms/migrations/0003_auto_20180912_1632.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0004_auto_20181119_1507.py` & `coderedcms-3.0.4/coderedcms/migrations/0004_auto_20181119_1507.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0005_auto_20181214_2214.py` & `coderedcms-3.0.4/coderedcms/migrations/0005_auto_20181214_2214.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0006_mailchimpapisettings.py` & `coderedcms-3.0.4/coderedcms/migrations/0006_mailchimpapisettings.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0007_auto_20190114_1515.py` & `coderedcms-3.0.4/coderedcms/migrations/0007_auto_20190114_1515.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0008_auto_20190122_1242.py` & `coderedcms-3.0.4/coderedcms/migrations/0008_auto_20190122_1242.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0009_auto_20190201_1546.py` & `coderedcms-3.0.4/coderedcms/migrations/0009_auto_20190201_1546.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0010_auto_20190320_1231.py` & `coderedcms-3.0.4/coderedcms/migrations/0010_auto_20190320_1231.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0010_generalsettings_email.py` & `coderedcms-3.0.4/coderedcms/migrations/0010_generalsettings_email.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0013_pagepreview_templates.py` & `coderedcms-3.0.4/coderedcms/migrations/0013_pagepreview_templates.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0014_classifiers.py` & `coderedcms-3.0.4/coderedcms/migrations/0014_classifiers.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0015_coderedsessionformsubmission_coderedsubmissionrevision.py` & `coderedcms-3.0.4/coderedcms/migrations/0015_coderedsessionformsubmission_coderedsubmissionrevision.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0016_auto_20191025_1620.py` & `coderedcms-3.0.4/coderedcms/migrations/0016_auto_20191025_1620.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0018_auto_20200805_1702.py` & `coderedcms-3.0.4/coderedcms/migrations/0018_auto_20200805_1702.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0019_spelling_corrections.py` & `coderedcms-3.0.4/coderedcms/migrations/0019_spelling_corrections.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0020_auto_20210527_1030.py` & `coderedcms-3.0.4/coderedcms/migrations/0020_auto_20210527_1030.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0021_auto_20210730_1637.py` & `coderedcms-3.0.4/coderedcms/migrations/0021_auto_20210730_1637.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0022_auto_20210731_1853.py` & `coderedcms-3.0.4/coderedcms/migrations/0022_auto_20210731_1853.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0023_auto_20210908_1702.py` & `coderedcms-3.0.4/coderedcms/migrations/0023_auto_20210908_1702.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0024_analyticssettings.py` & `coderedcms-3.0.4/coderedcms/migrations/0024_analyticssettings.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0026_auto_20220513_1627.py` & `coderedcms-3.0.4/coderedcms/migrations/0026_auto_20220513_1627.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0027_auto_20220603_1142.py` & `coderedcms-3.0.4/coderedcms/migrations/0027_auto_20220603_1142.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0028_auto_20220609_1532.py` & `coderedcms-3.0.4/coderedcms/migrations/0028_auto_20220609_1532.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0029_multinavs.py` & `coderedcms-3.0.4/coderedcms/migrations/0029_multinavs.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0030_alter_coderedtag_tag.py` & `coderedcms-3.0.4/coderedcms/migrations/0030_alter_coderedtag_tag.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0031_wagtail3.py` & `coderedcms-3.0.4/coderedcms/migrations/0031_wagtail3.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0032_accordion_accordionpanel.py` & `coderedcms-3.0.4/coderedcms/migrations/0032_accordion_accordionpanel.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0033_alter_coderedpage_struct_org_actions_and_more.py` & `coderedcms-3.0.4/coderedcms/migrations/0033_alter_coderedpage_struct_org_actions_and_more.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0035_remove_googleapisettings_site_and_more.py` & `coderedcms-3.0.4/coderedcms/migrations/0035_remove_googleapisettings_site_and_more.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0036_filmstrip_filmpanel.py` & `coderedcms-3.0.4/coderedcms/migrations/0036_filmstrip_filmpanel.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0037_coderedpage_related_classifier_term_and_more.py` & `coderedcms-3.0.4/coderedcms/migrations/0037_coderedpage_related_classifier_term_and_more.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0038_alter_classifier_slug.py` & `coderedcms-3.0.4/coderedcms/migrations/0038_alter_classifier_slug.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/migrations/0039_alter_classifierterm_slug.py` & `coderedcms-3.0.4/coderedcms/migrations/0039_alter_classifierterm_slug.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/models/integration_models.py` & `coderedcms-3.0.4/coderedcms/models/integration_models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/models/page_models.py` & `coderedcms-3.0.4/coderedcms/models/page_models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/models/snippet_models.py` & `coderedcms-3.0.4/coderedcms/models/snippet_models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/models/tests/test_navbars_and_footers.py` & `coderedcms-3.0.4/coderedcms/models/tests/test_navbars_and_footers.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/models/tests/test_page_models.py` & `coderedcms-3.0.4/coderedcms/models/tests/test_page_models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/models/tests/test_wagtailsettings_models.py` & `coderedcms-3.0.4/coderedcms/models/tests/test_wagtailsettings_models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/models/wagtailsettings_models.py` & `coderedcms-3.0.4/coderedcms/models/wagtailsettings_models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/basic/.editorconfig` & `coderedcms-3.0.4/coderedcms/project_template/basic/.editorconfig`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/basic/.gitignore` & `coderedcms-3.0.4/coderedcms/project_template/basic/.gitignore`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/basic/README.md` & `coderedcms-3.0.4/coderedcms/project_template/basic/README.md`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/basic/project_name/settings/base.py` & `coderedcms-3.0.4/coderedcms/project_template/basic/project_name/settings/base.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/basic/project_name/settings/prod.py` & `coderedcms-3.0.4/coderedcms/project_template/basic/project_name/settings/prod.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/basic/project_name/urls.py` & `coderedcms-3.0.4/coderedcms/project_template/basic/project_name/urls.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/basic/pyproject.toml` & `coderedcms-3.0.4/coderedcms/project_template/basic/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/basic/website/migrations/0001_initial.py` & `coderedcms-3.0.4/coderedcms/project_template/basic/website/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/basic/website/migrations/0002_initial_data.py` & `coderedcms-3.0.4/coderedcms/project_template/basic/website/migrations/0002_initial_data.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/basic/website/models.py` & `coderedcms-3.0.4/coderedcms/project_template/basic/website/models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/pro/.editorconfig` & `coderedcms-3.0.4/coderedcms/project_template/pro/.editorconfig`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/pro/.gitignore` & `coderedcms-3.0.4/coderedcms/project_template/pro/.gitignore`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/pro/README.md` & `coderedcms-3.0.4/coderedcms/project_template/pro/README.md`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/pro/custom_media/migrations/0001_initial.py` & `coderedcms-3.0.4/coderedcms/project_template/pro/custom_media/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/pro/custom_media/models.py` & `coderedcms-3.0.4/coderedcms/project_template/pro/custom_media/models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/pro/custom_user/admin.py` & `coderedcms-3.0.4/coderedcms/project_template/pro/custom_user/admin.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/pro/custom_user/migrations/0001_initial.py` & `coderedcms-3.0.4/coderedcms/project_template/pro/custom_user/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/pro/custom_user/models.py` & `coderedcms-3.0.4/coderedcms/project_template/pro/custom_user/models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/pro/project_name/settings/base.py` & `coderedcms-3.0.4/coderedcms/project_template/pro/project_name/settings/base.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/pro/project_name/settings/prod.py` & `coderedcms-3.0.4/coderedcms/project_template/pro/project_name/settings/prod.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/pro/project_name/urls.py` & `coderedcms-3.0.4/coderedcms/project_template/pro/project_name/urls.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/pro/pyproject.toml` & `coderedcms-3.0.4/coderedcms/project_template/pro/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/pro/website/migrations/0001_initial.py` & `coderedcms-3.0.4/coderedcms/project_template/pro/website/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/pro/website/migrations/0002_initial_data.py` & `coderedcms-3.0.4/coderedcms/project_template/pro/website/migrations/0002_initial_data.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/pro/website/models.py` & `coderedcms-3.0.4/coderedcms/project_template/pro/website/models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/pro/website/static/website/src/_variables.scss` & `coderedcms-3.0.4/coderedcms/project_template/pro/website/static/website/src/_variables.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/pro/website/static/website/src/custom.scss` & `coderedcms-3.0.4/coderedcms/project_template/pro/website/static/website/src/custom.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/project_template/pro/website/templates/coderedcms/pages/base.html` & `coderedcms-3.0.4/coderedcms/project_template/pro/website/templates/coderedcms/pages/base.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/settings.py` & `coderedcms-3.0.4/coderedcms/settings.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/css/crx-admin.css` & `coderedcms-3.0.4/coderedcms/static/coderedcms/css/crx-admin.css`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/css/crx-front.css` & `coderedcms-3.0.4/coderedcms/static/coderedcms/css/crx-front.css`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/css/crx-front.css.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/css/crx-front.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/css/crx-front.min.css` & `coderedcms-3.0.4/coderedcms/static/coderedcms/css/crx-front.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/js/crx-editor.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/js/crx-editor.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/js/crx-events.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/js/crx-events.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/js/crx-front.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/js/crx-front.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/js/crx-maps.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/js/crx-maps.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/js/crx-streamforms.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/js/crx-streamforms.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/scss/_crx-location.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/scss/_crx-location.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/scss/_crx-navbar.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/scss/_crx-navbar.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/scss/_crx-pricelist.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/scss/_crx-pricelist.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/LICENSE` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/LICENSE`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.css` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.css.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.min.css` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.css` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.css.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.min.css` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.css` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.css.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.min.css` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.min.css.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.css` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.css.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.min.css` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.css` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.css.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.min.css` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.min.css.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.js.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.min.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.min.js.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js.map` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/dist/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/alert.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/alert.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/base-component.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/base-component.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/button.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/button.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/carousel.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/carousel.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/collapse.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/collapse.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dom/data.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dom/data.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dom/event-handler.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dom/event-handler.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dom/manipulator.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dom/manipulator.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dom/selector-engine.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dom/selector-engine.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dropdown.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/dropdown.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/modal.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/modal.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/offcanvas.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/offcanvas.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/popover.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/popover.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/scrollspy.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/scrollspy.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tab.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tab.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/toast.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/toast.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tooltip.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/tooltip.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/backdrop.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/backdrop.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/component-functions.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/component-functions.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/config.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/config.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/focustrap.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/focustrap.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/index.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/index.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/sanitizer.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/sanitizer.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/scrollbar.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/scrollbar.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/swipe.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/swipe.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/template-factory.js` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/js/src/util/template-factory.js`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_accordion.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_accordion.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_alert.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_alert.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_badge.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_badge.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_breadcrumb.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_button-group.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_button-group.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_buttons.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_buttons.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_card.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_card.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_carousel.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_carousel.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_close.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_close.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_containers.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_containers.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_dropdown.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_functions.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_functions.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_grid.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_grid.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_images.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_images.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_list-group.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_list-group.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_maps.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_maps.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_mixins.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_modal.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_modal.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_nav.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_navbar.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_navbar.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_offcanvas.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_pagination.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_pagination.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_placeholders.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_placeholders.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_popover.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_popover.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_progress.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_progress.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_reboot.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_reboot.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_root.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_root.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_spinners.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_spinners.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_tables.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_tables.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_toasts.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_toasts.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_tooltip.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_type.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_type.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_utilities.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_utilities.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_variables-dark.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_variables-dark.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/_variables.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap-grid.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_floating-labels.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-check.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-control.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-range.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-select.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_input-group.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_labels.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_colored-links.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_colored-links.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_icon-link.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_icon-link.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_position.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_alert.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_alert.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_border-radius.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_breakpoints.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_buttons.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_caret.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_deprecate.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_forms.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_gradients.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_grid.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_list-group.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_list-group.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_table-variants.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_transition.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_utilities.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_visually-hidden.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/mixins/_color-modes.test.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/mixins/_color-modes.test.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/mixins/_utilities.test.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/mixins/_utilities.test.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/utilities/_api.test.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/tests/utilities/_api.test.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/utilities/_api.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/static/coderedcms/vendor/bootstrap/scss/vendor/_rfs.scss` & `coderedcms-3.0.4/coderedcms/static/coderedcms/vendor/bootstrap/scss/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/500.html` & `coderedcms-3.0.4/coderedcms/templates/500.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/accordion_block.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/accordion_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/article_block_card.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/article_block_card.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/base_link_block.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/base_link_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/button_block.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/button_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/card_block.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/card_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/card_blurb.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/card_blurb.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/card_foot.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/card_foot.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/card_head.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/card_head.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/card_head_foot.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/card_head_foot.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/card_img.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/card_img.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/carousel_block.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/carousel_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/content_wall_block.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/content_wall_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/download_block.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/download_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/film_strip_block.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/film_strip_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/google_map.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/google_map.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/hero_block.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/hero_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/image_gallery_block.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/image_gallery_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/image_link_block.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/image_link_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/modal_block.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/modal_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/pagelist_article_media.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/pagelist_article_media.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/pagelist_list_group.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/pagelist_list_group.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/pagepreview_card.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/pagepreview_card.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/pagepreview_form.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/pagepreview_form.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/pricelistitem_block.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/pricelistitem_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/blocks/table_block.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/blocks/table_block.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/formfields/mailchimp/subscriber_integration_js.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/formfields/mailchimp/subscriber_integration_js.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/formfields/mailchimp/subscriber_integration_widget.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/formfields/mailchimp/subscriber_integration_widget.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-check-square-o.svg` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-check-square-o.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-font.svg` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-font.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-hand-pointer-o.svg` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-hand-pointer-o.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-hashtag.svg` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-hashtag.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-header.svg` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-header.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-list-alt.svg` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-list-alt.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-puzzle-piece.svg` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-puzzle-piece.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-recycle.svg` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-recycle.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-universal-access.svg` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-universal-access.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/icons/cr-usd.svg` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/icons/cr-usd.svg`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/classifier_dropdowns.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/classifier_dropdowns.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/classifier_nav.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/classifier_nav.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/ical/calendar.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/ical/calendar.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/ical/single_ical_button.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/ical/single_ical_button.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/pagination.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/includes/stream_forms/render_field.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/includes/stream_forms/render_field.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/article_index_page.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/article_index_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/article_page.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/article_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/article_page.search.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/article_page.search.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/base.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/base.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/event_index_page.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/event_index_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/event_page.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/event_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/form_page.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/form_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/form_page.mini.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/form_page.mini.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/location_index_page.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/location_index_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/location_page.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/location_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/search.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/search.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/stream_form_page.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/stream_form_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/pages/web_page.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/pages/web_page.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/snippets/navbar.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/snippets/navbar.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/coderedcms/widgets/checkbox_classifiers.html` & `coderedcms-3.0.4/coderedcms/templates/coderedcms/widgets/checkbox_classifiers.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/wagtailadmin/base.html` & `coderedcms-3.0.4/coderedcms/templates/wagtailadmin/base.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html` & `coderedcms-3.0.4/coderedcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/wagtailcore/password_required.html` & `coderedcms-3.0.4/coderedcms/templates/wagtailcore/password_required.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/wagtailembeds/embed_frontend.html` & `coderedcms-3.0.4/coderedcms/templates/wagtailembeds/embed_frontend.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/wagtailforms/list_submissions.html` & `coderedcms-3.0.4/coderedcms/templates/wagtailforms/list_submissions.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templates/wagtailimportexport/import_from_csv.html` & `coderedcms-3.0.4/coderedcms/templates/wagtailimportexport/import_from_csv.html`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/templatetags/coderedcms_tags.py` & `coderedcms-3.0.4/coderedcms/templatetags/coderedcms_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from bs4 import BeautifulSoup
 from django import template
 from django.db.models.query import QuerySet
 from django.forms import ClearableFileInput
 from django.utils.html import mark_safe
 from wagtail.models import Collection
-from wagtail.images.models import Image
+from wagtail.images import get_image_model
 
 from coderedcms import utils, __version__
 from coderedcms.blocks import CoderedAdvSettings
 from coderedcms.forms import SearchForm
 from coderedcms.models.snippet_models import Navbar, Footer
 from coderedcms.settings import crx_settings as crx_settings_obj
 from coderedcms.settings import get_bootstrap_setting
@@ -61,15 +61,15 @@
         return curr_url == other_url
     return False
 
 
 @register.simple_tag
 def get_pictures(collection_id):
     collection = Collection.objects.get(id=collection_id)
-    return Image.objects.filter(collection=collection)
+    return get_image_model().objects.filter(collection=collection)
 
 
 @register.simple_tag(takes_context=True)
 def get_navbar_css(context):
     layout = LayoutSettings.for_request(context["request"])
     fixed = "fixed-top" if layout.navbar_fixed else ""
     return " ".join(
```

### Comparing `coderedcms-3.0.3/coderedcms/tests/settings.py` & `coderedcms-3.0.4/coderedcms/tests/settings.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/tests/test_bin.py` & `coderedcms-3.0.4/coderedcms/tests/test_bin.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/tests/test_templates.py` & `coderedcms-3.0.4/coderedcms/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/tests/test_templatetags.py` & `coderedcms-3.0.4/coderedcms/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/tests/test_urls.py` & `coderedcms-3.0.4/coderedcms/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/tests/testapp/migrations/0001_initial.py` & `coderedcms-3.0.4/coderedcms/tests/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/tests/testapp/migrations/0002_initial.py` & `coderedcms-3.0.4/coderedcms/tests/testapp/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/tests/testapp/migrations/0003_eventindexpage_eventoccurrence_eventpage_locationindexpage_locationpage.py` & `coderedcms-3.0.4/coderedcms/tests/testapp/migrations/0003_eventindexpage_eventoccurrence_eventpage_locationindexpage_locationpage.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/tests/testapp/migrations/0004_streamformconfirmemail_streamformpage.py` & `coderedcms-3.0.4/coderedcms/tests/testapp/migrations/0004_streamformconfirmemail_streamformpage.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/tests/testapp/migrations/0005_auto_20210908_1741.py` & `coderedcms-3.0.4/coderedcms/tests/testapp/migrations/0005_auto_20210908_1741.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/tests/testapp/migrations/0006_indextestpage.py` & `coderedcms-3.0.4/coderedcms/tests/testapp/migrations/0006_indextestpage.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/tests/testapp/migrations/0007_auto_20210910_1614.py` & `coderedcms-3.0.4/coderedcms/tests/testapp/migrations/0007_auto_20210910_1614.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/tests/testapp/models.py` & `coderedcms-3.0.4/coderedcms/tests/testapp/models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/tests/urls.py` & `coderedcms-3.0.4/coderedcms/tests/urls.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/urls.py` & `coderedcms-3.0.4/coderedcms/urls.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/utils.py` & `coderedcms-3.0.4/coderedcms/utils.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/views.py` & `coderedcms-3.0.4/coderedcms/views.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/wagtail_flexible_forms/LICENSE` & `coderedcms-3.0.4/coderedcms/wagtail_flexible_forms/LICENSE`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/wagtail_flexible_forms/blocks.py` & `coderedcms-3.0.4/coderedcms/wagtail_flexible_forms/blocks.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/wagtail_flexible_forms/edit_handlers.py` & `coderedcms-3.0.4/coderedcms/wagtail_flexible_forms/edit_handlers.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/wagtail_flexible_forms/models.py` & `coderedcms-3.0.4/coderedcms/wagtail_flexible_forms/models.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/wagtail_hooks.py` & `coderedcms-3.0.4/coderedcms/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms/widgets.py` & `coderedcms-3.0.4/coderedcms/widgets.py`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/coderedcms.egg-info/PKG-INFO` & `coderedcms-3.0.4/coderedcms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coderedcms
-Version: 3.0.3
+Version: 3.0.4
 Summary: Wagtail-based CMS by CodeRed for building marketing websites.
 Home-page: https://github.com/coderedcorp/coderedcms
 Author: CodeRed LLC
 Author-email: info@coderedcorp.com
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `coderedcms-3.0.3/coderedcms.egg-info/SOURCES.txt` & `coderedcms-3.0.4/coderedcms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coderedcms-3.0.3/setup.py` & `coderedcms-3.0.4/setup.py`

 * *Files identical despite different names*

