# Comparing `tmp/distyll_info-0.2.2.tar.gz` & `tmp/distyll_info-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distyll_info-0.2.2.tar", max compression
+gzip compressed data, was "distyll_info-0.2.3.tar", max compression
```

## Comparing `distyll_info-0.2.2.tar` & `distyll_info-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1058 2024-03-05 21:09:40.618601 distyll_info-0.2.2/README.md
--rw-r--r--   0        0        0      588 2024-03-05 21:29:13.492164 distyll_info-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      109 2024-03-05 21:28:53.223453 distyll_info-0.2.2/src/distyll/__init__.py
--rw-r--r--   0        0        0      110 2024-03-05 20:48:18.972098 distyll_info-0.2.2/src/distyll/config.py
--rw-r--r--   0        0        0     2143 2024-03-05 21:20:46.794751 distyll_info-0.2.2/src/distyll/db.py
--rw-r--r--   0        0        0      186 2024-03-05 19:57:41.677116 distyll_info-0.2.2/src/distyll/loggerconfig.py
--rw-r--r--   0        0        0       89 2024-03-05 21:28:53.227286 distyll_info-0.2.2/src/distyll/text/__init__.py
--rw-r--r--   0        0        0     2938 2024-03-05 20:52:11.237125 distyll_info-0.2.2/src/distyll/text/text.py
--rw-r--r--   0        0        0      104 2024-03-05 21:28:53.229015 distyll_info-0.2.2/src/distyll/transcripts/__init__.py
--rw-r--r--   0        0        0     2617 2024-03-05 20:53:15.041741 distyll_info-0.2.2/src/distyll/transcripts/transcripts.py
--rw-r--r--   0        0        0    11674 2024-03-05 21:28:53.292900 distyll_info-0.2.2/src/distyll/utils.py
--rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 distyll_info-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-03-05 21:09:40.618601 distyll_info-0.2.3/README.md
+-rw-r--r--   0        0        0      588 2024-05-18 11:51:44.304115 distyll_info-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      109 2024-05-18 11:51:33.424409 distyll_info-0.2.3/src/distyll/__init__.py
+-rw-r--r--   0        0        0      141 2024-05-18 11:47:11.878086 distyll_info-0.2.3/src/distyll/config.py
+-rw-r--r--   0        0        0     3951 2024-05-18 11:51:18.309898 distyll_info-0.2.3/src/distyll/db.py
+-rw-r--r--   0        0        0      186 2024-03-05 19:57:41.677116 distyll_info-0.2.3/src/distyll/loggerconfig.py
+-rw-r--r--   0        0        0       89 2024-03-05 21:28:53.227286 distyll_info-0.2.3/src/distyll/text/__init__.py
+-rw-r--r--   0        0        0     2938 2024-03-05 20:52:11.237125 distyll_info-0.2.3/src/distyll/text/text.py
+-rw-r--r--   0        0        0      104 2024-03-05 21:28:53.229015 distyll_info-0.2.3/src/distyll/transcripts/__init__.py
+-rw-r--r--   0        0        0     2617 2024-03-05 20:53:15.041741 distyll_info-0.2.3/src/distyll/transcripts/transcripts.py
+-rw-r--r--   0        0        0    11674 2024-03-05 21:28:53.292900 distyll_info-0.2.3/src/distyll/utils.py
+-rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 distyll_info-0.2.3/PKG-INFO
```

### Comparing `distyll_info-0.2.2/README.md` & `distyll_info-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `distyll_info-0.2.2/pyproject.toml` & `distyll_info-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "distyll-info"
-version = "0.2.2"
+version = "0.2.3"
 description = "Information parsing assistant"
 authors = ["JP Hwang <61258750+databyjp@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "distyll", from="src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `distyll_info-0.2.2/src/distyll/text/text.py` & `distyll_info-0.2.3/src/distyll/text/text.py`

 * *Files identical despite different names*

### Comparing `distyll_info-0.2.2/src/distyll/transcripts/transcripts.py` & `distyll_info-0.2.3/src/distyll/transcripts/transcripts.py`

 * *Files identical despite different names*

### Comparing `distyll_info-0.2.2/src/distyll/utils.py` & `distyll_info-0.2.3/src/distyll/utils.py`

 * *Files identical despite different names*

### Comparing `distyll_info-0.2.2/PKG-INFO` & `distyll_info-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distyll-info
-Version: 0.2.2
+Version: 0.2.3
 Summary: Information parsing assistant
 License: MIT
 Author: JP Hwang
 Author-email: 61258750+databyjp@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

