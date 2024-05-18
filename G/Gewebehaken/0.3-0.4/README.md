# Comparing `tmp/Gewebehaken-0.3.tar.gz` & `tmp/gewebehaken-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Gewebehaken-0.3.tar", last modified: Sat Dec  3 23:40:53 2022, max compression
+gzip compressed data, was "gewebehaken-0.4.tar", last modified: Sat May 18 12:38:01 2024, max compression
```

## Comparing `Gewebehaken-0.3.tar` & `gewebehaken-0.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 kupperschmidt  (1000) kupperschmidt  (1000)        0 2022-12-03 23:40:53.665672 Gewebehaken-0.3/
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)     1131 2022-12-03 23:32:14.000000 Gewebehaken-0.3/CHANGES.rst
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)     1069 2022-12-03 23:32:14.000000 Gewebehaken-0.3/LICENSE
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)      141 2022-12-03 23:32:14.000000 Gewebehaken-0.3/MANIFEST.in
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)     2775 2022-12-03 23:40:53.665672 Gewebehaken-0.3/PKG-INFO
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)      788 2022-12-03 23:32:14.000000 Gewebehaken-0.3/README.rst
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)      250 2022-12-03 23:32:14.000000 Gewebehaken-0.3/pyproject.toml
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)       26 2022-12-03 23:32:14.000000 Gewebehaken-0.3/requirements-release.txt
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)       14 2022-12-03 23:32:14.000000 Gewebehaken-0.3/requirements-test.txt
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)       42 2022-12-03 23:32:14.000000 Gewebehaken-0.3/requirements.txt
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)     1207 2022-12-03 23:40:53.665672 Gewebehaken-0.3/setup.cfg
-drwxr-xr-x   0 kupperschmidt  (1000) kupperschmidt  (1000)        0 2022-12-03 23:40:53.657672 Gewebehaken-0.3/src/
-drwxr-xr-x   0 kupperschmidt  (1000) kupperschmidt  (1000)        0 2022-12-03 23:40:53.661672 Gewebehaken-0.3/src/Gewebehaken.egg-info/
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)     2775 2022-12-03 23:40:53.000000 Gewebehaken-0.3/src/Gewebehaken.egg-info/PKG-INFO
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)      717 2022-12-03 23:40:53.000000 Gewebehaken-0.3/src/Gewebehaken.egg-info/SOURCES.txt
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)        1 2022-12-03 23:40:53.000000 Gewebehaken-0.3/src/Gewebehaken.egg-info/dependency_links.txt
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)       53 2022-12-03 23:40:53.000000 Gewebehaken-0.3/src/Gewebehaken.egg-info/entry_points.txt
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)        1 2022-12-03 23:33:22.000000 Gewebehaken-0.3/src/Gewebehaken.egg-info/not-zip-safe
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)       42 2022-12-03 23:40:53.000000 Gewebehaken-0.3/src/Gewebehaken.egg-info/requires.txt
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)       12 2022-12-03 23:40:53.000000 Gewebehaken-0.3/src/Gewebehaken.egg-info/top_level.txt
-drwxr-xr-x   0 kupperschmidt  (1000) kupperschmidt  (1000)        0 2022-12-03 23:40:53.661672 Gewebehaken-0.3/src/gewebehaken/
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)       16 2022-12-03 23:32:14.000000 Gewebehaken-0.3/src/gewebehaken/__init__.py
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)      922 2022-12-03 23:32:14.000000 Gewebehaken-0.3/src/gewebehaken/app.py
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)     1264 2022-12-03 23:32:14.000000 Gewebehaken-0.3/src/gewebehaken/cli.py
-drwxr-xr-x   0 kupperschmidt  (1000) kupperschmidt  (1000)        0 2022-12-03 23:40:53.661672 Gewebehaken-0.3/src/gewebehaken/hooks/
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)        0 2022-12-03 23:32:14.000000 Gewebehaken-0.3/src/gewebehaken/hooks/__init__.py
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)     2902 2022-12-03 23:32:14.000000 Gewebehaken-0.3/src/gewebehaken/hooks/gitlab.py
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)     1338 2022-12-03 23:32:14.000000 Gewebehaken-0.3/src/gewebehaken/hooks/twitter.py
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)     1378 2022-12-03 23:32:14.000000 Gewebehaken-0.3/src/gewebehaken/util.py
-drwxr-xr-x   0 kupperschmidt  (1000) kupperschmidt  (1000)        0 2022-12-03 23:40:53.665672 Gewebehaken-0.3/tests/
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)        0 2022-12-03 23:32:14.000000 Gewebehaken-0.3/tests/__init__.py
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)      155 2022-12-03 23:32:14.000000 Gewebehaken-0.3/tests/conftest.py
-drwxr-xr-x   0 kupperschmidt  (1000) kupperschmidt  (1000)        0 2022-12-03 23:40:53.665672 Gewebehaken-0.3/tests/hooks/
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)        0 2022-12-03 23:32:14.000000 Gewebehaken-0.3/tests/hooks/__init__.py
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)    19401 2022-12-03 23:32:14.000000 Gewebehaken-0.3/tests/hooks/test_gitlab.py
--rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)     1070 2022-12-03 23:32:14.000000 Gewebehaken-0.3/tests/hooks/test_twitter.py
+drwxr-xr-x   0 kupperschmidt  (1000) kupperschmidt  (1000)        0 2024-05-18 12:38:01.639278 gewebehaken-0.4/
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)     1373 2024-05-18 12:34:43.000000 gewebehaken-0.4/CHANGES.rst
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)     1069 2024-05-18 11:28:19.000000 gewebehaken-0.4/LICENSE
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)      141 2022-12-03 23:30:32.000000 gewebehaken-0.4/MANIFEST.in
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)     3057 2024-05-18 12:38:01.639278 gewebehaken-0.4/PKG-INFO
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)      788 2024-05-18 11:58:02.000000 gewebehaken-0.4/README.rst
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)      254 2024-05-18 12:28:02.000000 gewebehaken-0.4/pyproject.toml
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)       26 2024-05-18 12:27:11.000000 gewebehaken-0.4/requirements-release.txt
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)       14 2024-05-18 12:26:01.000000 gewebehaken-0.4/requirements-test.txt
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)       44 2024-05-18 12:04:19.000000 gewebehaken-0.4/requirements.txt
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)     1171 2024-05-18 12:38:01.639278 gewebehaken-0.4/setup.cfg
+drwxr-xr-x   0 kupperschmidt  (1000) kupperschmidt  (1000)        0 2024-05-18 12:38:01.631278 gewebehaken-0.4/src/
+drwxr-xr-x   0 kupperschmidt  (1000) kupperschmidt  (1000)        0 2024-05-18 12:38:01.635278 gewebehaken-0.4/src/Gewebehaken.egg-info/
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)     3057 2024-05-18 12:38:01.000000 gewebehaken-0.4/src/Gewebehaken.egg-info/PKG-INFO
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)      717 2024-05-18 12:38:01.000000 gewebehaken-0.4/src/Gewebehaken.egg-info/SOURCES.txt
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)        1 2024-05-18 12:38:01.000000 gewebehaken-0.4/src/Gewebehaken.egg-info/dependency_links.txt
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)       53 2024-05-18 12:38:01.000000 gewebehaken-0.4/src/Gewebehaken.egg-info/entry_points.txt
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)        1 2021-02-26 00:03:22.000000 gewebehaken-0.4/src/Gewebehaken.egg-info/not-zip-safe
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)       44 2024-05-18 12:38:01.000000 gewebehaken-0.4/src/Gewebehaken.egg-info/requires.txt
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)       12 2024-05-18 12:38:01.000000 gewebehaken-0.4/src/Gewebehaken.egg-info/top_level.txt
+drwxr-xr-x   0 kupperschmidt  (1000) kupperschmidt  (1000)        0 2024-05-18 12:38:01.635278 gewebehaken-0.4/src/gewebehaken/
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)       16 2024-05-18 12:35:17.000000 gewebehaken-0.4/src/gewebehaken/__init__.py
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)      922 2024-05-18 11:28:00.000000 gewebehaken-0.4/src/gewebehaken/app.py
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)     1264 2024-05-18 11:28:22.000000 gewebehaken-0.4/src/gewebehaken/cli.py
+drwxr-xr-x   0 kupperschmidt  (1000) kupperschmidt  (1000)        0 2024-05-18 12:38:01.635278 gewebehaken-0.4/src/gewebehaken/hooks/
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)        0 2021-02-26 00:38:48.000000 gewebehaken-0.4/src/gewebehaken/hooks/__init__.py
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)     2902 2024-05-18 11:28:06.000000 gewebehaken-0.4/src/gewebehaken/hooks/gitlab.py
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)     1338 2024-05-18 11:28:17.000000 gewebehaken-0.4/src/gewebehaken/hooks/twitter.py
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)     1378 2024-05-18 11:27:58.000000 gewebehaken-0.4/src/gewebehaken/util.py
+drwxr-xr-x   0 kupperschmidt  (1000) kupperschmidt  (1000)        0 2024-05-18 12:38:01.635278 gewebehaken-0.4/tests/
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)        0 2021-02-25 18:25:59.000000 gewebehaken-0.4/tests/__init__.py
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)      155 2021-02-25 22:52:43.000000 gewebehaken-0.4/tests/conftest.py
+drwxr-xr-x   0 kupperschmidt  (1000) kupperschmidt  (1000)        0 2024-05-18 12:38:01.635278 gewebehaken-0.4/tests/hooks/
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)        0 2021-02-25 18:25:59.000000 gewebehaken-0.4/tests/hooks/__init__.py
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)    19401 2021-02-25 22:58:20.000000 gewebehaken-0.4/tests/hooks/test_gitlab.py
+-rw-r--r--   0 kupperschmidt  (1000) kupperschmidt  (1000)     1070 2021-02-26 03:42:45.000000 gewebehaken-0.4/tests/hooks/test_twitter.py
```

### Comparing `Gewebehaken-0.3/LICENSE` & `gewebehaken-0.4/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2015-2022 Jochen Kupperschmidt
+Copyright (c) 2015-2024 Jochen Kupperschmidt
 
 Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation
 files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the
