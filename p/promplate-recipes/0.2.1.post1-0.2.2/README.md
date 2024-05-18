# Comparing `tmp/promplate_recipes-0.2.1.post1.tar.gz` & `tmp/promplate_recipes-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promplate_recipes-0.2.1.post1.tar", last modified: Thu May 16 12:25:57 2024, max compression
+gzip compressed data, was "promplate_recipes-0.2.2.tar", last modified: Sat May 18 02:41:20 2024, max compression
```

## Comparing `promplate_recipes-0.2.1.post1.tar` & `promplate_recipes-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,9 @@
--rw-r--r--   0        0        0      200 2024-04-10 06:40:35.413855 promplate_recipes-0.2.1.post1/promplate_recipes/__init__.py
--rw-r--r--   0        0        0     2191 2024-05-16 12:21:26.190215 promplate_recipes-0.2.1.post1/promplate_recipes/context.py
--rw-r--r--   0        0        0       54 2024-05-16 12:25:50.750377 promplate_recipes-0.2.1.post1/promplate_recipes/version.py
--rw-r--r--   0        0        0      697 2024-05-16 12:25:57.972896 promplate_recipes-0.2.1.post1/pyproject.toml
--rw-r--r--   0        0        0      214 1970-01-01 00:00:00.000000 promplate_recipes-0.2.1.post1/PKG-INFO
+-rw-r--r--   0        0        0      405 2024-05-18 02:37:49.089513 promplate_recipes-0.2.2/README.md
+-rw-r--r--   0        0        0      200 2024-04-10 06:40:35.413855 promplate_recipes-0.2.2/promplate_recipes/__init__.py
+-rw-r--r--   0        0        0     2191 2024-05-16 12:21:26.190215 promplate_recipes-0.2.2/promplate_recipes/context.py
+-rw-r--r--   0        0        0      310 2024-05-18 02:13:00.872909 promplate_recipes-0.2.2/promplate_recipes/functional/_common.py
+-rw-r--r--   0        0        0      959 2024-05-18 02:16:05.089644 promplate_recipes-0.2.2/promplate_recipes/functional/component.py
+-rw-r--r--   0        0        0     2694 2024-05-18 02:16:14.920200 promplate_recipes-0.2.2/promplate_recipes/functional/node.py
+-rw-r--r--   0        0        0       48 2024-05-18 02:21:37.450478 promplate_recipes-0.2.2/promplate_recipes/version.py
+-rw-r--r--   0        0        0      712 2024-05-18 02:41:20.370098 promplate_recipes-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 promplate_recipes-0.2.2/PKG-INFO
```

### Comparing `promplate_recipes-0.2.1.post1/promplate_recipes/context.py` & `promplate_recipes-0.2.2/promplate_recipes/context.py`

 * *Files identical despite different names*

### Comparing `promplate_recipes-0.2.1.post1/pyproject.toml` & `promplate_recipes-0.2.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,16 @@
     { name = "Muspi Merol", email = "me@promplate.dev" },
 ]
 dependencies = [
     "promplate~=0.3.4",
     "python-box~=7.1.1",
 ]
 requires-python = ">=3.10"
-version = "0.2.1.post1"
+readme = "README.md"
+version = "0.2.2"
 
 [project.license]
 text = "MIT"
 
 [tool.pdm]
 distribution = true
```

