# Comparing `tmp/gdmty_drf_firebase_auth-24.5.2.tar.gz` & `tmp/gdmty_drf_firebase_auth-24.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdmty_drf_firebase_auth-24.5.2.tar", last modified: Thu May  9 20:27:18 2024, max compression
+gzip compressed data, was "gdmty_drf_firebase_auth-24.5.3.tar", last modified: Sat May 18 11:03:44 2024, max compression
```

## Comparing `gdmty_drf_firebase_auth-24.5.2.tar` & `gdmty_drf_firebase_auth-24.5.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 20:27:18.176599 gdmty_drf_firebase_auth-24.5.2/
--rw-rw-rw-   0        0        0    11552 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.2/LICENSE
--rw-rw-rw-   0        0        0       51 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0    20224 2024-05-09 20:27:18.176599 gdmty_drf_firebase_auth-24.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     5806 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.2/README.md
--rw-rw-rw-   0        0        0     1645 2024-05-09 20:27:07.000000 gdmty_drf_firebase_auth-24.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 20:27:18.177599 gdmty_drf_firebase_auth-24.5.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-09 20:27:18.152355 gdmty_drf_firebase_auth-24.5.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-09 20:27:18.166408 gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/
--rw-rw-rw-   0        0        0     1653 2024-05-09 20:27:07.000000 gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/__init__.py
--rw-rw-rw-   0        0        0      877 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/admin.py
--rw-rw-rw-   0        0        0      888 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/apps.py
--rw-rw-rw-   0        0        0     8660 2024-05-09 20:26:48.000000 gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/authentication.py
-drwxrwxrwx   0        0        0        0 2024-05-09 20:27:18.173463 gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/migrations/
--rw-rw-rw-   0        0        0     1119 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      698 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/migrations/0002_initial.py
--rw-rw-rw-   0        0        0        0 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/migrations/__init__.py
--rw-rw-rw-   0        0        0     1759 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/models.py
--rw-rw-rw-   0        0        0     2388 2024-05-09 19:44:01.000000 gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/settings.py
--rw-rw-rw-   0        0        0      743 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/tests.py
--rw-rw-rw-   0        0        0     2184 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/utils.py
--rw-rw-rw-   0        0        0      705 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/views.py
-drwxrwxrwx   0        0        0        0 2024-05-09 20:27:18.174463 gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth.egg-info/
--rw-rw-rw-   0        0        0    20224 2024-05-09 20:27:18.000000 gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      807 2024-05-09 20:27:18.000000 gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 20:27:18.000000 gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2024-05-09 20:27:18.000000 gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-09 20:27:18.000000 gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 11:03:44.144928 gdmty_drf_firebase_auth-24.5.3/
+-rw-rw-rw-   0        0        0    11552 2023-12-25 20:47:02.000000 gdmty_drf_firebase_auth-24.5.3/LICENSE
+-rw-rw-rw-   0        0        0       51 2023-12-25 21:56:12.000000 gdmty_drf_firebase_auth-24.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    20226 2024-05-18 11:03:44.144928 gdmty_drf_firebase_auth-24.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5806 2024-05-12 00:50:45.000000 gdmty_drf_firebase_auth-24.5.3/README.md
+-rw-rw-rw-   0        0        0     1647 2024-05-18 11:03:17.000000 gdmty_drf_firebase_auth-24.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-18 11:03:44.145920 gdmty_drf_firebase_auth-24.5.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-18 11:03:44.122408 gdmty_drf_firebase_auth-24.5.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-18 11:03:44.136985 gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/
+-rw-rw-rw-   0        0        0     1653 2024-05-18 11:03:17.000000 gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/__init__.py
+-rw-rw-rw-   0        0        0      877 2024-05-12 00:50:45.000000 gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/admin.py
+-rw-rw-rw-   0        0        0      888 2024-05-12 00:50:45.000000 gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/apps.py
+-rw-rw-rw-   0        0        0     8660 2024-05-12 00:50:45.000000 gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/authentication.py
+drwxrwxrwx   0        0        0        0 2024-05-18 11:03:44.142412 gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/migrations/
+-rw-rw-rw-   0        0        0     1119 2023-12-25 20:43:48.000000 gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      698 2023-12-25 20:43:48.000000 gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/migrations/0002_initial.py
+-rw-rw-rw-   0        0        0        0 2023-12-25 16:40:22.000000 gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1759 2024-05-12 00:50:45.000000 gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/models.py
+-rw-rw-rw-   0        0        0     2388 2024-05-12 00:50:45.000000 gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/settings.py
+-rw-rw-rw-   0        0        0      743 2024-05-12 00:50:45.000000 gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/tests.py
+-rw-rw-rw-   0        0        0     2184 2024-05-12 00:50:45.000000 gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/utils.py
+-rw-rw-rw-   0        0        0      705 2024-05-12 00:50:45.000000 gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/views.py
+drwxrwxrwx   0        0        0        0 2024-05-18 11:03:44.143915 gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth.egg-info/
+-rw-rw-rw-   0        0        0    20226 2024-05-18 11:03:44.000000 gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      807 2024-05-18 11:03:44.000000 gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 11:03:44.000000 gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      132 2024-05-18 11:03:44.000000 gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-18 11:03:44.000000 gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth.egg-info/top_level.txt
```

### Comparing `gdmty_drf_firebase_auth-24.5.2/LICENSE` & `gdmty_drf_firebase_auth-24.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.5.2/PKG-INFO` & `gdmty_drf_firebase_auth-24.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdmty-drf-firebase-auth
-Version: 24.5.2
+Version: 24.5.3
 Summary: Custom Django Rest Framework authentication backend than can be used with many firebase projects at same time, and storing as local users.
 Author-email: Gobierno de Monterrey <cesar.benjamin@monterrey.gob.mx>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -213,15 +213,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django<6.0,>=4.2