```

### Comparing `Gewebehaken-0.3/PKG-INFO` & `gewebehaken-0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 Metadata-Version: 2.1
 Name: Gewebehaken
-Version: 0.3
+Version: 0.4
 Summary: A framework to provide HTTP endpoints for incoming webhooks
 Home-page: https://github.com/homeworkprod/gewebehaken
 Author: Jochen Kupperschmidt
 Author-email: homework@nwsnet.de
 License: MIT
 Keywords: webhook
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: blinker==1.8.2
+Requires-Dist: Flask==3.0.3
+Requires-Dist: Werkzeug==3.0.3
 
 ===========
 Gewebehaken
 ===========
 
 A framework to provide HTTP endpoints for incoming webhooks.
 
 Currently supported:
 
 - GitLab
 - Twitter (via Zapier)
 
-:Copyright: 2015-2022 `Jochen Kupperschmidt <https://homework.nwsnet.de/>`_
+:Copyright: 2015-2024 `Jochen Kupperschmidt <https://homework.nwsnet.de/>`_
 :License: MIT, see LICENSE for details.
 
 
 Code Status
 ===========
 
 |badge_github-actions_test|
@@ -46,25 +48,39 @@
    :alt: Testing Status
    :target: https://github.com/homeworkprod/gewebehaken/actions/workflows/test.yml
 
 
 Requirements
 ============
 
