# Comparing `tmp/vitriolic-3.3.9.tar.gz` & `tmp/vitriolic-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vitriolic-3.3.9.tar", last modified: Wed May  8 12:46:30 2024, max compression
+gzip compressed data, was "vitriolic-3.4.0.tar", last modified: Fri May 17 23:21:08 2024, max compression
```

## Comparing `vitriolic-3.3.9.tar` & `vitriolic-3.4.0.tar`

### file list

```diff
@@ -1,1225 +1,1225 @@
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.534271 vitriolic-3.3.9/
--rw-r--r--   0 gary       (501) staff       (20)      436 2019-10-18 22:04:04.000000 vitriolic-3.3.9/.editorconfig
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.881462 vitriolic-3.3.9/.github/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.967790 vitriolic-3.3.9/.github/workflows/
--rw-r--r--   0 gary       (501) staff       (20)     1153 2024-02-09 07:02:29.000000 vitriolic-3.3.9/.github/workflows/django.yml
--rw-r--r--   0 gary       (501) staff       (20)       80 2023-05-21 21:21:54.000000 vitriolic-3.3.9/.gitignore
--rw-r--r--   0 gary       (501) staff       (20)      476 2019-10-18 22:04:04.000000 vitriolic-3.3.9/.pre-commit-config.yaml
--rw-r--r--   0 gary       (501) staff       (20)     1302 2019-10-18 22:04:04.000000 vitriolic-3.3.9/ISSUES.md
--rw-r--r--   0 gary       (501) staff       (20)     1524 2019-10-18 22:04:04.000000 vitriolic-3.3.9/LICENSE
--rw-r--r--   0 gary       (501) staff       (20)      862 2022-06-12 11:19:40.000000 vitriolic-3.3.9/MANIFEST.in
--rw-r--r--   0 gary       (501) staff       (20)     5002 2024-05-08 12:46:30.533518 vitriolic-3.3.9/PKG-INFO
--rw-r--r--   0 gary       (501) staff       (20)     1118 2023-05-21 21:14:55.000000 vitriolic-3.3.9/README.md
--rw-r--r--   0 gary       (501) staff       (20)     1990 2024-04-13 04:07:31.000000 vitriolic-3.3.9/pyproject.toml
--rw-r--r--   0 gary       (501) staff       (20)      170 2023-05-21 21:14:55.000000 vitriolic-3.3.9/renovate.json
--rw-r--r--   0 gary       (501) staff       (20)       38 2024-05-08 12:46:30.534424 vitriolic-3.3.9/setup.cfg
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.969825 vitriolic-3.3.9/tests/
--rw-r--r--   0 gary       (501) staff       (20)      110 2019-10-31 21:17:24.000000 vitriolic-3.3.9/tests/.coveragerc
--rw-r--r--   0 gary       (501) staff       (20)       32 2019-10-31 21:17:24.000000 vitriolic-3.3.9/tests/.gitignore
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/__init__.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.974099 vitriolic-3.3.9/tests/example_app/
--rw-r--r--   0 gary       (501) staff       (20)      157 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/example_app/__init__.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.974994 vitriolic-3.3.9/tests/example_app/fixtures/
--rw-r--r--   0 gary       (501) staff       (20)     1626 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/example_app/fixtures/query_string.json
--rw-r--r--   0 gary       (501) staff       (20)      162 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/example_app/forms.py
--rw-r--r--   0 gary       (501) staff       (20)      465 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/example_app/models.py
--rw-r--r--   0 gary       (501) staff       (20)     6846 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tests/example_app/sites.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.882688 vitriolic-3.3.9/tests/example_app/templates/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.884328 vitriolic-3.3.9/tests/example_app/templates/example_app/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.977194 vitriolic-3.3.9/tests/example_app/templates/example_app/context/
--rw-r--r--   0 gary       (501) staff       (20)       15 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/example_app/templates/example_app/context/env.html
--rw-r--r--   0 gary       (501) staff       (20)       11 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/example_app/templates/example_app/context/site.html
--rw-r--r--   0 gary       (501) staff       (20)       16 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/example_app/templates/example_app/context/tz.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.977942 vitriolic-3.3.9/tests/example_app/templates/example_app/datetime/
--rw-r--r--   0 gary       (501) staff       (20)       82 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/example_app/templates/example_app/datetime/edit.related.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.982220 vitriolic-3.3.9/tests/example_app/templates/example_app/generic/
--rw-r--r--   0 gary       (501) staff       (20)      282 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/example_app/templates/example_app/generic/detail.html
--rw-r--r--   0 gary       (501) staff       (20)      404 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/example_app/templates/example_app/generic/edit.html
--rw-r--r--   0 gary       (501) staff       (20)      461 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/example_app/templates/example_app/generic/edit_multiple.html
--rw-r--r--   0 gary       (501) staff       (20)      356 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/example_app/templates/example_app/generic/list.html
--rw-r--r--   0 gary       (501) staff       (20)      649 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/example_app/templates/example_app/generic/permissions.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.883978 vitriolic-3.3.9/tests/example_app/templates/example_app/pagination/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.982944 vitriolic-3.3.9/tests/example_app/templates/example_app/pagination/testdatetimefield/
--rw-r--r--   0 gary       (501) staff       (20)      313 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/example_app/templates/example_app/pagination/testdatetimefield/list.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.884638 vitriolic-3.3.9/tests/example_app/templates/example_app/querystring/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.983674 vitriolic-3.3.9/tests/example_app/templates/example_app/querystring/testdatetimefield/
--rw-r--r--   0 gary       (501) staff       (20)      314 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/example_app/templates/example_app/querystring/testdatetimefield/list.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.985120 vitriolic-3.3.9/tests/example_app/tests/
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/example_app/tests/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)      683 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tests/example_app/tests/factories.py
--rw-r--r--   0 gary       (501) staff       (20)      953 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tests/example_app/urls.py
--rw-r--r--   0 gary       (501) staff       (20)      141 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/example_app/views.py
--rwxr-xr-x   0 gary       (501) staff       (20)      815 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/manage.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.988200 vitriolic-3.3.9/tests/vitriolic/
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/vitriolic/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)     5754 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tests/vitriolic/settings.py
--rw-r--r--   0 gary       (501) staff       (20)      438 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tests/vitriolic/urls.py
--rw-r--r--   0 gary       (501) staff       (20)      396 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tests/vitriolic/wsgi.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.988912 vitriolic-3.3.9/touchtechnology/
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/__init__.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.993603 vitriolic-3.3.9/touchtechnology/admin/
--rw-r--r--   0 gary       (501) staff       (20)      109 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)     3485 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/apps.py
--rw-r--r--   0 gary       (501) staff       (20)     4923 2024-04-13 04:06:41.000000 vitriolic-3.3.9/touchtechnology/admin/base.py
--rw-r--r--   0 gary       (501) staff       (20)     1594 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/forms.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.891212 vitriolic-3.3.9/touchtechnology/admin/locale/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.887945 vitriolic-3.3.9/touchtechnology/admin/locale/de/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.995025 vitriolic-3.3.9/touchtechnology/admin/locale/de/LC_MESSAGES/
--rw-r--r--   0 gary       (501) staff       (20)      421 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/admin/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 gary       (501) staff       (20)     2804 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/admin/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.889375 vitriolic-3.3.9/touchtechnology/admin/locale/en-AU/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.996518 vitriolic-3.3.9/touchtechnology/admin/locale/en-AU/LC_MESSAGES/
--rw-r--r--   0 gary       (501) staff       (20)      378 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/admin/locale/en-AU/LC_MESSAGES/django.mo
--rw-r--r--   0 gary       (501) staff       (20)     2757 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/admin/locale/en-AU/LC_MESSAGES/django.po
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.890636 vitriolic-3.3.9/touchtechnology/admin/locale/fr/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.998176 vitriolic-3.3.9/touchtechnology/admin/locale/fr/LC_MESSAGES/
--rw-r--r--   0 gary       (501) staff       (20)      971 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/admin/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 gary       (501) staff       (20)     3234 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/admin/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.891584 vitriolic-3.3.9/touchtechnology/admin/locale/ja/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.001025 vitriolic-3.3.9/touchtechnology/admin/locale/ja/LC_MESSAGES/
--rw-r--r--   0 gary       (501) staff       (20)      414 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/admin/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 gary       (501) staff       (20)     2797 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/admin/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0 gary       (501) staff       (20)      825 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/mixins.py
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/models.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.004898 vitriolic-3.3.9/touchtechnology/admin/sites/
--rw-r--r--   0 gary       (501) staff       (20)       76 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/sites/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)     5959 2024-04-13 04:06:43.000000 vitriolic-3.3.9/touchtechnology/admin/sites/admin.py
--rw-r--r--   0 gary       (501) staff       (20)     6045 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/sites/auth.py
--rw-r--r--   0 gary       (501) staff       (20)     1529 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/sites/settings.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.915872 vitriolic-3.3.9/touchtechnology/admin/static/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.009101 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/
--rw-r--r--   0 gary       (501) staff       (20)      425 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/CHANGELOG.md
--rw-r--r--   0 gary       (501) staff       (20)    14386 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/Gruntfile.js
--rw-r--r--   0 gary       (501) staff       (20)      641 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/bower.json
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.894770 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.019272 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/css/
--rw-r--r--   0 gary       (501) staff       (20)    26132 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/css/bootstrap-theme.css
--rw-r--r--   0 gary       (501) staff       (20)    47706 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/css/bootstrap-theme.css.map
--rw-r--r--   0 gary       (501) staff       (20)    23409 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/css/bootstrap-theme.min.css
--rw-r--r--   0 gary       (501) staff       (20)    25648 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/css/bootstrap-theme.min.css.map
--rw-r--r--   0 gary       (501) staff       (20)   146010 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/css/bootstrap.css
--rw-r--r--   0 gary       (501) staff       (20)   389287 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/css/bootstrap.css.map
--rw-r--r--   0 gary       (501) staff       (20)   121200 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/css/bootstrap.min.css
--rw-r--r--   0 gary       (501) staff       (20)   542194 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/css/bootstrap.min.css.map
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.025349 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/fonts/
--rw-r--r--   0 gary       (501) staff       (20)    20127 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 gary       (501) staff       (20)   108738 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 gary       (501) staff       (20)    45404 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 gary       (501) staff       (20)    23424 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 gary       (501) staff       (20)    18028 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.028076 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/js/
--rw-r--r--   0 gary       (501) staff       (20)    69707 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/js/bootstrap.js
--rw-r--r--   0 gary       (501) staff       (20)    37045 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/js/bootstrap.min.js
--rw-r--r--   0 gary       (501) staff       (20)      484 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/js/npm.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.034125 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/grunt/
--rw-r--r--   0 gary       (501) staff       (20)      990 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/grunt/bs-commonjs-generator.js
--rw-r--r--   0 gary       (501) staff       (20)     1405 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/grunt/bs-glyphicons-data-generator.js
--rw-r--r--   0 gary       (501) staff       (20)     6075 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/grunt/bs-lessdoc-parser.js
--rw-r--r--   0 gary       (501) staff       (20)     1349 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/grunt/bs-raw-files-generator.js
--rwxr-xr-x   0 gary       (501) staff       (20)     2909 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/grunt/change-version.js
--rw-r--r--   0 gary       (501) staff       (20)     1395 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/grunt/configBridge.json
--rw-r--r--   0 gary       (501) staff       (20)    93626 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/grunt/npm-shrinkwrap.json
--rw-r--r--   0 gary       (501) staff       (20)     1439 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/grunt/sauce_browsers.yml
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.046447 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/
--rw-r--r--   0 gary       (501) staff       (20)     4838 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/affix.js
--rw-r--r--   0 gary       (501) staff       (20)     2284 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/alert.js
--rw-r--r--   0 gary       (501) staff       (20)     3824 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/button.js
--rw-r--r--   0 gary       (501) staff       (20)     7141 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/carousel.js
--rw-r--r--   0 gary       (501) staff       (20)     5991 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/collapse.js
--rw-r--r--   0 gary       (501) staff       (20)     4743 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/dropdown.js
--rw-r--r--   0 gary       (501) staff       (20)     9987 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/modal.js
--rw-r--r--   0 gary       (501) staff       (20)     3163 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/popover.js
--rw-r--r--   0 gary       (501) staff       (20)     4707 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/scrollspy.js
--rw-r--r--   0 gary       (501) staff       (20)     3905 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/tab.js
--rw-r--r--   0 gary       (501) staff       (20)    16719 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/tooltip.js
--rw-r--r--   0 gary       (501) staff       (20)     1831 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/transition.js
--rw-r--r--   0 gary       (501) staff       (20)      964 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/package.js
--rw-r--r--   0 gary       (501) staff       (20)     2200 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/package.json
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.051002 vitriolic-3.3.9/touchtechnology/admin/static/css/
--rw-r--r--   0 gary       (501) staff       (20)       84 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/css/Makefile
--rw-r--r--   0 gary       (501) staff       (20)     1172 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/css/custom.css
--rw-r--r--   0 gary       (501) staff       (20)     1373 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/css/custom.less
--rwxr-xr-x   0 gary       (501) staff       (20)    51742 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/css/mvpready-admin.css
--rwxr-xr-x   0 gary       (501) staff       (20)    39265 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/css/mvpready-landing.css
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.073687 vitriolic-3.3.9/touchtechnology/admin/static/flot/
--rwxr-xr-x   0 gary       (501) staff       (20)      413 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/.bower.json
--rwxr-xr-x   0 gary       (501) staff       (20)       40 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/.gitignore
--rwxr-xr-x   0 gary       (501) staff       (20)       35 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/.travis.yml
--rwxr-xr-x   0 gary       (501) staff       (20)     1069 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/LICENSE.txt
--rwxr-xr-x   0 gary       (501) staff       (20)      285 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/Makefile
--rwxr-xr-x   0 gary       (501) staff       (20)      114 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/component.json
--rwxr-xr-x   0 gary       (501) staff       (20)    41943 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/excanvas.js
--rwxr-xr-x   0 gary       (501) staff       (20)    19314 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/excanvas.min.js
--rwxr-xr-x   0 gary       (501) staff       (20)      837 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/flot.jquery.json
--rwxr-xr-x   0 gary       (501) staff       (20)     6151 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.colorhelpers.js
--rwxr-xr-x   0 gary       (501) staff       (20)     9599 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.canvas.js
--rwxr-xr-x   0 gary       (501) staff       (20)     6033 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.categories.js
--rwxr-xr-x   0 gary       (501) staff       (20)     5419 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.crosshair.js
--rwxr-xr-x   0 gary       (501) staff       (20)    12614 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.errorbars.js
--rwxr-xr-x   0 gary       (501) staff       (20)     5257 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.fillbetween.js
--rwxr-xr-x   0 gary       (501) staff       (20)     7360 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.image.js
--rwxr-xr-x   0 gary       (501) staff       (20)   122971 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.js
--rwxr-xr-x   0 gary       (501) staff       (20)    14216 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.navigate.js
--rwxr-xr-x   0 gary       (501) staff       (20)    23809 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.pie.js
--rwxr-xr-x   0 gary       (501) staff       (20)     3314 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.resize.js
--rwxr-xr-x   0 gary       (501) staff       (20)    13141 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.selection.js
--rwxr-xr-x   0 gary       (501) staff       (20)     7090 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.stack.js
--rwxr-xr-x   0 gary       (501) staff       (20)     2505 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.symbol.js
--rwxr-xr-x   0 gary       (501) staff       (20)     4480 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.threshold.js
--rwxr-xr-x   0 gary       (501) staff       (20)    11768 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.time.js
--rwxr-xr-x   0 gary       (501) staff       (20)   266057 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.js
--rwxr-xr-x   0 gary       (501) staff       (20)      154 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot/package.json
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.076577 vitriolic-3.3.9/touchtechnology/admin/static/flot.tooltip/
--rwxr-xr-x   0 gary       (501) staff       (20)      532 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot.tooltip/.bower.json
--rwxr-xr-x   0 gary       (501) staff       (20)      212 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot.tooltip/bower.json
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.082149 vitriolic-3.3.9/touchtechnology/admin/static/flot.tooltip/js/
--rwxr-xr-x   0 gary       (501) staff       (20)    19415 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot.tooltip/js/excanvas.min.js
--rwxr-xr-x   0 gary       (501) staff       (20)   122971 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot.tooltip/js/jquery.flot.js
--rwxr-xr-x   0 gary       (501) staff       (20)    19258 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot.tooltip/js/jquery.flot.tooltip.js
--rwxr-xr-x   0 gary       (501) staff       (20)     7380 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot.tooltip/js/jquery.flot.tooltip.min.js
--rwxr-xr-x   0 gary       (501) staff       (20)    18958 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/flot.tooltip/js/jquery.flot.tooltip.source.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.085185 vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/
--rwxr-xr-x   0 gary       (501) staff       (20)      696 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/.bower.json
--rwxr-xr-x   0 gary       (501) staff       (20)      301 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/.gitignore
--rwxr-xr-x   0 gary       (501) staff       (20)      427 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/.npmignore
--rwxr-xr-x   0 gary       (501) staff       (20)      412 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/bower.json
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.087356 vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/css/
--rwxr-xr-x   0 gary       (501) staff       (20)    37414 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/css/font-awesome.css
--rwxr-xr-x   0 gary       (501) staff       (20)    21778 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/css/font-awesome.css.map
--rwxr-xr-x   0 gary       (501) staff       (20)    31000 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/css/font-awesome.min.css
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.092937 vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/fonts/
--rwxr-xr-x   0 gary       (501) staff       (20)   134808 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/fonts/FontAwesome.otf
--rwxr-xr-x   0 gary       (501) staff       (20)   165742 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/fonts/fontawesome-webfont.eot
--rwxr-xr-x   0 gary       (501) staff       (20)   444379 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/fonts/fontawesome-webfont.svg
--rwxr-xr-x   0 gary       (501) staff       (20)   165548 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/fonts/fontawesome-webfont.ttf
--rwxr-xr-x   0 gary       (501) staff       (20)    98024 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/fonts/fontawesome-webfont.woff
--rwxr-xr-x   0 gary       (501) staff       (20)    77160 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.093625 vitriolic-3.3.9/touchtechnology/admin/static/img/
--rwxr-xr-x   0 gary       (501) staff       (20)    49582 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/img/logo.png
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.095403 vitriolic-3.3.9/touchtechnology/admin/static/jquery/
--rwxr-xr-x   0 gary       (501) staff       (20)      730 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/.bower.json
--rwxr-xr-x   0 gary       (501) staff       (20)     1099 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/MIT-LICENSE.txt
--rwxr-xr-x   0 gary       (501) staff       (20)      425 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/bower.json
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.162208 vitriolic-3.3.9/touchtechnology/admin/static/jquery/dist/
--rwxr-xr-x   0 gary       (501) staff       (20)   282766 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/dist/jquery.js
--rwxr-xr-x   0 gary       (501) staff       (20)    95821 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/dist/jquery.min.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.176338 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.179133 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/ajax/
--rwxr-xr-x   0 gary       (501) staff       (20)     2516 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/ajax/jsonp.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1681 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/ajax/load.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1476 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/ajax/parseJSON.js
--rwxr-xr-x   0 gary       (501) staff       (20)      650 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/ajax/parseXML.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1964 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/ajax/script.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.180212 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/ajax/var/
--rwxr-xr-x   0 gary       (501) staff       (20)       73 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/ajax/var/nonce.js
--rwxr-xr-x   0 gary       (501) staff       (20)       40 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/ajax/var/rquery.js
--rwxr-xr-x   0 gary       (501) staff       (20)     5786 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/ajax/xhr.js
--rwxr-xr-x   0 gary       (501) staff       (20)    21812 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/ajax.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.182990 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/attributes/
--rwxr-xr-x   0 gary       (501) staff       (20)     7263 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/attributes/attr.js
--rwxr-xr-x   0 gary       (501) staff       (20)     4116 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/attributes/classes.js
--rwxr-xr-x   0 gary       (501) staff       (20)     3138 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/attributes/prop.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1994 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/attributes/support.js
--rwxr-xr-x   0 gary       (501) staff       (20)     4303 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/attributes/val.js
--rwxr-xr-x   0 gary       (501) staff       (20)      200 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/attributes.js
--rwxr-xr-x   0 gary       (501) staff       (20)     5506 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/callbacks.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.185796 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/core/
--rwxr-xr-x   0 gary       (501) staff       (20)     1219 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/core/access.js
--rwxr-xr-x   0 gary       (501) staff       (20)     3716 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/core/init.js
--rwxr-xr-x   0 gary       (501) staff       (20)      938 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/core/parseHTML.js
--rwxr-xr-x   0 gary       (501) staff       (20)     3896 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/core/ready.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.186369 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/core/var/
--rwxr-xr-x   0 gary       (501) staff       (20)       91 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/core/var/rsingleTag.js
--rwxr-xr-x   0 gary       (501) staff       (20)    12500 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/core.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.189971 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/css/
--rwxr-xr-x   0 gary       (501) staff       (20)      785 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/css/addGetHookIf.js
--rwxr-xr-x   0 gary       (501) staff       (20)     3307 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/css/curCSS.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1907 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/css/defaultDisplay.js
--rwxr-xr-x   0 gary       (501) staff       (20)      542 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/css/hiddenVisibleSelectors.js
--rwxr-xr-x   0 gary       (501) staff       (20)     4823 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/css/support.js
--rwxr-xr-x   0 gary       (501) staff       (20)      555 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/css/swap.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.192544 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/css/var/
--rwxr-xr-x   0 gary       (501) staff       (20)       70 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/css/var/cssExpand.js
--rwxr-xr-x   0 gary       (501) staff       (20)      355 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/css/var/isHidden.js
--rwxr-xr-x   0 gary       (501) staff       (20)       45 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/css/var/rmargin.js
--rwxr-xr-x   0 gary       (501) staff       (20)      113 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/css/var/rnumnonpx.js
--rwxr-xr-x   0 gary       (501) staff       (20)    14612 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/css.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.193563 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/data/
--rwxr-xr-x   0 gary       (501) staff       (20)      567 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/data/accepts.js
--rwxr-xr-x   0 gary       (501) staff       (20)      438 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/data/support.js
--rwxr-xr-x   0 gary       (501) staff       (20)     8509 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/data.js
--rwxr-xr-x   0 gary       (501) staff       (20)     4413 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/deferred.js
--rwxr-xr-x   0 gary       (501) staff       (20)      223 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/deprecated.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1881 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/dimensions.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.195397 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/effects/
--rwxr-xr-x   0 gary       (501) staff       (20)     3034 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/effects/Tween.js
--rwxr-xr-x   0 gary       (501) staff       (20)      225 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/effects/animatedSelector.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1459 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/effects/support.js
--rwxr-xr-x   0 gary       (501) staff       (20)    17243 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/effects.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.197256 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/event/
--rwxr-xr-x   0 gary       (501) staff       (20)     1094 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/event/alias.js
--rwxr-xr-x   0 gary       (501) staff       (20)      641 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/event/support.js
--rwxr-xr-x   0 gary       (501) staff       (20)    30072 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/event.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.198649 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/exports/
--rwxr-xr-x   0 gary       (501) staff       (20)     1006 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/exports/amd.js
--rwxr-xr-x   0 gary       (501) staff       (20)      641 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/exports/global.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1405 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/intro.js
--rwxr-xr-x   0 gary       (501) staff       (20)      571 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/jquery.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.199612 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/manipulation/
--rwxr-xr-x   0 gary       (501) staff       (20)      240 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/manipulation/_evalUrl.js
--rwxr-xr-x   0 gary       (501) staff       (20)     2476 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/manipulation/support.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.200080 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/manipulation/var/
--rwxr-xr-x   0 gary       (501) staff       (20)       59 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/manipulation/var/rcheckableType.js
--rwxr-xr-x   0 gary       (501) staff       (20)    20616 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/manipulation.js
--rwxr-xr-x   0 gary       (501) staff       (20)     5856 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/offset.js
--rwxr-xr-x   0 gary       (501) staff       (20)        5 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/outro.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.200547 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/queue/
--rwxr-xr-x   0 gary       (501) staff       (20)      561 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/queue/delay.js
--rwxr-xr-x   0 gary       (501) staff       (20)     3071 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/queue.js
--rwxr-xr-x   0 gary       (501) staff       (20)      294 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/selector-sizzle.js
--rwxr-xr-x   0 gary       (501) staff       (20)       33 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/selector.js
--rwxr-xr-x   0 gary       (501) staff       (20)     3211 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/serialize.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.911322 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/sizzle/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.201684 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/sizzle/dist/
--rwxr-xr-x   0 gary       (501) staff       (20)    58579 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/sizzle/dist/sizzle.js
--rwxr-xr-x   0 gary       (501) staff       (20)    18574 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/sizzle/dist/sizzle.min.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1697 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/support.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.202305 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/traversing/
--rwxr-xr-x   0 gary       (501) staff       (20)     2466 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/traversing/findFilter.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.202768 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/traversing/var/
--rwxr-xr-x   0 gary       (501) staff       (20)      110 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/traversing/var/rneedsContext.js
--rwxr-xr-x   0 gary       (501) staff       (20)     4575 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/traversing.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.208625 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/var/
--rwxr-xr-x   0 gary       (501) staff       (20)       64 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/var/class2type.js
--rwxr-xr-x   0 gary       (501) staff       (20)       84 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/var/concat.js
--rwxr-xr-x   0 gary       (501) staff       (20)       36 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/var/deletedIds.js
--rwxr-xr-x   0 gary       (501) staff       (20)       92 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/var/hasOwn.js
--rwxr-xr-x   0 gary       (501) staff       (20)       85 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/var/indexOf.js
--rwxr-xr-x   0 gary       (501) staff       (20)       80 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/var/pnum.js
--rwxr-xr-x   0 gary       (501) staff       (20)       82 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/var/push.js
--rwxr-xr-x   0 gary       (501) staff       (20)       42 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/var/rnotwhite.js
--rwxr-xr-x   0 gary       (501) staff       (20)       83 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/var/slice.js
--rwxr-xr-x   0 gary       (501) staff       (20)       50 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/var/strundefined.js
--rwxr-xr-x   0 gary       (501) staff       (20)       99 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/var/support.js
--rwxr-xr-x   0 gary       (501) staff       (20)       86 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/var/toString.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1456 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/wrap.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.098201 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/
--rwxr-xr-x   0 gary       (501) staff       (20)      999 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/.bower.json
--rwxr-xr-x   0 gary       (501) staff       (20)      739 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/bower.json
--rwxr-xr-x   0 gary       (501) staff       (20)     1659 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/icheck.jquery.json
--rwxr-xr-x   0 gary       (501) staff       (20)    14136 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/icheck.js
--rwxr-xr-x   0 gary       (501) staff       (20)     4931 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/icheck.min.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.098751 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/
--rwxr-xr-x   0 gary       (501) staff       (20)     1568 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/all.css
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.114686 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/
--rwxr-xr-x   0 gary       (501) staff       (20)    12513 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/_all.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1302 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/aero.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1520 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/aero.png
--rwxr-xr-x   0 gary       (501) staff       (20)     3218 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/aero@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1302 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/blue.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1518 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/blue.png
--rwxr-xr-x   0 gary       (501) staff       (20)     3217 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/blue@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1243 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/flat.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1515 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/flat.png
--rwxr-xr-x   0 gary       (501) staff       (20)     3217 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/flat@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1317 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/green.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1444 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/green.png
--rwxr-xr-x   0 gary       (501) staff       (20)     3117 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/green@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1302 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/grey.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1516 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/grey.png
--rwxr-xr-x   0 gary       (501) staff       (20)     3217 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/grey@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1332 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/orange.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1518 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/orange.png
--rwxr-xr-x   0 gary       (501) staff       (20)     3275 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/orange@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1302 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/pink.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1522 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/pink.png
--rwxr-xr-x   0 gary       (501) staff       (20)     3218 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/pink@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1332 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/purple.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1519 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/purple.png
--rwxr-xr-x   0 gary       (501) staff       (20)     3218 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/purple@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1287 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/red.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1516 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/red.png
--rwxr-xr-x   0 gary       (501) staff       (20)     3276 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/red@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1332 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/yellow.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1516 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/yellow.png
--rwxr-xr-x   0 gary       (501) staff       (20)     3216 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/yellow@2x.png
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.116058 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/futurico/
--rwxr-xr-x   0 gary       (501) staff       (20)     1295 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/futurico/futurico.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1734 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/futurico/futurico.png
--rwxr-xr-x   0 gary       (501) staff       (20)     3446 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/futurico/futurico@2x.png
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.122236 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/
--rwxr-xr-x   0 gary       (501) staff       (20)    20429 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/_all.css
--rwxr-xr-x   0 gary       (501) staff       (20)     2096 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/aero.css
--rwxr-xr-x   0 gary       (501) staff       (20)     2096 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/blue.css
--rwxr-xr-x   0 gary       (501) staff       (20)     2118 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/green.css
--rwxr-xr-x   0 gary       (501) staff       (20)     2096 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/grey.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1977 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/line.css
--rwxr-xr-x   0 gary       (501) staff       (20)      588 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/line.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1073 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/line@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     2134 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/orange.css
--rwxr-xr-x   0 gary       (501) staff       (20)     2096 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/pink.css
--rwxr-xr-x   0 gary       (501) staff       (20)     2140 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/purple.css
--rwxr-xr-x   0 gary       (501) staff       (20)     2074 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/red.css
--rwxr-xr-x   0 gary       (501) staff       (20)     2140 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/yellow.css
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.138378 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/
--rwxr-xr-x   0 gary       (501) staff       (20)    14474 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/_all.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1500 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/aero.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1151 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/aero.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1409 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/aero@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1500 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/blue.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1132 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/blue.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1410 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/blue@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1517 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/green.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1143 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/green.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1408 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/green@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1500 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/grey.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1142 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/grey.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1407 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/grey@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1437 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/minimal.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1114 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/minimal.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1410 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/minimal@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1534 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/orange.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1139 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/orange.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1407 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/orange@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1500 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/pink.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1150 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/pink.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1409 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/pink@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1534 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/purple.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1132 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/purple.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1409 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/purple@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1483 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/red.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1130 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/red.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1410 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/red@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1534 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/yellow.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1135 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/yellow.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1406 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/yellow@2x.png
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.140171 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/polaris/
--rwxr-xr-x   0 gary       (501) staff       (20)     1431 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/polaris/polaris.css
--rwxr-xr-x   0 gary       (501) staff       (20)     6401 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/polaris/polaris.png
--rwxr-xr-x   0 gary       (501) staff       (20)    16760 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/polaris/polaris@2x.png
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.160019 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/
--rwxr-xr-x   0 gary       (501) staff       (20)    14331 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/_all.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1485 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/aero.css
--rwxr-xr-x   0 gary       (501) staff       (20)     2167 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/aero.png
--rwxr-xr-x   0 gary       (501) staff       (20)     4455 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/aero@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1485 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/blue.css
--rwxr-xr-x   0 gary       (501) staff       (20)     2185 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/blue.png
--rwxr-xr-x   0 gary       (501) staff       (20)     4485 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/blue@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1502 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/green.css
--rwxr-xr-x   0 gary       (501) staff       (20)     2193 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/green.png
--rwxr-xr-x   0 gary       (501) staff       (20)     4498 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/green@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1485 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/grey.css
--rwxr-xr-x   0 gary       (501) staff       (20)     2186 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/grey.png
--rwxr-xr-x   0 gary       (501) staff       (20)     4483 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/grey@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1519 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/orange.css
--rwxr-xr-x   0 gary       (501) staff       (20)     2181 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/orange.png
--rwxr-xr-x   0 gary       (501) staff       (20)     4474 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/orange@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1485 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/pink.css
--rwxr-xr-x   0 gary       (501) staff       (20)     2189 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/pink.png
--rwxr-xr-x   0 gary       (501) staff       (20)     4479 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/pink@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1519 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/purple.css
--rwxr-xr-x   0 gary       (501) staff       (20)     2188 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/purple.png
--rwxr-xr-x   0 gary       (501) staff       (20)     4501 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/purple@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1468 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/red.css
--rwxr-xr-x   0 gary       (501) staff       (20)     2190 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/red.png
--rwxr-xr-x   0 gary       (501) staff       (20)     4490 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/red@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1420 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/square.css
--rwxr-xr-x   0 gary       (501) staff       (20)     2175 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/square.png
--rwxr-xr-x   0 gary       (501) staff       (20)     4478 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/square@2x.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1519 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/yellow.css
--rwxr-xr-x   0 gary       (501) staff       (20)     2131 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/yellow.png
--rwxr-xr-x   0 gary       (501) staff       (20)     4385 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/yellow@2x.png
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.211020 vitriolic-3.3.9/touchtechnology/admin/static/js/
--rw-r--r--   0 gary       (501) staff       (20)    30121 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/URI.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.212919 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.218055 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/
--rwxr-xr-x   0 gary       (501) staff       (20)     1682 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/area.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1853 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/auto.js
--rwxr-xr-x   0 gary       (501) staff       (20)      857 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/donut.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1130 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/horizontal.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1747 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/line.js
--rwxr-xr-x   0 gary       (501) staff       (20)      798 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/pie.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1053 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/scatter.js
--rwxr-xr-x   0 gary       (501) staff       (20)     2128 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/stacked-area.js
--rwxr-xr-x   0 gary       (501) staff       (20)      998 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/stacked-horizontal.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1542 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/stacked-vertical.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1818 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/vertical.js
--rwxr-xr-x   0 gary       (501) staff       (20)     3612 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/form-plugins.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.218512 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/json/
--rwxr-xr-x   0 gary       (501) staff       (20)     1440 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/json/table_data_small.json
--rwxr-xr-x   0 gary       (501) staff       (20)      145 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/page-icons.js
--rwxr-xr-x   0 gary       (501) staff       (20)      217 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/pricing.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.218962 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/reports/
--rwxr-xr-x   0 gary       (501) staff       (20)     1569 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/reports/line.js
--rwxr-xr-x   0 gary       (501) staff       (20)      138 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/demos/validation.js
--rwxr-xr-x   0 gary       (501) staff       (20)      855 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/mvpready-account.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1513 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/mvpready-admin.js
--rwxr-xr-x   0 gary       (501) staff       (20)     3738 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/mvpready-core.js
--rwxr-xr-x   0 gary       (501) staff       (20)     4491 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/js/mvpready-helpers.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.249243 vitriolic-3.3.9/touchtechnology/admin/static/select2/
--rwxr-xr-x   0 gary       (501) staff       (20)      526 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/.bower.json
--rwxr-xr-x   0 gary       (501) staff       (20)        7 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/.gitignore
--rwxr-xr-x   0 gary       (501) staff       (20)      206 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/bower.json
--rwxr-xr-x   0 gary       (501) staff       (20)     1732 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/component.json
--rwxr-xr-x   0 gary       (501) staff       (20)      637 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/composer.json
--rwxr-xr-x   0 gary       (501) staff       (20)      678 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/package.json
--rwxr-xr-x   0 gary       (501) staff       (20)     1490 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/release.sh
--rwxr-xr-x   0 gary       (501) staff       (20)     3347 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2-bootstrap.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1849 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2-spinner.gif
--rwxr-xr-x   0 gary       (501) staff       (20)    19457 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2.css
--rwxr-xr-x   0 gary       (501) staff       (20)     1030 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2.jquery.json
--rwxr-xr-x   0 gary       (501) staff       (20)   148536 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2.js
--rwxr-xr-x   0 gary       (501) staff       (20)    66596 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2.min.js
--rwxr-xr-x   0 gary       (501) staff       (20)      613 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2.png
--rwxr-xr-x   0 gary       (501) staff       (20)     1389 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_ar.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1003 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_az.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1081 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_bg.js
--rwxr-xr-x   0 gary       (501) staff       (20)      952 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_ca.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1988 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_cs.js
--rwxr-xr-x   0 gary       (501) staff       (20)      853 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_da.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1014 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_de.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1128 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_el.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1102 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_en.js.template
--rwxr-xr-x   0 gary       (501) staff       (20)     1177 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_es.js
--rwxr-xr-x   0 gary       (501) staff       (20)      886 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_et.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1313 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_eu.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1207 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_fa.js
--rwxr-xr-x   0 gary       (501) staff       (20)      940 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_fi.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1077 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_fr.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1339 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_gl.js
--rwxr-xr-x   0 gary       (501) staff       (20)      885 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_he.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1002 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_hr.js
--rwxr-xr-x   0 gary       (501) staff       (20)      802 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_hu.js
--rwxr-xr-x   0 gary       (501) staff       (20)      891 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_id.js
--rwxr-xr-x   0 gary       (501) staff       (20)      855 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_is.js
--rwxr-xr-x   0 gary       (501) staff       (20)      866 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_it.js
--rwxr-xr-x   0 gary       (501) staff       (20)      812 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_ja.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1078 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_ka.js
--rwxr-xr-x   0 gary       (501) staff       (20)      871 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_ko.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1144 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_lt.js
--rwxr-xr-x   0 gary       (501) staff       (20)      999 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_lv.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1064 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_mk.js
--rwxr-xr-x   0 gary       (501) staff       (20)      836 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_ms.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1145 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_nb.js
--rwxr-xr-x   0 gary       (501) staff       (20)      846 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_nl.js
--rwxr-xr-x   0 gary       (501) staff       (20)     2015 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_pl.js
--rwxr-xr-x   0 gary       (501) staff       (20)      969 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_pt-BR.js
--rwxr-xr-x   0 gary       (501) staff       (20)      891 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_pt-PT.js
--rwxr-xr-x   0 gary       (501) staff       (20)      902 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_ro.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1058 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_rs.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1171 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_ru.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1948 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_sk.js
--rwxr-xr-x   0 gary       (501) staff       (20)      847 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_sv.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1063 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_th.js
--rwxr-xr-x   0 gary       (501) staff       (20)      831 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_tr.js
--rwxr-xr-x   0 gary       (501) staff       (20)      904 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_ug-CN.js
--rwxr-xr-x   0 gary       (501) staff       (20)     1415 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_uk.js
--rwxr-xr-x   0 gary       (501) staff       (20)      959 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_vi.js
--rwxr-xr-x   0 gary       (501) staff       (20)      762 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_zh-CN.js
--rwxr-xr-x   0 gary       (501) staff       (20)      774 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_zh-TW.js
--rwxr-xr-x   0 gary       (501) staff       (20)      845 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/select2/select2x2.png
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.251838 vitriolic-3.3.9/touchtechnology/admin/static/slimscroll/
--rwxr-xr-x   0 gary       (501) staff       (20)     1224 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/slimscroll/.bower.json
--rwxr-xr-x   0 gary       (501) staff       (20)      943 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/slimscroll/bower.json
--rwxr-xr-x   0 gary       (501) staff       (20)    13657 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/slimscroll/jquery.slimscroll.js
--rwxr-xr-x   0 gary       (501) staff       (20)     4679 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/slimscroll/jquery.slimscroll.min.js
--rwxr-xr-x   0 gary       (501) staff       (20)      937 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/slimscroll/slimScroll.jquery.json
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.916083 vitriolic-3.3.9/touchtechnology/admin/static/touchtechnology/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.916538 vitriolic-3.3.9/touchtechnology/admin/static/touchtechnology/admin/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.252303 vitriolic-3.3.9/touchtechnology/admin/static/touchtechnology/admin/img/
--rw-r--r--   0 gary       (501) staff       (20)     8479 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/touchtechnology/admin/img/touch-technology.png
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.253802 vitriolic-3.3.9/touchtechnology/admin/static/touchtechnology/admin/js/
--rw-r--r--   0 gary       (501) staff       (20)     1003 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/touchtechnology/admin/js/modal_delete.js
--rw-r--r--   0 gary       (501) staff       (20)      357 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/touchtechnology/admin/js/resize.js
--rw-r--r--   0 gary       (501) staff       (20)     2043 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/static/touchtechnology/admin/js/tabs.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.255133 vitriolic-3.3.9/touchtechnology/admin/templates/
--rw-r--r--   0 gary       (501) staff       (20)      382 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/templates/403.html
--rw-r--r--   0 gary       (501) staff       (20)      357 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/templates/404.html
--rw-r--r--   0 gary       (501) staff       (20)      800 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/templates/40x.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.917577 vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.260390 vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/
--rw-r--r--   0 gary       (501) staff       (20)       14 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/_version.html
--rw-r--r--   0 gary       (501) staff       (20)     7240 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/base.html
--rw-r--r--   0 gary       (501) staff       (20)     3967 2019-12-07 04:40:37.000000 vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/edit.html
--rw-r--r--   0 gary       (501) staff       (20)      420 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/edit.multiple.html
--rw-r--r--   0 gary       (501) staff       (20)      379 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/edit.related.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.260954 vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/group/
--rw-r--r--   0 gary       (501) staff       (20)     1203 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/group/list.inc.html
--rw-r--r--   0 gary       (501) staff       (20)      178 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/index.html
--rw-r--r--   0 gary       (501) staff       (20)      865 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/list.html
--rw-r--r--   0 gary       (501) staff       (20)     2438 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/permissions.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.261566 vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/settings/
--rw-r--r--   0 gary       (501) staff       (20)      311 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/settings/index.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.262299 vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/user/
--rw-r--r--   0 gary       (501) staff       (20)     1428 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/user/list.inc.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.263908 vitriolic-3.3.9/touchtechnology/admin/templatetags/
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/templatetags/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)     1977 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/templatetags/admin.py
--rw-r--r--   0 gary       (501) staff       (20)     5261 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/templatetags/mvp_tags.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.266315 vitriolic-3.3.9/touchtechnology/admin/tests/
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/tests/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)     3642 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/tests/test_auth_site.py
--rw-r--r--   0 gary       (501) staff       (20)      485 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/tests/test_authentication.py
--rw-r--r--   0 gary       (501) staff       (20)     1453 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/admin/tests/test_mptt_order.py
--rw-r--r--   0 gary       (501) staff       (20)     1576 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/admin/tests/test_mvp_tags.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.275966 vitriolic-3.3.9/touchtechnology/common/
--rw-r--r--   0 gary       (501) staff       (20)      181 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/__init__.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.277472 vitriolic-3.3.9/touchtechnology/common/backends/
--rw-r--r--   0 gary       (501) staff       (20)      157 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/backends/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)     1294 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/backends/auth.py
--rw-r--r--   0 gary       (501) staff       (20)     2861 2024-04-13 04:07:40.000000 vitriolic-3.3.9/touchtechnology/common/backends/cache.py
--rw-r--r--   0 gary       (501) staff       (20)      499 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/context_processors.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.278414 vitriolic-3.3.9/touchtechnology/common/db/
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/db/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)     7030 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/db/models.py
--rw-r--r--   0 gary       (501) staff       (20)     2020 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/debugging.py
--rw-r--r--   0 gary       (501) staff       (20)     1626 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/decorators.py
--rw-r--r--   0 gary       (501) staff       (20)      947 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/default_settings.py
--rw-r--r--   0 gary       (501) staff       (20)       82 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/exceptions.py
--rw-r--r--   0 gary       (501) staff       (20)      728 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/fields.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.282365 vitriolic-3.3.9/touchtechnology/common/forms/
--rw-r--r--   0 gary       (501) staff       (20)      640 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/forms/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)     7475 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/forms/auth.py
--rw-r--r--   0 gary       (501) staff       (20)     9664 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/forms/fields.py
--rw-r--r--   0 gary       (501) staff       (20)     1446 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/forms/iter.py
--rw-r--r--   0 gary       (501) staff       (20)     3763 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/forms/mixins.py
--rw-r--r--   0 gary       (501) staff       (20)     2401 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/forms/tz.py
--rw-r--r--   0 gary       (501) staff       (20)     8100 2024-04-13 04:07:44.000000 vitriolic-3.3.9/touchtechnology/common/forms/widgets.py
--rw-r--r--   0 gary       (501) staff       (20)     1468 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/forms_lazy.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.922233 vitriolic-3.3.9/touchtechnology/common/locale/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.920774 vitriolic-3.3.9/touchtechnology/common/locale/de/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.283332 vitriolic-3.3.9/touchtechnology/common/locale/de/LC_MESSAGES/
--rw-r--r--   0 gary       (501) staff       (20)      420 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/common/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 gary       (501) staff       (20)     9606 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/common/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.921510 vitriolic-3.3.9/touchtechnology/common/locale/en-AU/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.284356 vitriolic-3.3.9/touchtechnology/common/locale/en-AU/LC_MESSAGES/
--rw-r--r--   0 gary       (501) staff       (20)      378 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/common/locale/en-AU/LC_MESSAGES/django.mo
--rw-r--r--   0 gary       (501) staff       (20)     9560 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/common/locale/en-AU/LC_MESSAGES/django.po
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.921977 vitriolic-3.3.9/touchtechnology/common/locale/fr/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.285502 vitriolic-3.3.9/touchtechnology/common/locale/fr/LC_MESSAGES/
--rw-r--r--   0 gary       (501) staff       (20)     9033 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/common/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 gary       (501) staff       (20)    14080 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/common/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.922653 vitriolic-3.3.9/touchtechnology/common/locale/ja/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.286637 vitriolic-3.3.9/touchtechnology/common/locale/ja/LC_MESSAGES/
--rw-r--r--   0 gary       (501) staff       (20)      413 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/common/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 gary       (501) staff       (20)     9599 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/common/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0 gary       (501) staff       (20)     1898 2019-10-31 21:17:24.000000 vitriolic-3.3.9/touchtechnology/common/middleware.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.291048 vitriolic-3.3.9/touchtechnology/common/migrations/
--rw-r--r--   0 gary       (501) staff       (20)     5737 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/migrations/0001_initial.py
--rw-r--r--   0 gary       (501) staff       (20)      556 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/migrations/0002_sitemapnode_last_modified.py
--rw-r--r--   0 gary       (501) staff       (20)      485 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/migrations/0003_drop_pythonpackage.py
--rw-r--r--   0 gary       (501) staff       (20)      518 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/migrations/0004_sitemapnode_kwargs.py
--rw-r--r--   0 gary       (501) staff       (20)      742 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/migrations/0005_sitemapnode_populate_kwargs.py
--rw-r--r--   0 gary       (501) staff       (20)     2763 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/migrations/0006_model_definition_sync.py
--rw-r--r--   0 gary       (501) staff       (20)      896 2023-05-21 21:21:54.000000 vitriolic-3.3.9/touchtechnology/common/migrations/0007_auto_20220808_1144.py
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/migrations/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)     1826 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/mixins.py
--rw-r--r--   0 gary       (501) staff       (20)     7578 2022-08-10 12:47:18.000000 vitriolic-3.3.9/touchtechnology/common/models.py
--rw-r--r--   0 gary       (501) staff       (20)     1902 2022-07-03 21:48:02.000000 vitriolic-3.3.9/touchtechnology/common/prince.py
--rw-r--r--   0 gary       (501) staff       (20)     1157 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/routers.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.291556 vitriolic-3.3.9/touchtechnology/common/shim/
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/shim/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)     1472 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/sitemaps.py
--rw-r--r--   0 gary       (501) staff       (20)    39360 2024-04-14 00:51:21.000000 vitriolic-3.3.9/touchtechnology/common/sites.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.292116 vitriolic-3.3.9/touchtechnology/common/static/
--rw-r--r--   0 gary       (501) staff       (20)     3510 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/static/sitemap.xsl
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.924253 vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.924971 vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.292756 vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/css/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.299467 vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/css/froala_themes/
--rw-r--r--   0 gary       (501) staff       (20)    29097 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/css/froala_themes/dark.css
--rw-r--r--   0 gary       (501) staff       (20)    25448 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/css/froala_themes/dark.min.css
--rw-r--r--   0 gary       (501) staff       (20)    29096 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/css/froala_themes/gray.css
--rw-r--r--   0 gary       (501) staff       (20)    25546 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/css/froala_themes/gray.min.css
--rw-r--r--   0 gary       (501) staff       (20)    25675 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/css/froala_themes/red.css
--rw-r--r--   0 gary       (501) staff       (20)    22607 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/css/froala_themes/red.min.css
--rw-r--r--   0 gary       (501) staff       (20)    29287 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/css/froala_themes/royal.css
--rw-r--r--   0 gary       (501) staff       (20)    25735 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/css/froala_themes/royal.min.css
--rw-r--r--   0 gary       (501) staff       (20)       56 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/css/location_widget.css
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.300637 vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/js/
--rw-r--r--   0 gary       (501) staff       (20)      466 2024-03-27 20:05:17.000000 vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/js/froala.js
--rw-r--r--   0 gary       (501) staff       (20)     3139 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/js/location_widget.js
--rw-r--r--   0 gary       (501) staff       (20)     5244 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/storage.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.303698 vitriolic-3.3.9/touchtechnology/common/templates/
--rw-r--r--   0 gary       (501) staff       (20)      248 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/templates/404.html
--rw-r--r--   0 gary       (501) staff       (20)      345 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/templates/500.html
--rw-r--r--   0 gary       (501) staff       (20)     2924 2023-05-21 02:08:30.000000 vitriolic-3.3.9/touchtechnology/common/templates/base.html
--rw-r--r--   0 gary       (501) staff       (20)      284 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/templates/http4xx.html
--rw-r--r--   0 gary       (501) staff       (20)      157 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/templates/http5xx.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.305437 vitriolic-3.3.9/touchtechnology/common/templates/mvp/
--rw-r--r--   0 gary       (501) staff       (20)       23 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/templates/mvp/list.html
--rw-r--r--   0 gary       (501) staff       (20)     4959 2022-08-17 11:43:30.000000 vitriolic-3.3.9/touchtechnology/common/templates/mvp/list.inc.html
--rw-r--r--   0 gary       (501) staff       (20)      455 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/templates/mvp/list.split.inc.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.311544 vitriolic-3.3.9/touchtechnology/common/templates/registration/
--rw-r--r--   0 gary       (501) staff       (20)       94 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/templates/registration/base.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.312347 vitriolic-3.3.9/touchtechnology/common/templates/registration/email/
--rw-r--r--   0 gary       (501) staff       (20)      438 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/templates/registration/email/_base.html
--rw-r--r--   0 gary       (501) staff       (20)      403 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/templates/registration/logged_out.html
--rw-r--r--   0 gary       (501) staff       (20)     1338 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/templates/registration/login.html
--rw-r--r--   0 gary       (501) staff       (20)      572 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/templates/registration/password_change_done.html
--rw-r--r--   0 gary       (501) staff       (20)      863 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/templates/registration/password_change_form.html
--rw-r--r--   0 gary       (501) staff       (20)      434 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/templates/registration/password_reset_complete.html
--rw-r--r--   0 gary       (501) staff       (20)      836 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/templates/registration/password_reset_confirm.html
--rw-r--r--   0 gary       (501) staff       (20)      331 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/templates/registration/password_reset_done.html
--rw-r--r--   0 gary       (501) staff       (20)      596 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/templates/registration/password_reset_email.html
--rw-r--r--   0 gary       (501) staff       (20)      587 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/templates/registration/password_reset_form.html
--rw-r--r--   0 gary       (501) staff       (20)     1285 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/templates/registration/profile.html
--rw-r--r--   0 gary       (501) staff       (20)      562 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/templates/sitemap.xml
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.927811 vitriolic-3.3.9/touchtechnology/common/templates/touchtechnology/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.313309 vitriolic-3.3.9/touchtechnology/common/templates/touchtechnology/common/
--rw-r--r--   0 gary       (501) staff       (20)      250 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/templates/touchtechnology/common/index.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.317594 vitriolic-3.3.9/touchtechnology/common/templates/touchtechnology/common/templatetags/
--rw-r--r--   0 gary       (501) staff       (20)      877 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/templates/touchtechnology/common/templatetags/analytics.html
--rw-r--r--   0 gary       (501) staff       (20)      108 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/templates/touchtechnology/common/templatetags/context.html
--rw-r--r--   0 gary       (501) staff       (20)      593 2021-09-19 12:54:55.000000 vitriolic-3.3.9/touchtechnology/common/templates/touchtechnology/common/templatetags/field.html
--rw-r--r--   0 gary       (501) staff       (20)      162 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/templates/touchtechnology/common/templatetags/hostname.html
--rw-r--r--   0 gary       (501) staff       (20)     1217 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/templates/touchtechnology/common/templatetags/navigation.html
--rw-r--r--   0 gary       (501) staff       (20)      705 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/templates/touchtechnology/common/templatetags/pagination.html
--rw-r--r--   0 gary       (501) staff       (20)      124 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/templates/touchtechnology/common/templatetags/price.html
--rw-r--r--   0 gary       (501) staff       (20)      771 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/templates/touchtechnology/common/templatetags/version.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.318151 vitriolic-3.3.9/touchtechnology/common/templates/touchtechnology/twitter/
--rw-r--r--   0 gary       (501) staff       (20)      484 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/templates/touchtechnology/twitter/latest_tweets.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.319764 vitriolic-3.3.9/touchtechnology/common/templatetags/
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/templatetags/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)    16163 2024-04-14 00:51:21.000000 vitriolic-3.3.9/touchtechnology/common/templatetags/common.py
--rw-r--r--   0 gary       (501) staff       (20)      304 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/templatetags/dashboard.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.327318 vitriolic-3.3.9/touchtechnology/common/tests/
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/tests/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)      839 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/tests/factories.py
--rw-r--r--   0 gary       (501) staff       (20)      247 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/tests/test_appcache.py
--rw-r--r--   0 gary       (501) staff       (20)     5856 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/tests/test_authentication.py
--rw-r--r--   0 gary       (501) staff       (20)     2796 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/tests/test_fields.py
--rw-r--r--   0 gary       (501) staff       (20)     6609 2023-05-21 21:14:55.000000 vitriolic-3.3.9/touchtechnology/common/tests/test_forms.py
--rw-r--r--   0 gary       (501) staff       (20)     7871 2019-11-18 20:58:58.000000 vitriolic-3.3.9/touchtechnology/common/tests/test_generic_views.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.328916 vitriolic-3.3.9/touchtechnology/common/tests/test_html/
--rw-r--r--   0 gary       (501) staff       (20)     5553 2023-05-21 21:14:55.000000 vitriolic-3.3.9/touchtechnology/common/tests/test_html/select_date_time_field_initial.html
--rw-r--r--   0 gary       (501) staff       (20)    45496 2023-05-21 21:14:55.000000 vitriolic-3.3.9/touchtechnology/common/tests/test_html/select_date_time_field_initial_tz.html
--rw-r--r--   0 gary       (501) staff       (20)      355 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/tests/test_models.py
--rw-r--r--   0 gary       (501) staff       (20)      991 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/tests/test_pagination.py
--rw-r--r--   0 gary       (501) staff       (20)      135 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/tests/test_sitemaps.py
--rw-r--r--   0 gary       (501) staff       (20)     2624 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/tests/test_storage.py
--rw-r--r--   0 gary       (501) staff       (20)     7771 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/tests/test_templates.py
--rw-r--r--   0 gary       (501) staff       (20)     3132 2023-05-21 21:14:55.000000 vitriolic-3.3.9/touchtechnology/common/tests/test_timezone.py
--rw-r--r--   0 gary       (501) staff       (20)      600 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/common/tests/test_timezone_forms.py
--rw-r--r--   0 gary       (501) staff       (20)     3053 2023-05-21 21:14:55.000000 vitriolic-3.3.9/touchtechnology/common/tests/test_utils.py
--rw-r--r--   0 gary       (501) staff       (20)      280 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/urls.py
--rw-r--r--   0 gary       (501) staff       (20)     8156 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/utils.py
--rw-r--r--   0 gary       (501) staff       (20)     1424 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/common/views.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.336527 vitriolic-3.3.9/touchtechnology/content/
--rw-r--r--   0 gary       (501) staff       (20)       66 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)    22525 2023-02-16 20:24:29.000000 vitriolic-3.3.9/touchtechnology/content/admin.py
--rw-r--r--   0 gary       (501) staff       (20)     1058 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/app_settings.py
--rw-r--r--   0 gary       (501) staff       (20)      563 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/content/apps.py
--rw-r--r--   0 gary       (501) staff       (20)     9447 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/content/forms.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.930757 vitriolic-3.3.9/touchtechnology/content/locale/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.929585 vitriolic-3.3.9/touchtechnology/content/locale/de/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.337550 vitriolic-3.3.9/touchtechnology/content/locale/de/LC_MESSAGES/
--rw-r--r--   0 gary       (501) staff       (20)      420 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/content/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 gary       (501) staff       (20)     8711 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/content/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.930047 vitriolic-3.3.9/touchtechnology/content/locale/en-AU/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.338632 vitriolic-3.3.9/touchtechnology/content/locale/en-AU/LC_MESSAGES/
--rw-r--r--   0 gary       (501) staff       (20)      378 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/content/locale/en-AU/LC_MESSAGES/django.mo
--rw-r--r--   0 gary       (501) staff       (20)     8665 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/content/locale/en-AU/LC_MESSAGES/django.po
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.930502 vitriolic-3.3.9/touchtechnology/content/locale/fr/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.339663 vitriolic-3.3.9/touchtechnology/content/locale/fr/LC_MESSAGES/
--rw-r--r--   0 gary       (501) staff       (20)      419 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/content/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 gary       (501) staff       (20)     8710 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/content/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.930944 vitriolic-3.3.9/touchtechnology/content/locale/ja/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.340753 vitriolic-3.3.9/touchtechnology/content/locale/ja/LC_MESSAGES/
--rw-r--r--   0 gary       (501) staff       (20)      413 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/content/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 gary       (501) staff       (20)     8704 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/content/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0 gary       (501) staff       (20)    10324 2022-07-02 05:36:58.000000 vitriolic-3.3.9/touchtechnology/content/middleware.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.343956 vitriolic-3.3.9/touchtechnology/content/migrations/
--rw-r--r--   0 gary       (501) staff       (20)     9038 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/content/migrations/0001_initial.py
--rw-r--r--   0 gary       (501) staff       (20)      803 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/migrations/0002_last_modified.py
--rw-r--r--   0 gary       (501) staff       (20)      597 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/migrations/0003_auto_20160831_0608.py
--rw-r--r--   0 gary       (501) staff       (20)      692 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/migrations/0004_remove_placeholderkeywordargument.py
--rw-r--r--   0 gary       (501) staff       (20)     1104 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/migrations/0005_model_definition_sync.py
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/migrations/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)     6999 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/content/models.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.931964 vitriolic-3.3.9/touchtechnology/content/static/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.933033 vitriolic-3.3.9/touchtechnology/content/static/touchtechnology/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.932767 vitriolic-3.3.9/touchtechnology/content/static/touchtechnology/admin/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.344346 vitriolic-3.3.9/touchtechnology/content/static/touchtechnology/admin/css/
--rw-r--r--   0 gary       (501) staff       (20)      195 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/static/touchtechnology/admin/css/content.css
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.344862 vitriolic-3.3.9/touchtechnology/content/static/touchtechnology/admin/js/
--rw-r--r--   0 gary       (501) staff       (20)     1535 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/static/touchtechnology/admin/js/files.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.933219 vitriolic-3.3.9/touchtechnology/content/static/touchtechnology/content/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.345511 vitriolic-3.3.9/touchtechnology/content/static/touchtechnology/content/css/
--rw-r--r--   0 gary       (501) staff       (20)       33 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/static/touchtechnology/content/css/vi_admin.css
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.933703 vitriolic-3.3.9/touchtechnology/content/templates/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.933894 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.347954 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.352213 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/
--rw-r--r--   0 gary       (501) staff       (20)      601 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/base.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.352677 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/chunk/
--rw-r--r--   0 gary       (501) staff       (20)       88 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/chunk/edit.html
--rw-r--r--   0 gary       (501) staff       (20)       58 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/delete.html
--rw-r--r--   0 gary       (501) staff       (20)     1277 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/delete_confirm.html
--rw-r--r--   0 gary       (501) staff       (20)      150 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/edit.html
--rw-r--r--   0 gary       (501) staff       (20)      158 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/edit.related.html
--rw-r--r--   0 gary       (501) staff       (20)     1594 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/edit_application.html
--rw-r--r--   0 gary       (501) staff       (20)      128 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/edit_folder.html
--rw-r--r--   0 gary       (501) staff       (20)     1237 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/edit_page.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.354156 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/file/
--rw-r--r--   0 gary       (501) staff       (20)      203 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/file/delete_confirm.html
--rw-r--r--   0 gary       (501) staff       (20)      709 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/file/list.html
--rw-r--r--   0 gary       (501) staff       (20)     4886 2021-10-25 00:59:28.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/file/list.inc.html
--rw-r--r--   0 gary       (501) staff       (20)     2829 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/files.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.354690 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/folder/
--rw-r--r--   0 gary       (501) staff       (20)      145 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/folder/delete_confirm.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.355169 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/placeholder/
--rw-r--r--   0 gary       (501) staff       (20)     1080 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/placeholder/list.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.356095 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/redirect/
--rw-r--r--   0 gary       (501) staff       (20)       88 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/redirect/edit.html
--rw-r--r--   0 gary       (501) staff       (20)      597 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/redirect/list.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.357097 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/sitemapnode/
--rw-r--r--   0 gary       (501) staff       (20)     1080 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/sitemapnode/list.html
--rw-r--r--   0 gary       (501) staff       (20)     1801 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/sitemapnode/list.inc.html
--rw-r--r--   0 gary       (501) staff       (20)      151 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/base.html
--rw-r--r--   0 gary       (501) staff       (20)      253 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/folder.html
--rw-r--r--   0 gary       (501) staff       (20)      401 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/folder.nav.html
--rw-r--r--   0 gary       (501) staff       (20)      288 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/page.html
--rw-r--r--   0 gary       (501) staff       (20)      479 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/page_content.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.357915 vitriolic-3.3.9/touchtechnology/content/templatetags/
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/templatetags/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)      407 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/content/templatetags/content.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.359182 vitriolic-3.3.9/touchtechnology/content/tests/
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/tests/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)      292 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/content/tests/factories.py
--rw-r--r--   0 gary       (501) staff       (20)     3787 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/content/tests/test_admin.py
--rw-r--r--   0 gary       (501) staff       (20)     2818 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/content/utils.py
--rw-r--r--   0 gary       (501) staff       (20)     2243 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/content/views.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.364406 vitriolic-3.3.9/touchtechnology/news/
--rw-r--r--   0 gary       (501) staff       (20)       91 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)     6281 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/admin.py
--rw-r--r--   0 gary       (501) staff       (20)      928 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/app_settings.py
--rw-r--r--   0 gary       (501) staff       (20)      283 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/apps.py
--rw-r--r--   0 gary       (501) staff       (20)     2561 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/decorators.py
--rw-r--r--   0 gary       (501) staff       (20)     1631 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/forms.py
--rw-r--r--   0 gary       (501) staff       (20)      257 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/news/image_processors.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.938733 vitriolic-3.3.9/touchtechnology/news/locale/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.937406 vitriolic-3.3.9/touchtechnology/news/locale/de/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.365426 vitriolic-3.3.9/touchtechnology/news/locale/de/LC_MESSAGES/
--rw-r--r--   0 gary       (501) staff       (20)      420 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/news/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 gary       (501) staff       (20)     4168 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/news/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.937858 vitriolic-3.3.9/touchtechnology/news/locale/en-AU/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.366484 vitriolic-3.3.9/touchtechnology/news/locale/en-AU/LC_MESSAGES/
--rw-r--r--   0 gary       (501) staff       (20)      378 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/news/locale/en-AU/LC_MESSAGES/django.mo
--rw-r--r--   0 gary       (501) staff       (20)     4122 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/news/locale/en-AU/LC_MESSAGES/django.po
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.938395 vitriolic-3.3.9/touchtechnology/news/locale/fr/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.367563 vitriolic-3.3.9/touchtechnology/news/locale/fr/LC_MESSAGES/
--rw-r--r--   0 gary       (501) staff       (20)      419 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/news/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 gary       (501) staff       (20)     4167 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/news/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.938922 vitriolic-3.3.9/touchtechnology/news/locale/ja/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.368606 vitriolic-3.3.9/touchtechnology/news/locale/ja/LC_MESSAGES/
--rw-r--r--   0 gary       (501) staff       (20)      378 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/news/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 gary       (501) staff       (20)     4122 2019-11-09 20:04:29.000000 vitriolic-3.3.9/touchtechnology/news/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.373420 vitriolic-3.3.9/touchtechnology/news/migrations/
--rw-r--r--   0 gary       (501) staff       (20)     5408 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/migrations/0001_initial.py
--rw-r--r--   0 gary       (501) staff       (20)      627 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/migrations/0002_article_last_modified.py
--rw-r--r--   0 gary       (501) staff       (20)      642 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/migrations/0003_category_last_modified.py
--rw-r--r--   0 gary       (501) staff       (20)     2365 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/migrations/0004_model_definition_sync.py
--rw-r--r--   0 gary       (501) staff       (20)      428 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/migrations/0005_auto_20191122_1340.py
--rw-r--r--   0 gary       (501) staff       (20)      438 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/migrations/0006_article_copy_field.py
--rw-r--r--   0 gary       (501) staff       (20)      679 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/migrations/0007_article_copy_field_data.py
--rw-r--r--   0 gary       (501) staff       (20)      234 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/migrations/0008_delete_articlecontent.py
--rw-r--r--   0 gary       (501) staff       (20)     1569 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/migrations/0009_translation.py
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/news/migrations/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)     5369 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/models.py
--rw-r--r--   0 gary       (501) staff       (20)      367 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/news/query.py
--rw-r--r--   0 gary       (501) staff       (20)     6316 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/sites.py
--rw-r--r--   0 gary       (501) staff       (20)     1723 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/syndication.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.939627 vitriolic-3.3.9/touchtechnology/news/templates/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.939808 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.375644 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/
--rw-r--r--   0 gary       (501) staff       (20)      977 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/_latest_articles.html
--rw-r--r--   0 gary       (501) staff       (20)      959 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/_related_list.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.940765 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/admin/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.376105 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/admin/article/
--rw-r--r--   0 gary       (501) staff       (20)     1048 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/admin/article/list.inc.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.376566 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/admin/category/
--rw-r--r--   0 gary       (501) staff       (20)      464 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/admin/category/list.inc.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.377063 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/admin/translation/
--rw-r--r--   0 gary       (501) staff       (20)      891 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/admin/translation/list.inc.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.380062 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/archive/
--rw-r--r--   0 gary       (501) staff       (20)      410 2019-12-16 12:53:13.000000 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/archive/_article_list.html
--rw-r--r--   0 gary       (501) staff       (20)      241 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/archive/base.html
--rw-r--r--   0 gary       (501) staff       (20)      276 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/archive/day.html
--rw-r--r--   0 gary       (501) staff       (20)      572 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/archive/index.html
--rw-r--r--   0 gary       (501) staff       (20)      274 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/archive/month.html
--rw-r--r--   0 gary       (501) staff       (20)      425 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/archive/year.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.380981 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/article/
--rw-r--r--   0 gary       (501) staff       (20)     1741 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/article/detail.html
--rw-r--r--   0 gary       (501) staff       (20)     1170 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/article/list.html
--rw-r--r--   0 gary       (501) staff       (20)      205 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/base.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.381961 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/feeds/
--rw-r--r--   0 gary       (501) staff       (20)       24 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/feeds/description.html
--rw-r--r--   0 gary       (501) staff       (20)       24 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/feeds/title.html
--rw-r--r--   0 gary       (501) staff       (20)      607 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/feeds.html
--rw-r--r--   0 gary       (501) staff       (20)      264 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/index.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.382414 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/translation/
--rw-r--r--   0 gary       (501) staff       (20)      360 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/translation/detail.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.383224 vitriolic-3.3.9/touchtechnology/news/templatetags/
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/news/templatetags/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)     1864 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/templatetags/news.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.384973 vitriolic-3.3.9/touchtechnology/news/tests/
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/touchtechnology/news/tests/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)      982 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/tests/factories.py
--rw-r--r--   0 gary       (501) staff       (20)     2557 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/tests/test_admin.py
--rw-r--r--   0 gary       (501) staff       (20)     3442 2022-06-12 11:19:40.000000 vitriolic-3.3.9/touchtechnology/news/tests/test_site.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.385426 vitriolic-3.3.9/tournamentcontrol/
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/__init__.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.397384 vitriolic-3.3.9/tournamentcontrol/competition/
--rw-r--r--   0 gary       (501) staff       (20)      366 2019-11-19 06:59:00.000000 vitriolic-3.3.9/tournamentcontrol/competition/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)    82709 2024-05-08 12:45:02.000000 vitriolic-3.3.9/tournamentcontrol/competition/admin.py
--rw-r--r--   0 gary       (501) staff       (20)     2796 2023-02-16 20:24:29.000000 vitriolic-3.3.9/tournamentcontrol/competition/apps.py
--rw-r--r--   0 gary       (501) staff       (20)     4268 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/calc.py
--rw-r--r--   0 gary       (501) staff       (20)     1361 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/constants.py
--rw-r--r--   0 gary       (501) staff       (20)    10746 2023-07-23 01:57:06.000000 vitriolic-3.3.9/tournamentcontrol/competition/dashboard.py
--rw-r--r--   0 gary       (501) staff       (20)    12977 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/decorators.py
--rw-r--r--   0 gary       (501) staff       (20)    18623 2023-02-16 20:24:29.000000 vitriolic-3.3.9/tournamentcontrol/competition/draw.py
--rw-r--r--   0 gary       (501) staff       (20)      269 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/fields.py
--rw-r--r--   0 gary       (501) staff       (20)    71011 2024-05-08 12:46:22.000000 vitriolic-3.3.9/tournamentcontrol/competition/forms.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.944855 vitriolic-3.3.9/tournamentcontrol/competition/locale/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.943666 vitriolic-3.3.9/tournamentcontrol/competition/locale/de/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.398359 vitriolic-3.3.9/tournamentcontrol/competition/locale/de/LC_MESSAGES/
--rw-r--r--   0 gary       (501) staff       (20)      421 2019-11-09 20:04:29.000000 vitriolic-3.3.9/tournamentcontrol/competition/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 gary       (501) staff       (20)    63237 2019-11-09 20:04:29.000000 vitriolic-3.3.9/tournamentcontrol/competition/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.944131 vitriolic-3.3.9/tournamentcontrol/competition/locale/en-AU/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.399406 vitriolic-3.3.9/tournamentcontrol/competition/locale/en-AU/LC_MESSAGES/
--rw-r--r--   0 gary       (501) staff       (20)      429 2019-11-09 20:04:29.000000 vitriolic-3.3.9/tournamentcontrol/competition/locale/en-AU/LC_MESSAGES/django.mo
--rw-r--r--   0 gary       (501) staff       (20)    63245 2019-11-09 20:04:29.000000 vitriolic-3.3.9/tournamentcontrol/competition/locale/en-AU/LC_MESSAGES/django.po
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.944590 vitriolic-3.3.9/tournamentcontrol/competition/locale/fr/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.400519 vitriolic-3.3.9/tournamentcontrol/competition/locale/fr/LC_MESSAGES/
--rw-r--r--   0 gary       (501) staff       (20)      420 2019-11-09 20:04:29.000000 vitriolic-3.3.9/tournamentcontrol/competition/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 gary       (501) staff       (20)    63236 2019-11-09 20:04:29.000000 vitriolic-3.3.9/tournamentcontrol/competition/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.945047 vitriolic-3.3.9/tournamentcontrol/competition/locale/ja/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.401832 vitriolic-3.3.9/tournamentcontrol/competition/locale/ja/LC_MESSAGES/
--rw-r--r--   0 gary       (501) staff       (20)      414 2019-11-09 20:04:29.000000 vitriolic-3.3.9/tournamentcontrol/competition/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 gary       (501) staff       (20)    63230 2019-11-09 20:04:29.000000 vitriolic-3.3.9/tournamentcontrol/competition/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.402509 vitriolic-3.3.9/tournamentcontrol/competition/management/
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/management/__init__.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.403494 vitriolic-3.3.9/tournamentcontrol/competition/management/commands/
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/management/commands/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)     1899 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/management/commands/produce_rank.py
--rw-r--r--   0 gary       (501) staff       (20)      467 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/managers.py
--rw-r--r--   0 gary       (501) staff       (20)     4705 2023-07-16 02:28:16.000000 vitriolic-3.3.9/tournamentcontrol/competition/merge.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.428391 vitriolic-3.3.9/tournamentcontrol/competition/migrations/
--rw-r--r--   0 gary       (501) staff       (20)    52844 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0001_initial.py
--rw-r--r--   0 gary       (501) staff       (20)      530 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0002_division_draft.py
--rw-r--r--   0 gary       (501) staff       (20)      447 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0003_division_draft_data.py
--rw-r--r--   0 gary       (501) staff       (20)      508 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0004_alter_person_gender.py
--rw-r--r--   0 gary       (501) staff       (20)     1005 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0005_alter_club_facebook_youtube_position.py
--rw-r--r--   0 gary       (501) staff       (20)      792 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0006_sportingpulse_import_fields.py
--rw-r--r--   0 gary       (501) staff       (20)     1626 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0007_match_videos.py
--rw-r--r--   0 gary       (501) staff       (20)     1510 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0008_nullable_statistics.py
--rw-r--r--   0 gary       (501) staff       (20)      317 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0009_remove_byeteam.py
--rw-r--r--   0 gary       (501) staff       (20)      697 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0010_remove_match_video_approved_by.py
--rw-r--r--   0 gary       (501) staff       (20)      997 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0011_custom_twitter_ladderpoints_fields.py
--rw-r--r--   0 gary       (501) staff       (20)     1455 2022-07-18 07:51:12.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0012_hashtag_include_symbol.py
--rw-r--r--   0 gary       (501) staff       (20)      611 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0013_statistic_played_field.py
--rw-r--r--   0 gary       (501) staff       (20)      580 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0014_match_play_at_blank.py
--rw-r--r--   0 gary       (501) staff       (20)      693 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0015_person_user_relation.py
--rw-r--r--   0 gary       (501) staff       (20)      653 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0016_season_forfeit_notifications.py
--rw-r--r--   0 gary       (501) staff       (20)     5746 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0017_ranking_feature.py
--rw-r--r--   0 gary       (501) staff       (20)    10513 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0018_resync_field_and_model_defs.py
--rw-r--r--   0 gary       (501) staff       (20)      532 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0019_auto_20161210_0922.py
--rw-r--r--   0 gary       (501) staff       (20)     3954 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0020_competition__add__person_uuid.py
--rw-r--r--   0 gary       (501) staff       (20)     1146 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0021_competition__data__person_uuid.py
--rw-r--r--   0 gary       (501) staff       (20)     4676 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0022_competition__remove__person_id.py
--rw-r--r--   0 gary       (501) staff       (20)      533 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0023_competition__add__match_uuid.py
--rw-r--r--   0 gary       (501) staff       (20)      679 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0023_competition__add__match_uuid_data.py
--rw-r--r--   0 gary       (501) staff       (20)     1017 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0023_competition__add__match_uuid_finalize.py
--rw-r--r--   0 gary       (501) staff       (20)      686 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0024_auto_20170203_0619.py
--rw-r--r--   0 gary       (501) staff       (20)      985 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0025_matchvideo_baseline.py
--rw-r--r--   0 gary       (501) staff       (20)      863 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0026_matchvideo.py
--rw-r--r--   0 gary       (501) staff       (20)      644 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0027_matchvideo_data.py
--rw-r--r--   0 gary       (501) staff       (20)      471 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0028_drop_matchvideo.py
--rw-r--r--   0 gary       (501) staff       (20)     1748 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0029_seasonreferee.py
--rw-r--r--   0 gary       (501) staff       (20)      848 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0030_match_referees.py
--rw-r--r--   0 gary       (501) staff       (20)    20487 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0031_model_definition_sync.py
--rw-r--r--   0 gary       (501) staff       (20)      957 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0032_resave_all_matches.py
--rw-r--r--   0 gary       (501) staff       (20)     1326 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0033_matchscoresheet.py
--rw-r--r--   0 gary       (501) staff       (20)     1529 2019-10-31 21:17:24.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0034_orderedsitemapnode_add_copy_field.py
--rw-r--r--   0 gary       (501) staff       (20)      899 2019-11-14 06:38:25.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0035_season_disable_calendar.py
--rw-r--r--   0 gary       (501) staff       (20)     5155 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0036_auto_20191122_1340.py
--rw-r--r--   0 gary       (501) staff       (20)      392 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0037_alter_match_evaluated.py
--rw-r--r--   0 gary       (501) staff       (20)      457 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0038_match_live_stream.py
--rw-r--r--   0 gary       (501) staff       (20)      454 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0039_season_live_stream.py
--rw-r--r--   0 gary       (501) staff       (20)      645 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0040_season_live_stream_privacy.py
--rw-r--r--   0 gary       (501) staff       (20)      463 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0041_ground_live_stream.py
--rw-r--r--   0 gary       (501) staff       (20)      482 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0042_ground_external_identifier.py
--rw-r--r--   0 gary       (501) staff       (20)      492 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0043_alter_ground_external_identifier.py
--rw-r--r--   0 gary       (501) staff       (20)      492 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0044_match_live_stream_bind.py
--rw-r--r--   0 gary       (501) staff       (20)      477 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0045_ground_stream_key.py
--rw-r--r--   0 gary       (501) staff       (20)      436 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0046_alter_match_live_stream_bind.py
--rw-r--r--   0 gary       (501) staff       (20)     1648 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0047_season_live_stream_oauth2.py
--rw-r--r--   0 gary       (501) staff       (20)      405 2023-07-16 04:15:02.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0048_season_live_stream_thumbnail.py
--rw-r--r--   0 gary       (501) staff       (20)      419 2023-07-16 04:15:02.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/0049_match_live_stream_thumbnail.py
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/migrations/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)     1517 2019-10-31 21:17:24.000000 vitriolic-3.3.9/tournamentcontrol/competition/mixins.py
--rw-r--r--   0 gary       (501) staff       (20)    71869 2024-05-08 12:45:02.000000 vitriolic-3.3.9/tournamentcontrol/competition/models.py
--rw-r--r--   0 gary       (501) staff       (20)     5029 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/query.py
--rw-r--r--   0 gary       (501) staff       (20)    12590 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/rank.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.429093 vitriolic-3.3.9/tournamentcontrol/competition/rest/
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-31 21:17:24.000000 vitriolic-3.3.9/tournamentcontrol/competition/rest/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)      267 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/rest/urls.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.434499 vitriolic-3.3.9/tournamentcontrol/competition/rest/v1/
--rw-r--r--   0 gary       (501) staff       (20)     1475 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/rest/v1/_247.py
--rw-r--r--   0 gary       (501) staff       (20)       65 2019-10-31 21:17:24.000000 vitriolic-3.3.9/tournamentcontrol/competition/rest/v1/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)     3540 2022-07-17 22:00:23.000000 vitriolic-3.3.9/tournamentcontrol/competition/rest/v1/_birdi.py
--rw-r--r--   0 gary       (501) staff       (20)     1203 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/rest/v1/_routers.py
--rw-r--r--   0 gary       (501) staff       (20)      726 2019-10-31 21:17:24.000000 vitriolic-3.3.9/tournamentcontrol/competition/rest/v1/club.py
--rw-r--r--   0 gary       (501) staff       (20)     1116 2019-10-31 21:17:24.000000 vitriolic-3.3.9/tournamentcontrol/competition/rest/v1/competition.py
--rw-r--r--   0 gary       (501) staff       (20)     3309 2022-07-18 07:51:12.000000 vitriolic-3.3.9/tournamentcontrol/competition/rest/v1/division.py
--rw-r--r--   0 gary       (501) staff       (20)     2112 2019-10-31 21:17:24.000000 vitriolic-3.3.9/tournamentcontrol/competition/rest/v1/season.py
--rw-r--r--   0 gary       (501) staff       (20)      817 2019-10-31 21:17:24.000000 vitriolic-3.3.9/tournamentcontrol/competition/rest/v1/stage.py
--rw-r--r--   0 gary       (501) staff       (20)      244 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/rest/v1/urls.py
--rw-r--r--   0 gary       (501) staff       (20)      501 2019-10-31 21:17:24.000000 vitriolic-3.3.9/tournamentcontrol/competition/rest/v1/viewsets.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.438549 vitriolic-3.3.9/tournamentcontrol/competition/signals/
--rw-r--r--   0 gary       (501) staff       (20)     1100 2023-02-16 20:24:29.000000 vitriolic-3.3.9/tournamentcontrol/competition/signals/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)       86 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/signals/custom.py
--rw-r--r--   0 gary       (501) staff       (20)      580 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/signals/decorators.py
--rw-r--r--   0 gary       (501) staff       (20)     6972 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/signals/ladders.py
--rw-r--r--   0 gary       (501) staff       (20)     5204 2023-02-16 20:24:29.000000 vitriolic-3.3.9/tournamentcontrol/competition/signals/matches.py
--rw-r--r--   0 gary       (501) staff       (20)      505 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/signals/places.py
--rw-r--r--   0 gary       (501) staff       (20)      451 2022-07-25 12:16:49.000000 vitriolic-3.3.9/tournamentcontrol/competition/signals/teams.py
--rw-r--r--   0 gary       (501) staff       (20)    43575 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/sites.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.948920 vitriolic-3.3.9/tournamentcontrol/competition/static/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.947701 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.445135 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/css/
--rw-r--r--   0 gary       (501) staff       (20)     4823 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.bootstrap.css
--rw-r--r--   0 gary       (501) staff       (20)     4216 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.bootstrap.min.css
--rw-r--r--   0 gary       (501) staff       (20)     2924 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.foundation.css
--rw-r--r--   0 gary       (501) staff       (20)     2580 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.foundation.min.css
--rw-r--r--   0 gary       (501) staff       (20)    16019 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.jqueryui.css
--rw-r--r--   0 gary       (501) staff       (20)    14069 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.jqueryui.min.css
--rw-r--r--   0 gary       (501) staff       (20)    15423 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/css/jquery.dataTables.css
--rw-r--r--   0 gary       (501) staff       (20)    13587 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/css/jquery.dataTables.min.css
--rw-r--r--   0 gary       (501) staff       (20)    14229 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/css/jquery.dataTables_themeroller.css
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.447980 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/images/
--rw-r--r--   0 gary       (501) staff       (20)      160 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/images/sort_asc.png
--rw-r--r--   0 gary       (501) staff       (20)      148 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/images/sort_asc_disabled.png
--rw-r--r--   0 gary       (501) staff       (20)      201 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/images/sort_both.png
--rw-r--r--   0 gary       (501) staff       (20)      158 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/images/sort_desc.png
--rw-r--r--   0 gary       (501) staff       (20)      146 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/images/sort_desc_disabled.png
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.452749 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/js/
--rw-r--r--   0 gary       (501) staff       (20)     4544 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.bootstrap.js
--rw-r--r--   0 gary       (501) staff       (20)     1960 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.bootstrap.min.js
--rw-r--r--   0 gary       (501) staff       (20)     4331 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.foundation.js
--rw-r--r--   0 gary       (501) staff       (20)     2090 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.foundation.min.js
--rw-r--r--   0 gary       (501) staff       (20)     4486 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.jqueryui.js
--rw-r--r--   0 gary       (501) staff       (20)     2647 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.jqueryui.min.js
--rw-r--r--   0 gary       (501) staff       (20)   447282 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/js/jquery.dataTables.js
--rw-r--r--   0 gary       (501) staff       (20)    82638 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/js/jquery.dataTables.min.js
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.948220 vitriolic-3.3.9/tournamentcontrol/competition/static/bootstrap/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.948531 vitriolic-3.3.9/tournamentcontrol/competition/static/bootstrap/dist/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.455695 vitriolic-3.3.9/tournamentcontrol/competition/static/bootstrap/dist/fonts/
--rw-r--r--   0 gary       (501) staff       (20)    20127 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/bootstrap/dist/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 gary       (501) staff       (20)   108738 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/bootstrap/dist/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 gary       (501) staff       (20)    45404 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/bootstrap/dist/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 gary       (501) staff       (20)    23424 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/bootstrap/dist/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 gary       (501) staff       (20)    18028 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/bootstrap/dist/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.949113 vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.950002 vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.458765 vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/css/
--rw-r--r--   0 gary       (501) staff       (20)     7410 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/css/vi_admin.css
--rw-r--r--   0 gary       (501) staff       (20)      668 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/css/vi_grid.css
--rw-r--r--   0 gary       (501) staff       (20)      763 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/css/vi_runsheet.css
--rw-r--r--   0 gary       (501) staff       (20)     1176 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/css/vi_scorecards.css
--rw-r--r--   0 gary       (501) staff       (20)      257 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/css/vi_signon.css
--rw-r--r--   0 gary       (501) staff       (20)      393 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/css/vi_team.css
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.459223 vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/img/
--rw-r--r--   0 gary       (501) staff       (20)      649 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/img/report.png
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.460676 vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/js/
--rw-r--r--   0 gary       (501) staff       (20)     1542 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/js/formset.js
--rw-r--r--   0 gary       (501) staff       (20)     1541 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/js/match_results.js
--rw-r--r--   0 gary       (501) staff       (20)      312 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/js/team.js
--rw-r--r--   0 gary       (501) staff       (20)     1978 2023-07-16 13:50:45.000000 vitriolic-3.3.9/tournamentcontrol/competition/tasks.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.950727 vitriolic-3.3.9/tournamentcontrol/competition/templates/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.463858 vitriolic-3.3.9/tournamentcontrol/competition/templates/competition/
--rw-r--r--   0 gary       (501) staff       (20)      457 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/competition/rankpoints_archive.html
--rw-r--r--   0 gary       (501) staff       (20)      533 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/competition/rankpoints_archive_day.html
--rw-r--r--   0 gary       (501) staff       (20)       52 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/competition/rankpoints_archive_month.html
--rw-r--r--   0 gary       (501) staff       (20)       52 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/competition/rankpoints_archive_year.html
--rw-r--r--   0 gary       (501) staff       (20)       26 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/competition/rankpoints_base.html
--rw-r--r--   0 gary       (501) staff       (20)      734 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/competition/rankpoints_detail.html
--rw-r--r--   0 gary       (501) staff       (20)     1386 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/competition/rankpoints_team.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.961336 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.464820 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/calculator/
--rw-r--r--   0 gary       (501) staff       (20)     4258 2023-02-16 20:24:29.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/calculator/index.html
--rw-r--r--   0 gary       (501) staff       (20)      168 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/calculator/live.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.478231 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/
--rw-r--r--   0 gary       (501) staff       (20)     1162 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/_club_opponent.html
--rw-r--r--   0 gary       (501) staff       (20)       46 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/_match_title.txt
--rw-r--r--   0 gary       (501) staff       (20)      192 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/_score.html
--rw-r--r--   0 gary       (501) staff       (20)      178 2022-07-18 07:51:12.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/_stage_group_position.txt
--rw-r--r--   0 gary       (501) staff       (20)      588 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/_team_opponent.html
--rw-r--r--   0 gary       (501) staff       (20)       54 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/_win_lose_team.txt
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.487633 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/
--rw-r--r--   0 gary       (501) staff       (20)      308 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/base.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.489026 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/club/
--rw-r--r--   0 gary       (501) staff       (20)      597 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/club/edit.html
--rw-r--r--   0 gary       (501) staff       (20)      301 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/club/list.inc.html
--rw-r--r--   0 gary       (501) staff       (20)     1203 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/club/team.inc.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.489535 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/clubassociation/
--rw-r--r--   0 gary       (501) staff       (20)      314 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/clubassociation/list.inc.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.489988 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/competition/
--rw-r--r--   0 gary       (501) staff       (20)      407 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/competition/list.inc.html
--rw-r--r--   0 gary       (501) staff       (20)       58 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/delete.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.491064 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/division/
--rw-r--r--   0 gary       (501) staff       (20)     1952 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/division/edit.html
--rw-r--r--   0 gary       (501) staff       (20)      740 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/division/list.inc.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.491544 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/divisionexclusiondate/
--rw-r--r--   0 gary       (501) staff       (20)      297 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/divisionexclusiondate/list.inc.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.492089 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/draw_generation/
--rw-r--r--   0 gary       (501) staff       (20)      495 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/draw_generation/wizard.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.492570 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/drawformat/
--rw-r--r--   0 gary       (501) staff       (20)      383 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/drawformat/list.inc.html
--rw-r--r--   0 gary       (501) staff       (20)     2941 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/grid.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.493050 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/ground/
--rw-r--r--   0 gary       (501) staff       (20)      824 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/ground/list.inc.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.493559 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/ladderentry/
--rw-r--r--   0 gary       (501) staff       (20)      947 2019-10-31 21:17:24.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/ladderentry/list.inc.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.495454 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/
--rw-r--r--   0 gary       (501) staff       (20)     3828 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/dates.html
--rw-r--r--   0 gary       (501) staff       (20)      241 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/edit.html
--rw-r--r--   0 gary       (501) staff       (20)      901 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/list.inc.html
--rw-r--r--   0 gary       (501) staff       (20)     4076 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/schedule.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.495955 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/tournament/
--rw-r--r--   0 gary       (501) staff       (20)      280 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/tournament/dates.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.496480 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/weekly/
--rw-r--r--   0 gary       (501) staff       (20)       69 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/weekly/dates.html
--rw-r--r--   0 gary       (501) staff       (20)     2636 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match_detail.html
--rw-r--r--   0 gary       (501) staff       (20)     3976 2019-10-31 21:17:24.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match_results.html
--rw-r--r--   0 gary       (501) staff       (20)     1420 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match_washout.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.497437 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/matchscoresheet/
--rw-r--r--   0 gary       (501) staff       (20)      294 2019-10-31 21:17:24.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/matchscoresheet/edit.html
--rw-r--r--   0 gary       (501) staff       (20)      383 2019-10-31 21:17:24.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/matchscoresheet/list.inc.html
--rw-r--r--   0 gary       (501) staff       (20)      697 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/mvp.html
--rw-r--r--   0 gary       (501) staff       (20)     2094 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/officials.html
--rw-r--r--   0 gary       (501) staff       (20)     1391 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/officials_list.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.498443 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/person/
--rw-r--r--   0 gary       (501) staff       (20)      597 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/person/edit.html
--rw-r--r--   0 gary       (501) staff       (20)     1375 2019-10-31 21:17:24.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/person/list.inc.html
--rw-r--r--   0 gary       (501) staff       (20)     2127 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/progress_matches.html
--rw-r--r--   0 gary       (501) staff       (20)     2690 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/progress_teams.html
--rw-r--r--   0 gary       (501) staff       (20)      731 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/reschedule.html
--rw-r--r--   0 gary       (501) staff       (20)      380 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/runsheet.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.499436 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/scorecards/
--rw-r--r--   0 gary       (501) staff       (20)      908 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/scorecards/report.html
--rw-r--r--   0 gary       (501) staff       (20)      174 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/scorecards/wait.html
--rw-r--r--   0 gary       (501) staff       (20)     3107 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/scorecards.html
--rw-r--r--   0 gary       (501) staff       (20)     2452 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/scorers.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.500830 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season/
--rw-r--r--   0 gary       (501) staff       (20)     3229 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season/edit.html
--rw-r--r--   0 gary       (501) staff       (20)     1495 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season/list.inc.html
--rw-r--r--   0 gary       (501) staff       (20)     2303 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season/timeslots.html
--rw-r--r--   0 gary       (501) staff       (20)     3751 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season_report.html
--rw-r--r--   0 gary       (501) staff       (20)     1774 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season_summary.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.501352 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/seasonexclusiondate/
--rw-r--r--   0 gary       (501) staff       (20)      297 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/seasonexclusiondate/list.inc.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.501819 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/seasonmatchtime/
--rw-r--r--   0 gary       (501) staff       (20)      512 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/seasonmatchtime/list.inc.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.502290 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/seasonreferee/
--rw-r--r--   0 gary       (501) staff       (20)      767 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/seasonreferee/list.inc.html
--rw-r--r--   0 gary       (501) staff       (20)     2365 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/signon.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.502766 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/simplescorematchstatistic/
--rw-r--r--   0 gary       (501) staff       (20)      761 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/simplescorematchstatistic/list.inc.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.503246 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/stage/
--rw-r--r--   0 gary       (501) staff       (20)     1148 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/stage/list.inc.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.503718 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/stagegroup/
--rw-r--r--   0 gary       (501) staff       (20)      386 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/stagegroup/list.inc.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.504189 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/team/
--rw-r--r--   0 gary       (501) staff       (20)      906 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/team/list.inc.html
--rw-r--r--   0 gary       (501) staff       (20)     1642 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/team_members.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.504672 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/teamassociation/
--rw-r--r--   0 gary       (501) staff       (20)      540 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/teamassociation/list.inc.html
--rw-r--r--   0 gary       (501) staff       (20)      222 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/wait.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.505641 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.506126 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/progress/
--rw-r--r--   0 gary       (501) staff       (20)     1130 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/progress/stages.html
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/reports.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.507283 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/results/
--rw-r--r--   0 gary       (501) staff       (20)     1135 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/results/basic.html
--rw-r--r--   0 gary       (501) staff       (20)     1830 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/results/detailed.html
--rw-r--r--   0 gary       (501) staff       (20)     1194 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/scoresheets.html
--rw-r--r--   0 gary       (501) staff       (20)      661 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/base.html
--rw-r--r--   0 gary       (501) staff       (20)     4328 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/club.html
--rw-r--r--   0 gary       (501) staff       (20)      390 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/compare.html
--rw-r--r--   0 gary       (501) staff       (20)     1198 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/competition.html
--rw-r--r--   0 gary       (501) staff       (20)     5419 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/division.html
--rw-r--r--   0 gary       (501) staff       (20)      301 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/divisiongroup.html
--rw-r--r--   0 gary       (501) staff       (20)      272 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/draw.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.509162 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/draw_format/
--rw-r--r--   0 gary       (501) staff       (20)      698 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/draw_format/16.txt
--rw-r--r--   0 gary       (501) staff       (20)       78 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/draw_format/4.txt
--rw-r--r--   0 gary       (501) staff       (20)      139 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/draw_format/6.txt
--rw-r--r--   0 gary       (501) staff       (20)      341 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/draw_format/8.txt
--rw-r--r--   0 gary       (501) staff       (20)     1055 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/forfeit.html
--rw-r--r--   0 gary       (501) staff       (20)     1444 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/forfeit_list.html
--rw-r--r--   0 gary       (501) staff       (20)      867 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/index.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.510180 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/ladder/
--rw-r--r--   0 gary       (501) staff       (20)     4161 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/ladder/pool.html
--rw-r--r--   0 gary       (501) staff       (20)     3015 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/ladder/standard.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:29.960685 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/match/
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.511159 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/match/live_stream/
--rw-r--r--   0 gary       (501) staff       (20)        0 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/match/live_stream/description.txt
--rw-r--r--   0 gary       (501) staff       (20)        0 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/match/live_stream/title.txt
--rw-r--r--   0 gary       (501) staff       (20)     2276 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/match.html
--rw-r--r--   0 gary       (501) staff       (20)     2214 2020-03-02 19:23:34.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/match_detail.html
--rw-r--r--   0 gary       (501) staff       (20)     3284 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/next_date.html
--rw-r--r--   0 gary       (501) staff       (20)     1678 2022-06-12 11:19:15.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/results.html
--rw-r--r--   0 gary       (501) staff       (20)     4005 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/runsheet.html
--rw-r--r--   0 gary       (501) staff       (20)      360 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/runsheet_list.html
--rw-r--r--   0 gary       (501) staff       (20)     2877 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/season.html
--rw-r--r--   0 gary       (501) staff       (20)     3212 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/season_videos.html
--rw-r--r--   0 gary       (501) staff       (20)     4619 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/stage.html
--rw-r--r--   0 gary       (501) staff       (20)     1274 2023-05-21 21:21:54.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/stream.html
--rw-r--r--   0 gary       (501) staff       (20)     4483 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/team.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.512040 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/templatetags/
--rw-r--r--   0 gary       (501) staff       (20)      702 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/templatetags/preview.html
--rw-r--r--   0 gary       (501) staff       (20)      704 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/templatetags/statistics.html
--rw-r--r--   0 gary       (501) staff       (20)      369 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/videos.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.517365 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/
--rw-r--r--   0 gary       (501) staff       (20)      418 2019-12-17 12:14:26.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/_base.html
--rw-r--r--   0 gary       (501) staff       (20)     2841 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/_registration_form.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.517804 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/admin/
--rw-r--r--   0 gary       (501) staff       (20)       62 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/admin/base.html
--rw-r--r--   0 gary       (501) staff       (20)       50 2019-12-17 12:14:30.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/base.html
--rw-r--r--   0 gary       (501) staff       (20)      588 2019-12-17 12:14:06.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/club_members.html
--rw-r--r--   0 gary       (501) staff       (20)      774 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/club_teams.html
--rw-r--r--   0 gary       (501) staff       (20)       96 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/delete.html
--rw-r--r--   0 gary       (501) staff       (20)      752 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/index.html
--rw-r--r--   0 gary       (501) staff       (20)      559 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/officials.html
--rw-r--r--   0 gary       (501) staff       (20)      564 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/officials_list.html
--rw-r--r--   0 gary       (501) staff       (20)       63 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/registration_form.html
--rw-r--r--   0 gary       (501) staff       (20)     1471 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/team_members.html
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.518644 vitriolic-3.3.9/tournamentcontrol/competition/templatetags/
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/templatetags/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)     7703 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/templatetags/competition.py
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.524618 vitriolic-3.3.9/tournamentcontrol/competition/tests/
--rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.3.9/tournamentcontrol/competition/tests/__init__.py
--rw-r--r--   0 gary       (501) staff       (20)     6820 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/tests/factories.py
--rw-r--r--   0 gary       (501) staff       (20)    38099 2024-04-14 00:51:21.000000 vitriolic-3.3.9/tournamentcontrol/competition/tests/test_competition_admin.py
--rw-r--r--   0 gary       (501) staff       (20)    11889 2022-07-02 05:40:48.000000 vitriolic-3.3.9/tournamentcontrol/competition/tests/test_competition_site.py
--rw-r--r--   0 gary       (501) staff       (20)     1837 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/tests/test_dashboard.py
--rw-r--r--   0 gary       (501) staff       (20)     2299 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/tests/test_draw.py
--rw-r--r--   0 gary       (501) staff       (20)     1434 2023-10-26 06:01:12.000000 vitriolic-3.3.9/tournamentcontrol/competition/tests/test_forms.py
--rw-r--r--   0 gary       (501) staff       (20)     7104 2023-05-21 21:14:55.000000 vitriolic-3.3.9/tournamentcontrol/competition/tests/test_formsets.py
--rw-r--r--   0 gary       (501) staff       (20)     4308 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/tests/test_rank.py
--rw-r--r--   0 gary       (501) staff       (20)     1925 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/tests/test_signals.py
--rw-r--r--   0 gary       (501) staff       (20)     1240 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/tests/test_utils.py
--rw-r--r--   0 gary       (501) staff       (20)      339 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/tests/urls.py
--rw-r--r--   0 gary       (501) staff       (20)    17484 2024-05-08 12:45:02.000000 vitriolic-3.3.9/tournamentcontrol/competition/utils.py
--rw-r--r--   0 gary       (501) staff       (20)      227 2022-06-12 11:19:40.000000 vitriolic-3.3.9/tournamentcontrol/competition/validators.py
--rw-r--r--   0 gary       (501) staff       (20)     8084 2022-07-03 22:11:56.000000 vitriolic-3.3.9/tournamentcontrol/competition/wizards.py
--rw-r--r--   0 gary       (501) staff       (20)      820 2024-04-14 00:51:21.000000 vitriolic-3.3.9/tox.ini
-drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-08 12:46:30.528483 vitriolic-3.3.9/vitriolic.egg-info/
--rw-r--r--   0 gary       (501) staff       (20)     5002 2024-05-08 12:46:29.000000 vitriolic-3.3.9/vitriolic.egg-info/PKG-INFO
--rw-r--r--   0 gary       (501) staff       (20)    60266 2024-05-08 12:46:29.000000 vitriolic-3.3.9/vitriolic.egg-info/SOURCES.txt
--rw-r--r--   0 gary       (501) staff       (20)        1 2024-05-08 12:46:29.000000 vitriolic-3.3.9/vitriolic.egg-info/dependency_links.txt
--rw-r--r--   0 gary       (501) staff       (20)        1 2024-05-05 00:47:14.000000 vitriolic-3.3.9/vitriolic.egg-info/not-zip-safe
--rw-r--r--   0 gary       (501) staff       (20)      626 2024-05-08 12:46:29.000000 vitriolic-3.3.9/vitriolic.egg-info/requires.txt
--rw-r--r--   0 gary       (501) staff       (20)       34 2024-05-08 12:46:29.000000 vitriolic-3.3.9/vitriolic.egg-info/top_level.txt
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.298427 vitriolic-3.4.0/
+-rw-r--r--   0 gary       (501) staff       (20)      436 2019-10-18 22:04:04.000000 vitriolic-3.4.0/.editorconfig
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.627415 vitriolic-3.4.0/.github/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.676015 vitriolic-3.4.0/.github/workflows/
+-rw-r--r--   0 gary       (501) staff       (20)     1153 2024-02-09 07:02:29.000000 vitriolic-3.4.0/.github/workflows/django.yml
+-rw-r--r--   0 gary       (501) staff       (20)       80 2023-05-21 21:21:54.000000 vitriolic-3.4.0/.gitignore
+-rw-r--r--   0 gary       (501) staff       (20)      476 2019-10-18 22:04:04.000000 vitriolic-3.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 gary       (501) staff       (20)     1302 2019-10-18 22:04:04.000000 vitriolic-3.4.0/ISSUES.md
+-rw-r--r--   0 gary       (501) staff       (20)     1524 2019-10-18 22:04:04.000000 vitriolic-3.4.0/LICENSE
+-rw-r--r--   0 gary       (501) staff       (20)      862 2022-06-12 11:19:40.000000 vitriolic-3.4.0/MANIFEST.in
+-rw-r--r--   0 gary       (501) staff       (20)     5002 2024-05-17 23:21:08.297567 vitriolic-3.4.0/PKG-INFO
+-rw-r--r--   0 gary       (501) staff       (20)     1118 2023-05-21 21:14:55.000000 vitriolic-3.4.0/README.md
+-rw-r--r--   0 gary       (501) staff       (20)     1990 2024-04-13 04:07:31.000000 vitriolic-3.4.0/pyproject.toml
+-rw-r--r--   0 gary       (501) staff       (20)      170 2023-05-21 21:14:55.000000 vitriolic-3.4.0/renovate.json
+-rw-r--r--   0 gary       (501) staff       (20)       38 2024-05-17 23:21:08.298566 vitriolic-3.4.0/setup.cfg
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.677399 vitriolic-3.4.0/tests/
+-rw-r--r--   0 gary       (501) staff       (20)      110 2019-10-31 21:17:24.000000 vitriolic-3.4.0/tests/.coveragerc
+-rw-r--r--   0 gary       (501) staff       (20)       32 2019-10-31 21:17:24.000000 vitriolic-3.4.0/tests/.gitignore
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/__init__.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.679630 vitriolic-3.4.0/tests/example_app/
+-rw-r--r--   0 gary       (501) staff       (20)      157 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/example_app/__init__.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.680161 vitriolic-3.4.0/tests/example_app/fixtures/
+-rw-r--r--   0 gary       (501) staff       (20)     1626 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/example_app/fixtures/query_string.json
+-rw-r--r--   0 gary       (501) staff       (20)      162 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/example_app/forms.py
+-rw-r--r--   0 gary       (501) staff       (20)      465 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/example_app/models.py
+-rw-r--r--   0 gary       (501) staff       (20)     6846 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tests/example_app/sites.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.628300 vitriolic-3.4.0/tests/example_app/templates/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.629155 vitriolic-3.4.0/tests/example_app/templates/example_app/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.681347 vitriolic-3.4.0/tests/example_app/templates/example_app/context/
+-rw-r--r--   0 gary       (501) staff       (20)       15 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/example_app/templates/example_app/context/env.html
+-rw-r--r--   0 gary       (501) staff       (20)       11 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/example_app/templates/example_app/context/site.html
+-rw-r--r--   0 gary       (501) staff       (20)       16 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/example_app/templates/example_app/context/tz.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.681868 vitriolic-3.4.0/tests/example_app/templates/example_app/datetime/
+-rw-r--r--   0 gary       (501) staff       (20)       82 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/example_app/templates/example_app/datetime/edit.related.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.683984 vitriolic-3.4.0/tests/example_app/templates/example_app/generic/
+-rw-r--r--   0 gary       (501) staff       (20)      282 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/example_app/templates/example_app/generic/detail.html
+-rw-r--r--   0 gary       (501) staff       (20)      404 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/example_app/templates/example_app/generic/edit.html
+-rw-r--r--   0 gary       (501) staff       (20)      461 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/example_app/templates/example_app/generic/edit_multiple.html
+-rw-r--r--   0 gary       (501) staff       (20)      356 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/example_app/templates/example_app/generic/list.html
+-rw-r--r--   0 gary       (501) staff       (20)      649 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/example_app/templates/example_app/generic/permissions.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.628996 vitriolic-3.4.0/tests/example_app/templates/example_app/pagination/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.684504 vitriolic-3.4.0/tests/example_app/templates/example_app/pagination/testdatetimefield/
+-rw-r--r--   0 gary       (501) staff       (20)      313 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/example_app/templates/example_app/pagination/testdatetimefield/list.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.629273 vitriolic-3.4.0/tests/example_app/templates/example_app/querystring/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.685040 vitriolic-3.4.0/tests/example_app/templates/example_app/querystring/testdatetimefield/
+-rw-r--r--   0 gary       (501) staff       (20)      314 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/example_app/templates/example_app/querystring/testdatetimefield/list.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.685823 vitriolic-3.4.0/tests/example_app/tests/
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/example_app/tests/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)      683 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tests/example_app/tests/factories.py
+-rw-r--r--   0 gary       (501) staff       (20)      953 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tests/example_app/urls.py
+-rw-r--r--   0 gary       (501) staff       (20)      141 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/example_app/views.py
+-rwxr-xr-x   0 gary       (501) staff       (20)      815 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/manage.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.688111 vitriolic-3.4.0/tests/vitriolic/
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/vitriolic/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)     5754 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tests/vitriolic/settings.py
+-rw-r--r--   0 gary       (501) staff       (20)      438 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tests/vitriolic/urls.py
+-rw-r--r--   0 gary       (501) staff       (20)      396 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tests/vitriolic/wsgi.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.688809 vitriolic-3.4.0/touchtechnology/
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/__init__.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.692213 vitriolic-3.4.0/touchtechnology/admin/
+-rw-r--r--   0 gary       (501) staff       (20)      109 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)     3485 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/apps.py
+-rw-r--r--   0 gary       (501) staff       (20)     4923 2024-04-13 04:06:41.000000 vitriolic-3.4.0/touchtechnology/admin/base.py
+-rw-r--r--   0 gary       (501) staff       (20)     1594 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/forms.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.631069 vitriolic-3.4.0/touchtechnology/admin/locale/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.630315 vitriolic-3.4.0/touchtechnology/admin/locale/de/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.693146 vitriolic-3.4.0/touchtechnology/admin/locale/de/LC_MESSAGES/
+-rw-r--r--   0 gary       (501) staff       (20)      421 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/admin/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 gary       (501) staff       (20)     2804 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/admin/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.630607 vitriolic-3.4.0/touchtechnology/admin/locale/en-AU/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.694169 vitriolic-3.4.0/touchtechnology/admin/locale/en-AU/LC_MESSAGES/
+-rw-r--r--   0 gary       (501) staff       (20)      378 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/admin/locale/en-AU/LC_MESSAGES/django.mo
+-rw-r--r--   0 gary       (501) staff       (20)     2757 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/admin/locale/en-AU/LC_MESSAGES/django.po
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.630900 vitriolic-3.4.0/touchtechnology/admin/locale/fr/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.695372 vitriolic-3.4.0/touchtechnology/admin/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 gary       (501) staff       (20)      971 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/admin/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 gary       (501) staff       (20)     3234 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/admin/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.631194 vitriolic-3.4.0/touchtechnology/admin/locale/ja/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.696461 vitriolic-3.4.0/touchtechnology/admin/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 gary       (501) staff       (20)      414 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/admin/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 gary       (501) staff       (20)     2797 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/admin/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0 gary       (501) staff       (20)      825 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/mixins.py
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/models.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.698790 vitriolic-3.4.0/touchtechnology/admin/sites/
+-rw-r--r--   0 gary       (501) staff       (20)       76 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/sites/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)     5959 2024-04-13 04:06:43.000000 vitriolic-3.4.0/touchtechnology/admin/sites/admin.py
+-rw-r--r--   0 gary       (501) staff       (20)     6045 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/sites/auth.py
+-rw-r--r--   0 gary       (501) staff       (20)     1529 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/sites/settings.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.641580 vitriolic-3.4.0/touchtechnology/admin/static/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.702717 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/
+-rw-r--r--   0 gary       (501) staff       (20)      425 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/CHANGELOG.md
+-rw-r--r--   0 gary       (501) staff       (20)    14386 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/Gruntfile.js
+-rw-r--r--   0 gary       (501) staff       (20)      641 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/bower.json
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.632299 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.708688 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/css/
+-rw-r--r--   0 gary       (501) staff       (20)    26132 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/css/bootstrap-theme.css
+-rw-r--r--   0 gary       (501) staff       (20)    47706 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/css/bootstrap-theme.css.map
+-rw-r--r--   0 gary       (501) staff       (20)    23409 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/css/bootstrap-theme.min.css
+-rw-r--r--   0 gary       (501) staff       (20)    25648 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/css/bootstrap-theme.min.css.map
+-rw-r--r--   0 gary       (501) staff       (20)   146010 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/css/bootstrap.css
+-rw-r--r--   0 gary       (501) staff       (20)   389287 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/css/bootstrap.css.map
+-rw-r--r--   0 gary       (501) staff       (20)   121200 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/css/bootstrap.min.css
+-rw-r--r--   0 gary       (501) staff       (20)   542194 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/css/bootstrap.min.css.map
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.711916 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/fonts/
+-rw-r--r--   0 gary       (501) staff       (20)    20127 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 gary       (501) staff       (20)   108738 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 gary       (501) staff       (20)    45404 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 gary       (501) staff       (20)    23424 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 gary       (501) staff       (20)    18028 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.713629 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/js/
+-rw-r--r--   0 gary       (501) staff       (20)    69707 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/js/bootstrap.js
+-rw-r--r--   0 gary       (501) staff       (20)    37045 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/js/bootstrap.min.js
+-rw-r--r--   0 gary       (501) staff       (20)      484 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/js/npm.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.717911 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/grunt/
+-rw-r--r--   0 gary       (501) staff       (20)      990 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/grunt/bs-commonjs-generator.js
+-rw-r--r--   0 gary       (501) staff       (20)     1405 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/grunt/bs-glyphicons-data-generator.js
+-rw-r--r--   0 gary       (501) staff       (20)     6075 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/grunt/bs-lessdoc-parser.js
+-rw-r--r--   0 gary       (501) staff       (20)     1349 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/grunt/bs-raw-files-generator.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     2909 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/grunt/change-version.js
+-rw-r--r--   0 gary       (501) staff       (20)     1395 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/grunt/configBridge.json
+-rw-r--r--   0 gary       (501) staff       (20)    93626 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/grunt/npm-shrinkwrap.json
+-rw-r--r--   0 gary       (501) staff       (20)     1439 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/grunt/sauce_browsers.yml
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.725776 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/
+-rw-r--r--   0 gary       (501) staff       (20)     4838 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/affix.js
+-rw-r--r--   0 gary       (501) staff       (20)     2284 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/alert.js
+-rw-r--r--   0 gary       (501) staff       (20)     3824 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/button.js
+-rw-r--r--   0 gary       (501) staff       (20)     7141 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/carousel.js
+-rw-r--r--   0 gary       (501) staff       (20)     5991 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/collapse.js
+-rw-r--r--   0 gary       (501) staff       (20)     4743 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/dropdown.js
+-rw-r--r--   0 gary       (501) staff       (20)     9987 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/modal.js
+-rw-r--r--   0 gary       (501) staff       (20)     3163 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/popover.js
+-rw-r--r--   0 gary       (501) staff       (20)     4707 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/scrollspy.js
+-rw-r--r--   0 gary       (501) staff       (20)     3905 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/tab.js
+-rw-r--r--   0 gary       (501) staff       (20)    16719 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/tooltip.js
+-rw-r--r--   0 gary       (501) staff       (20)     1831 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/transition.js
+-rw-r--r--   0 gary       (501) staff       (20)      964 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/package.js
+-rw-r--r--   0 gary       (501) staff       (20)     2200 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/package.json
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.730282 vitriolic-3.4.0/touchtechnology/admin/static/css/
+-rw-r--r--   0 gary       (501) staff       (20)       84 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/css/Makefile
+-rw-r--r--   0 gary       (501) staff       (20)     1172 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/css/custom.css
+-rw-r--r--   0 gary       (501) staff       (20)     1373 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/css/custom.less
+-rwxr-xr-x   0 gary       (501) staff       (20)    51742 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/css/mvpready-admin.css
+-rwxr-xr-x   0 gary       (501) staff       (20)    39265 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/css/mvpready-landing.css
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.750880 vitriolic-3.4.0/touchtechnology/admin/static/flot/
+-rwxr-xr-x   0 gary       (501) staff       (20)      413 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/.bower.json
+-rwxr-xr-x   0 gary       (501) staff       (20)       40 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/.gitignore
+-rwxr-xr-x   0 gary       (501) staff       (20)       35 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/.travis.yml
+-rwxr-xr-x   0 gary       (501) staff       (20)     1069 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/LICENSE.txt
+-rwxr-xr-x   0 gary       (501) staff       (20)      285 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/Makefile
+-rwxr-xr-x   0 gary       (501) staff       (20)      114 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/component.json
+-rwxr-xr-x   0 gary       (501) staff       (20)    41943 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/excanvas.js
+-rwxr-xr-x   0 gary       (501) staff       (20)    19314 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/excanvas.min.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      837 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/flot.jquery.json
+-rwxr-xr-x   0 gary       (501) staff       (20)     6151 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.colorhelpers.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     9599 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.canvas.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     6033 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.categories.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     5419 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.crosshair.js
+-rwxr-xr-x   0 gary       (501) staff       (20)    12614 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.errorbars.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     5257 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.fillbetween.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     7360 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.image.js
+-rwxr-xr-x   0 gary       (501) staff       (20)   122971 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.js
+-rwxr-xr-x   0 gary       (501) staff       (20)    14216 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.navigate.js
+-rwxr-xr-x   0 gary       (501) staff       (20)    23809 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.pie.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     3314 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.resize.js
+-rwxr-xr-x   0 gary       (501) staff       (20)    13141 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.selection.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     7090 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.stack.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     2505 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.symbol.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     4480 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.threshold.js
+-rwxr-xr-x   0 gary       (501) staff       (20)    11768 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.time.js
+-rwxr-xr-x   0 gary       (501) staff       (20)   266057 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      154 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot/package.json
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.752042 vitriolic-3.4.0/touchtechnology/admin/static/flot.tooltip/
+-rwxr-xr-x   0 gary       (501) staff       (20)      532 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot.tooltip/.bower.json
+-rwxr-xr-x   0 gary       (501) staff       (20)      212 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot.tooltip/bower.json
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.755736 vitriolic-3.4.0/touchtechnology/admin/static/flot.tooltip/js/
+-rwxr-xr-x   0 gary       (501) staff       (20)    19415 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot.tooltip/js/excanvas.min.js
+-rwxr-xr-x   0 gary       (501) staff       (20)   122971 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot.tooltip/js/jquery.flot.js
+-rwxr-xr-x   0 gary       (501) staff       (20)    19258 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot.tooltip/js/jquery.flot.tooltip.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     7380 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot.tooltip/js/jquery.flot.tooltip.min.js
+-rwxr-xr-x   0 gary       (501) staff       (20)    18958 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/flot.tooltip/js/jquery.flot.tooltip.source.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.757652 vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/
+-rwxr-xr-x   0 gary       (501) staff       (20)      696 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/.bower.json
+-rwxr-xr-x   0 gary       (501) staff       (20)      301 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/.gitignore
+-rwxr-xr-x   0 gary       (501) staff       (20)      427 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/.npmignore
+-rwxr-xr-x   0 gary       (501) staff       (20)      412 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/bower.json
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.771492 vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/css/
+-rwxr-xr-x   0 gary       (501) staff       (20)    37414 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/css/font-awesome.css
+-rwxr-xr-x   0 gary       (501) staff       (20)    21778 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/css/font-awesome.css.map
+-rwxr-xr-x   0 gary       (501) staff       (20)    31000 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/css/font-awesome.min.css
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.786008 vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/fonts/
+-rwxr-xr-x   0 gary       (501) staff       (20)   134808 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/fonts/FontAwesome.otf
+-rwxr-xr-x   0 gary       (501) staff       (20)   165742 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/fonts/fontawesome-webfont.eot
+-rwxr-xr-x   0 gary       (501) staff       (20)   444379 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/fonts/fontawesome-webfont.svg
+-rwxr-xr-x   0 gary       (501) staff       (20)   165548 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/fonts/fontawesome-webfont.ttf
+-rwxr-xr-x   0 gary       (501) staff       (20)    98024 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/fonts/fontawesome-webfont.woff
+-rwxr-xr-x   0 gary       (501) staff       (20)    77160 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.786840 vitriolic-3.4.0/touchtechnology/admin/static/img/
+-rwxr-xr-x   0 gary       (501) staff       (20)    49582 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/img/logo.png
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.789388 vitriolic-3.4.0/touchtechnology/admin/static/jquery/
+-rwxr-xr-x   0 gary       (501) staff       (20)      730 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/.bower.json
+-rwxr-xr-x   0 gary       (501) staff       (20)     1099 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/MIT-LICENSE.txt
+-rwxr-xr-x   0 gary       (501) staff       (20)      425 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/bower.json
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.885126 vitriolic-3.4.0/touchtechnology/admin/static/jquery/dist/
+-rwxr-xr-x   0 gary       (501) staff       (20)   282766 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/dist/jquery.js
+-rwxr-xr-x   0 gary       (501) staff       (20)    95821 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/dist/jquery.min.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.901261 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.907654 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/ajax/
+-rwxr-xr-x   0 gary       (501) staff       (20)     2516 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/ajax/jsonp.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1681 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/ajax/load.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1476 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/ajax/parseJSON.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      650 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/ajax/parseXML.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1964 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/ajax/script.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.908492 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/ajax/var/
+-rwxr-xr-x   0 gary       (501) staff       (20)       73 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/ajax/var/nonce.js
+-rwxr-xr-x   0 gary       (501) staff       (20)       40 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/ajax/var/rquery.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     5786 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/ajax/xhr.js
+-rwxr-xr-x   0 gary       (501) staff       (20)    21812 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/ajax.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.910797 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/attributes/
+-rwxr-xr-x   0 gary       (501) staff       (20)     7263 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/attributes/attr.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     4116 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/attributes/classes.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     3138 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/attributes/prop.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1994 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/attributes/support.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     4303 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/attributes/val.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      200 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/attributes.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     5506 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/callbacks.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.912679 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/core/
+-rwxr-xr-x   0 gary       (501) staff       (20)     1219 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/core/access.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     3716 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/core/init.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      938 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/core/parseHTML.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     3896 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/core/ready.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.913092 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/core/var/
+-rwxr-xr-x   0 gary       (501) staff       (20)       91 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/core/var/rsingleTag.js
+-rwxr-xr-x   0 gary       (501) staff       (20)    12500 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/core.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.915589 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/css/
+-rwxr-xr-x   0 gary       (501) staff       (20)      785 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/css/addGetHookIf.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     3307 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/css/curCSS.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1907 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/css/defaultDisplay.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      542 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/css/hiddenVisibleSelectors.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     4823 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/css/support.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      555 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/css/swap.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.917183 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/css/var/
+-rwxr-xr-x   0 gary       (501) staff       (20)       70 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/css/var/cssExpand.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      355 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/css/var/isHidden.js
+-rwxr-xr-x   0 gary       (501) staff       (20)       45 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/css/var/rmargin.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      113 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/css/var/rnumnonpx.js
+-rwxr-xr-x   0 gary       (501) staff       (20)    14612 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/css.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.918011 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/data/
+-rwxr-xr-x   0 gary       (501) staff       (20)      567 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/data/accepts.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      438 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/data/support.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     8509 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/data.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     4413 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/deferred.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      223 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/deprecated.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1881 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/dimensions.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.919216 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/effects/
+-rwxr-xr-x   0 gary       (501) staff       (20)     3034 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/effects/Tween.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      225 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/effects/animatedSelector.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1459 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/effects/support.js
+-rwxr-xr-x   0 gary       (501) staff       (20)    17243 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/effects.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.920004 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/event/
+-rwxr-xr-x   0 gary       (501) staff       (20)     1094 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/event/alias.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      641 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/event/support.js
+-rwxr-xr-x   0 gary       (501) staff       (20)    30072 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/event.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.920837 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/exports/
+-rwxr-xr-x   0 gary       (501) staff       (20)     1006 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/exports/amd.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      641 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/exports/global.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1405 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/intro.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      571 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/jquery.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.921735 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/manipulation/
+-rwxr-xr-x   0 gary       (501) staff       (20)      240 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/manipulation/_evalUrl.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     2476 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/manipulation/support.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.922216 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/manipulation/var/
+-rwxr-xr-x   0 gary       (501) staff       (20)       59 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/manipulation/var/rcheckableType.js
+-rwxr-xr-x   0 gary       (501) staff       (20)    20616 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/manipulation.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     5856 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/offset.js
+-rwxr-xr-x   0 gary       (501) staff       (20)        5 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/outro.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.922856 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/queue/
+-rwxr-xr-x   0 gary       (501) staff       (20)      561 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/queue/delay.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     3071 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/queue.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      294 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/selector-sizzle.js
+-rwxr-xr-x   0 gary       (501) staff       (20)       33 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/selector.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     3211 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/serialize.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.639158 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/sizzle/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.924277 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/sizzle/dist/
+-rwxr-xr-x   0 gary       (501) staff       (20)    58579 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/sizzle/dist/sizzle.js
+-rwxr-xr-x   0 gary       (501) staff       (20)    18574 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/sizzle/dist/sizzle.min.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1697 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/support.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.924979 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/traversing/
+-rwxr-xr-x   0 gary       (501) staff       (20)     2466 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/traversing/findFilter.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.925612 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/traversing/var/
+-rwxr-xr-x   0 gary       (501) staff       (20)      110 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/traversing/var/rneedsContext.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     4575 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/traversing.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.940361 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/var/
+-rwxr-xr-x   0 gary       (501) staff       (20)       64 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/var/class2type.js
+-rwxr-xr-x   0 gary       (501) staff       (20)       84 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/var/concat.js
+-rwxr-xr-x   0 gary       (501) staff       (20)       36 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/var/deletedIds.js
+-rwxr-xr-x   0 gary       (501) staff       (20)       92 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/var/hasOwn.js
+-rwxr-xr-x   0 gary       (501) staff       (20)       85 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/var/indexOf.js
+-rwxr-xr-x   0 gary       (501) staff       (20)       80 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/var/pnum.js
+-rwxr-xr-x   0 gary       (501) staff       (20)       82 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/var/push.js
+-rwxr-xr-x   0 gary       (501) staff       (20)       42 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/var/rnotwhite.js
+-rwxr-xr-x   0 gary       (501) staff       (20)       83 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/var/slice.js
+-rwxr-xr-x   0 gary       (501) staff       (20)       50 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/var/strundefined.js
+-rwxr-xr-x   0 gary       (501) staff       (20)       99 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/var/support.js
+-rwxr-xr-x   0 gary       (501) staff       (20)       86 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/var/toString.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1456 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/wrap.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.794732 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/
+-rwxr-xr-x   0 gary       (501) staff       (20)      999 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/.bower.json
+-rwxr-xr-x   0 gary       (501) staff       (20)      739 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/bower.json
+-rwxr-xr-x   0 gary       (501) staff       (20)     1659 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/icheck.jquery.json
+-rwxr-xr-x   0 gary       (501) staff       (20)    14136 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/icheck.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     4931 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/icheck.min.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.796069 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/
+-rwxr-xr-x   0 gary       (501) staff       (20)     1568 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/all.css
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.823028 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/
+-rwxr-xr-x   0 gary       (501) staff       (20)    12513 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/_all.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1302 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/aero.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1520 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/aero.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     3218 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/aero@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1302 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/blue.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1518 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/blue.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     3217 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/blue@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1243 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/flat.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1515 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/flat.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     3217 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/flat@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1317 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/green.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1444 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/green.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     3117 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/green@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1302 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/grey.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1516 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/grey.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     3217 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/grey@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1332 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/orange.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1518 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/orange.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     3275 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/orange@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1302 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/pink.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1522 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/pink.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     3218 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/pink@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1332 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/purple.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1519 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/purple.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     3218 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/purple@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1287 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/red.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1516 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/red.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     3276 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/red@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1332 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/yellow.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1516 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/yellow.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     3216 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/yellow@2x.png
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.826318 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/futurico/
+-rwxr-xr-x   0 gary       (501) staff       (20)     1295 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/futurico/futurico.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1734 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/futurico/futurico.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     3446 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/futurico/futurico@2x.png
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.835270 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/
+-rwxr-xr-x   0 gary       (501) staff       (20)    20429 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/_all.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     2096 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/aero.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     2096 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/blue.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     2118 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/green.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     2096 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/grey.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1977 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/line.css
+-rwxr-xr-x   0 gary       (501) staff       (20)      588 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/line.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1073 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/line@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     2134 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/orange.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     2096 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/pink.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     2140 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/purple.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     2074 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/red.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     2140 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/yellow.css
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.855731 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/
+-rwxr-xr-x   0 gary       (501) staff       (20)    14474 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/_all.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1500 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/aero.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1151 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/aero.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1409 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/aero@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1500 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/blue.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1132 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/blue.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1410 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/blue@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1517 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/green.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1143 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/green.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1408 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/green@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1500 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/grey.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1142 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/grey.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1407 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/grey@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1437 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/minimal.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1114 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/minimal.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1410 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/minimal@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1534 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/orange.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1139 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/orange.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1407 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/orange@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1500 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/pink.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1150 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/pink.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1409 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/pink@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1534 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/purple.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1132 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/purple.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1409 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/purple@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1483 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/red.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1130 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/red.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1410 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/red@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1534 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/yellow.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1135 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/yellow.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1406 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/yellow@2x.png
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.857750 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/polaris/
+-rwxr-xr-x   0 gary       (501) staff       (20)     1431 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/polaris/polaris.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     6401 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/polaris/polaris.png
+-rwxr-xr-x   0 gary       (501) staff       (20)    16760 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/polaris/polaris@2x.png
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.882610 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/
+-rwxr-xr-x   0 gary       (501) staff       (20)    14331 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/_all.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1485 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/aero.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     2167 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/aero.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     4455 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/aero@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1485 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/blue.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     2185 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/blue.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     4485 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/blue@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1502 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/green.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     2193 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/green.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     4498 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/green@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1485 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/grey.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     2186 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/grey.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     4483 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/grey@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1519 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/orange.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     2181 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/orange.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     4474 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/orange@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1485 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/pink.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     2189 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/pink.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     4479 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/pink@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1519 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/purple.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     2188 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/purple.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     4501 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/purple@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1468 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/red.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     2190 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/red.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     4490 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/red@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1420 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/square.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     2175 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/square.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     4478 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/square@2x.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1519 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/yellow.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     2131 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/yellow.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     4385 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/yellow@2x.png
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.947057 vitriolic-3.4.0/touchtechnology/admin/static/js/
+-rw-r--r--   0 gary       (501) staff       (20)    30121 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/URI.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.949750 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.956732 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/
+-rwxr-xr-x   0 gary       (501) staff       (20)     1682 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/area.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1853 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/auto.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      857 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/donut.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1130 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/horizontal.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1747 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/line.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      798 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/pie.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1053 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/scatter.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     2128 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/stacked-area.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      998 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/stacked-horizontal.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1542 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/stacked-vertical.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1818 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/vertical.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     3612 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/form-plugins.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.957145 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/json/
+-rwxr-xr-x   0 gary       (501) staff       (20)     1440 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/json/table_data_small.json
+-rwxr-xr-x   0 gary       (501) staff       (20)      145 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/page-icons.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      217 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/pricing.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.957558 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/reports/
+-rwxr-xr-x   0 gary       (501) staff       (20)     1569 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/reports/line.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      138 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/demos/validation.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      855 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/mvpready-account.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1513 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/mvpready-admin.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     3738 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/mvpready-core.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     4491 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/js/mvpready-helpers.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.996371 vitriolic-3.4.0/touchtechnology/admin/static/select2/
+-rwxr-xr-x   0 gary       (501) staff       (20)      526 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/.bower.json
+-rwxr-xr-x   0 gary       (501) staff       (20)        7 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/.gitignore
+-rwxr-xr-x   0 gary       (501) staff       (20)      206 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/bower.json
+-rwxr-xr-x   0 gary       (501) staff       (20)     1732 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/component.json
+-rwxr-xr-x   0 gary       (501) staff       (20)      637 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/composer.json
+-rwxr-xr-x   0 gary       (501) staff       (20)      678 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/package.json
+-rwxr-xr-x   0 gary       (501) staff       (20)     1490 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/release.sh
+-rwxr-xr-x   0 gary       (501) staff       (20)     3347 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2-bootstrap.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1849 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2-spinner.gif
+-rwxr-xr-x   0 gary       (501) staff       (20)    19457 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2.css
+-rwxr-xr-x   0 gary       (501) staff       (20)     1030 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2.jquery.json
+-rwxr-xr-x   0 gary       (501) staff       (20)   148536 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2.js
+-rwxr-xr-x   0 gary       (501) staff       (20)    66596 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2.min.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      613 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2.png
+-rwxr-xr-x   0 gary       (501) staff       (20)     1389 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_ar.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1003 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_az.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1081 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_bg.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      952 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_ca.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1988 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_cs.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      853 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_da.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1014 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_de.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1128 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_el.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1102 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_en.js.template
+-rwxr-xr-x   0 gary       (501) staff       (20)     1177 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_es.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      886 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_et.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1313 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_eu.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1207 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_fa.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      940 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_fi.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1077 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_fr.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1339 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_gl.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      885 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_he.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1002 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_hr.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      802 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_hu.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      891 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_id.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      855 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_is.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      866 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_it.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      812 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_ja.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1078 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_ka.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      871 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_ko.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1144 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_lt.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      999 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_lv.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1064 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_mk.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      836 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_ms.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1145 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_nb.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      846 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_nl.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     2015 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_pl.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      969 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_pt-BR.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      891 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_pt-PT.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      902 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_ro.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1058 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_rs.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1171 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_ru.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1948 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_sk.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      847 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_sv.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1063 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_th.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      831 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_tr.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      904 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_ug-CN.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     1415 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_uk.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      959 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_vi.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      762 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_zh-CN.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      774 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_zh-TW.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      845 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/select2/select2x2.png
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.000081 vitriolic-3.4.0/touchtechnology/admin/static/slimscroll/
+-rwxr-xr-x   0 gary       (501) staff       (20)     1224 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/slimscroll/.bower.json
+-rwxr-xr-x   0 gary       (501) staff       (20)      943 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/slimscroll/bower.json
+-rwxr-xr-x   0 gary       (501) staff       (20)    13657 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/slimscroll/jquery.slimscroll.js
+-rwxr-xr-x   0 gary       (501) staff       (20)     4679 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/slimscroll/jquery.slimscroll.min.js
+-rwxr-xr-x   0 gary       (501) staff       (20)      937 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/slimscroll/slimScroll.jquery.json
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.641714 vitriolic-3.4.0/touchtechnology/admin/static/touchtechnology/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.642027 vitriolic-3.4.0/touchtechnology/admin/static/touchtechnology/admin/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.000690 vitriolic-3.4.0/touchtechnology/admin/static/touchtechnology/admin/img/
+-rw-r--r--   0 gary       (501) staff       (20)     8479 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/touchtechnology/admin/img/touch-technology.png
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.002626 vitriolic-3.4.0/touchtechnology/admin/static/touchtechnology/admin/js/
+-rw-r--r--   0 gary       (501) staff       (20)     1003 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/touchtechnology/admin/js/modal_delete.js
+-rw-r--r--   0 gary       (501) staff       (20)      357 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/touchtechnology/admin/js/resize.js
+-rw-r--r--   0 gary       (501) staff       (20)     2043 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/static/touchtechnology/admin/js/tabs.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.004496 vitriolic-3.4.0/touchtechnology/admin/templates/
+-rw-r--r--   0 gary       (501) staff       (20)      382 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/templates/403.html
+-rw-r--r--   0 gary       (501) staff       (20)      357 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/templates/404.html
+-rw-r--r--   0 gary       (501) staff       (20)      800 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/templates/40x.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.642609 vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.008863 vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/
+-rw-r--r--   0 gary       (501) staff       (20)       14 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/_version.html
+-rw-r--r--   0 gary       (501) staff       (20)     7240 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/base.html
+-rw-r--r--   0 gary       (501) staff       (20)     3967 2019-12-07 04:40:37.000000 vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/edit.html
+-rw-r--r--   0 gary       (501) staff       (20)      420 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/edit.multiple.html
+-rw-r--r--   0 gary       (501) staff       (20)      379 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/edit.related.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.009293 vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/group/
+-rw-r--r--   0 gary       (501) staff       (20)     1203 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/group/list.inc.html
+-rw-r--r--   0 gary       (501) staff       (20)      178 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/index.html
+-rw-r--r--   0 gary       (501) staff       (20)      865 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/list.html
+-rw-r--r--   0 gary       (501) staff       (20)     2438 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/permissions.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.009809 vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/settings/
+-rw-r--r--   0 gary       (501) staff       (20)      311 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/settings/index.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.010258 vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/user/
+-rw-r--r--   0 gary       (501) staff       (20)     1428 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/user/list.inc.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.011514 vitriolic-3.4.0/touchtechnology/admin/templatetags/
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/templatetags/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)     1977 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/templatetags/admin.py
+-rw-r--r--   0 gary       (501) staff       (20)     5261 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/templatetags/mvp_tags.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.013800 vitriolic-3.4.0/touchtechnology/admin/tests/
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/tests/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)     3642 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/tests/test_auth_site.py
+-rw-r--r--   0 gary       (501) staff       (20)      485 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/tests/test_authentication.py
+-rw-r--r--   0 gary       (501) staff       (20)     1453 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/admin/tests/test_mptt_order.py
+-rw-r--r--   0 gary       (501) staff       (20)     1576 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/admin/tests/test_mvp_tags.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.026474 vitriolic-3.4.0/touchtechnology/common/
+-rw-r--r--   0 gary       (501) staff       (20)      181 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/__init__.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.028370 vitriolic-3.4.0/touchtechnology/common/backends/
+-rw-r--r--   0 gary       (501) staff       (20)      157 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/backends/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)     1294 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/backends/auth.py
+-rw-r--r--   0 gary       (501) staff       (20)     2861 2024-04-13 04:07:40.000000 vitriolic-3.4.0/touchtechnology/common/backends/cache.py
+-rw-r--r--   0 gary       (501) staff       (20)      499 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/context_processors.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.029507 vitriolic-3.4.0/touchtechnology/common/db/
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/db/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)     7030 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/db/models.py
+-rw-r--r--   0 gary       (501) staff       (20)     2020 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/debugging.py
+-rw-r--r--   0 gary       (501) staff       (20)     1626 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/decorators.py
+-rw-r--r--   0 gary       (501) staff       (20)      947 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/default_settings.py
+-rw-r--r--   0 gary       (501) staff       (20)       82 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/exceptions.py
+-rw-r--r--   0 gary       (501) staff       (20)      728 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/fields.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.033628 vitriolic-3.4.0/touchtechnology/common/forms/
+-rw-r--r--   0 gary       (501) staff       (20)      640 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/forms/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)     7475 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/forms/auth.py
+-rw-r--r--   0 gary       (501) staff       (20)     9664 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/forms/fields.py
+-rw-r--r--   0 gary       (501) staff       (20)     1446 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/forms/iter.py
+-rw-r--r--   0 gary       (501) staff       (20)     3763 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/forms/mixins.py
+-rw-r--r--   0 gary       (501) staff       (20)     2401 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/forms/tz.py
+-rw-r--r--   0 gary       (501) staff       (20)     8100 2024-04-13 04:07:44.000000 vitriolic-3.4.0/touchtechnology/common/forms/widgets.py
+-rw-r--r--   0 gary       (501) staff       (20)     1468 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/forms_lazy.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.645663 vitriolic-3.4.0/touchtechnology/common/locale/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.644924 vitriolic-3.4.0/touchtechnology/common/locale/de/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.034934 vitriolic-3.4.0/touchtechnology/common/locale/de/LC_MESSAGES/
+-rw-r--r--   0 gary       (501) staff       (20)      420 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/common/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 gary       (501) staff       (20)     9606 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/common/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.645207 vitriolic-3.4.0/touchtechnology/common/locale/en-AU/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.036214 vitriolic-3.4.0/touchtechnology/common/locale/en-AU/LC_MESSAGES/
+-rw-r--r--   0 gary       (501) staff       (20)      378 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/common/locale/en-AU/LC_MESSAGES/django.mo
+-rw-r--r--   0 gary       (501) staff       (20)     9560 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/common/locale/en-AU/LC_MESSAGES/django.po
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.645479 vitriolic-3.4.0/touchtechnology/common/locale/fr/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.037511 vitriolic-3.4.0/touchtechnology/common/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 gary       (501) staff       (20)     9033 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/common/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 gary       (501) staff       (20)    14080 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/common/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.645778 vitriolic-3.4.0/touchtechnology/common/locale/ja/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.038893 vitriolic-3.4.0/touchtechnology/common/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 gary       (501) staff       (20)      413 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/common/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 gary       (501) staff       (20)     9599 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/common/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0 gary       (501) staff       (20)     1898 2019-10-31 21:17:24.000000 vitriolic-3.4.0/touchtechnology/common/middleware.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.042338 vitriolic-3.4.0/touchtechnology/common/migrations/
+-rw-r--r--   0 gary       (501) staff       (20)     5737 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/migrations/0001_initial.py
+-rw-r--r--   0 gary       (501) staff       (20)      556 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/migrations/0002_sitemapnode_last_modified.py
+-rw-r--r--   0 gary       (501) staff       (20)      485 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/migrations/0003_drop_pythonpackage.py
+-rw-r--r--   0 gary       (501) staff       (20)      518 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/migrations/0004_sitemapnode_kwargs.py
+-rw-r--r--   0 gary       (501) staff       (20)      742 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/migrations/0005_sitemapnode_populate_kwargs.py
+-rw-r--r--   0 gary       (501) staff       (20)     2763 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/migrations/0006_model_definition_sync.py
+-rw-r--r--   0 gary       (501) staff       (20)      896 2023-05-21 21:21:54.000000 vitriolic-3.4.0/touchtechnology/common/migrations/0007_auto_20220808_1144.py
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/migrations/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)     1826 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/mixins.py
+-rw-r--r--   0 gary       (501) staff       (20)     7578 2022-08-10 12:47:18.000000 vitriolic-3.4.0/touchtechnology/common/models.py
+-rw-r--r--   0 gary       (501) staff       (20)     1902 2022-07-03 21:48:02.000000 vitriolic-3.4.0/touchtechnology/common/prince.py
+-rw-r--r--   0 gary       (501) staff       (20)     1157 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/routers.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.042705 vitriolic-3.4.0/touchtechnology/common/shim/
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/shim/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)     1472 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/sitemaps.py
+-rw-r--r--   0 gary       (501) staff       (20)    39360 2024-04-14 00:51:21.000000 vitriolic-3.4.0/touchtechnology/common/sites.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.043022 vitriolic-3.4.0/touchtechnology/common/static/
+-rw-r--r--   0 gary       (501) staff       (20)     3510 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/static/sitemap.xsl
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.646585 vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.647263 vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.043460 vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/css/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.048278 vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/css/froala_themes/
+-rw-r--r--   0 gary       (501) staff       (20)    29097 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/css/froala_themes/dark.css
+-rw-r--r--   0 gary       (501) staff       (20)    25448 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/css/froala_themes/dark.min.css
+-rw-r--r--   0 gary       (501) staff       (20)    29096 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/css/froala_themes/gray.css
+-rw-r--r--   0 gary       (501) staff       (20)    25546 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/css/froala_themes/gray.min.css
+-rw-r--r--   0 gary       (501) staff       (20)    25675 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/css/froala_themes/red.css
+-rw-r--r--   0 gary       (501) staff       (20)    22607 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/css/froala_themes/red.min.css
+-rw-r--r--   0 gary       (501) staff       (20)    29287 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/css/froala_themes/royal.css
+-rw-r--r--   0 gary       (501) staff       (20)    25735 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/css/froala_themes/royal.min.css
+-rw-r--r--   0 gary       (501) staff       (20)       56 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/css/location_widget.css
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.049225 vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/js/
+-rw-r--r--   0 gary       (501) staff       (20)      466 2024-03-27 20:05:17.000000 vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/js/froala.js
+-rw-r--r--   0 gary       (501) staff       (20)     3139 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/js/location_widget.js
+-rw-r--r--   0 gary       (501) staff       (20)     5244 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/storage.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.051685 vitriolic-3.4.0/touchtechnology/common/templates/
+-rw-r--r--   0 gary       (501) staff       (20)      248 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/templates/404.html
+-rw-r--r--   0 gary       (501) staff       (20)      345 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/templates/500.html
+-rw-r--r--   0 gary       (501) staff       (20)     2924 2023-05-21 02:08:30.000000 vitriolic-3.4.0/touchtechnology/common/templates/base.html
+-rw-r--r--   0 gary       (501) staff       (20)      284 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/templates/http4xx.html
+-rw-r--r--   0 gary       (501) staff       (20)      157 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/templates/http5xx.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.053384 vitriolic-3.4.0/touchtechnology/common/templates/mvp/
+-rw-r--r--   0 gary       (501) staff       (20)       23 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/templates/mvp/list.html
+-rw-r--r--   0 gary       (501) staff       (20)     4959 2022-08-17 11:43:30.000000 vitriolic-3.4.0/touchtechnology/common/templates/mvp/list.inc.html
+-rw-r--r--   0 gary       (501) staff       (20)      455 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/templates/mvp/list.split.inc.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.058131 vitriolic-3.4.0/touchtechnology/common/templates/registration/
+-rw-r--r--   0 gary       (501) staff       (20)       94 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/templates/registration/base.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.058444 vitriolic-3.4.0/touchtechnology/common/templates/registration/email/
+-rw-r--r--   0 gary       (501) staff       (20)      438 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/templates/registration/email/_base.html
+-rw-r--r--   0 gary       (501) staff       (20)      403 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/templates/registration/logged_out.html
+-rw-r--r--   0 gary       (501) staff       (20)     1338 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/templates/registration/login.html
+-rw-r--r--   0 gary       (501) staff       (20)      572 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/templates/registration/password_change_done.html
+-rw-r--r--   0 gary       (501) staff       (20)      863 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/templates/registration/password_change_form.html
+-rw-r--r--   0 gary       (501) staff       (20)      434 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/templates/registration/password_reset_complete.html
+-rw-r--r--   0 gary       (501) staff       (20)      836 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/templates/registration/password_reset_confirm.html
+-rw-r--r--   0 gary       (501) staff       (20)      331 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/templates/registration/password_reset_done.html
+-rw-r--r--   0 gary       (501) staff       (20)      596 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/templates/registration/password_reset_email.html
+-rw-r--r--   0 gary       (501) staff       (20)      587 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/templates/registration/password_reset_form.html
+-rw-r--r--   0 gary       (501) staff       (20)     1285 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/templates/registration/profile.html
+-rw-r--r--   0 gary       (501) staff       (20)      562 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/templates/sitemap.xml
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.648551 vitriolic-3.4.0/touchtechnology/common/templates/touchtechnology/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.058753 vitriolic-3.4.0/touchtechnology/common/templates/touchtechnology/common/
+-rw-r--r--   0 gary       (501) staff       (20)      250 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/templates/touchtechnology/common/index.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.062137 vitriolic-3.4.0/touchtechnology/common/templates/touchtechnology/common/templatetags/
+-rw-r--r--   0 gary       (501) staff       (20)      877 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/templates/touchtechnology/common/templatetags/analytics.html
+-rw-r--r--   0 gary       (501) staff       (20)      108 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/templates/touchtechnology/common/templatetags/context.html
+-rw-r--r--   0 gary       (501) staff       (20)      593 2021-09-19 12:54:55.000000 vitriolic-3.4.0/touchtechnology/common/templates/touchtechnology/common/templatetags/field.html
+-rw-r--r--   0 gary       (501) staff       (20)      162 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/templates/touchtechnology/common/templatetags/hostname.html
+-rw-r--r--   0 gary       (501) staff       (20)     1217 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/templates/touchtechnology/common/templatetags/navigation.html
+-rw-r--r--   0 gary       (501) staff       (20)      705 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/templates/touchtechnology/common/templatetags/pagination.html
+-rw-r--r--   0 gary       (501) staff       (20)      124 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/templates/touchtechnology/common/templatetags/price.html
+-rw-r--r--   0 gary       (501) staff       (20)      771 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/templates/touchtechnology/common/templatetags/version.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.062687 vitriolic-3.4.0/touchtechnology/common/templates/touchtechnology/twitter/
+-rw-r--r--   0 gary       (501) staff       (20)      484 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/templates/touchtechnology/twitter/latest_tweets.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.063846 vitriolic-3.4.0/touchtechnology/common/templatetags/
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/templatetags/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)    16163 2024-04-14 00:51:21.000000 vitriolic-3.4.0/touchtechnology/common/templatetags/common.py
+-rw-r--r--   0 gary       (501) staff       (20)      304 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/templatetags/dashboard.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.069721 vitriolic-3.4.0/touchtechnology/common/tests/
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/tests/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)      839 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/tests/factories.py
+-rw-r--r--   0 gary       (501) staff       (20)      247 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/tests/test_appcache.py
+-rw-r--r--   0 gary       (501) staff       (20)     5856 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/tests/test_authentication.py
+-rw-r--r--   0 gary       (501) staff       (20)     2796 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/tests/test_fields.py
+-rw-r--r--   0 gary       (501) staff       (20)     6609 2023-05-21 21:14:55.000000 vitriolic-3.4.0/touchtechnology/common/tests/test_forms.py
+-rw-r--r--   0 gary       (501) staff       (20)     7871 2019-11-18 20:58:58.000000 vitriolic-3.4.0/touchtechnology/common/tests/test_generic_views.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.070492 vitriolic-3.4.0/touchtechnology/common/tests/test_html/
+-rw-r--r--   0 gary       (501) staff       (20)     5553 2023-05-21 21:14:55.000000 vitriolic-3.4.0/touchtechnology/common/tests/test_html/select_date_time_field_initial.html
+-rw-r--r--   0 gary       (501) staff       (20)    45496 2023-05-21 21:14:55.000000 vitriolic-3.4.0/touchtechnology/common/tests/test_html/select_date_time_field_initial_tz.html
+-rw-r--r--   0 gary       (501) staff       (20)      355 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/tests/test_models.py
+-rw-r--r--   0 gary       (501) staff       (20)      991 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/tests/test_pagination.py
+-rw-r--r--   0 gary       (501) staff       (20)      135 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/tests/test_sitemaps.py
+-rw-r--r--   0 gary       (501) staff       (20)     2624 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/tests/test_storage.py
+-rw-r--r--   0 gary       (501) staff       (20)     7771 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/tests/test_templates.py
+-rw-r--r--   0 gary       (501) staff       (20)     3132 2023-05-21 21:14:55.000000 vitriolic-3.4.0/touchtechnology/common/tests/test_timezone.py
+-rw-r--r--   0 gary       (501) staff       (20)      600 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/common/tests/test_timezone_forms.py
+-rw-r--r--   0 gary       (501) staff       (20)     3053 2023-05-21 21:14:55.000000 vitriolic-3.4.0/touchtechnology/common/tests/test_utils.py
+-rw-r--r--   0 gary       (501) staff       (20)      280 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/urls.py
+-rw-r--r--   0 gary       (501) staff       (20)     8156 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/utils.py
+-rw-r--r--   0 gary       (501) staff       (20)     1424 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/common/views.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.077203 vitriolic-3.4.0/touchtechnology/content/
+-rw-r--r--   0 gary       (501) staff       (20)       66 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)    22525 2023-02-16 20:24:29.000000 vitriolic-3.4.0/touchtechnology/content/admin.py
+-rw-r--r--   0 gary       (501) staff       (20)     1058 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/app_settings.py
+-rw-r--r--   0 gary       (501) staff       (20)      563 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/content/apps.py
+-rw-r--r--   0 gary       (501) staff       (20)     9447 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/content/forms.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.650986 vitriolic-3.4.0/touchtechnology/content/locale/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.649950 vitriolic-3.4.0/touchtechnology/content/locale/de/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.078540 vitriolic-3.4.0/touchtechnology/content/locale/de/LC_MESSAGES/
+-rw-r--r--   0 gary       (501) staff       (20)      420 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/content/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 gary       (501) staff       (20)     8711 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/content/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.650484 vitriolic-3.4.0/touchtechnology/content/locale/en-AU/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.079509 vitriolic-3.4.0/touchtechnology/content/locale/en-AU/LC_MESSAGES/
+-rw-r--r--   0 gary       (501) staff       (20)      378 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/content/locale/en-AU/LC_MESSAGES/django.mo
+-rw-r--r--   0 gary       (501) staff       (20)     8665 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/content/locale/en-AU/LC_MESSAGES/django.po
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.650818 vitriolic-3.4.0/touchtechnology/content/locale/fr/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.080645 vitriolic-3.4.0/touchtechnology/content/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 gary       (501) staff       (20)      419 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/content/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 gary       (501) staff       (20)     8710 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/content/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.651100 vitriolic-3.4.0/touchtechnology/content/locale/ja/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.081619 vitriolic-3.4.0/touchtechnology/content/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 gary       (501) staff       (20)      413 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/content/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 gary       (501) staff       (20)     8704 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/content/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0 gary       (501) staff       (20)    10324 2022-07-02 05:36:58.000000 vitriolic-3.4.0/touchtechnology/content/middleware.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.084321 vitriolic-3.4.0/touchtechnology/content/migrations/
+-rw-r--r--   0 gary       (501) staff       (20)     9038 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/content/migrations/0001_initial.py
+-rw-r--r--   0 gary       (501) staff       (20)      803 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/migrations/0002_last_modified.py
+-rw-r--r--   0 gary       (501) staff       (20)      597 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/migrations/0003_auto_20160831_0608.py
+-rw-r--r--   0 gary       (501) staff       (20)      692 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/migrations/0004_remove_placeholderkeywordargument.py
+-rw-r--r--   0 gary       (501) staff       (20)     1104 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/migrations/0005_model_definition_sync.py
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/migrations/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)     6999 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/content/models.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.651538 vitriolic-3.4.0/touchtechnology/content/static/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.652118 vitriolic-3.4.0/touchtechnology/content/static/touchtechnology/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.651930 vitriolic-3.4.0/touchtechnology/content/static/touchtechnology/admin/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.084751 vitriolic-3.4.0/touchtechnology/content/static/touchtechnology/admin/css/
+-rw-r--r--   0 gary       (501) staff       (20)      195 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/static/touchtechnology/admin/css/content.css
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.085332 vitriolic-3.4.0/touchtechnology/content/static/touchtechnology/admin/js/
+-rw-r--r--   0 gary       (501) staff       (20)     1535 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/static/touchtechnology/admin/js/files.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.652321 vitriolic-3.4.0/touchtechnology/content/static/touchtechnology/content/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.085956 vitriolic-3.4.0/touchtechnology/content/static/touchtechnology/content/css/
+-rw-r--r--   0 gary       (501) staff       (20)       33 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/static/touchtechnology/content/css/vi_admin.css
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.652632 vitriolic-3.4.0/touchtechnology/content/templates/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.652750 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.088466 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.092719 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/
+-rw-r--r--   0 gary       (501) staff       (20)      601 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/base.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.093266 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/chunk/
+-rw-r--r--   0 gary       (501) staff       (20)       88 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/chunk/edit.html
+-rw-r--r--   0 gary       (501) staff       (20)       58 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/delete.html
+-rw-r--r--   0 gary       (501) staff       (20)     1277 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/delete_confirm.html
+-rw-r--r--   0 gary       (501) staff       (20)      150 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/edit.html
+-rw-r--r--   0 gary       (501) staff       (20)      158 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/edit.related.html
+-rw-r--r--   0 gary       (501) staff       (20)     1594 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/edit_application.html
+-rw-r--r--   0 gary       (501) staff       (20)      128 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/edit_folder.html
+-rw-r--r--   0 gary       (501) staff       (20)     1237 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/edit_page.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.095023 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/file/
+-rw-r--r--   0 gary       (501) staff       (20)      203 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/file/delete_confirm.html
+-rw-r--r--   0 gary       (501) staff       (20)      709 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/file/list.html
+-rw-r--r--   0 gary       (501) staff       (20)     4886 2021-10-25 00:59:28.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/file/list.inc.html
+-rw-r--r--   0 gary       (501) staff       (20)     2829 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/files.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.095695 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/folder/
+-rw-r--r--   0 gary       (501) staff       (20)      145 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/folder/delete_confirm.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.096219 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/placeholder/
+-rw-r--r--   0 gary       (501) staff       (20)     1080 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/placeholder/list.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.097245 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/redirect/
+-rw-r--r--   0 gary       (501) staff       (20)       88 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/redirect/edit.html
+-rw-r--r--   0 gary       (501) staff       (20)      597 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/redirect/list.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.098280 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/sitemapnode/
+-rw-r--r--   0 gary       (501) staff       (20)     1080 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/sitemapnode/list.html
+-rw-r--r--   0 gary       (501) staff       (20)     1801 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/sitemapnode/list.inc.html
+-rw-r--r--   0 gary       (501) staff       (20)      151 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/base.html
+-rw-r--r--   0 gary       (501) staff       (20)      253 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/folder.html
+-rw-r--r--   0 gary       (501) staff       (20)      401 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/folder.nav.html
+-rw-r--r--   0 gary       (501) staff       (20)      288 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/page.html
+-rw-r--r--   0 gary       (501) staff       (20)      479 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/page_content.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.099236 vitriolic-3.4.0/touchtechnology/content/templatetags/
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/templatetags/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)      407 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/content/templatetags/content.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.103152 vitriolic-3.4.0/touchtechnology/content/tests/
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/tests/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)      292 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/content/tests/factories.py
+-rw-r--r--   0 gary       (501) staff       (20)     3787 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/content/tests/test_admin.py
+-rw-r--r--   0 gary       (501) staff       (20)     2818 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/content/utils.py
+-rw-r--r--   0 gary       (501) staff       (20)     2243 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/content/views.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.110843 vitriolic-3.4.0/touchtechnology/news/
+-rw-r--r--   0 gary       (501) staff       (20)       91 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)     6281 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/admin.py
+-rw-r--r--   0 gary       (501) staff       (20)      928 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/app_settings.py
+-rw-r--r--   0 gary       (501) staff       (20)      283 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/apps.py
+-rw-r--r--   0 gary       (501) staff       (20)     2561 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/decorators.py
+-rw-r--r--   0 gary       (501) staff       (20)     1631 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/forms.py
+-rw-r--r--   0 gary       (501) staff       (20)      257 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/news/image_processors.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.656030 vitriolic-3.4.0/touchtechnology/news/locale/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.655149 vitriolic-3.4.0/touchtechnology/news/locale/de/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.111739 vitriolic-3.4.0/touchtechnology/news/locale/de/LC_MESSAGES/
+-rw-r--r--   0 gary       (501) staff       (20)      420 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/news/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 gary       (501) staff       (20)     4168 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/news/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.655491 vitriolic-3.4.0/touchtechnology/news/locale/en-AU/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.112718 vitriolic-3.4.0/touchtechnology/news/locale/en-AU/LC_MESSAGES/
+-rw-r--r--   0 gary       (501) staff       (20)      378 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/news/locale/en-AU/LC_MESSAGES/django.mo
+-rw-r--r--   0 gary       (501) staff       (20)     4122 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/news/locale/en-AU/LC_MESSAGES/django.po
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.655855 vitriolic-3.4.0/touchtechnology/news/locale/fr/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.113528 vitriolic-3.4.0/touchtechnology/news/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 gary       (501) staff       (20)      419 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/news/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 gary       (501) staff       (20)     4167 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/news/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.656147 vitriolic-3.4.0/touchtechnology/news/locale/ja/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.114569 vitriolic-3.4.0/touchtechnology/news/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 gary       (501) staff       (20)      378 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/news/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 gary       (501) staff       (20)     4122 2019-11-09 20:04:29.000000 vitriolic-3.4.0/touchtechnology/news/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.118390 vitriolic-3.4.0/touchtechnology/news/migrations/
+-rw-r--r--   0 gary       (501) staff       (20)     5408 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/migrations/0001_initial.py
+-rw-r--r--   0 gary       (501) staff       (20)      627 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/migrations/0002_article_last_modified.py
+-rw-r--r--   0 gary       (501) staff       (20)      642 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/migrations/0003_category_last_modified.py
+-rw-r--r--   0 gary       (501) staff       (20)     2365 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/migrations/0004_model_definition_sync.py
+-rw-r--r--   0 gary       (501) staff       (20)      428 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/migrations/0005_auto_20191122_1340.py
+-rw-r--r--   0 gary       (501) staff       (20)      438 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/migrations/0006_article_copy_field.py
+-rw-r--r--   0 gary       (501) staff       (20)      679 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/migrations/0007_article_copy_field_data.py
+-rw-r--r--   0 gary       (501) staff       (20)      234 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/migrations/0008_delete_articlecontent.py
+-rw-r--r--   0 gary       (501) staff       (20)     1569 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/migrations/0009_translation.py
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/news/migrations/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)     5369 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/models.py
+-rw-r--r--   0 gary       (501) staff       (20)      367 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/news/query.py
+-rw-r--r--   0 gary       (501) staff       (20)     6316 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/sites.py
+-rw-r--r--   0 gary       (501) staff       (20)     1723 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/syndication.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.656584 vitriolic-3.4.0/touchtechnology/news/templates/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.656700 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.120303 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/
+-rw-r--r--   0 gary       (501) staff       (20)      977 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/_latest_articles.html
+-rw-r--r--   0 gary       (501) staff       (20)      959 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/_related_list.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.657320 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/admin/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.120824 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/admin/article/
+-rw-r--r--   0 gary       (501) staff       (20)     1048 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/admin/article/list.inc.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.121304 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/admin/category/
+-rw-r--r--   0 gary       (501) staff       (20)      464 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/admin/category/list.inc.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.121707 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/admin/translation/
+-rw-r--r--   0 gary       (501) staff       (20)      891 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/admin/translation/list.inc.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.124487 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/archive/
+-rw-r--r--   0 gary       (501) staff       (20)      410 2019-12-16 12:53:13.000000 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/archive/_article_list.html
+-rw-r--r--   0 gary       (501) staff       (20)      241 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/archive/base.html
+-rw-r--r--   0 gary       (501) staff       (20)      276 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/archive/day.html
+-rw-r--r--   0 gary       (501) staff       (20)      572 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/archive/index.html
+-rw-r--r--   0 gary       (501) staff       (20)      274 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/archive/month.html
+-rw-r--r--   0 gary       (501) staff       (20)      425 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/archive/year.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.125584 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/article/
+-rw-r--r--   0 gary       (501) staff       (20)     1741 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/article/detail.html
+-rw-r--r--   0 gary       (501) staff       (20)     1170 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/article/list.html
+-rw-r--r--   0 gary       (501) staff       (20)      205 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/base.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.126799 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/feeds/
+-rw-r--r--   0 gary       (501) staff       (20)       24 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/feeds/description.html
+-rw-r--r--   0 gary       (501) staff       (20)       24 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/feeds/title.html
+-rw-r--r--   0 gary       (501) staff       (20)      607 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/feeds.html
+-rw-r--r--   0 gary       (501) staff       (20)      264 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/index.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.127354 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/translation/
+-rw-r--r--   0 gary       (501) staff       (20)      360 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/translation/detail.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.128360 vitriolic-3.4.0/touchtechnology/news/templatetags/
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/news/templatetags/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)     1864 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/templatetags/news.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.130264 vitriolic-3.4.0/touchtechnology/news/tests/
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/touchtechnology/news/tests/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)      982 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/tests/factories.py
+-rw-r--r--   0 gary       (501) staff       (20)     2557 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/tests/test_admin.py
+-rw-r--r--   0 gary       (501) staff       (20)     3442 2022-06-12 11:19:40.000000 vitriolic-3.4.0/touchtechnology/news/tests/test_site.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.131269 vitriolic-3.4.0/tournamentcontrol/
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/__init__.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.154575 vitriolic-3.4.0/tournamentcontrol/competition/
+-rw-r--r--   0 gary       (501) staff       (20)      366 2019-11-19 06:59:00.000000 vitriolic-3.4.0/tournamentcontrol/competition/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)    83489 2024-05-17 23:16:24.000000 vitriolic-3.4.0/tournamentcontrol/competition/admin.py
+-rw-r--r--   0 gary       (501) staff       (20)     2796 2023-02-16 20:24:29.000000 vitriolic-3.4.0/tournamentcontrol/competition/apps.py
+-rw-r--r--   0 gary       (501) staff       (20)     4268 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/calc.py
+-rw-r--r--   0 gary       (501) staff       (20)     1361 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/constants.py
+-rw-r--r--   0 gary       (501) staff       (20)    10746 2023-07-23 01:57:06.000000 vitriolic-3.4.0/tournamentcontrol/competition/dashboard.py
+-rw-r--r--   0 gary       (501) staff       (20)    12977 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/decorators.py
+-rw-r--r--   0 gary       (501) staff       (20)    18643 2024-05-17 23:16:24.000000 vitriolic-3.4.0/tournamentcontrol/competition/draw.py
+-rw-r--r--   0 gary       (501) staff       (20)      269 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/fields.py
+-rw-r--r--   0 gary       (501) staff       (20)    71293 2024-05-17 23:16:24.000000 vitriolic-3.4.0/tournamentcontrol/competition/forms.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.659802 vitriolic-3.4.0/tournamentcontrol/competition/locale/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.658995 vitriolic-3.4.0/tournamentcontrol/competition/locale/de/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.155912 vitriolic-3.4.0/tournamentcontrol/competition/locale/de/LC_MESSAGES/
+-rw-r--r--   0 gary       (501) staff       (20)      421 2019-11-09 20:04:29.000000 vitriolic-3.4.0/tournamentcontrol/competition/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 gary       (501) staff       (20)    63237 2019-11-09 20:04:29.000000 vitriolic-3.4.0/tournamentcontrol/competition/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.659285 vitriolic-3.4.0/tournamentcontrol/competition/locale/en-AU/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.156958 vitriolic-3.4.0/tournamentcontrol/competition/locale/en-AU/LC_MESSAGES/
+-rw-r--r--   0 gary       (501) staff       (20)      429 2019-11-09 20:04:29.000000 vitriolic-3.4.0/tournamentcontrol/competition/locale/en-AU/LC_MESSAGES/django.mo
+-rw-r--r--   0 gary       (501) staff       (20)    63245 2019-11-09 20:04:29.000000 vitriolic-3.4.0/tournamentcontrol/competition/locale/en-AU/LC_MESSAGES/django.po
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.659602 vitriolic-3.4.0/tournamentcontrol/competition/locale/fr/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.158107 vitriolic-3.4.0/tournamentcontrol/competition/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 gary       (501) staff       (20)      420 2019-11-09 20:04:29.000000 vitriolic-3.4.0/tournamentcontrol/competition/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 gary       (501) staff       (20)    63236 2019-11-09 20:04:29.000000 vitriolic-3.4.0/tournamentcontrol/competition/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.659928 vitriolic-3.4.0/tournamentcontrol/competition/locale/ja/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.159251 vitriolic-3.4.0/tournamentcontrol/competition/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 gary       (501) staff       (20)      414 2019-11-09 20:04:29.000000 vitriolic-3.4.0/tournamentcontrol/competition/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 gary       (501) staff       (20)    63230 2019-11-09 20:04:29.000000 vitriolic-3.4.0/tournamentcontrol/competition/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.159726 vitriolic-3.4.0/tournamentcontrol/competition/management/
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/management/__init__.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.160339 vitriolic-3.4.0/tournamentcontrol/competition/management/commands/
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/management/commands/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)     1899 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/management/commands/produce_rank.py
+-rw-r--r--   0 gary       (501) staff       (20)      467 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/managers.py
+-rw-r--r--   0 gary       (501) staff       (20)     4705 2023-07-16 02:28:16.000000 vitriolic-3.4.0/tournamentcontrol/competition/merge.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.184780 vitriolic-3.4.0/tournamentcontrol/competition/migrations/
+-rw-r--r--   0 gary       (501) staff       (20)    52844 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0001_initial.py
+-rw-r--r--   0 gary       (501) staff       (20)      530 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0002_division_draft.py
+-rw-r--r--   0 gary       (501) staff       (20)      447 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0003_division_draft_data.py
+-rw-r--r--   0 gary       (501) staff       (20)      508 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0004_alter_person_gender.py
+-rw-r--r--   0 gary       (501) staff       (20)     1005 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0005_alter_club_facebook_youtube_position.py
+-rw-r--r--   0 gary       (501) staff       (20)      792 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0006_sportingpulse_import_fields.py
+-rw-r--r--   0 gary       (501) staff       (20)     1626 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0007_match_videos.py
+-rw-r--r--   0 gary       (501) staff       (20)     1510 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0008_nullable_statistics.py
+-rw-r--r--   0 gary       (501) staff       (20)      317 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0009_remove_byeteam.py
+-rw-r--r--   0 gary       (501) staff       (20)      697 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0010_remove_match_video_approved_by.py
+-rw-r--r--   0 gary       (501) staff       (20)      997 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0011_custom_twitter_ladderpoints_fields.py
+-rw-r--r--   0 gary       (501) staff       (20)     1455 2022-07-18 07:51:12.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0012_hashtag_include_symbol.py
+-rw-r--r--   0 gary       (501) staff       (20)      611 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0013_statistic_played_field.py
+-rw-r--r--   0 gary       (501) staff       (20)      580 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0014_match_play_at_blank.py
+-rw-r--r--   0 gary       (501) staff       (20)      693 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0015_person_user_relation.py
+-rw-r--r--   0 gary       (501) staff       (20)      653 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0016_season_forfeit_notifications.py
+-rw-r--r--   0 gary       (501) staff       (20)     5746 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0017_ranking_feature.py
+-rw-r--r--   0 gary       (501) staff       (20)    10513 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0018_resync_field_and_model_defs.py
+-rw-r--r--   0 gary       (501) staff       (20)      532 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0019_auto_20161210_0922.py
+-rw-r--r--   0 gary       (501) staff       (20)     3954 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0020_competition__add__person_uuid.py
+-rw-r--r--   0 gary       (501) staff       (20)     1146 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0021_competition__data__person_uuid.py
+-rw-r--r--   0 gary       (501) staff       (20)     4676 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0022_competition__remove__person_id.py
+-rw-r--r--   0 gary       (501) staff       (20)      533 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0023_competition__add__match_uuid.py
+-rw-r--r--   0 gary       (501) staff       (20)      679 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0023_competition__add__match_uuid_data.py
+-rw-r--r--   0 gary       (501) staff       (20)     1017 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0023_competition__add__match_uuid_finalize.py
+-rw-r--r--   0 gary       (501) staff       (20)      686 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0024_auto_20170203_0619.py
+-rw-r--r--   0 gary       (501) staff       (20)      985 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0025_matchvideo_baseline.py
+-rw-r--r--   0 gary       (501) staff       (20)      863 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0026_matchvideo.py
+-rw-r--r--   0 gary       (501) staff       (20)      644 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0027_matchvideo_data.py
+-rw-r--r--   0 gary       (501) staff       (20)      471 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0028_drop_matchvideo.py
+-rw-r--r--   0 gary       (501) staff       (20)     1748 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0029_seasonreferee.py
+-rw-r--r--   0 gary       (501) staff       (20)      848 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0030_match_referees.py
+-rw-r--r--   0 gary       (501) staff       (20)    20487 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0031_model_definition_sync.py
+-rw-r--r--   0 gary       (501) staff       (20)      957 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0032_resave_all_matches.py
+-rw-r--r--   0 gary       (501) staff       (20)     1326 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0033_matchscoresheet.py
+-rw-r--r--   0 gary       (501) staff       (20)     1529 2019-10-31 21:17:24.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0034_orderedsitemapnode_add_copy_field.py
+-rw-r--r--   0 gary       (501) staff       (20)      899 2019-11-14 06:38:25.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0035_season_disable_calendar.py
+-rw-r--r--   0 gary       (501) staff       (20)     5155 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0036_auto_20191122_1340.py
+-rw-r--r--   0 gary       (501) staff       (20)      392 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0037_alter_match_evaluated.py
+-rw-r--r--   0 gary       (501) staff       (20)      457 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0038_match_live_stream.py
+-rw-r--r--   0 gary       (501) staff       (20)      454 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0039_season_live_stream.py
+-rw-r--r--   0 gary       (501) staff       (20)      645 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0040_season_live_stream_privacy.py
+-rw-r--r--   0 gary       (501) staff       (20)      463 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0041_ground_live_stream.py
+-rw-r--r--   0 gary       (501) staff       (20)      482 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0042_ground_external_identifier.py
+-rw-r--r--   0 gary       (501) staff       (20)      492 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0043_alter_ground_external_identifier.py
+-rw-r--r--   0 gary       (501) staff       (20)      492 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0044_match_live_stream_bind.py
+-rw-r--r--   0 gary       (501) staff       (20)      477 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0045_ground_stream_key.py
+-rw-r--r--   0 gary       (501) staff       (20)      436 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0046_alter_match_live_stream_bind.py
+-rw-r--r--   0 gary       (501) staff       (20)     1648 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0047_season_live_stream_oauth2.py
+-rw-r--r--   0 gary       (501) staff       (20)      405 2023-07-16 04:15:02.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0048_season_live_stream_thumbnail.py
+-rw-r--r--   0 gary       (501) staff       (20)      419 2023-07-16 04:15:02.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/0049_match_live_stream_thumbnail.py
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/migrations/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)     1517 2019-10-31 21:17:24.000000 vitriolic-3.4.0/tournamentcontrol/competition/mixins.py
+-rw-r--r--   0 gary       (501) staff       (20)    71869 2024-05-17 14:38:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/models.py
+-rw-r--r--   0 gary       (501) staff       (20)     5029 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/query.py
+-rw-r--r--   0 gary       (501) staff       (20)    12590 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/rank.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.185650 vitriolic-3.4.0/tournamentcontrol/competition/rest/
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-31 21:17:24.000000 vitriolic-3.4.0/tournamentcontrol/competition/rest/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)      267 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/rest/urls.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.197131 vitriolic-3.4.0/tournamentcontrol/competition/rest/v1/
+-rw-r--r--   0 gary       (501) staff       (20)     1475 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/rest/v1/_247.py
+-rw-r--r--   0 gary       (501) staff       (20)       65 2019-10-31 21:17:24.000000 vitriolic-3.4.0/tournamentcontrol/competition/rest/v1/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)     3540 2022-07-17 22:00:23.000000 vitriolic-3.4.0/tournamentcontrol/competition/rest/v1/_birdi.py
+-rw-r--r--   0 gary       (501) staff       (20)     1203 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/rest/v1/_routers.py
+-rw-r--r--   0 gary       (501) staff       (20)      726 2019-10-31 21:17:24.000000 vitriolic-3.4.0/tournamentcontrol/competition/rest/v1/club.py
+-rw-r--r--   0 gary       (501) staff       (20)     1116 2019-10-31 21:17:24.000000 vitriolic-3.4.0/tournamentcontrol/competition/rest/v1/competition.py
+-rw-r--r--   0 gary       (501) staff       (20)     3309 2022-07-18 07:51:12.000000 vitriolic-3.4.0/tournamentcontrol/competition/rest/v1/division.py
+-rw-r--r--   0 gary       (501) staff       (20)     2112 2019-10-31 21:17:24.000000 vitriolic-3.4.0/tournamentcontrol/competition/rest/v1/season.py
+-rw-r--r--   0 gary       (501) staff       (20)      817 2019-10-31 21:17:24.000000 vitriolic-3.4.0/tournamentcontrol/competition/rest/v1/stage.py
+-rw-r--r--   0 gary       (501) staff       (20)      244 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/rest/v1/urls.py
+-rw-r--r--   0 gary       (501) staff       (20)      501 2019-10-31 21:17:24.000000 vitriolic-3.4.0/tournamentcontrol/competition/rest/v1/viewsets.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.206028 vitriolic-3.4.0/tournamentcontrol/competition/signals/
+-rw-r--r--   0 gary       (501) staff       (20)     1100 2023-02-16 20:24:29.000000 vitriolic-3.4.0/tournamentcontrol/competition/signals/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)       86 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/signals/custom.py
+-rw-r--r--   0 gary       (501) staff       (20)      580 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/signals/decorators.py
+-rw-r--r--   0 gary       (501) staff       (20)     6972 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/signals/ladders.py
+-rw-r--r--   0 gary       (501) staff       (20)     5204 2023-02-16 20:24:29.000000 vitriolic-3.4.0/tournamentcontrol/competition/signals/matches.py
+-rw-r--r--   0 gary       (501) staff       (20)      505 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/signals/places.py
+-rw-r--r--   0 gary       (501) staff       (20)      451 2022-07-25 12:16:49.000000 vitriolic-3.4.0/tournamentcontrol/competition/signals/teams.py
+-rw-r--r--   0 gary       (501) staff       (20)    43575 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/sites.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.663011 vitriolic-3.4.0/tournamentcontrol/competition/static/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.662088 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.211477 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/css/
+-rw-r--r--   0 gary       (501) staff       (20)     4823 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.bootstrap.css
+-rw-r--r--   0 gary       (501) staff       (20)     4216 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.bootstrap.min.css
+-rw-r--r--   0 gary       (501) staff       (20)     2924 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.foundation.css
+-rw-r--r--   0 gary       (501) staff       (20)     2580 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.foundation.min.css
+-rw-r--r--   0 gary       (501) staff       (20)    16019 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.jqueryui.css
+-rw-r--r--   0 gary       (501) staff       (20)    14069 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.jqueryui.min.css
+-rw-r--r--   0 gary       (501) staff       (20)    15423 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/css/jquery.dataTables.css
+-rw-r--r--   0 gary       (501) staff       (20)    13587 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/css/jquery.dataTables.min.css
+-rw-r--r--   0 gary       (501) staff       (20)    14229 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/css/jquery.dataTables_themeroller.css
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.213690 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/images/
+-rw-r--r--   0 gary       (501) staff       (20)      160 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/images/sort_asc.png
+-rw-r--r--   0 gary       (501) staff       (20)      148 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/images/sort_asc_disabled.png
+-rw-r--r--   0 gary       (501) staff       (20)      201 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/images/sort_both.png
+-rw-r--r--   0 gary       (501) staff       (20)      158 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/images/sort_desc.png
+-rw-r--r--   0 gary       (501) staff       (20)      146 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/images/sort_desc_disabled.png
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.217436 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/js/
+-rw-r--r--   0 gary       (501) staff       (20)     4544 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.bootstrap.js
+-rw-r--r--   0 gary       (501) staff       (20)     1960 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.bootstrap.min.js
+-rw-r--r--   0 gary       (501) staff       (20)     4331 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.foundation.js
+-rw-r--r--   0 gary       (501) staff       (20)     2090 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.foundation.min.js
+-rw-r--r--   0 gary       (501) staff       (20)     4486 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.jqueryui.js
+-rw-r--r--   0 gary       (501) staff       (20)     2647 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.jqueryui.min.js
+-rw-r--r--   0 gary       (501) staff       (20)   447282 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/js/jquery.dataTables.js
+-rw-r--r--   0 gary       (501) staff       (20)    82638 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/js/jquery.dataTables.min.js
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.662402 vitriolic-3.4.0/tournamentcontrol/competition/static/bootstrap/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.662592 vitriolic-3.4.0/tournamentcontrol/competition/static/bootstrap/dist/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.219899 vitriolic-3.4.0/tournamentcontrol/competition/static/bootstrap/dist/fonts/
+-rw-r--r--   0 gary       (501) staff       (20)    20127 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/bootstrap/dist/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 gary       (501) staff       (20)   108738 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/bootstrap/dist/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 gary       (501) staff       (20)    45404 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/bootstrap/dist/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 gary       (501) staff       (20)    23424 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/bootstrap/dist/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 gary       (501) staff       (20)    18028 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/bootstrap/dist/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.663191 vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.663690 vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.222329 vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/css/
+-rw-r--r--   0 gary       (501) staff       (20)     7410 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/css/vi_admin.css
+-rw-r--r--   0 gary       (501) staff       (20)      668 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/css/vi_grid.css
+-rw-r--r--   0 gary       (501) staff       (20)      763 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/css/vi_runsheet.css
+-rw-r--r--   0 gary       (501) staff       (20)     1176 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/css/vi_scorecards.css
+-rw-r--r--   0 gary       (501) staff       (20)      257 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/css/vi_signon.css
+-rw-r--r--   0 gary       (501) staff       (20)      393 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/css/vi_team.css
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.222723 vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/img/
+-rw-r--r--   0 gary       (501) staff       (20)      649 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/img/report.png
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.224186 vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/js/
+-rw-r--r--   0 gary       (501) staff       (20)     1542 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/js/formset.js
+-rw-r--r--   0 gary       (501) staff       (20)     1541 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/js/match_results.js
+-rw-r--r--   0 gary       (501) staff       (20)      312 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/js/team.js
+-rw-r--r--   0 gary       (501) staff       (20)     1978 2023-07-16 13:50:45.000000 vitriolic-3.4.0/tournamentcontrol/competition/tasks.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.664181 vitriolic-3.4.0/tournamentcontrol/competition/templates/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.227095 vitriolic-3.4.0/tournamentcontrol/competition/templates/competition/
+-rw-r--r--   0 gary       (501) staff       (20)      457 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/competition/rankpoints_archive.html
+-rw-r--r--   0 gary       (501) staff       (20)      533 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/competition/rankpoints_archive_day.html
+-rw-r--r--   0 gary       (501) staff       (20)       52 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/competition/rankpoints_archive_month.html
+-rw-r--r--   0 gary       (501) staff       (20)       52 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/competition/rankpoints_archive_year.html
+-rw-r--r--   0 gary       (501) staff       (20)       26 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/competition/rankpoints_base.html
+-rw-r--r--   0 gary       (501) staff       (20)      734 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/competition/rankpoints_detail.html
+-rw-r--r--   0 gary       (501) staff       (20)     1386 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/competition/rankpoints_team.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.669839 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.228157 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/calculator/
+-rw-r--r--   0 gary       (501) staff       (20)     4258 2023-02-16 20:24:29.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/calculator/index.html
+-rw-r--r--   0 gary       (501) staff       (20)      168 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/calculator/live.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.240210 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/
+-rw-r--r--   0 gary       (501) staff       (20)     1162 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/_club_opponent.html
+-rw-r--r--   0 gary       (501) staff       (20)       46 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/_match_title.txt
+-rw-r--r--   0 gary       (501) staff       (20)      192 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/_score.html
+-rw-r--r--   0 gary       (501) staff       (20)      178 2022-07-18 07:51:12.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/_stage_group_position.txt
+-rw-r--r--   0 gary       (501) staff       (20)      588 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/_team_opponent.html
+-rw-r--r--   0 gary       (501) staff       (20)       54 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/_win_lose_team.txt
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.248551 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/
+-rw-r--r--   0 gary       (501) staff       (20)      308 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/base.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.249729 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/club/
+-rw-r--r--   0 gary       (501) staff       (20)      597 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/club/edit.html
+-rw-r--r--   0 gary       (501) staff       (20)      301 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/club/list.inc.html
+-rw-r--r--   0 gary       (501) staff       (20)     1203 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/club/team.inc.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.250126 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/clubassociation/
+-rw-r--r--   0 gary       (501) staff       (20)      314 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/clubassociation/list.inc.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.250493 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/competition/
+-rw-r--r--   0 gary       (501) staff       (20)      407 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/competition/list.inc.html
+-rw-r--r--   0 gary       (501) staff       (20)       58 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/delete.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.251342 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/division/
+-rw-r--r--   0 gary       (501) staff       (20)     1952 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/division/edit.html
+-rw-r--r--   0 gary       (501) staff       (20)      740 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/division/list.inc.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.251918 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/divisionexclusiondate/
+-rw-r--r--   0 gary       (501) staff       (20)      297 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/divisionexclusiondate/list.inc.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.252981 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/draw_generation/
+-rw-r--r--   0 gary       (501) staff       (20)      495 2024-05-17 14:42:36.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/draw_generation/wizard.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.253917 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/drawformat/
+-rw-r--r--   0 gary       (501) staff       (20)      383 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/drawformat/list.inc.html
+-rw-r--r--   0 gary       (501) staff       (20)     2941 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/grid.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.254587 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/ground/
+-rw-r--r--   0 gary       (501) staff       (20)      824 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/ground/list.inc.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.255789 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/ladderentry/
+-rw-r--r--   0 gary       (501) staff       (20)      947 2019-10-31 21:17:24.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/ladderentry/list.inc.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.259908 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/
+-rw-r--r--   0 gary       (501) staff       (20)     3828 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/dates.html
+-rw-r--r--   0 gary       (501) staff       (20)      241 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/edit.html
+-rw-r--r--   0 gary       (501) staff       (20)      901 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/list.inc.html
+-rw-r--r--   0 gary       (501) staff       (20)     4076 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/schedule.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.260496 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/tournament/
+-rw-r--r--   0 gary       (501) staff       (20)      280 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/tournament/dates.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.261095 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/weekly/
+-rw-r--r--   0 gary       (501) staff       (20)       69 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/weekly/dates.html
+-rw-r--r--   0 gary       (501) staff       (20)     2636 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match_detail.html
+-rw-r--r--   0 gary       (501) staff       (20)     3976 2019-10-31 21:17:24.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match_results.html
+-rw-r--r--   0 gary       (501) staff       (20)     1420 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match_washout.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.262138 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/matchscoresheet/
+-rw-r--r--   0 gary       (501) staff       (20)      294 2019-10-31 21:17:24.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/matchscoresheet/edit.html
+-rw-r--r--   0 gary       (501) staff       (20)      383 2019-10-31 21:17:24.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/matchscoresheet/list.inc.html
+-rw-r--r--   0 gary       (501) staff       (20)      697 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/mvp.html
+-rw-r--r--   0 gary       (501) staff       (20)     2094 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/officials.html
+-rw-r--r--   0 gary       (501) staff       (20)     1391 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/officials_list.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.263506 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/person/
+-rw-r--r--   0 gary       (501) staff       (20)      597 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/person/edit.html
+-rw-r--r--   0 gary       (501) staff       (20)     1375 2019-10-31 21:17:24.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/person/list.inc.html
+-rw-r--r--   0 gary       (501) staff       (20)     2127 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/progress_matches.html
+-rw-r--r--   0 gary       (501) staff       (20)     2690 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/progress_teams.html
+-rw-r--r--   0 gary       (501) staff       (20)      731 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/reschedule.html
+-rw-r--r--   0 gary       (501) staff       (20)      380 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/runsheet.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.264775 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/scorecards/
+-rw-r--r--   0 gary       (501) staff       (20)      908 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/scorecards/report.html
+-rw-r--r--   0 gary       (501) staff       (20)      174 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/scorecards/wait.html
+-rw-r--r--   0 gary       (501) staff       (20)     3107 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/scorecards.html
+-rw-r--r--   0 gary       (501) staff       (20)     2452 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/scorers.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.266544 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season/
+-rw-r--r--   0 gary       (501) staff       (20)     4028 2024-05-17 23:16:24.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season/edit.html
+-rw-r--r--   0 gary       (501) staff       (20)     1495 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season/list.inc.html
+-rw-r--r--   0 gary       (501) staff       (20)     2303 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season/timeslots.html
+-rw-r--r--   0 gary       (501) staff       (20)     3751 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season_report.html
+-rw-r--r--   0 gary       (501) staff       (20)     1774 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season_summary.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.266997 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/seasonexclusiondate/
+-rw-r--r--   0 gary       (501) staff       (20)      297 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/seasonexclusiondate/list.inc.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.267566 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/seasonmatchtime/
+-rw-r--r--   0 gary       (501) staff       (20)      512 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/seasonmatchtime/list.inc.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.268010 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/seasonreferee/
+-rw-r--r--   0 gary       (501) staff       (20)      767 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/seasonreferee/list.inc.html
+-rw-r--r--   0 gary       (501) staff       (20)     2365 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/signon.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.268423 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/simplescorematchstatistic/
+-rw-r--r--   0 gary       (501) staff       (20)      761 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/simplescorematchstatistic/list.inc.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.269024 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/stage/
+-rw-r--r--   0 gary       (501) staff       (20)     1148 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/stage/list.inc.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.269580 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/stagegroup/
+-rw-r--r--   0 gary       (501) staff       (20)      386 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/stagegroup/list.inc.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.270164 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/team/
+-rw-r--r--   0 gary       (501) staff       (20)      906 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/team/list.inc.html
+-rw-r--r--   0 gary       (501) staff       (20)     1642 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/team_members.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.270757 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/teamassociation/
+-rw-r--r--   0 gary       (501) staff       (20)      540 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/teamassociation/list.inc.html
+-rw-r--r--   0 gary       (501) staff       (20)      222 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/wait.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.271964 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.272639 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/progress/
+-rw-r--r--   0 gary       (501) staff       (20)     1130 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/progress/stages.html
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/reports.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.273833 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/results/
+-rw-r--r--   0 gary       (501) staff       (20)     1135 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/results/basic.html
+-rw-r--r--   0 gary       (501) staff       (20)     1830 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/results/detailed.html
+-rw-r--r--   0 gary       (501) staff       (20)     1194 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/scoresheets.html
+-rw-r--r--   0 gary       (501) staff       (20)      661 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/base.html
+-rw-r--r--   0 gary       (501) staff       (20)     4328 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/club.html
+-rw-r--r--   0 gary       (501) staff       (20)      390 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/compare.html
+-rw-r--r--   0 gary       (501) staff       (20)     1198 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/competition.html
+-rw-r--r--   0 gary       (501) staff       (20)     5419 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/division.html
+-rw-r--r--   0 gary       (501) staff       (20)      301 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/divisiongroup.html
+-rw-r--r--   0 gary       (501) staff       (20)      272 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/draw.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.276143 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/draw_format/
+-rw-r--r--   0 gary       (501) staff       (20)      698 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/draw_format/16.txt
+-rw-r--r--   0 gary       (501) staff       (20)       78 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/draw_format/4.txt
+-rw-r--r--   0 gary       (501) staff       (20)      139 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/draw_format/6.txt
+-rw-r--r--   0 gary       (501) staff       (20)      341 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/draw_format/8.txt
+-rw-r--r--   0 gary       (501) staff       (20)     1055 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/forfeit.html
+-rw-r--r--   0 gary       (501) staff       (20)     1444 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/forfeit_list.html
+-rw-r--r--   0 gary       (501) staff       (20)      867 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/index.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.277474 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/ladder/
+-rw-r--r--   0 gary       (501) staff       (20)     4161 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/ladder/pool.html
+-rw-r--r--   0 gary       (501) staff       (20)     3015 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/ladder/standard.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:07.669494 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/match/
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.278632 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/match/live_stream/
+-rw-r--r--   0 gary       (501) staff       (20)        0 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/match/live_stream/description.txt
+-rw-r--r--   0 gary       (501) staff       (20)        0 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/match/live_stream/title.txt
+-rw-r--r--   0 gary       (501) staff       (20)     2276 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/match.html
+-rw-r--r--   0 gary       (501) staff       (20)     2214 2020-03-02 19:23:34.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/match_detail.html
+-rw-r--r--   0 gary       (501) staff       (20)     3284 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/next_date.html
+-rw-r--r--   0 gary       (501) staff       (20)     1678 2022-06-12 11:19:15.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/results.html
+-rw-r--r--   0 gary       (501) staff       (20)     4005 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/runsheet.html
+-rw-r--r--   0 gary       (501) staff       (20)      360 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/runsheet_list.html
+-rw-r--r--   0 gary       (501) staff       (20)     2877 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/season.html
+-rw-r--r--   0 gary       (501) staff       (20)     3212 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/season_videos.html
+-rw-r--r--   0 gary       (501) staff       (20)     4619 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/stage.html
+-rw-r--r--   0 gary       (501) staff       (20)     1274 2023-05-21 21:21:54.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/stream.html
+-rw-r--r--   0 gary       (501) staff       (20)     4483 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/team.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.279423 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/templatetags/
+-rw-r--r--   0 gary       (501) staff       (20)      702 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/templatetags/preview.html
+-rw-r--r--   0 gary       (501) staff       (20)      704 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/templatetags/statistics.html
+-rw-r--r--   0 gary       (501) staff       (20)      369 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/videos.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.284004 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/
+-rw-r--r--   0 gary       (501) staff       (20)      418 2019-12-17 12:14:26.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/_base.html
+-rw-r--r--   0 gary       (501) staff       (20)     2841 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/_registration_form.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.284400 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/admin/
+-rw-r--r--   0 gary       (501) staff       (20)       62 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/admin/base.html
+-rw-r--r--   0 gary       (501) staff       (20)       50 2019-12-17 12:14:30.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/base.html
+-rw-r--r--   0 gary       (501) staff       (20)      588 2019-12-17 12:14:06.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/club_members.html
+-rw-r--r--   0 gary       (501) staff       (20)      774 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/club_teams.html
+-rw-r--r--   0 gary       (501) staff       (20)       96 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/delete.html
+-rw-r--r--   0 gary       (501) staff       (20)      752 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/index.html
+-rw-r--r--   0 gary       (501) staff       (20)      559 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/officials.html
+-rw-r--r--   0 gary       (501) staff       (20)      564 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/officials_list.html
+-rw-r--r--   0 gary       (501) staff       (20)       63 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/registration_form.html
+-rw-r--r--   0 gary       (501) staff       (20)     1471 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/team_members.html
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.285156 vitriolic-3.4.0/tournamentcontrol/competition/templatetags/
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/templatetags/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)     7703 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/templatetags/competition.py
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.290861 vitriolic-3.4.0/tournamentcontrol/competition/tests/
+-rw-r--r--   0 gary       (501) staff       (20)        0 2019-10-18 22:04:04.000000 vitriolic-3.4.0/tournamentcontrol/competition/tests/__init__.py
+-rw-r--r--   0 gary       (501) staff       (20)     6820 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/tests/factories.py
+-rw-r--r--   0 gary       (501) staff       (20)    38099 2024-04-14 00:51:21.000000 vitriolic-3.4.0/tournamentcontrol/competition/tests/test_competition_admin.py
+-rw-r--r--   0 gary       (501) staff       (20)    11889 2022-07-02 05:40:48.000000 vitriolic-3.4.0/tournamentcontrol/competition/tests/test_competition_site.py
+-rw-r--r--   0 gary       (501) staff       (20)     1837 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/tests/test_dashboard.py
+-rw-r--r--   0 gary       (501) staff       (20)     2299 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/tests/test_draw.py
+-rw-r--r--   0 gary       (501) staff       (20)     1434 2023-10-26 06:01:12.000000 vitriolic-3.4.0/tournamentcontrol/competition/tests/test_forms.py
+-rw-r--r--   0 gary       (501) staff       (20)     7104 2023-05-21 21:14:55.000000 vitriolic-3.4.0/tournamentcontrol/competition/tests/test_formsets.py
+-rw-r--r--   0 gary       (501) staff       (20)     4308 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/tests/test_rank.py
+-rw-r--r--   0 gary       (501) staff       (20)     1925 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/tests/test_signals.py
+-rw-r--r--   0 gary       (501) staff       (20)     1240 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/tests/test_utils.py
+-rw-r--r--   0 gary       (501) staff       (20)      339 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/tests/urls.py
+-rw-r--r--   0 gary       (501) staff       (20)    17484 2024-05-17 08:02:25.000000 vitriolic-3.4.0/tournamentcontrol/competition/utils.py
+-rw-r--r--   0 gary       (501) staff       (20)      227 2022-06-12 11:19:40.000000 vitriolic-3.4.0/tournamentcontrol/competition/validators.py
+-rw-r--r--   0 gary       (501) staff       (20)     8084 2024-05-17 14:39:05.000000 vitriolic-3.4.0/tournamentcontrol/competition/wizards.py
+-rw-r--r--   0 gary       (501) staff       (20)      820 2024-04-14 00:51:21.000000 vitriolic-3.4.0/tox.ini
+drwxr-xr-x   0 gary       (501) staff       (20)        0 2024-05-17 23:21:08.293889 vitriolic-3.4.0/vitriolic.egg-info/
+-rw-r--r--   0 gary       (501) staff       (20)     5002 2024-05-17 23:21:07.000000 vitriolic-3.4.0/vitriolic.egg-info/PKG-INFO
+-rw-r--r--   0 gary       (501) staff       (20)    60266 2024-05-17 23:21:07.000000 vitriolic-3.4.0/vitriolic.egg-info/SOURCES.txt
+-rw-r--r--   0 gary       (501) staff       (20)        1 2024-05-17 23:21:07.000000 vitriolic-3.4.0/vitriolic.egg-info/dependency_links.txt
+-rw-r--r--   0 gary       (501) staff       (20)        1 2024-05-17 23:21:06.000000 vitriolic-3.4.0/vitriolic.egg-info/not-zip-safe
+-rw-r--r--   0 gary       (501) staff       (20)      626 2024-05-17 23:21:07.000000 vitriolic-3.4.0/vitriolic.egg-info/requires.txt
+-rw-r--r--   0 gary       (501) staff       (20)       34 2024-05-17 23:21:07.000000 vitriolic-3.4.0/vitriolic.egg-info/top_level.txt
```

### Comparing `vitriolic-3.3.9/.github/workflows/django.yml` & `vitriolic-3.4.0/.github/workflows/django.yml`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/ISSUES.md` & `vitriolic-3.4.0/ISSUES.md`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/LICENSE` & `vitriolic-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/MANIFEST.in` & `vitriolic-3.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/PKG-INFO` & `vitriolic-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitriolic
-Version: 3.3.9
+Version: 3.4.0
 Summary: A suite of packages for the Django framework to provide integrated Content Management and Sports Administration functionality for sporting associations.
 Author-email: Gary Reynolds <gary@touch.asn.au>
 License: BSD 3-Clause License
         
         Copyright (c) 2016, Touch Technology Pty Ltd
         All rights reserved.
