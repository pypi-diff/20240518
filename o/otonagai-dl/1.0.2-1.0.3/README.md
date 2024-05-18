# Comparing `tmp/otonagai_dl-1.0.2.tar.gz` & `tmp/otonagai_dl-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otonagai_dl-1.0.2.tar", max compression
+gzip compressed data, was "otonagai_dl-1.0.3.tar", max compression
```

## Comparing `otonagai_dl-1.0.2.tar` & `otonagai_dl-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      226 2024-05-17 06:29:48.933720 otonagai_dl-1.0.2/otonagai_dl/main.py
--rw-r--r--   0        0        0        0 2024-05-07 09:23:59.995430 otonagai_dl-1.0.2/otonagai_dl/src/__init__.py
--rw-r--r--   0        0        0     6824 2024-05-18 11:05:43.333195 otonagai_dl-1.0.2/otonagai_dl/src/controller.py
--rw-r--r--   0        0        0        0 2024-05-07 09:25:40.767261 otonagai_dl-1.0.2/otonagai_dl/src/hobby_link_jp_scraper/__init__.py
--rw-r--r--   0        0        0     1347 2024-05-17 05:46:07.038979 otonagai_dl-1.0.2/otonagai_dl/src/hobby_link_jp_scraper/hlj_batch.py
--rw-r--r--   0        0        0     4383 2024-05-17 06:32:03.828672 otonagai_dl-1.0.2/otonagai_dl/src/hobby_link_jp_scraper/hlj_dl.py
--rw-r--r--   0        0        0     2554 2024-05-15 10:46:22.439118 otonagai_dl-1.0.2/otonagai_dl/src/hobby_link_jp_scraper/hlj_ui.py
--rw-r--r--   0        0        0      422 2024-05-18 12:07:13.340683 otonagai_dl-1.0.2/otonagai_dl/src/log_system.py
--rw-r--r--   0        0        0     3693 2024-05-18 11:31:17.507722 otonagai_dl-1.0.2/otonagai_dl/src/menu.py
--rw-r--r--   0        0        0     9230 2024-05-17 06:41:10.963559 otonagai_dl-1.0.2/otonagai_dl/src/model.py
--rw-r--r--   0        0        0     3431 2024-05-18 12:14:01.518347 otonagai_dl-1.0.2/otonagai_dl/src/utils.py
--rw-r--r--   0        0        0     6736 2024-05-15 10:45:41.837124 otonagai_dl-1.0.2/otonagai_dl/src/view.py
--rw-r--r--   0        0        0      544 2024-05-18 12:14:09.416893 otonagai_dl-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      695 2024-05-17 06:43:17.878317 otonagai_dl-1.0.2/README.md
--rw-r--r--   0        0        0     1392 1970-01-01 00:00:00.000000 otonagai_dl-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      226 2024-05-17 06:29:48.933720 otonagai_dl-1.0.3/otonagai_dl/main.py
+-rw-r--r--   0        0        0        0 2024-05-07 09:23:59.995430 otonagai_dl-1.0.3/otonagai_dl/src/__init__.py
+-rw-r--r--   0        0        0     6824 2024-05-18 11:05:43.333195 otonagai_dl-1.0.3/otonagai_dl/src/controller.py
+-rw-r--r--   0        0        0        0 2024-05-07 09:25:40.767261 otonagai_dl-1.0.3/otonagai_dl/src/hobby_link_jp_scraper/__init__.py
+-rw-r--r--   0        0        0     1347 2024-05-17 05:46:07.038979 otonagai_dl-1.0.3/otonagai_dl/src/hobby_link_jp_scraper/hlj_batch.py
+-rw-r--r--   0        0        0     4383 2024-05-17 06:32:03.828672 otonagai_dl-1.0.3/otonagai_dl/src/hobby_link_jp_scraper/hlj_dl.py
+-rw-r--r--   0        0        0     2554 2024-05-15 10:46:22.439118 otonagai_dl-1.0.3/otonagai_dl/src/hobby_link_jp_scraper/hlj_ui.py
+-rw-r--r--   0        0        0      418 2024-05-18 12:16:33.233471 otonagai_dl-1.0.3/otonagai_dl/src/log_system.py
+-rw-r--r--   0        0        0     3693 2024-05-18 11:31:17.507722 otonagai_dl-1.0.3/otonagai_dl/src/menu.py
+-rw-r--r--   0        0        0     9230 2024-05-17 06:41:10.963559 otonagai_dl-1.0.3/otonagai_dl/src/model.py
+-rw-r--r--   0        0        0     3431 2024-05-18 12:14:01.518347 otonagai_dl-1.0.3/otonagai_dl/src/utils.py
+-rw-r--r--   0        0        0     6736 2024-05-15 10:45:41.837124 otonagai_dl-1.0.3/otonagai_dl/src/view.py
+-rw-r--r--   0        0        0      544 2024-05-18 12:16:42.523539 otonagai_dl-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      695 2024-05-17 06:43:17.878317 otonagai_dl-1.0.3/README.md
+-rw-r--r--   0        0        0     1392 1970-01-01 00:00:00.000000 otonagai_dl-1.0.3/PKG-INFO
```

### Comparing `otonagai_dl-1.0.2/otonagai_dl/src/controller.py` & `otonagai_dl-1.0.3/otonagai_dl/src/controller.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.2/otonagai_dl/src/hobby_link_jp_scraper/hlj_batch.py` & `otonagai_dl-1.0.3/otonagai_dl/src/hobby_link_jp_scraper/hlj_batch.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.2/otonagai_dl/src/hobby_link_jp_scraper/hlj_dl.py` & `otonagai_dl-1.0.3/otonagai_dl/src/hobby_link_jp_scraper/hlj_dl.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.2/otonagai_dl/src/hobby_link_jp_scraper/hlj_ui.py` & `otonagai_dl-1.0.3/otonagai_dl/src/hobby_link_jp_scraper/hlj_ui.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.2/otonagai_dl/src/menu.py` & `otonagai_dl-1.0.3/otonagai_dl/src/menu.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.2/otonagai_dl/src/model.py` & `otonagai_dl-1.0.3/otonagai_dl/src/model.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.2/otonagai_dl/src/utils.py` & `otonagai_dl-1.0.3/otonagai_dl/src/utils.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.2/otonagai_dl/src/view.py` & `otonagai_dl-1.0.3/otonagai_dl/src/view.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.2/pyproject.toml` & `otonagai_dl-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "otonagai-dl"
-version = "1.0.2"
+version = "1.0.3"
 description = "A basic CLI tool to keep track of your favourite anime/manga/comics/pop culture merchandise"
 authors = ["Clavin Dsouza <clavind12@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rich = "^13.7.1"
```

### Comparing `otonagai_dl-1.0.2/README.md` & `otonagai_dl-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.2/PKG-INFO` & `otonagai_dl-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otonagai-dl
-Version: 1.0.2
+Version: 1.0.3
 Summary: A basic CLI tool to keep track of your favourite anime/manga/comics/pop culture merchandise
 Author: Clavin Dsouza
 Author-email: clavind12@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