-- Python 3.7+
+- Python 3.9+
 - Dependencies: blinker_, Flask_, Werkzeug_
 
 .. _blinker: https://blinker.readthedocs.io/
 .. _Flask: https://palletsprojects.com/p/flask/
 .. _Werkzeug: https://palletsprojects.com/p/werkzeug/
 
 Changelog
 =========
 
 
+0.4 (2024-05-18)
+----------------
+
+- Added support for Python 3.11.
+
+- Dropped support for Python 3.7 and 3.8.
+
+- Updated blinker to v1.8.2 (from v1.5).
+
+- Updated Flask to v3.0.3 (from v2.2.2).
+
+- Updated Werkzeug to v3.0.3 (from v2.2.2).
+
+
 0.3 (2022-12-04)
 -----------------
 
 - Added support for Python 3.10.
 
 - Updated blinker to v1.5 (from v1.4).
```

### Comparing `Gewebehaken-0.3/README.rst` & `gewebehaken-0.4/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 A framework to provide HTTP endpoints for incoming webhooks.
 
 Currently supported:
 
 - GitLab
 - Twitter (via Zapier)
 
-:Copyright: 2015-2022 `Jochen Kupperschmidt <https://homework.nwsnet.de/>`_
+:Copyright: 2015-2024 `Jochen Kupperschmidt <https://homework.nwsnet.de/>`_
 :License: MIT, see LICENSE for details.
 
 
 Code Status
 ===========
 
 |badge_github-actions_test|
