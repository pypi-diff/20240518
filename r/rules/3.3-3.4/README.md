# Comparing `tmp/rules-3.3.tar.gz` & `tmp/rules-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rules-3.3.tar", last modified: Wed Mar 23 08:53:50 2022, max compression
+gzip compressed data, was "rules-3.4.tar", last modified: Sat May 18 10:40:52 2024, max compression
```

## Comparing `rules-3.3.tar` & `rules-3.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:53:50.128957 rules-3.3/
--rw-r--r--   0 runner    (1001) docker     (121)     3388 2022-03-23 08:53:37.000000 rules-3.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-03-23 08:53:37.000000 rules-3.3/INSTALL
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-03-23 08:53:37.000000 rules-3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-03-23 08:53:37.000000 rules-3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    37815 2022-03-23 08:53:50.128957 rules-3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    36911 2022-03-23 08:53:37.000000 rules-3.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-03-23 08:53:37.000000 rules-3.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:53:50.124957 rules-3.3/rules/
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-03-23 08:53:37.000000 rules-3.3/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-03-23 08:53:37.000000 rules-3.3/rules/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:53:50.124957 rules-3.3/rules/contrib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 08:53:37.000000 rules-3.3/rules/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2121 2022-03-23 08:53:37.000000 rules-3.3/rules/contrib/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     3129 2022-03-23 08:53:37.000000 rules-3.3/rules/contrib/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2808 2022-03-23 08:53:37.000000 rules-3.3/rules/contrib/rest_framework.py
--rw-r--r--   0 runner    (1001) docker     (121)    10298 2022-03-23 08:53:37.000000 rules-3.3/rules/contrib/views.py
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-03-23 08:53:37.000000 rules-3.3/rules/permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)    10317 2022-03-23 08:53:37.000000 rules-3.3/rules/predicates.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 08:53:37.000000 rules-3.3/rules/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-03-23 08:53:37.000000 rules-3.3/rules/rulesets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:53:50.124957 rules-3.3/rules/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 08:53:37.000000 rules-3.3/rules/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-03-23 08:53:37.000000 rules-3.3/rules/templatetags/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:53:50.124957 rules-3.3/rules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    37815 2022-03-23 08:53:49.000000 rules-3.3/rules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-03-23 08:53:50.000000 rules-3.3/rules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 08:53:49.000000 rules-3.3/rules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 08:53:48.000000 rules-3.3/rules.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-23 08:53:50.000000 rules-3.3/rules.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      160 2022-03-23 08:53:37.000000 rules-3.3/runtests.sh
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-03-23 08:53:50.128957 rules-3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1817 2022-03-23 08:53:37.000000 rules-3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:53:50.124957 rules-3.3/tests/
--rwxr-xr-x   0 runner    (1001) docker     (121)      250 2022-03-23 08:53:37.000000 rules-3.3/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:53:50.124957 rules-3.3/tests/testapp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 08:53:37.000000 rules-3.3/tests/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-03-23 08:53:37.000000 rules-3.3/tests/testapp/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:53:50.124957 rules-3.3/tests/testapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1817 2022-03-23 08:53:37.000000 rules-3.3/tests/testapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 08:53:37.000000 rules-3.3/tests/testapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-03-23 08:53:37.000000 rules-3.3/tests/testapp/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-03-23 08:53:37.000000 rules-3.3/tests/testapp/rules.py
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-03-23 08:53:37.000000 rules-3.3/tests/testapp/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:53:50.128957 rules-3.3/tests/testapp/templates/
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-03-23 08:53:37.000000 rules-3.3/tests/testapp/templates/empty.html
--rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-03-23 08:53:37.000000 rules-3.3/tests/testapp/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     2551 2022-03-23 08:53:37.000000 rules-3.3/tests/testapp/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:53:50.128957 rules-3.3/tests/testsuite/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 08:53:37.000000 rules-3.3/tests/testsuite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:53:50.128957 rules-3.3/tests/testsuite/contrib/
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-03-23 08:53:37.000000 rules-3.3/tests/testsuite/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-03-23 08:53:37.000000 rules-3.3/tests/testsuite/contrib/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-03-23 08:53:37.000000 rules-3.3/tests/testsuite/contrib/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-03-23 08:53:37.000000 rules-3.3/tests/testsuite/contrib/test_predicates.py
--rw-r--r--   0 runner    (1001) docker     (121)     2923 2022-03-23 08:53:37.000000 rules-3.3/tests/testsuite/contrib/test_rest_framework.py
--rw-r--r--   0 runner    (1001) docker     (121)     3627 2022-03-23 08:53:37.000000 rules-3.3/tests/testsuite/contrib/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (121)     9323 2022-03-23 08:53:37.000000 rules-3.3/tests/testsuite/contrib/test_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-03-23 08:53:37.000000 rules-3.3/tests/testsuite/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)    12870 2022-03-23 08:53:37.000000 rules-3.3/tests/testsuite/test_predicates.py
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-03-23 08:53:37.000000 rules-3.3/tests/testsuite/test_rulesets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:40:52.081651 rules-3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-18 10:40:48.000000 rules-3.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-18 10:40:48.000000 rules-3.4/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-18 10:40:48.000000 rules-3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-18 10:40:48.000000 rules-3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    38303 2024-05-18 10:40:52.081651 rules-3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    37367 2024-05-18 10:40:48.000000 rules-3.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-18 10:40:48.000000 rules-3.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:40:52.073651 rules-3.4/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-18 10:40:48.000000 rules-3.4/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-18 10:40:48.000000 rules-3.4/rules/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:40:52.077651 rules-3.4/rules/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 10:40:48.000000 rules-3.4/rules/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-18 10:40:48.000000 rules-3.4/rules/contrib/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-18 10:40:48.000000 rules-3.4/rules/contrib/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-18 10:40:48.000000 rules-3.4/rules/contrib/rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10298 2024-05-18 10:40:48.000000 rules-3.4/rules/contrib/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-18 10:40:48.000000 rules-3.4/rules/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-18 10:40:48.000000 rules-3.4/rules/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 10:40:48.000000 rules-3.4/rules/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-18 10:40:48.000000 rules-3.4/rules/rulesets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:40:52.077651 rules-3.4/rules/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 10:40:48.000000 rules-3.4/rules/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-18 10:40:48.000000 rules-3.4/rules/templatetags/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:40:52.081651 rules-3.4/rules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    38303 2024-05-18 10:40:52.000000 rules-3.4/rules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-18 10:40:52.000000 rules-3.4/rules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 10:40:52.000000 rules-3.4/rules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 10:40:51.000000 rules-3.4/rules.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-18 10:40:52.000000 rules-3.4/rules.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      160 2024-05-18 10:40:48.000000 rules-3.4/runtests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-18 10:40:52.081651 rules-3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-18 10:40:48.000000 rules-3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:40:52.077651 rules-3.4/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      250 2024-05-18 10:40:48.000000 rules-3.4/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:40:52.077651 rules-3.4/tests/testapp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 10:40:48.000000 rules-3.4/tests/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-18 10:40:48.000000 rules-3.4/tests/testapp/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:40:52.077651 rules-3.4/tests/testapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-18 10:40:48.000000 rules-3.4/tests/testapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 10:40:48.000000 rules-3.4/tests/testapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-18 10:40:48.000000 rules-3.4/tests/testapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-18 10:40:48.000000 rules-3.4/tests/testapp/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-18 10:40:48.000000 rules-3.4/tests/testapp/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:40:52.077651 rules-3.4/tests/testapp/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-18 10:40:48.000000 rules-3.4/tests/testapp/templates/empty.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-18 10:40:48.000000 rules-3.4/tests/testapp/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-18 10:40:48.000000 rules-3.4/tests/testapp/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:40:52.077651 rules-3.4/tests/testsuite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 10:40:48.000000 rules-3.4/tests/testsuite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:40:52.081651 rules-3.4/tests/testsuite/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-18 10:40:48.000000 rules-3.4/tests/testsuite/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-18 10:40:48.000000 rules-3.4/tests/testsuite/contrib/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-18 10:40:48.000000 rules-3.4/tests/testsuite/contrib/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-18 10:40:48.000000 rules-3.4/tests/testsuite/contrib/test_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-18 10:40:48.000000 rules-3.4/tests/testsuite/contrib/test_rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-18 10:40:48.000000 rules-3.4/tests/testsuite/contrib/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-18 10:40:48.000000 rules-3.4/tests/testsuite/contrib/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-18 10:40:48.000000 rules-3.4/tests/testsuite/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-05-18 10:40:48.000000 rules-3.4/tests/testsuite/test_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-18 10:40:48.000000 rules-3.4/tests/testsuite/test_rulesets.py
```

### Comparing `rules-3.3/CHANGELOG.md` & `rules-3.4/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+## v3.4.0 - 2024/05/18
+
+- Add support for Django 4.2 and 5.0
+- Add support for Python 3.11 and 3.12
+- Drop support for EOL Python 3.7
+- Drop support for EOL Django 2.2 and 4.0
+- Fix bug: type annotations were not used because ``py.typed`` was not always
+  installed.
+
 ## v3.3.0 - 2022/03/23
 
 - Introduce type annotations for common APIs
 
 ## v3.2.1 - 2022/03/02
 
 - Fixed incorrect Django versions mentioned in CHANGELOG