```

### Comparing `vitriolic-3.3.9/README.md` & `vitriolic-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/pyproject.toml` & `vitriolic-3.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tests/example_app/fixtures/query_string.json` & `vitriolic-3.4.0/tests/example_app/fixtures/query_string.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tests/example_app/sites.py` & `vitriolic-3.4.0/tests/example_app/sites.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tests/example_app/templates/example_app/generic/permissions.html` & `vitriolic-3.4.0/tests/example_app/templates/example_app/generic/permissions.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tests/example_app/tests/factories.py` & `vitriolic-3.4.0/tests/example_app/tests/factories.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tests/example_app/urls.py` & `vitriolic-3.4.0/tests/example_app/urls.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tests/manage.py` & `vitriolic-3.4.0/tests/manage.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tests/vitriolic/settings.py` & `vitriolic-3.4.0/tests/vitriolic/settings.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/apps.py` & `vitriolic-3.4.0/touchtechnology/admin/apps.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/base.py` & `vitriolic-3.4.0/touchtechnology/admin/base.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/forms.py` & `vitriolic-3.4.0/touchtechnology/admin/forms.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/locale/de/LC_MESSAGES/django.po` & `vitriolic-3.4.0/touchtechnology/admin/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/locale/en-AU/LC_MESSAGES/django.po` & `vitriolic-3.4.0/touchtechnology/admin/locale/en-AU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/locale/fr/LC_MESSAGES/django.mo` & `vitriolic-3.4.0/touchtechnology/admin/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/locale/fr/LC_MESSAGES/django.po` & `vitriolic-3.4.0/touchtechnology/admin/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/locale/ja/LC_MESSAGES/django.po` & `vitriolic-3.4.0/touchtechnology/admin/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/mixins.py` & `vitriolic-3.4.0/touchtechnology/admin/mixins.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/sites/admin.py` & `vitriolic-3.4.0/touchtechnology/admin/sites/admin.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/sites/auth.py` & `vitriolic-3.4.0/touchtechnology/admin/sites/auth.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/sites/settings.py` & `vitriolic-3.4.0/touchtechnology/admin/sites/settings.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/Gruntfile.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/bower.json` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/bower.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/css/bootstrap-theme.css` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/css/bootstrap-theme.css.map` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/css/bootstrap-theme.min.css` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/css/bootstrap-theme.min.css.map` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/css/bootstrap-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/css/bootstrap.css` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/css/bootstrap.css.map` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/css/bootstrap.min.css` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/css/bootstrap.min.css.map` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/fonts/glyphicons-halflings-regular.eot` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/fonts/glyphicons-halflings-regular.svg` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/fonts/glyphicons-halflings-regular.ttf` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/fonts/glyphicons-halflings-regular.woff` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/fonts/glyphicons-halflings-regular.woff2` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/js/bootstrap.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/dist/js/bootstrap.min.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/grunt/bs-commonjs-generator.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/grunt/bs-commonjs-generator.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/grunt/bs-glyphicons-data-generator.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/grunt/bs-glyphicons-data-generator.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/grunt/bs-lessdoc-parser.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/grunt/bs-lessdoc-parser.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/grunt/bs-raw-files-generator.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/grunt/bs-raw-files-generator.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/grunt/change-version.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/grunt/change-version.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/grunt/configBridge.json` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/grunt/configBridge.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/grunt/npm-shrinkwrap.json` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/grunt/npm-shrinkwrap.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/grunt/sauce_browsers.yml` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/grunt/sauce_browsers.yml`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/affix.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/affix.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/alert.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/alert.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/button.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/button.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/carousel.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/carousel.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/collapse.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/collapse.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/dropdown.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/dropdown.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/modal.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/modal.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/popover.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/popover.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/scrollspy.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/scrollspy.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/tab.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/tab.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/tooltip.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/tooltip.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/js/transition.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/js/transition.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/package.js` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/package.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/bootstrap/package.json` & `vitriolic-3.4.0/touchtechnology/admin/static/bootstrap/package.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/css/custom.css` & `vitriolic-3.4.0/touchtechnology/admin/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/css/custom.less` & `vitriolic-3.4.0/touchtechnology/admin/static/css/custom.less`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/css/mvpready-admin.css` & `vitriolic-3.4.0/touchtechnology/admin/static/css/mvpready-admin.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/css/mvpready-landing.css` & `vitriolic-3.4.0/touchtechnology/admin/static/css/mvpready-landing.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/LICENSE.txt` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/excanvas.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/excanvas.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/excanvas.min.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/excanvas.min.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/flot.jquery.json` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/flot.jquery.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.colorhelpers.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.colorhelpers.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.canvas.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.canvas.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.categories.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.categories.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.crosshair.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.crosshair.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.errorbars.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.errorbars.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.fillbetween.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.fillbetween.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.image.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.image.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.navigate.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.navigate.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.pie.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.pie.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.resize.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.resize.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.selection.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.selection.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.stack.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.stack.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.symbol.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.symbol.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.threshold.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.threshold.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.flot.time.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.flot.time.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot/jquery.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot/jquery.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot.tooltip/.bower.json` & `vitriolic-3.4.0/touchtechnology/admin/static/flot.tooltip/.bower.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot.tooltip/js/excanvas.min.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot.tooltip/js/excanvas.min.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot.tooltip/js/jquery.flot.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot.tooltip/js/jquery.flot.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot.tooltip/js/jquery.flot.tooltip.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot.tooltip/js/jquery.flot.tooltip.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot.tooltip/js/jquery.flot.tooltip.min.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot.tooltip/js/jquery.flot.tooltip.min.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/flot.tooltip/js/jquery.flot.tooltip.source.js` & `vitriolic-3.4.0/touchtechnology/admin/static/flot.tooltip/js/jquery.flot.tooltip.source.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/.bower.json` & `vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/.bower.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/css/font-awesome.css` & `vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/css/font-awesome.css.map` & `vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/css/font-awesome.css.map`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/css/font-awesome.min.css` & `vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/fonts/FontAwesome.otf` & `vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/fonts/fontawesome-webfont.eot` & `vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/fonts/fontawesome-webfont.svg` & `vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/fonts/fontawesome-webfont.ttf` & `vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/fonts/fontawesome-webfont.woff` & `vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/fontawesome/fonts/fontawesome-webfont.woff2` & `vitriolic-3.4.0/touchtechnology/admin/static/fontawesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/img/logo.png` & `vitriolic-3.4.0/touchtechnology/admin/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/.bower.json` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/.bower.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/MIT-LICENSE.txt` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/dist/jquery.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/dist/jquery.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/dist/jquery.min.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/dist/jquery.min.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/ajax/jsonp.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/ajax/jsonp.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/ajax/load.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/ajax/load.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/ajax/parseJSON.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/ajax/parseJSON.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/ajax/parseXML.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/ajax/parseXML.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/ajax/script.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/ajax/script.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/ajax/xhr.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/ajax/xhr.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/ajax.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/ajax.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/attributes/attr.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/attributes/attr.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/attributes/classes.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/attributes/classes.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/attributes/prop.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/attributes/prop.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/attributes/support.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/attributes/support.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/attributes/val.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/attributes/val.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/callbacks.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/callbacks.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/core/access.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/core/access.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/core/init.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/core/init.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/core/parseHTML.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/core/parseHTML.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/core/ready.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/core/ready.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/core.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/core.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/css/addGetHookIf.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/css/addGetHookIf.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/css/curCSS.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/css/curCSS.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/css/defaultDisplay.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/css/defaultDisplay.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/css/hiddenVisibleSelectors.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/css/hiddenVisibleSelectors.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/css/support.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/css/support.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/css/swap.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/css/swap.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/css.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/css.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/data/accepts.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/data/accepts.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/data.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/data.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/deferred.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/deferred.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/dimensions.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/dimensions.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/effects/Tween.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/effects/Tween.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/effects/support.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/effects/support.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/effects.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/effects.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/event/alias.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/event/alias.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/event/support.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/event/support.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/event.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/event.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/exports/amd.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/exports/amd.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/exports/global.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/exports/global.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/intro.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/intro.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/jquery.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/jquery.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/manipulation/support.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/manipulation/support.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/manipulation.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/manipulation.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/offset.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/offset.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/queue/delay.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/queue/delay.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/queue.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/queue.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/serialize.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/serialize.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/sizzle/dist/sizzle.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/sizzle/dist/sizzle.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/sizzle/dist/sizzle.min.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/sizzle/dist/sizzle.min.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/support.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/support.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/traversing/findFilter.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/traversing/findFilter.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/traversing.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/traversing.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery/src/wrap.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery/src/wrap.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/.bower.json` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/.bower.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/bower.json` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/bower.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/icheck.jquery.json` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/icheck.jquery.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/icheck.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/icheck.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/icheck.min.js` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/icheck.min.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/all.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/all.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/_all.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/_all.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/aero.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/aero.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/aero.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/aero.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/aero@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/aero@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/blue.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/blue.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/blue.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/blue.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/blue@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/blue@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/flat.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/flat.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/flat.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/flat.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/flat@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/flat@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/green.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/green.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/green.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/green.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/green@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/green@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/grey.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/grey.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/grey.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/grey.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/grey@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/grey@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/orange.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/orange.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/orange.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/orange.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/orange@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/orange@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/pink.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/pink.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/pink.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/pink.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/pink@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/pink@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/purple.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/purple.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/purple.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/purple.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/purple@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/purple@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/red.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/red.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/red.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/red.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/red@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/red@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/yellow.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/yellow.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/yellow.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/yellow.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/flat/yellow@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/flat/yellow@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/futurico/futurico.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/futurico/futurico.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/futurico/futurico.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/futurico/futurico.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/futurico/futurico@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/futurico/futurico@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/_all.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/_all.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/aero.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/aero.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/blue.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/blue.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/green.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/green.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/grey.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/grey.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/line.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/line.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/line.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/line.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/line@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/line@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/orange.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/orange.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/pink.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/pink.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/purple.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/purple.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/red.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/red.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/line/yellow.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/line/yellow.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/_all.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/_all.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/aero.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/aero.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/aero.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/aero.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/aero@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/aero@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/blue.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/blue.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/blue.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/blue.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/blue@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/blue@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/green.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/green.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/green.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/green.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/green@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/green@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/grey.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/grey.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/grey.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/grey.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/grey@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/grey@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/minimal.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/minimal.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/minimal.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/minimal.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/minimal@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/minimal@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/orange.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/orange.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/orange.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/orange.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/orange@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/orange@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/pink.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/pink.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/pink.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/pink.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/pink@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/pink@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/purple.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/purple.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/purple.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/purple.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/purple@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/purple@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/red.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/red.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/red.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/red.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/red@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/red@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/yellow.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/yellow.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/yellow.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/yellow.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/minimal/yellow@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/minimal/yellow@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/polaris/polaris.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/polaris/polaris.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/polaris/polaris.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/polaris/polaris.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/polaris/polaris@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/polaris/polaris@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/_all.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/_all.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/aero.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/aero.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/aero.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/aero.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/aero@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/aero@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/blue.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/blue.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/blue.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/blue.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/blue@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/blue@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/green.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/green.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/green.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/green.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/green@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/green@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/grey.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/grey.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/grey.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/grey.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/grey@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/grey@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/orange.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/orange.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/orange.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/orange.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/orange@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/orange@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/pink.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/pink.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/pink.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/pink.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/pink@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/pink@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/purple.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/purple.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/purple.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/purple.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/purple@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/purple@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/red.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/red.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/red.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/red.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/red@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/red@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/square.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/square.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/square.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/square.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/square@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/square@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/yellow.css` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/yellow.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/yellow.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/yellow.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/jquery-icheck/skins/square/yellow@2x.png` & `vitriolic-3.4.0/touchtechnology/admin/static/jquery-icheck/skins/square/yellow@2x.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/js/URI.js` & `vitriolic-3.4.0/touchtechnology/admin/static/js/URI.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/area.js` & `vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/area.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/auto.js` & `vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/auto.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/donut.js` & `vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/donut.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/horizontal.js` & `vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/horizontal.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/line.js` & `vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/line.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/pie.js` & `vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/pie.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/scatter.js` & `vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/scatter.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/stacked-area.js` & `vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/stacked-area.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/stacked-horizontal.js` & `vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/stacked-horizontal.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/stacked-vertical.js` & `vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/stacked-vertical.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/js/demos/flot/vertical.js` & `vitriolic-3.4.0/touchtechnology/admin/static/js/demos/flot/vertical.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/js/demos/form-plugins.js` & `vitriolic-3.4.0/touchtechnology/admin/static/js/demos/form-plugins.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/js/demos/json/table_data_small.json` & `vitriolic-3.4.0/touchtechnology/admin/static/js/demos/json/table_data_small.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/js/demos/reports/line.js` & `vitriolic-3.4.0/touchtechnology/admin/static/js/demos/reports/line.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/js/mvpready-account.js` & `vitriolic-3.4.0/touchtechnology/admin/static/js/mvpready-account.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/js/mvpready-admin.js` & `vitriolic-3.4.0/touchtechnology/admin/static/js/mvpready-admin.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/js/mvpready-core.js` & `vitriolic-3.4.0/touchtechnology/admin/static/js/mvpready-core.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/js/mvpready-helpers.js` & `vitriolic-3.4.0/touchtechnology/admin/static/js/mvpready-helpers.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/.bower.json` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/.bower.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/component.json` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/component.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/composer.json` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/composer.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/package.json` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/package.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/release.sh` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/release.sh`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2-bootstrap.css` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2-bootstrap.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2-spinner.gif` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2-spinner.gif`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2.css` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2.jquery.json` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2.jquery.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2.min.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2.min.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2.png` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_ar.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_ar.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_az.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_az.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_bg.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_bg.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_ca.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_ca.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_cs.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_cs.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_da.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_da.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_de.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_de.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_el.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_el.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_en.js.template` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_en.js.template`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_es.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_es.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_et.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_et.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_eu.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_eu.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_fa.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_fa.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_fi.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_fi.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_fr.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_fr.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_gl.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_gl.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_he.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_he.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_hr.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_hr.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_hu.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_hu.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_id.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_id.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_is.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_is.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_it.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_it.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_ja.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_ja.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_ka.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_ka.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_ko.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_ko.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_lt.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_lt.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_lv.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_lv.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_mk.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_mk.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_ms.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_ms.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_nb.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_nb.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_nl.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_nl.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_pl.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_pl.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_pt-BR.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_pt-BR.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_pt-PT.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_pt-PT.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_ro.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_ro.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_rs.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_rs.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_ru.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_ru.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_sk.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_sk.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_sv.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_sv.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_th.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_th.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_tr.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_tr.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_ug-CN.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_ug-CN.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_uk.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_uk.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_vi.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_vi.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_zh-CN.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_zh-CN.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2_locale_zh-TW.js` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2_locale_zh-TW.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/select2/select2x2.png` & `vitriolic-3.4.0/touchtechnology/admin/static/select2/select2x2.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/slimscroll/.bower.json` & `vitriolic-3.4.0/touchtechnology/admin/static/slimscroll/.bower.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/slimscroll/bower.json` & `vitriolic-3.4.0/touchtechnology/admin/static/slimscroll/bower.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/slimscroll/jquery.slimscroll.js` & `vitriolic-3.4.0/touchtechnology/admin/static/slimscroll/jquery.slimscroll.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/slimscroll/jquery.slimscroll.min.js` & `vitriolic-3.4.0/touchtechnology/admin/static/slimscroll/jquery.slimscroll.min.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/slimscroll/slimScroll.jquery.json` & `vitriolic-3.4.0/touchtechnology/admin/static/slimscroll/slimScroll.jquery.json`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/touchtechnology/admin/img/touch-technology.png` & `vitriolic-3.4.0/touchtechnology/admin/static/touchtechnology/admin/img/touch-technology.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/touchtechnology/admin/js/modal_delete.js` & `vitriolic-3.4.0/touchtechnology/admin/static/touchtechnology/admin/js/modal_delete.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/static/touchtechnology/admin/js/tabs.js` & `vitriolic-3.4.0/touchtechnology/admin/static/touchtechnology/admin/js/tabs.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/templates/40x.html` & `vitriolic-3.4.0/touchtechnology/admin/templates/40x.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/base.html` & `vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/base.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/edit.html` & `vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/edit.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/group/list.inc.html` & `vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/group/list.inc.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/list.html` & `vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/list.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/permissions.html` & `vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/permissions.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/templates/touchtechnology/admin/user/list.inc.html` & `vitriolic-3.4.0/touchtechnology/admin/templates/touchtechnology/admin/user/list.inc.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/templatetags/admin.py` & `vitriolic-3.4.0/touchtechnology/admin/templatetags/admin.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/templatetags/mvp_tags.py` & `vitriolic-3.4.0/touchtechnology/admin/templatetags/mvp_tags.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/tests/test_auth_site.py` & `vitriolic-3.4.0/touchtechnology/admin/tests/test_auth_site.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/tests/test_mptt_order.py` & `vitriolic-3.4.0/touchtechnology/admin/tests/test_mptt_order.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/admin/tests/test_mvp_tags.py` & `vitriolic-3.4.0/touchtechnology/admin/tests/test_mvp_tags.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/backends/auth.py` & `vitriolic-3.4.0/touchtechnology/common/backends/auth.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/backends/cache.py` & `vitriolic-3.4.0/touchtechnology/common/backends/cache.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/db/models.py` & `vitriolic-3.4.0/touchtechnology/common/db/models.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/debugging.py` & `vitriolic-3.4.0/touchtechnology/common/debugging.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/decorators.py` & `vitriolic-3.4.0/touchtechnology/common/decorators.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/default_settings.py` & `vitriolic-3.4.0/touchtechnology/common/default_settings.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/fields.py` & `vitriolic-3.4.0/touchtechnology/common/fields.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/forms/__init__.py` & `vitriolic-3.4.0/touchtechnology/common/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/forms/auth.py` & `vitriolic-3.4.0/touchtechnology/common/forms/auth.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/forms/fields.py` & `vitriolic-3.4.0/touchtechnology/common/forms/fields.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/forms/iter.py` & `vitriolic-3.4.0/touchtechnology/common/forms/iter.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/forms/mixins.py` & `vitriolic-3.4.0/touchtechnology/common/forms/mixins.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/forms/tz.py` & `vitriolic-3.4.0/touchtechnology/common/forms/tz.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/forms/widgets.py` & `vitriolic-3.4.0/touchtechnology/common/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/forms_lazy.py` & `vitriolic-3.4.0/touchtechnology/common/forms_lazy.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/locale/de/LC_MESSAGES/django.po` & `vitriolic-3.4.0/touchtechnology/common/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/locale/en-AU/LC_MESSAGES/django.po` & `vitriolic-3.4.0/touchtechnology/common/locale/en-AU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/locale/fr/LC_MESSAGES/django.mo` & `vitriolic-3.4.0/touchtechnology/common/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/locale/fr/LC_MESSAGES/django.po` & `vitriolic-3.4.0/touchtechnology/common/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/locale/ja/LC_MESSAGES/django.po` & `vitriolic-3.4.0/touchtechnology/common/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/middleware.py` & `vitriolic-3.4.0/touchtechnology/common/middleware.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/migrations/0001_initial.py` & `vitriolic-3.4.0/touchtechnology/common/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/migrations/0002_sitemapnode_last_modified.py` & `vitriolic-3.4.0/touchtechnology/common/migrations/0002_sitemapnode_last_modified.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/migrations/0004_sitemapnode_kwargs.py` & `vitriolic-3.4.0/touchtechnology/common/migrations/0004_sitemapnode_kwargs.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/migrations/0005_sitemapnode_populate_kwargs.py` & `vitriolic-3.4.0/touchtechnology/common/migrations/0005_sitemapnode_populate_kwargs.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/migrations/0006_model_definition_sync.py` & `vitriolic-3.4.0/touchtechnology/common/migrations/0006_model_definition_sync.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/migrations/0007_auto_20220808_1144.py` & `vitriolic-3.4.0/touchtechnology/common/migrations/0007_auto_20220808_1144.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/mixins.py` & `vitriolic-3.4.0/touchtechnology/common/mixins.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/models.py` & `vitriolic-3.4.0/touchtechnology/common/models.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/prince.py` & `vitriolic-3.4.0/touchtechnology/common/prince.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/routers.py` & `vitriolic-3.4.0/touchtechnology/common/routers.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/sitemaps.py` & `vitriolic-3.4.0/touchtechnology/common/sitemaps.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/sites.py` & `vitriolic-3.4.0/touchtechnology/common/sites.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/static/sitemap.xsl` & `vitriolic-3.4.0/touchtechnology/common/static/sitemap.xsl`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/css/froala_themes/dark.css` & `vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/css/froala_themes/dark.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/css/froala_themes/dark.min.css` & `vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/css/froala_themes/dark.min.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/css/froala_themes/gray.css` & `vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/css/froala_themes/gray.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/css/froala_themes/gray.min.css` & `vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/css/froala_themes/gray.min.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/css/froala_themes/red.css` & `vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/css/froala_themes/red.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/css/froala_themes/red.min.css` & `vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/css/froala_themes/red.min.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/css/froala_themes/royal.css` & `vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/css/froala_themes/royal.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/css/froala_themes/royal.min.css` & `vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/css/froala_themes/royal.min.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/static/touchtechnology/common/js/location_widget.js` & `vitriolic-3.4.0/touchtechnology/common/static/touchtechnology/common/js/location_widget.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/storage.py` & `vitriolic-3.4.0/touchtechnology/common/storage.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/templates/base.html` & `vitriolic-3.4.0/touchtechnology/common/templates/base.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/templates/mvp/list.inc.html` & `vitriolic-3.4.0/touchtechnology/common/templates/mvp/list.inc.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/templates/registration/login.html` & `vitriolic-3.4.0/touchtechnology/common/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/templates/registration/password_change_done.html` & `vitriolic-3.4.0/touchtechnology/common/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/templates/registration/password_change_form.html` & `vitriolic-3.4.0/touchtechnology/common/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/templates/registration/password_reset_confirm.html` & `vitriolic-3.4.0/touchtechnology/common/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/templates/registration/password_reset_email.html` & `vitriolic-3.4.0/touchtechnology/common/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/templates/registration/password_reset_form.html` & `vitriolic-3.4.0/touchtechnology/common/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/templates/registration/profile.html` & `vitriolic-3.4.0/touchtechnology/common/templates/registration/profile.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/templates/sitemap.xml` & `vitriolic-3.4.0/touchtechnology/common/templates/sitemap.xml`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/templates/touchtechnology/common/templatetags/analytics.html` & `vitriolic-3.4.0/touchtechnology/common/templates/touchtechnology/common/templatetags/analytics.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/templates/touchtechnology/common/templatetags/field.html` & `vitriolic-3.4.0/touchtechnology/common/templates/touchtechnology/common/templatetags/field.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/templates/touchtechnology/common/templatetags/navigation.html` & `vitriolic-3.4.0/touchtechnology/common/templates/touchtechnology/common/templatetags/navigation.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/templates/touchtechnology/common/templatetags/pagination.html` & `vitriolic-3.4.0/touchtechnology/common/templates/touchtechnology/common/templatetags/pagination.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/templates/touchtechnology/common/templatetags/version.html` & `vitriolic-3.4.0/touchtechnology/common/templates/touchtechnology/common/templatetags/version.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/templatetags/common.py` & `vitriolic-3.4.0/touchtechnology/common/templatetags/common.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/tests/factories.py` & `vitriolic-3.4.0/touchtechnology/common/tests/factories.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/tests/test_authentication.py` & `vitriolic-3.4.0/touchtechnology/common/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/tests/test_fields.py` & `vitriolic-3.4.0/touchtechnology/common/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/tests/test_forms.py` & `vitriolic-3.4.0/touchtechnology/common/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/tests/test_generic_views.py` & `vitriolic-3.4.0/touchtechnology/common/tests/test_generic_views.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/tests/test_html/select_date_time_field_initial.html` & `vitriolic-3.4.0/touchtechnology/common/tests/test_html/select_date_time_field_initial.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/tests/test_html/select_date_time_field_initial_tz.html` & `vitriolic-3.4.0/touchtechnology/common/tests/test_html/select_date_time_field_initial_tz.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/tests/test_pagination.py` & `vitriolic-3.4.0/touchtechnology/common/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/tests/test_storage.py` & `vitriolic-3.4.0/touchtechnology/common/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/tests/test_templates.py` & `vitriolic-3.4.0/touchtechnology/common/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/tests/test_timezone.py` & `vitriolic-3.4.0/touchtechnology/common/tests/test_timezone.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/tests/test_timezone_forms.py` & `vitriolic-3.4.0/touchtechnology/common/tests/test_timezone_forms.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/tests/test_utils.py` & `vitriolic-3.4.0/touchtechnology/common/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/utils.py` & `vitriolic-3.4.0/touchtechnology/common/utils.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/common/views.py` & `vitriolic-3.4.0/touchtechnology/common/views.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/admin.py` & `vitriolic-3.4.0/touchtechnology/content/admin.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/app_settings.py` & `vitriolic-3.4.0/touchtechnology/content/app_settings.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/apps.py` & `vitriolic-3.4.0/touchtechnology/content/apps.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/forms.py` & `vitriolic-3.4.0/touchtechnology/content/forms.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/locale/de/LC_MESSAGES/django.po` & `vitriolic-3.4.0/touchtechnology/content/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/locale/en-AU/LC_MESSAGES/django.po` & `vitriolic-3.4.0/touchtechnology/content/locale/en-AU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/locale/fr/LC_MESSAGES/django.po` & `vitriolic-3.4.0/touchtechnology/content/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/locale/ja/LC_MESSAGES/django.po` & `vitriolic-3.4.0/touchtechnology/content/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/middleware.py` & `vitriolic-3.4.0/touchtechnology/content/middleware.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/migrations/0001_initial.py` & `vitriolic-3.4.0/touchtechnology/content/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/migrations/0002_last_modified.py` & `vitriolic-3.4.0/touchtechnology/content/migrations/0002_last_modified.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/migrations/0003_auto_20160831_0608.py` & `vitriolic-3.4.0/touchtechnology/content/migrations/0003_auto_20160831_0608.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/migrations/0004_remove_placeholderkeywordargument.py` & `vitriolic-3.4.0/touchtechnology/content/migrations/0004_remove_placeholderkeywordargument.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/migrations/0005_model_definition_sync.py` & `vitriolic-3.4.0/touchtechnology/content/migrations/0005_model_definition_sync.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/models.py` & `vitriolic-3.4.0/touchtechnology/content/models.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/static/touchtechnology/admin/js/files.js` & `vitriolic-3.4.0/touchtechnology/content/static/touchtechnology/admin/js/files.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/base.html` & `vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/base.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/delete_confirm.html` & `vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/delete_confirm.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/edit_application.html` & `vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/edit_application.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/edit_page.html` & `vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/edit_page.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/file/list.html` & `vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/file/list.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/file/list.inc.html` & `vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/file/list.inc.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/files.html` & `vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/files.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/placeholder/list.html` & `vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/placeholder/list.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/redirect/list.html` & `vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/redirect/list.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/sitemapnode/list.html` & `vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/sitemapnode/list.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/templates/touchtechnology/content/admin/sitemapnode/list.inc.html` & `vitriolic-3.4.0/touchtechnology/content/templates/touchtechnology/content/admin/sitemapnode/list.inc.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/tests/test_admin.py` & `vitriolic-3.4.0/touchtechnology/content/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/utils.py` & `vitriolic-3.4.0/touchtechnology/content/utils.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/content/views.py` & `vitriolic-3.4.0/touchtechnology/content/views.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/admin.py` & `vitriolic-3.4.0/touchtechnology/news/admin.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/app_settings.py` & `vitriolic-3.4.0/touchtechnology/news/app_settings.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/decorators.py` & `vitriolic-3.4.0/touchtechnology/news/decorators.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/forms.py` & `vitriolic-3.4.0/touchtechnology/news/forms.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/locale/de/LC_MESSAGES/django.po` & `vitriolic-3.4.0/touchtechnology/news/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/locale/en-AU/LC_MESSAGES/django.po` & `vitriolic-3.4.0/touchtechnology/news/locale/en-AU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/locale/fr/LC_MESSAGES/django.po` & `vitriolic-3.4.0/touchtechnology/news/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/locale/ja/LC_MESSAGES/django.po` & `vitriolic-3.4.0/touchtechnology/news/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/migrations/0001_initial.py` & `vitriolic-3.4.0/touchtechnology/news/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/migrations/0002_article_last_modified.py` & `vitriolic-3.4.0/touchtechnology/news/migrations/0002_article_last_modified.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/migrations/0003_category_last_modified.py` & `vitriolic-3.4.0/touchtechnology/news/migrations/0003_category_last_modified.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/migrations/0004_model_definition_sync.py` & `vitriolic-3.4.0/touchtechnology/news/migrations/0004_model_definition_sync.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/migrations/0007_article_copy_field_data.py` & `vitriolic-3.4.0/touchtechnology/news/migrations/0007_article_copy_field_data.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/migrations/0009_translation.py` & `vitriolic-3.4.0/touchtechnology/news/migrations/0009_translation.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/models.py` & `vitriolic-3.4.0/touchtechnology/news/models.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/sites.py` & `vitriolic-3.4.0/touchtechnology/news/sites.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/syndication.py` & `vitriolic-3.4.0/touchtechnology/news/syndication.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/_latest_articles.html` & `vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/_latest_articles.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/_related_list.html` & `vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/_related_list.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/admin/article/list.inc.html` & `vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/admin/article/list.inc.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/admin/translation/list.inc.html` & `vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/admin/translation/list.inc.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/archive/index.html` & `vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/archive/index.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/article/detail.html` & `vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/article/detail.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/article/list.html` & `vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/article/list.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/templates/touchtechnology/news/feeds.html` & `vitriolic-3.4.0/touchtechnology/news/templates/touchtechnology/news/feeds.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/templatetags/news.py` & `vitriolic-3.4.0/touchtechnology/news/templatetags/news.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/tests/factories.py` & `vitriolic-3.4.0/touchtechnology/news/tests/factories.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/tests/test_admin.py` & `vitriolic-3.4.0/touchtechnology/news/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/touchtechnology/news/tests/test_site.py` & `vitriolic-3.4.0/touchtechnology/news/tests/test_site.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/admin.py` & `vitriolic-3.4.0/tournamentcontrol/competition/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     DrawFormat,
     Ground,
     LadderEntry,
     LadderSummary,
     Match,
     MatchScoreSheet,
     Person,