@@ -22,13 +22,13 @@
    :alt: Testing Status
    :target: https://github.com/homeworkprod/gewebehaken/actions/workflows/test.yml
 
 
 Requirements
 ============
 
-- Python 3.7+
+- Python 3.9+
 - Dependencies: blinker_, Flask_, Werkzeug_
 
 .. _blinker: https://blinker.readthedocs.io/
 .. _Flask: https://palletsprojects.com/p/flask/
 .. _Werkzeug: https://palletsprojects.com/p/werkzeug/
```

### Comparing `Gewebehaken-0.3/setup.cfg` & `gewebehaken-0.4/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -9,43 +9,42 @@
 url = https://github.com/homeworkprod/gewebehaken
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Internet :: WWW/HTTP
 license = MIT
 license_files = LICENSE
 keywords = webhook
 platforms = any
 
 [options]
 zip_safe = False
 install_requires = 
-	blinker==1.5
-	Flask==2.2.2
-	Werkzeug==2.2.2
-python_requires = >=3.7
+	blinker==1.8.2
+	Flask==3.0.3
+	Werkzeug==3.0.3
+python_requires = >=3.9
 packages = find:
 package_dir = =src
 
 [options.entry_points]
 console_scripts = 
 	gewebehaken = gewebehaken.cli:main
 
 [options.packages.find]
 where = src
 
 [mypy]
 ignore_missing_imports = True
 no_implicit_optional = True
-python_version = 3.7
+python_version = 3.9
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `Gewebehaken-0.3/src/Gewebehaken.egg-info/PKG-INFO` & `gewebehaken-0.4/src/Gewebehaken.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 Metadata-Version: 2.1
 Name: Gewebehaken
-Version: 0.3
+Version: 0.4
 Summary: A framework to provide HTTP endpoints for incoming webhooks
 Home-page: https://github.com/homeworkprod/gewebehaken
 Author: Jochen Kupperschmidt
 Author-email: homework@nwsnet.de
 License: MIT
 Keywords: webhook
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: blinker==1.8.2
+Requires-Dist: Flask==3.0.3
+Requires-Dist: Werkzeug==3.0.3
 
 ===========
 Gewebehaken
 ===========
 
 A framework to provide HTTP endpoints for incoming webhooks.
 
 Currently supported:
 
 - GitLab
 - Twitter (via Zapier)
 
-:Copyright: 2015-2022 `Jochen Kupperschmidt <https://homework.nwsnet.de/>`_
+:Copyright: 2015-2024 `Jochen Kupperschmidt <https://homework.nwsnet.de/>`_
 :License: MIT, see LICENSE for details.
 
 
 Code Status
 ===========
 
 |badge_github-actions_test|
@@ -46,25 +48,39 @@
    :alt: Testing Status
    :target: https://github.com/homeworkprod/gewebehaken/actions/workflows/test.yml
 
 
 Requirements
 ============
 