```

### Comparing `rules-3.3/LICENSE` & `rules-3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rules-3.3/PKG-INFO` & `rules-3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: rules
-Version: 3.3
+Version: 3.4
 Summary: Awesome Django authorization, without the database
 Home-page: http://github.com/dfunckt/django-rules
 Author: Akis Kesoglou
 Author-email: akiskesoglou@gmail.com
 Maintainer: Akis Kesoglou
 Maintainer-email: akiskesoglou@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 
 rules
 ^^^^^
 
 ``rules`` is a tiny but powerful app providing object-level permissions to
 Django, without requiring a database. At its core, it is a generic framework
@@ -77,14 +77,15 @@
 - `How to install`_
 
   - `Configuring Django`_
 
 - `Using Rules`_
 
   - `Creating predicates`_
+  - `Dynamic predicates`_
   - `Setting up rules`_
   - `Combining predicates`_
 
 - `Using Rules with Django`_
 
   - `Permissions`_
   - `Permissions in models`_
@@ -105,17 +106,17 @@
 - `API Reference`_
 - `Licence`_
 
 
 Requirements
 ============
 
-``rules`` requires Python 3.7 or newer. The last version to support Python 2.7
+``rules`` requires Python 3.8 or newer. The last version to support Python 2.7
 is ``rules`` 2.2. It can optionally integrate with Django, in which case