+    Place,
     Season,
     SeasonAssociation,
     SeasonExclusionDate,
     SeasonMatchTime,
     SeasonReferee,
     SimpleScoreMatchStatistic,
     Stage,
@@ -97,14 +98,15 @@
 from tournamentcontrol.competition.sites import CompetitionAdminMixin
 from tournamentcontrol.competition.tasks import (
     generate_pdf_grid,
     generate_pdf_scorecards,
     set_youtube_thumbnail,
 )
 from tournamentcontrol.competition.utils import (
+    FauxQueryset,
     generate_fixture_grid,
     generate_scorecards,
     legitimate_bye_match,
     match_unplayed,
     team_needs_progressing,
 )
 from tournamentcontrol.competition.wizards import DrawGenerationWizard
@@ -1809,14 +1811,19 @@
         matches = Match.objects.filter(
             match_unplayed,
             stage__division__season=season,
             stage__division__season__competition=competition,
         )
 
         dates = matches.dates("date", "day")
+
+        if not dates:
+            messages.error(request, _("No matches are available for rescheduling."))
+            return self.redirect(season.urls["edit"])
+
         redirect_to = season.urls["edit"]
 
         if request.method == "POST":
             formset = RescheduleDateFormSet(
                 matches=matches, dates=dates, data=request.POST
             )
             if formset.is_valid():