-- Python 3.7+
+- Python 3.9+
 - Dependencies: blinker_, Flask_, Werkzeug_
 
 .. _blinker: https://blinker.readthedocs.io/
 .. _Flask: https://palletsprojects.com/p/flask/
 .. _Werkzeug: https://palletsprojects.com/p/werkzeug/
 
 Changelog
 =========
 
 
+0.4 (2024-05-18)
+----------------
+
+- Added support for Python 3.11.
+
+- Dropped support for Python 3.7 and 3.8.
+
+- Updated blinker to v1.8.2 (from v1.5).
+
+- Updated Flask to v3.0.3 (from v2.2.2).
+
+- Updated Werkzeug to v3.0.3 (from v2.2.2).
+
+
 0.3 (2022-12-04)
 -----------------
 
 - Added support for Python 3.10.
 
 - Updated blinker to v1.5 (from v1.4).
```

### Comparing `Gewebehaken-0.3/src/Gewebehaken.egg-info/SOURCES.txt` & `gewebehaken-0.4/src/Gewebehaken.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Gewebehaken-0.3/src/gewebehaken/app.py` & `gewebehaken-0.4/src/gewebehaken/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Gewebehaken
 ~~~~~~~~~~~
 
 The WSGI application
 
-:Copyright: 2015-2022 Jochen Kupperschmidt
+:Copyright: 2015-2024 Jochen Kupperschmidt
 :License: MIT, see LICENSE for details.
 """
 
 import logging
 from logging import FileHandler, Formatter
 
 from flask import Flask
```

### Comparing `Gewebehaken-0.3/src/gewebehaken/cli.py` & `gewebehaken-0.4/src/gewebehaken/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Gewebehaken
 ~~~~~~~~~~~
 
 Command-line interface
 
-:Copyright: 2015-2022 Jochen Kupperschmidt
+:Copyright: 2015-2024 Jochen Kupperschmidt
 :License: MIT, see LICENSE for details.
 """
 
 from argparse import ArgumentParser
 
 from .app import create_app
```

### Comparing `Gewebehaken-0.3/src/gewebehaken/hooks/gitlab.py` & `gewebehaken-0.4/src/gewebehaken/hooks/gitlab.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 instances.
 
 The hooks can be configured – and tested – in GitLab_ per project
 via "Settings → Web Hooks".
 
 .. _GitLab: https://gitlab.com/
 
-:Copyright: 2015-2022 Jochen Kupperschmidt
+:Copyright: 2015-2024 Jochen Kupperschmidt
 :License: MIT, see LICENSE for details.
 """
 
 from enum import Enum
 
 from blinker import signal
 from flask import abort, Blueprint, request
```

### Comparing `Gewebehaken-0.3/src/gewebehaken/hooks/twitter.py` & `gewebehaken-0.4/src/gewebehaken/hooks/twitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 service. The corresponding "zaps" must be configured to send a JSON
 request body with at least the fields defined in the view functions
 below.
 
 .. _Twitter: https://twitter.com/
 .. _Zapier: https://zapier.com/
 
-:Copyright: 2015-2022 Jochen Kupperschmidt
+:Copyright: 2015-2024 Jochen Kupperschmidt
 :License: MIT, see LICENSE for details.
 """
 
 from blinker import signal
 from flask import Blueprint, request
 
 from ..util import get_all_or_400, log_incoming_request_data, respond_no_content
```

### Comparing `Gewebehaken-0.3/src/gewebehaken/util.py` & `gewebehaken-0.4/src/gewebehaken/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Gewebehaken
 ~~~~~~~~~~~
 
 Utilities
 
-:Copyright: 2015-2022 Jochen Kupperschmidt
+:Copyright: 2015-2024 Jochen Kupperschmidt
 :License: MIT, see LICENSE for details.
 """
 
 from functools import wraps
 from pprint import pformat
 
 from flask import abort, current_app, Response
```

### Comparing `Gewebehaken-0.3/tests/hooks/test_gitlab.py` & `gewebehaken-0.4/tests/hooks/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `Gewebehaken-0.3/tests/hooks/test_twitter.py` & `gewebehaken-0.4/tests/hooks/test_twitter.py`

 * *Files identical despite different names*