-requires Django 2.2 or newer.
+requires Django 3.2 or newer.
 
 *Note*: At any given moment in time, ``rules`` will maintain support for all
 currently supported Django versions, while dropping support for those versions
 that reached end-of-life in minor releases. See the `Supported Versions`_
 section on Django Project website for the current state and timeline.
 
 .. _Supported Versions: https://www.djangoproject.com/download/#supported-versions
@@ -241,14 +242,36 @@
 Predicates can do pretty much anything with the given arguments, but must
 always return ``True`` if the condition they check is true, ``False``
 otherwise. ``rules`` comes with several predefined predicates that you may
 read about later on in `API Reference`_, that are mostly useful when dealing
 with `authorization in Django`_.
 
 
+Dynamic predicates
+-------------------
+
+If needed predicates can be created dynamically depending on parameters:
+
+.. code:: python
+
+    import rules
+
+
+    def role_is(role_id):
+        @rules.predicate
+        def user_has_role(user):
+            return user.role.id == role_id
+
+        return user_has_role
+
+
+    rules.add_perm("reports.view_report_abc", role_is(12))
+    rules.add_perm("reports.view_report_xyz", role_is(13))
+
+
 Setting up rules
 ----------------
 
 Let's pretend that we want to let authors edit or delete their books, but not
 books written by other authors. So, essentially, what determines whether an
 author *can edit* or *can delete* a given book is *whether they are its
 author*.
@@ -1137,9 +1160,7 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
 OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
 HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
-
-
```

### Comparing `rules-3.3/README.rst` & `rules-3.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 - `How to install`_
 
   - `Configuring Django`_
 
 - `Using Rules`_
 
   - `Creating predicates`_