@@ -1877,18 +1884,35 @@
 
         queryset = (
             manager.select_related("stage__division__season")
             .filter(where)
             .order_by("stage__division__order", "round", "datetime", "play_at")
         )
 
+        venues = collections.OrderedDict()
+        for venue in season.venues.all():
+            venues.setdefault(venue, [])
+
+        for ground in Ground.objects.select_related("venue").filter(venue__in=venues):
+            venues[ground.venue].append(ground)
+
+        places = FauxQueryset(Place)
+        for venue, grounds in venues.items():
+            places.append(venue)
+            for ground in grounds:
+                places.append(ground)
+
         return self.generic_edit_multiple(
             request,
             queryset,
             formset_class=MatchScheduleFormSet,
+            formset_kwargs={
+                "places": places,
+                "timeslots": season.get_timeslots(date),
+            },
             post_save_redirect=self.redirect(season.urls["edit"]),
             templates=self.template_path("match/schedule.html"),
             extra_context=extra_context,
         )
 
     @competition_by_pk_m
     @staff_login_required_m
```

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/apps.py` & `vitriolic-3.4.0/tournamentcontrol/competition/apps.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/calc.py` & `vitriolic-3.4.0/tournamentcontrol/competition/calc.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/constants.py` & `vitriolic-3.4.0/tournamentcontrol/competition/constants.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/dashboard.py` & `vitriolic-3.4.0/tournamentcontrol/competition/dashboard.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/decorators.py` & `vitriolic-3.4.0/tournamentcontrol/competition/decorators.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/draw.py` & `vitriolic-3.4.0/tournamentcontrol/competition/draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,15 +367,15 @@
     def __iter__(self, *args, **kwargs):
         return iter(self.iterable)
 
     def __len__(self):
         return len(self.iterable)
 
     def __repr__(self):
-        return repr(self.iterable)
+        return f"<MatchCollection: {self.iterable!r}>"
 
     def add(self, match_id, match):
         self.keyed.setdefault(match_id, []).append(match)
         self.iterable.append(match)
 
     def get(self, match_id):
         return self.keyed.get(match_id)
```

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/forms.py` & `vitriolic-3.4.0/tournamentcontrol/competition/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -806,15 +806,15 @@
 
     class Meta:
         model = DrawFormat
         fields = ("name", "text", "teams", "is_final")
 
 
 class BaseMatchFormMixin(BootstrapFormControlMixin):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, timeslots=None, *args, **kwargs):
         super(BaseMatchFormMixin, self).__init__(*args, **kwargs)
 
         # set the queryset of the `home_team` and `away_team` fields
         team_ids = self.instance.stage.division.teams.values_list("id", flat=True)
         undecided_team_ids = self.instance.stage.undecided_teams.values_list(
             "id", flat=True
         )