+Requires-Dist: django<6.0,>=4.1.3
 Requires-Dist: firebase-admin
 Requires-Dist: djangorestframework
 Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
```

### Comparing `gdmty_drf_firebase_auth-24.5.2/README.md` & `gdmty_drf_firebase_auth-24.5.3/README.md`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.5.2/pyproject.toml` & `gdmty_drf_firebase_auth-24.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,45 +2,45 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gdmty-drf-firebase-auth"
-version = "24.5.2"
+version = "24.5.3"
 description = "Custom Django Rest Framework authentication backend than can be used with many firebase projects at same time, and storing as local users."
 readme = "README.md"
 authors = [{ name="Gobierno de Monterrey", email="cesar.benjamin@monterrey.gob.mx" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Framework :: Django",
 ]
 keywords = ["django", "firebase", "jwt", "authentication"]
 dependencies = [
-    "django >= 4.2, < 6.0",
+    "django >= 4.1.3, < 6.0",
     "firebase-admin",
     "djangorestframework",
     "tomli; python_version < '3.11'",
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 "Homepage" = "https://github.com/SIGAMty/gdmty-drf-firebase-auth"
 "Bug Tracker" = "https://github.com/SIGAMty/gdmty-drf-firebase-auth/issues"
 
 [tool.bumpver]
-current_version = "24.5.2"
+current_version = "24.5.3"
 version_pattern = "MAJOR.MINOR.PATCH[-PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = true
```

### Comparing `gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/__init__.py` & `gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 This package also adds support for login
 with email and password, and also adds support for
 custom user models. And is fully integrated with gdmty-id.
 
 """
 
 __title__ = 'gdmty_drf_firebase_auth'
-__version__ = '24.5.2'
+__version__ = '24.5.3'
 __description__ = (
     'Custom Django Rest Framework authentication backend for '
     'parsing Firebase uid tokens and storing as local users.'
     'This package is a fork of django-firebase-auth '
     'with some fixes and improvements. '
     'This package also adds support for login '
     'with email and password, and also adds support for '
```

### Comparing `gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/admin.py` & `gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/admin.py`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/apps.py` & `gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/apps.py`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/authentication.py` & `gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/migrations/0001_initial.py` & `gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/migrations/0002_initial.py` & `gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/models.py` & `gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/models.py`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/settings.py` & `gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/settings.py`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/tests.py` & `gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/tests.py`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/utils.py` & `gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/utils.py`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth/views.py` & `gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth/views.py`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth.egg-info/PKG-INFO` & `gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdmty-drf-firebase-auth
-Version: 24.5.2
+Version: 24.5.3
 Summary: Custom Django Rest Framework authentication backend than can be used with many firebase projects at same time, and storing as local users.
 Author-email: Gobierno de Monterrey <cesar.benjamin@monterrey.gob.mx>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -213,15 +213,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django<6.0,>=4.2
+Requires-Dist: django<6.0,>=4.1.3
 Requires-Dist: firebase-admin
 Requires-Dist: djangorestframework
 Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
```

### Comparing `gdmty_drf_firebase_auth-24.5.2/src/gdmty_drf_firebase_auth.egg-info/SOURCES.txt` & `gdmty_drf_firebase_auth-24.5.3/src/gdmty_drf_firebase_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