+  - `Dynamic predicates`_
   - `Setting up rules`_
   - `Combining predicates`_
 
 - `Using Rules with Django`_
 
   - `Permissions`_
   - `Permissions in models`_
@@ -80,17 +81,17 @@
 - `API Reference`_
 - `Licence`_
 
 
 Requirements
 ============
 
-``rules`` requires Python 3.7 or newer. The last version to support Python 2.7
+``rules`` requires Python 3.8 or newer. The last version to support Python 2.7
 is ``rules`` 2.2. It can optionally integrate with Django, in which case
-requires Django 2.2 or newer.
+requires Django 3.2 or newer.
 
 *Note*: At any given moment in time, ``rules`` will maintain support for all
 currently supported Django versions, while dropping support for those versions
 that reached end-of-life in minor releases. See the `Supported Versions`_
 section on Django Project website for the current state and timeline.
 
 .. _Supported Versions: https://www.djangoproject.com/download/#supported-versions
@@ -216,14 +217,36 @@
 Predicates can do pretty much anything with the given arguments, but must
 always return ``True`` if the condition they check is true, ``False``
 otherwise. ``rules`` comes with several predefined predicates that you may
 read about later on in `API Reference`_, that are mostly useful when dealing
 with `authorization in Django`_.
 
 
+Dynamic predicates
+-------------------
+
+If needed predicates can be created dynamically depending on parameters:
+
+.. code:: python
+
+    import rules
+
+
+    def role_is(role_id):
+        @rules.predicate
+        def user_has_role(user):
+            return user.role.id == role_id
+
+        return user_has_role
+
+
+    rules.add_perm("reports.view_report_abc", role_is(12))
+    rules.add_perm("reports.view_report_xyz", role_is(13))
+
+
 Setting up rules
 ----------------
 
 Let's pretend that we want to let authors edit or delete their books, but not
 books written by other authors. So, essentially, what determines whether an
 author *can edit* or *can delete* a given book is *whether they are its
 author*.
```

### Comparing `rules-3.3/rules/contrib/admin.py` & `rules-3.4/rules/contrib/admin.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/rules/contrib/models.py` & `rules-3.4/rules/contrib/models.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/rules/contrib/rest_framework.py` & `rules-3.4/rules/contrib/rest_framework.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/rules/contrib/views.py` & `rules-3.4/rules/contrib/views.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/rules/permissions.py` & `rules-3.4/rules/permissions.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/rules/predicates.py` & `rules-3.4/rules/predicates.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,21 +60,21 @@
         # fn can be a callable with any of the following signatures:
         #   - fn(obj=None, target=None)
         #   - fn(obj=None)
         #   - fn()
         assert callable(fn), "The given predicate is not callable."
         innerfn = fn
         if isinstance(fn, Predicate):