@@ -825,19 +825,15 @@
                 if field in self.fields:
                     self.fields[field].queryset = self.fields[field].queryset.filter(
                         id__in=ids
                     )
 
         # If the season has timeslot rules, substitute the default SelectTime
         # field for a drop-down list of timeslots.
-        if self.instance.stage.division.season.timeslots.exists():
-            timeslots = self.instance.stage.division.season.get_timeslots(
-                self.instance.date
-            )
-
+        if timeslots:
             if self.instance.home_team and self.instance.home_team.timeslots_after:
                 timeslots = [
                     timeslot
                     for timeslot in timeslots
                     if timeslot >= self.instance.home_team.timeslots_after
                 ]
 
@@ -1253,44 +1249,50 @@
         fields = ("is_washout",)
 
 
 MatchWashoutFormSet = modelformset_factory(Match, extra=0, form=MatchWashoutForm)
 
 
 class MatchScheduleForm(BaseMatchFormMixin, ModelForm):
-    def __init__(self, ignore_clashes=False, *args, **kwargs):
+    def __init__(self, ignore_clashes=False, places=None, *args, **kwargs):
         super(MatchScheduleForm, self).__init__(*args, **kwargs)
         self.ignore_clashes = ignore_clashes
 
         tzinfo = timezone.get_current_timezone()
