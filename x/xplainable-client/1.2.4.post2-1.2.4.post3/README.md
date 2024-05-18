# Comparing `tmp/xplainable_client-1.2.4.post2.tar.gz` & `tmp/xplainable_client-1.2.4.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xplainable_client-1.2.4.post2.tar", last modified: Sat May 18 02:28:21 2024, max compression
+gzip compressed data, was "xplainable_client-1.2.4.post3.tar", last modified: Sat May 18 02:38:51 2024, max compression
```

## Comparing `xplainable_client-1.2.4.post2.tar` & `xplainable_client-1.2.4.post3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 02:28:21.833180 xplainable_client-1.2.4.post2/
--rw-rw-rw-   0        0        0     3325 2024-03-12 06:45:15.000000 xplainable_client-1.2.4.post2/.gitignore
--rw-rw-rw-   0        0        0    35184 2024-03-14 02:05:34.000000 xplainable_client-1.2.4.post2/LICENSE
--rw-rw-rw-   0        0        0    45383 2024-05-18 02:28:21.831680 xplainable_client-1.2.4.post2/PKG-INFO
--rw-rw-rw-   0        0        0     4042 2024-03-09 02:04:58.000000 xplainable_client-1.2.4.post2/README.md
--rw-rw-rw-   0        0        0     1494 2024-05-17 23:36:00.000000 xplainable_client-1.2.4.post2/_build.py
--rw-rw-rw-   0        0        0       29 2024-05-18 02:28:15.000000 xplainable_client-1.2.4.post2/_version.py
--rw-rw-rw-   0        0        0      119 2024-03-09 02:04:58.000000 xplainable_client-1.2.4.post2/config.py
--rw-rw-rw-   0        0        0      392 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post2/docker-compose.yaml
--rw-rw-rw-   0        0        0      895 2024-05-18 02:27:23.000000 xplainable_client-1.2.4.post2/pyproject.toml
--rw-rw-rw-   0        0        0      152 2024-05-17 05:49:28.000000 xplainable_client-1.2.4.post2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 02:28:21.833180 xplainable_client-1.2.4.post2/setup.cfg
--rw-rw-rw-   0        0        0      873 2024-05-18 02:28:15.000000 xplainable_client-1.2.4.post2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 02:28:21.795680 xplainable_client-1.2.4.post2/tests/
--rw-rw-rw-   0        0        0     1337 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post2/tests/nanoid.sql
--rw-rw-rw-   0        0        0     2856 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post2/tests/prod-db.sql
--rw-rw-rw-   0        0        0      277 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post2/tests/test_model.py
--rw-rw-rw-   0        0        0      191 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post2/tests/test_test.py
-drwxrwxrwx   0        0        0        0 2024-05-18 02:28:21.798180 xplainable_client-1.2.4.post2/thebadboycorner/
--rw-rw-rw-   0        0        0     1596 2024-05-17 07:15:41.000000 xplainable_client-1.2.4.post2/thebadboycorner/clf_model_test_jason.py
--rw-rw-rw-   0        0        0      198 2024-05-17 06:08:34.000000 xplainable_client-1.2.4.post2/thebadboycorner/test.py
-drwxrwxrwx   0        0        0        0 2024-05-18 02:28:21.800680 xplainable_client-1.2.4.post2/xplainable_client/
--rw-rw-rw-   0        0        0       28 2024-05-17 06:02:17.000000 xplainable_client-1.2.4.post2/xplainable_client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 02:28:21.821179 xplainable_client-1.2.4.post2/xplainable_client/client/
--rw-rw-rw-   0        0        0      975 2024-05-17 06:08:34.000000 xplainable_client-1.2.4.post2/xplainable_client/client/__init__.py
--rw-rw-rw-   0        0        0      129 2024-05-10 01:22:33.000000 xplainable_client-1.2.4.post2/xplainable_client/client/_client_cog_base.py
--rw-rw-rw-   0        0        0     7535 2024-05-17 05:57:53.000000 xplainable_client-1.2.4.post2/xplainable_client/client/_collections.py
--rw-rw-rw-   0        0        0     1295 2024-05-16 08:25:13.000000 xplainable_client-1.2.4.post2/xplainable_client/client/_datasets.py
--rw-rw-rw-   0        0        0    14993 2024-05-17 05:59:23.000000 xplainable_client-1.2.4.post2/xplainable_client/client/_deployments.py
--rw-rw-rw-   0        0        0     1254 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post2/xplainable_client/client/_gpt.py
--rw-rw-rw-   0        0        0     1266 2024-05-17 05:59:23.000000 xplainable_client-1.2.4.post2/xplainable_client/client/_inference.py
--rw-rw-rw-   0        0        0     8179 2024-05-17 07:08:08.000000 xplainable_client-1.2.4.post2/xplainable_client/client/_misc.py
--rw-rw-rw-   0        0        0    21423 2024-05-17 07:11:19.000000 xplainable_client-1.2.4.post2/xplainable_client/client/_models.py
--rw-rw-rw-   0        0        0     9609 2024-05-17 07:08:08.000000 xplainable_client-1.2.4.post2/xplainable_client/client/_preprocessing.py
--rw-rw-rw-   0        0        0     4135 2024-05-17 06:47:34.000000 xplainable_client-1.2.4.post2/xplainable_client/client/_session.py
-drwxrwxrwx   0        0        0        0 2024-05-18 02:28:21.828679 xplainable_client-1.2.4.post2/xplainable_client/client/utils/
--rw-rw-rw-   0        0        0      127 2024-05-17 07:10:23.000000 xplainable_client-1.2.4.post2/xplainable_client/client/utils/__init__.py
--rw-rw-rw-   0        0        0     1334 2024-03-09 02:04:58.000000 xplainable_client-1.2.4.post2/xplainable_client/client/utils/encoders.py
--rw-rw-rw-   0        0        0      987 2024-05-17 05:57:23.000000 xplainable_client-1.2.4.post2/xplainable_client/client/utils/helpers.py
--rw-rw-rw-   0        0        0     6633 2024-05-17 07:08:08.000000 xplainable_client-1.2.4.post2/xplainable_client/client/utils/metrics.py
--rw-rw-rw-   0        0        0     3122 2024-03-09 02:04:58.000000 xplainable_client-1.2.4.post2/xplainable_client/client/utils/model_parsers.py
--rw-rw-rw-   0        0        0    10818 2024-03-14 02:05:34.000000 xplainable_client-1.2.4.post2/xplainable_client/client/utils/scanner.py
--rw-rw-rw-   0        0        0      125 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post2/xplainable_client/pytest.ini
-drwxrwxrwx   0        0        0        0 2024-05-18 02:28:21.830180 xplainable_client-1.2.4.post2/xplainable_client.egg-info/
--rw-rw-rw-   0        0        0    45383 2024-05-18 02:28:21.000000 xplainable_client-1.2.4.post2/xplainable_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1206 2024-05-18 02:28:21.000000 xplainable_client-1.2.4.post2/xplainable_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 02:28:21.000000 xplainable_client-1.2.4.post2/xplainable_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2024-05-18 02:28:21.000000 xplainable_client-1.2.4.post2/xplainable_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       51 2024-05-18 02:28:21.000000 xplainable_client-1.2.4.post2/xplainable_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 02:38:51.571044 xplainable_client-1.2.4.post3/
+-rw-rw-rw-   0        0        0     3325 2024-03-12 06:45:15.000000 xplainable_client-1.2.4.post3/.gitignore
+-rw-rw-rw-   0        0        0    35184 2024-03-14 02:05:34.000000 xplainable_client-1.2.4.post3/LICENSE
+-rw-rw-rw-   0        0        0    45382 2024-05-18 02:38:51.569544 xplainable_client-1.2.4.post3/PKG-INFO
+-rw-rw-rw-   0        0        0     4042 2024-03-09 02:04:58.000000 xplainable_client-1.2.4.post3/README.md
+-rw-rw-rw-   0        0        0     1494 2024-05-17 23:36:00.000000 xplainable_client-1.2.4.post3/_build.py
+-rw-rw-rw-   0        0        0       29 2024-05-18 02:38:47.000000 xplainable_client-1.2.4.post3/_version.py
+-rw-rw-rw-   0        0        0      119 2024-03-09 02:04:58.000000 xplainable_client-1.2.4.post3/config.py
+-rw-rw-rw-   0        0        0      392 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post3/docker-compose.yaml
+-rw-rw-rw-   0        0        0      895 2024-05-18 02:38:47.000000 xplainable_client-1.2.4.post3/pyproject.toml
+-rw-rw-rw-   0        0        0      152 2024-05-17 05:49:28.000000 xplainable_client-1.2.4.post3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 02:38:51.571044 xplainable_client-1.2.4.post3/setup.cfg
+-rw-rw-rw-   0        0        0      872 2024-05-18 02:38:47.000000 xplainable_client-1.2.4.post3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:38:51.532544 xplainable_client-1.2.4.post3/tests/
+-rw-rw-rw-   0        0        0     1337 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post3/tests/nanoid.sql
+-rw-rw-rw-   0        0        0     2856 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post3/tests/prod-db.sql
+-rw-rw-rw-   0        0        0      277 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post3/tests/test_model.py
+-rw-rw-rw-   0        0        0      191 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post3/tests/test_test.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:38:51.535044 xplainable_client-1.2.4.post3/thebadboycorner/
+-rw-rw-rw-   0        0        0     1596 2024-05-17 07:15:41.000000 xplainable_client-1.2.4.post3/thebadboycorner/clf_model_test_jason.py
+-rw-rw-rw-   0        0        0      198 2024-05-17 06:08:34.000000 xplainable_client-1.2.4.post3/thebadboycorner/test.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:38:51.537545 xplainable_client-1.2.4.post3/xplainable_client/
+-rw-rw-rw-   0        0        0       28 2024-05-17 06:02:17.000000 xplainable_client-1.2.4.post3/xplainable_client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:38:51.558044 xplainable_client-1.2.4.post3/xplainable_client/client/
+-rw-rw-rw-   0        0        0      975 2024-05-17 06:08:34.000000 xplainable_client-1.2.4.post3/xplainable_client/client/__init__.py
+-rw-rw-rw-   0        0        0      129 2024-05-10 01:22:33.000000 xplainable_client-1.2.4.post3/xplainable_client/client/_client_cog_base.py
+-rw-rw-rw-   0        0        0     7535 2024-05-17 05:57:53.000000 xplainable_client-1.2.4.post3/xplainable_client/client/_collections.py
+-rw-rw-rw-   0        0        0     1295 2024-05-16 08:25:13.000000 xplainable_client-1.2.4.post3/xplainable_client/client/_datasets.py
+-rw-rw-rw-   0        0        0    14993 2024-05-17 05:59:23.000000 xplainable_client-1.2.4.post3/xplainable_client/client/_deployments.py
+-rw-rw-rw-   0        0        0     1254 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post3/xplainable_client/client/_gpt.py
+-rw-rw-rw-   0        0        0     1266 2024-05-17 05:59:23.000000 xplainable_client-1.2.4.post3/xplainable_client/client/_inference.py
+-rw-rw-rw-   0        0        0     8179 2024-05-17 07:08:08.000000 xplainable_client-1.2.4.post3/xplainable_client/client/_misc.py
+-rw-rw-rw-   0        0        0    21423 2024-05-17 07:11:19.000000 xplainable_client-1.2.4.post3/xplainable_client/client/_models.py
+-rw-rw-rw-   0        0        0     9609 2024-05-17 07:08:08.000000 xplainable_client-1.2.4.post3/xplainable_client/client/_preprocessing.py
+-rw-rw-rw-   0        0        0     4135 2024-05-17 06:47:34.000000 xplainable_client-1.2.4.post3/xplainable_client/client/_session.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:38:51.566545 xplainable_client-1.2.4.post3/xplainable_client/client/utils/
+-rw-rw-rw-   0        0        0      127 2024-05-17 07:10:23.000000 xplainable_client-1.2.4.post3/xplainable_client/client/utils/__init__.py
+-rw-rw-rw-   0        0        0     1334 2024-03-09 02:04:58.000000 xplainable_client-1.2.4.post3/xplainable_client/client/utils/encoders.py
+-rw-rw-rw-   0        0        0      987 2024-05-17 05:57:23.000000 xplainable_client-1.2.4.post3/xplainable_client/client/utils/helpers.py
+-rw-rw-rw-   0        0        0     6633 2024-05-17 07:08:08.000000 xplainable_client-1.2.4.post3/xplainable_client/client/utils/metrics.py
+-rw-rw-rw-   0        0        0     3122 2024-03-09 02:04:58.000000 xplainable_client-1.2.4.post3/xplainable_client/client/utils/model_parsers.py
+-rw-rw-rw-   0        0        0    10818 2024-03-14 02:05:34.000000 xplainable_client-1.2.4.post3/xplainable_client/client/utils/scanner.py
+-rw-rw-rw-   0        0        0      125 2024-05-17 05:10:32.000000 xplainable_client-1.2.4.post3/xplainable_client/pytest.ini
+drwxrwxrwx   0        0        0        0 2024-05-18 02:38:51.568045 xplainable_client-1.2.4.post3/xplainable_client.egg-info/
+-rw-rw-rw-   0        0        0    45382 2024-05-18 02:38:51.000000 xplainable_client-1.2.4.post3/xplainable_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1206 2024-05-18 02:38:51.000000 xplainable_client-1.2.4.post3/xplainable_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 02:38:51.000000 xplainable_client-1.2.4.post3/xplainable_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2024-05-18 02:38:51.000000 xplainable_client-1.2.4.post3/xplainable_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       51 2024-05-18 02:38:51.000000 xplainable_client-1.2.4.post3/xplainable_client.egg-info/top_level.txt
```

### Comparing `xplainable_client-1.2.4.post2/.gitignore` & `xplainable_client-1.2.4.post3/.gitignore`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/LICENSE` & `xplainable_client-1.2.4.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/PKG-INFO` & `xplainable_client-1.2.4.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xplainable-client
-Version: 1.2.4.post2
+Version: 1.2.4.post3
 Summary: The client for persisting and deploying models to Xplainable cloud.
 Author: xplainable pty ltd
 Author-email: xplainable pty ltd <contact@xplainable.io>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -667,15 +667,15 @@
         <https://www.gnu.org/licenses/>.
         
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ipywidgets==8.0.6
 Requires-Dist: numpy>=1.26
 Requires-Dist: pandas>=1.5.2
 Requires-Dist: pyperclip==1.8.2
 Requires-Dist: Requests==2.31.0
```