-            fn, num_args, var_args, name = (
+            innerfn, num_args, var_args, name = (
                 fn.fn,
                 fn.num_args,
                 fn.var_args,
                 name or fn.name,
             )
-            innerfn = fn
+            fn = innerfn
         elif isinstance(fn, partial):
             innerfn = fn.func
             argspec = getfullargspec(innerfn)
             var_args = argspec.varargs is not None
             num_args = len(argspec.args) - len(fn.args)
             if ismethod(innerfn):
                 num_args -= 1  # skip `self`
```

### Comparing `rules-3.3/rules/rulesets.py` & `rules-3.4/rules/rulesets.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/rules.egg-info/PKG-INFO` & `rules-3.4/rules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: rules
-Version: 3.3
+Version: 3.4
 Summary: Awesome Django authorization, without the database
 Home-page: http://github.com/dfunckt/django-rules
 Author: Akis Kesoglou
 Author-email: akiskesoglou@gmail.com
 Maintainer: Akis Kesoglou
 Maintainer-email: akiskesoglou@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 
 rules
 ^^^^^
 
 ``rules`` is a tiny but powerful app providing object-level permissions to
 Django, without requiring a database. At its core, it is a generic framework
@@ -77,14 +77,15 @@
 - `How to install`_
 
   - `Configuring Django`_
 
 - `Using Rules`_
 
   - `Creating predicates`_
+  - `Dynamic predicates`_
   - `Setting up rules`_
   - `Combining predicates`_
 
 - `Using Rules with Django`_
 
   - `Permissions`_
   - `Permissions in models`_
@@ -105,17 +106,17 @@
 - `API Reference`_
 - `Licence`_
 
 
 Requirements
 ============
 
-``rules`` requires Python 3.7 or newer. The last version to support Python 2.7
+``rules`` requires Python 3.8 or newer. The last version to support Python 2.7
 is ``rules`` 2.2. It can optionally integrate with Django, in which case
-requires Django 2.2 or newer.
+requires Django 3.2 or newer.
 
 *Note*: At any given moment in time, ``rules`` will maintain support for all
 currently supported Django versions, while dropping support for those versions
 that reached end-of-life in minor releases. See the `Supported Versions`_
 section on Django Project website for the current state and timeline.
 
 .. _Supported Versions: https://www.djangoproject.com/download/#supported-versions
@@ -241,14 +242,36 @@
 Predicates can do pretty much anything with the given arguments, but must
 always return ``True`` if the condition they check is true, ``False``
 otherwise. ``rules`` comes with several predefined predicates that you may
 read about later on in `API Reference`_, that are mostly useful when dealing
 with `authorization in Django`_.
 
 
+Dynamic predicates
+-------------------
+
+If needed predicates can be created dynamically depending on parameters:
+
+.. code:: python
+
+    import rules
+
+
+    def role_is(role_id):
+        @rules.predicate
+        def user_has_role(user):
+            return user.role.id == role_id
+
+        return user_has_role
+
+
+    rules.add_perm("reports.view_report_abc", role_is(12))
+    rules.add_perm("reports.view_report_xyz", role_is(13))
+
+
 Setting up rules
 ----------------
 
 Let's pretend that we want to let authors edit or delete their books, but not
 books written by other authors. So, essentially, what determines whether an
 author *can edit* or *can delete* a given book is *whether they are its
 author*.
@@ -1137,9 +1160,7 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
 OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
 HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
-
-
```

### Comparing `rules-3.3/rules.egg-info/SOURCES.txt` & `rules-3.4/rules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rules-3.3/setup.py` & `rules-3.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,22 +44,24 @@
     license="MIT",
     zip_safe=False,
     packages=[
         "rules",
         "rules.templatetags",
         "rules.contrib",
     ],
+    include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `rules-3.3/tests/testapp/migrations/0001_initial.py` & `rules-3.4/tests/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/tests/testapp/models.py` & `rules-3.4/tests/testapp/models.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/tests/testapp/rules.py` & `rules-3.4/tests/testapp/rules.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/tests/testapp/settings.py` & `rules-3.4/tests/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/tests/testapp/urls.py` & `rules-3.4/tests/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/tests/testapp/views.py` & `rules-3.4/tests/testapp/views.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/tests/testsuite/contrib/__init__.py` & `rules-3.4/tests/testsuite/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/tests/testsuite/contrib/test_admin.py` & `rules-3.4/tests/testsuite/contrib/test_admin.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/tests/testsuite/contrib/test_models.py` & `rules-3.4/tests/testsuite/contrib/test_models.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/tests/testsuite/contrib/test_predicates.py` & `rules-3.4/tests/testsuite/contrib/test_predicates.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/tests/testsuite/contrib/test_rest_framework.py` & `rules-3.4/tests/testsuite/contrib/test_rest_framework.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/tests/testsuite/contrib/test_templatetags.py` & `rules-3.4/tests/testsuite/contrib/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/tests/testsuite/contrib/test_views.py` & `rules-3.4/tests/testsuite/contrib/test_views.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/tests/testsuite/test_permissions.py` & `rules-3.4/tests/testsuite/test_permissions.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/tests/testsuite/test_predicates.py` & `rules-3.4/tests/testsuite/test_predicates.py`

 * *Files identical despite different names*

### Comparing `rules-3.3/tests/testsuite/test_rulesets.py` & `rules-3.4/tests/testsuite/test_rulesets.py`

 * *Files identical despite different names*