-        __, tzname = timezone_choice(tzinfo.zone)
+        __, tzname = timezone_choice(str(tzinfo))
 
         def label_from_instance(obj):
-            try:
-                label = f"{'-' * 3} {obj.ground.title}"
-            except ObjectDoesNotExist:
-                label = obj.venue.title
+            if isinstance(obj, Venue):
+                label = obj.title
+            elif isinstance(obj, Ground):
+                label = f"{'-' * 3} {obj.title}"
+            else:
+                label = f"{obj}"
+
             if settings.USE_TZ:
                 __, tz = timezone_choice(obj.timezone)
                 if tz != tzname:
                     label += " ({tz})".format(tz=tz)
             return label
 
-        venues = collections.OrderedDict()
-        for venue in self.instance.stage.division.season.venues.all():
-            venues.setdefault(venue, [])
-
-        for ground in Ground.objects.select_related("venue").filter(venue__in=venues):
-            venues[ground.venue].append(ground)
-
-        places = FauxQueryset(Place)
-        for venue, grounds in venues.items():
-            places.append(venue)
-            for ground in grounds:
-                places.append(ground)
+        if places is None:
+            venues = collections.OrderedDict()
+            for venue in self.instance.stage.division.season.venues.all():
+                venues.setdefault(venue, [])
+
+            for ground in Ground.objects.select_related("venue").filter(
+                venue__in=venues
+            ):
+                venues[ground.venue].append(ground)
+
+            places = FauxQueryset(Place)
+            for venue, grounds in venues.items():
+                places.append(venue)
+                for ground in grounds:
+                    places.append(ground)
 
         self.fields["play_at"].queryset = places
         self.fields["play_at"].label_from_instance = label_from_instance
         if not settings.USE_TZ:
             self.fields["play_at"].help_text = (
                 _(
                     "If not set, the timezone "
@@ -1351,14 +1353,19 @@
     ignore_clashes = forms.BooleanField(initial=0)
 
 
 BaseMatchScheduleFormSet = modelformset_factory(Match, extra=0, form=MatchScheduleForm)
 
 
 class MatchScheduleFormSet(BaseMatchScheduleFormSet):
+    def __init__(self, places, timeslots, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.places = places
+        self.timeslots = timeslots
+
     def _management_form(self):
         """
         Taken directly from ``django.forms.formsets.BaseFormSet`` and adjusted
         to make use of our custom ``ManagementForm`` subclass.
 
         TODO: provide a patch to upstream Django which allows a formset to
               configure, by way of class attribute, the ManagementForm class
@@ -1391,15 +1398,19 @@
     def _construct_form(self, i, **kwargs):
         # obtain the ManagementForm.cleaned_data or fake empty
         mfcd = getattr(self.management_form, "cleaned_data", {})
         # determine form properties
         ignore_clashes = bool(mfcd.get("ignore_clashes", False))
         # construct the form with our additional keyword arguments
         return super(MatchScheduleFormSet, self)._construct_form(
-            i, ignore_clashes=ignore_clashes, **kwargs
+            i,
+            ignore_clashes=ignore_clashes,
+            places=self.places,
+            timeslots=self.timeslots,
+            **kwargs,
         )
 
     def clean(self):
         if self.management_form.cleaned_data.get("ignore_clashes"):
             return
 
         if any(self.errors):
```

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/locale/de/LC_MESSAGES/django.po` & `vitriolic-3.4.0/tournamentcontrol/competition/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/locale/en-AU/LC_MESSAGES/django.po` & `vitriolic-3.4.0/tournamentcontrol/competition/locale/en-AU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/locale/fr/LC_MESSAGES/django.po` & `vitriolic-3.4.0/tournamentcontrol/competition/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/locale/ja/LC_MESSAGES/django.po` & `vitriolic-3.4.0/tournamentcontrol/competition/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/management/commands/produce_rank.py` & `vitriolic-3.4.0/tournamentcontrol/competition/management/commands/produce_rank.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/merge.py` & `vitriolic-3.4.0/tournamentcontrol/competition/merge.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0001_initial.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0002_division_draft.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0002_division_draft.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0005_alter_club_facebook_youtube_position.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0005_alter_club_facebook_youtube_position.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0006_sportingpulse_import_fields.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0006_sportingpulse_import_fields.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0007_match_videos.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0007_match_videos.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0008_nullable_statistics.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0008_nullable_statistics.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0010_remove_match_video_approved_by.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0010_remove_match_video_approved_by.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0011_custom_twitter_ladderpoints_fields.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0011_custom_twitter_ladderpoints_fields.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0012_hashtag_include_symbol.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0012_hashtag_include_symbol.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0013_statistic_played_field.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0013_statistic_played_field.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0014_match_play_at_blank.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0014_match_play_at_blank.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0015_person_user_relation.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0015_person_user_relation.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0016_season_forfeit_notifications.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0016_season_forfeit_notifications.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0017_ranking_feature.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0017_ranking_feature.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0018_resync_field_and_model_defs.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0018_resync_field_and_model_defs.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0019_auto_20161210_0922.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0019_auto_20161210_0922.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0020_competition__add__person_uuid.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0020_competition__add__person_uuid.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0021_competition__data__person_uuid.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0021_competition__data__person_uuid.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0022_competition__remove__person_id.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0022_competition__remove__person_id.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0023_competition__add__match_uuid.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0023_competition__add__match_uuid.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0023_competition__add__match_uuid_data.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0023_competition__add__match_uuid_data.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0023_competition__add__match_uuid_finalize.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0023_competition__add__match_uuid_finalize.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0024_auto_20170203_0619.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0024_auto_20170203_0619.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0025_matchvideo_baseline.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0025_matchvideo_baseline.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0026_matchvideo.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0026_matchvideo.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0027_matchvideo_data.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0027_matchvideo_data.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0029_seasonreferee.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0029_seasonreferee.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0030_match_referees.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0030_match_referees.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0031_model_definition_sync.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0031_model_definition_sync.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0032_resave_all_matches.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0032_resave_all_matches.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0033_matchscoresheet.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0033_matchscoresheet.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0034_orderedsitemapnode_add_copy_field.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0034_orderedsitemapnode_add_copy_field.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0035_season_disable_calendar.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0035_season_disable_calendar.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0036_auto_20191122_1340.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0036_auto_20191122_1340.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0040_season_live_stream_privacy.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0040_season_live_stream_privacy.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/migrations/0047_season_live_stream_oauth2.py` & `vitriolic-3.4.0/tournamentcontrol/competition/migrations/0047_season_live_stream_oauth2.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/mixins.py` & `vitriolic-3.4.0/tournamentcontrol/competition/mixins.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/models.py` & `vitriolic-3.4.0/tournamentcontrol/competition/models.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/query.py` & `vitriolic-3.4.0/tournamentcontrol/competition/query.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/rank.py` & `vitriolic-3.4.0/tournamentcontrol/competition/rank.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/rest/v1/_247.py` & `vitriolic-3.4.0/tournamentcontrol/competition/rest/v1/_247.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/rest/v1/_birdi.py` & `vitriolic-3.4.0/tournamentcontrol/competition/rest/v1/_birdi.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/rest/v1/_routers.py` & `vitriolic-3.4.0/tournamentcontrol/competition/rest/v1/_routers.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/rest/v1/club.py` & `vitriolic-3.4.0/tournamentcontrol/competition/rest/v1/club.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/rest/v1/competition.py` & `vitriolic-3.4.0/tournamentcontrol/competition/rest/v1/competition.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/rest/v1/division.py` & `vitriolic-3.4.0/tournamentcontrol/competition/rest/v1/division.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/rest/v1/season.py` & `vitriolic-3.4.0/tournamentcontrol/competition/rest/v1/season.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/rest/v1/stage.py` & `vitriolic-3.4.0/tournamentcontrol/competition/rest/v1/stage.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/signals/__init__.py` & `vitriolic-3.4.0/tournamentcontrol/competition/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/signals/decorators.py` & `vitriolic-3.4.0/tournamentcontrol/competition/signals/decorators.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/signals/ladders.py` & `vitriolic-3.4.0/tournamentcontrol/competition/signals/ladders.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/signals/matches.py` & `vitriolic-3.4.0/tournamentcontrol/competition/signals/matches.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/sites.py` & `vitriolic-3.4.0/tournamentcontrol/competition/sites.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.bootstrap.css` & `vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.bootstrap.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.bootstrap.min.css` & `vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.foundation.css` & `vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.foundation.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.foundation.min.css` & `vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.foundation.min.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.jqueryui.css` & `vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.jqueryui.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.jqueryui.min.css` & `vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/css/dataTables.jqueryui.min.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/css/jquery.dataTables.css` & `vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/css/jquery.dataTables.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/css/jquery.dataTables.min.css` & `vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/css/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/css/jquery.dataTables_themeroller.css` & `vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/css/jquery.dataTables_themeroller.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.bootstrap.js` & `vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.bootstrap.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.bootstrap.min.js` & `vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.foundation.js` & `vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.foundation.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.foundation.min.js` & `vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.foundation.min.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.jqueryui.js` & `vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.jqueryui.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.jqueryui.min.js` & `vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/js/dataTables.jqueryui.min.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/js/jquery.dataTables.js` & `vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/js/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/DataTables-1.10.12/js/jquery.dataTables.min.js` & `vitriolic-3.4.0/tournamentcontrol/competition/static/DataTables-1.10.12/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/bootstrap/dist/fonts/glyphicons-halflings-regular.eot` & `vitriolic-3.4.0/tournamentcontrol/competition/static/bootstrap/dist/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/bootstrap/dist/fonts/glyphicons-halflings-regular.svg` & `vitriolic-3.4.0/tournamentcontrol/competition/static/bootstrap/dist/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/bootstrap/dist/fonts/glyphicons-halflings-regular.ttf` & `vitriolic-3.4.0/tournamentcontrol/competition/static/bootstrap/dist/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/bootstrap/dist/fonts/glyphicons-halflings-regular.woff` & `vitriolic-3.4.0/tournamentcontrol/competition/static/bootstrap/dist/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/bootstrap/dist/fonts/glyphicons-halflings-regular.woff2` & `vitriolic-3.4.0/tournamentcontrol/competition/static/bootstrap/dist/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/css/vi_admin.css` & `vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/css/vi_admin.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/css/vi_grid.css` & `vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/css/vi_grid.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/css/vi_runsheet.css` & `vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/css/vi_runsheet.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/css/vi_scorecards.css` & `vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/css/vi_scorecards.css`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/img/report.png` & `vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/img/report.png`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/js/formset.js` & `vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/js/formset.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/static/tournamentcontrol/competition/js/match_results.js` & `vitriolic-3.4.0/tournamentcontrol/competition/static/tournamentcontrol/competition/js/match_results.js`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/tasks.py` & `vitriolic-3.4.0/tournamentcontrol/competition/tasks.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/competition/rankpoints_archive_day.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/competition/rankpoints_archive_day.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/competition/rankpoints_detail.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/competition/rankpoints_detail.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/competition/rankpoints_team.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/competition/rankpoints_team.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/calculator/index.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/calculator/index.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/_club_opponent.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/_club_opponent.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/_team_opponent.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/_team_opponent.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/club/edit.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/club/edit.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/club/team.inc.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/club/team.inc.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/division/edit.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/division/edit.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/division/list.inc.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/division/list.inc.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/grid.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/grid.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/ground/list.inc.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/ground/list.inc.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/ladderentry/list.inc.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/ladderentry/list.inc.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/dates.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/dates.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/list.inc.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/list.inc.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/schedule.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match/schedule.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match_detail.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match_detail.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match_results.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match_results.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match_washout.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/match_washout.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/mvp.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/mvp.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/officials.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/officials.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/officials_list.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/officials_list.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/person/edit.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/person/edit.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/person/list.inc.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/person/list.inc.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/progress_matches.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/progress_matches.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/progress_teams.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/progress_teams.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/reschedule.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/reschedule.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/scorecards/report.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/scorecards/report.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/scorecards.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/scorecards.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/scorers.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/scorers.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season/edit.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season/edit.html`

 * *Files 9% similar despite different names*

```diff
@@ -48,18 +48,35 @@
 										<i class="fa fa-asterisk fa-fw"></i>
 										<span class="hidden-sm hidden-xs">&nbsp;{% trans "Results" %}</span>
 									</a>
 									<a href="{% url 'admin:fixja:match-runsheet' object.competition.pk object.pk date|date:"Ymd" %}" class="btn btn-default btn-sm" role="button">
 										<i class="fa fa-clock-o fa-fw"></i>
 										<span class="hidden-sm hidden-xs">&nbsp;{% trans "Run Sheet" %}</span>
 									</a>
-									<a href="{% url 'admin:fixja:match-grid' object.competition.pk object.pk date|date:"Ymd" "pdf" %}" class="btn btn-default btn-sm" role="button">
+									<div class="btn-group">
+										<button type="button" class="btn btn-default btn-sm dropdown-toggle" data-toggle="dropdown" aria-expanded="false">
 										<i class="fa fa-table fa-fw"></i>
 										<span class="hidden-sm hidden-xs">&nbsp;{% trans "Matrix" %}</span>
-									</a>
+											<span class="caret"></span>
+										</button>
+										<ul class="dropdown-menu dropdown-menu-right" role="menu">
+											<li role="presentation">
+												<a href="{% url 'admin:fixja:match-grid' object.competition.pk object.pk date|date:"Ymd" "html" %}" role="button">
+													<i class="fa fa-html5 fa-fw"></i>
+													<span class="hidden-sm hidden-xs">&nbsp;{% trans "HTML" %}</span>
+												</a>
+											</li>
+											<li role="presentation">
+												<a href="{% url 'admin:fixja:match-grid' object.competition.pk object.pk date|date:"Ymd" "pdf" %}" role="button">
+													<i class="fa fa-file-pdf-o fa-fw"></i>
+													<span class="hidden-sm hidden-xs">&nbsp;{% trans "PDF" %}</span>
+												</a>
+											</li>
+										</ul>
+									</div>
 									<a href="{% url 'admin:competition:match-washout' object.competition.pk object.pk date|date:"Ymd" %}" class="btn btn-default btn-sm" role="button">
 										<i class="fa fa-umbrella fa-fw"></i>
 										<span class="hidden-sm hidden-xs">&nbsp;{% trans "Washout" %}</span>
 									</a>
 									<a href="{% url 'admin:fixja:scorecards' object.competition.pk object.pk date|date:"Ymd" "pdf" %}" class="btn btn-default btn-sm" role="button">
 										<i class="fa fa-print fa-fw"></i>
 										<span class="hidden-sm hidden-xs">&nbsp;{% trans "Scorecards" %}</span>
```

#### html2text {}

```diff
@@ -7,17 +7,18 @@
 ******** SScchheedduullee ********
 {{%% ttrraannss ""DDaattee"" %%}}
                              }" class="btn btn-default btn-sm" role="button">  
                              {% trans "Allocate" %}
                              }" class="btn btn-default btn-sm" role="button">  
                              {% trans "Results" %}
                              }" class="btn btn-default btn-sm" role="button">  
-}" role="button"> {{ date }} {% trans "Run Sheet" %}
-                             pdf" %}" class="btn btn-default btn-sm"
-                             role="button">  {% trans "Matrix" %}
+                             {% trans "Run Sheet" %}
+}" role="button"> {{ date }}  {% trans "Matrix" %}
+                                 * html" %}" role="button">  {% trans "HTML" %}
+                             pdf" %}" role="button">  {% trans "PDF" %}
                              }" class="btn btn-default btn-sm" role="button">  
                              {% trans "Washout" %}
                              pdf" %}" class="btn btn-default btn-sm"
                              role="button">  {% trans "Scorecards" %}
 {% blocktrans %}No stages have been generated yet.{% endblocktrans %}
 _{_%_ _t_r_a_n_s_ _"_R_e_s_c_h_e_d_u_l_e_"_ _%_}
 {% endif %} {% endblock %}
```

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season/list.inc.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season/list.inc.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season/timeslots.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season/timeslots.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season_report.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season_report.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season_summary.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/season_summary.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/seasonmatchtime/list.inc.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/seasonmatchtime/list.inc.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/seasonreferee/list.inc.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/seasonreferee/list.inc.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/signon.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/signon.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/simplescorematchstatistic/list.inc.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/simplescorematchstatistic/list.inc.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/stage/list.inc.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/stage/list.inc.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/team/list.inc.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/team/list.inc.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/team_members.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/team_members.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/teamassociation/list.inc.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/teamassociation/list.inc.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/progress/stages.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/progress/stages.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/results/basic.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/results/basic.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/results/detailed.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/results/detailed.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/scoresheets.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/admin/widgets/scoresheets.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/base.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/base.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/club.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/club.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/competition.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/competition.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/division.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/division.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/draw_format/16.txt` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/draw_format/16.txt`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/forfeit.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/forfeit.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/forfeit_list.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/forfeit_list.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/index.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/index.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/ladder/pool.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/ladder/pool.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/ladder/standard.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/ladder/standard.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/match.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/match.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/match_detail.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/match_detail.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/next_date.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/next_date.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/results.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/results.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/runsheet.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/runsheet.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/season.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/season.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/season_videos.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/season_videos.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/stage.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/stage.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/stream.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/stream.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/team.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/team.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/templatetags/preview.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/templatetags/preview.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/competition/templatetags/statistics.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/competition/templatetags/statistics.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/_registration_form.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/_registration_form.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/club_members.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/club_members.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/club_teams.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/club_teams.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/index.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/index.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/officials.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/officials.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/officials_list.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/officials_list.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templates/tournamentcontrol/rego/team_members.html` & `vitriolic-3.4.0/tournamentcontrol/competition/templates/tournamentcontrol/rego/team_members.html`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/templatetags/competition.py` & `vitriolic-3.4.0/tournamentcontrol/competition/templatetags/competition.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/tests/factories.py` & `vitriolic-3.4.0/tournamentcontrol/competition/tests/factories.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/tests/test_competition_admin.py` & `vitriolic-3.4.0/tournamentcontrol/competition/tests/test_competition_admin.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/tests/test_competition_site.py` & `vitriolic-3.4.0/tournamentcontrol/competition/tests/test_competition_site.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/tests/test_dashboard.py` & `vitriolic-3.4.0/tournamentcontrol/competition/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/tests/test_draw.py` & `vitriolic-3.4.0/tournamentcontrol/competition/tests/test_draw.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/tests/test_forms.py` & `vitriolic-3.4.0/tournamentcontrol/competition/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/tests/test_formsets.py` & `vitriolic-3.4.0/tournamentcontrol/competition/tests/test_formsets.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/tests/test_rank.py` & `vitriolic-3.4.0/tournamentcontrol/competition/tests/test_rank.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/tests/test_signals.py` & `vitriolic-3.4.0/tournamentcontrol/competition/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/tests/test_utils.py` & `vitriolic-3.4.0/tournamentcontrol/competition/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/utils.py` & `vitriolic-3.4.0/tournamentcontrol/competition/utils.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tournamentcontrol/competition/wizards.py` & `vitriolic-3.4.0/tournamentcontrol/competition/wizards.py`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/tox.ini` & `vitriolic-3.4.0/tox.ini`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/vitriolic.egg-info/PKG-INFO` & `vitriolic-3.4.0/vitriolic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitriolic
-Version: 3.3.9
+Version: 3.4.0
 Summary: A suite of packages for the Django framework to provide integrated Content Management and Sports Administration functionality for sporting associations.
 Author-email: Gary Reynolds <gary@touch.asn.au>
 License: BSD 3-Clause License
         
         Copyright (c) 2016, Touch Technology Pty Ltd
         All rights reserved.
```

### Comparing `vitriolic-3.3.9/vitriolic.egg-info/SOURCES.txt` & `vitriolic-3.4.0/vitriolic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vitriolic-3.3.9/vitriolic.egg-info/requires.txt` & `vitriolic-3.4.0/vitriolic.egg-info/requires.txt`

 * *Files identical despite different names*