### Comparing `xplainable_client-1.2.4.post2/README.md` & `xplainable_client-1.2.4.post3/README.md`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/_build.py` & `xplainable_client-1.2.4.post3/_build.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/pyproject.toml` & `xplainable_client-1.2.4.post3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages]
 find = {} 
 
 [project]
 name = "xplainable-client"
-version = "1.2.4.post2"
+version = "1.2.4.post3"
 authors = [
   { name="xplainable pty ltd", email="contact@xplainable.io" },
 ]
 description = "The client for persisting and deploying models to Xplainable cloud."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `xplainable_client-1.2.4.post2/setup.py` & `xplainable_client-1.2.4.post3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,23 +4,23 @@
     description = f.read()
 
 with open("LICENSE", "r") as f:
     license = f.read()
 
 setuptools.setup(
     name="xplainable-client",
-    version="1.2.4.post2",
+    version="1.2.4.post3",
     author="xplainable pty ltd",
     author_email="contact@xplainable.io",
     packages=["xplainable_client"],
     description="The client for persisting and deploying models to Xplainable cloud.",
     long_description=description,
     long_description_content_type="text/markdown",
     license=license,
-    python_requires='>=3.11',
+    python_requires='>=3.8',
     install_requires=[
         "ipywidgets==8.0.6",
         "numpy>=1.26",
         "pandas>=1.5.2",
         "pyperclip==1.8.2",
         "Requests==2.31.0",
         "scikit_learn",
```

### Comparing `xplainable_client-1.2.4.post2/tests/nanoid.sql` & `xplainable_client-1.2.4.post3/tests/nanoid.sql`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/tests/prod-db.sql` & `xplainable_client-1.2.4.post3/tests/prod-db.sql`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/thebadboycorner/clf_model_test_jason.py` & `xplainable_client-1.2.4.post3/thebadboycorner/clf_model_test_jason.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/xplainable_client/client/__init__.py` & `xplainable_client-1.2.4.post3/xplainable_client/client/__init__.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/xplainable_client/client/_collections.py` & `xplainable_client-1.2.4.post3/xplainable_client/client/_collections.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/xplainable_client/client/_datasets.py` & `xplainable_client-1.2.4.post3/xplainable_client/client/_datasets.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/xplainable_client/client/_deployments.py` & `xplainable_client-1.2.4.post3/xplainable_client/client/_deployments.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/xplainable_client/client/_gpt.py` & `xplainable_client-1.2.4.post3/xplainable_client/client/_gpt.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/xplainable_client/client/_inference.py` & `xplainable_client-1.2.4.post3/xplainable_client/client/_inference.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/xplainable_client/client/_misc.py` & `xplainable_client-1.2.4.post3/xplainable_client/client/_misc.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/xplainable_client/client/_models.py` & `xplainable_client-1.2.4.post3/xplainable_client/client/_models.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/xplainable_client/client/_preprocessing.py` & `xplainable_client-1.2.4.post3/xplainable_client/client/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/xplainable_client/client/_session.py` & `xplainable_client-1.2.4.post3/xplainable_client/client/_session.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/xplainable_client/client/utils/encoders.py` & `xplainable_client-1.2.4.post3/xplainable_client/client/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/xplainable_client/client/utils/helpers.py` & `xplainable_client-1.2.4.post3/xplainable_client/client/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/xplainable_client/client/utils/metrics.py` & `xplainable_client-1.2.4.post3/xplainable_client/client/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/xplainable_client/client/utils/model_parsers.py` & `xplainable_client-1.2.4.post3/xplainable_client/client/utils/model_parsers.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/xplainable_client/client/utils/scanner.py` & `xplainable_client-1.2.4.post3/xplainable_client/client/utils/scanner.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.4.post2/xplainable_client.egg-info/PKG-INFO` & `xplainable_client-1.2.4.post3/xplainable_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xplainable-client
-Version: 1.2.4.post2
+Version: 1.2.4.post3
 Summary: The client for persisting and deploying models to Xplainable cloud.
 Author: xplainable pty ltd
 Author-email: xplainable pty ltd <contact@xplainable.io>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -667,15 +667,15 @@
         <https://www.gnu.org/licenses/>.
         
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ipywidgets==8.0.6
 Requires-Dist: numpy>=1.26
 Requires-Dist: pandas>=1.5.2
 Requires-Dist: pyperclip==1.8.2
 Requires-Dist: Requests==2.31.0
```

### Comparing `xplainable_client-1.2.4.post2/xplainable_client.egg-info/SOURCES.txt` & `xplainable_client-1.2.4.post3/xplainable_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

