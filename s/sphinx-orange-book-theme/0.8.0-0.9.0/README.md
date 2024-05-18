# Comparing `tmp/sphinx_orange_book_theme-0.8.0.tar.gz` & `tmp/sphinx_orange_book_theme-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_orange_book_theme-0.8.0.tar", max compression
+gzip compressed data, was "sphinx_orange_book_theme-0.9.0.tar", max compression
```

## Comparing `sphinx_orange_book_theme-0.8.0.tar` & `sphinx_orange_book_theme-0.9.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-04-29 16:23:42.134320 sphinx_orange_book_theme-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     1812 2024-04-29 16:23:42.134320 sphinx_orange_book_theme-0.8.0/README.md
--rw-r--r--   0        0        0     2008 2024-04-29 16:23:42.137320 sphinx_orange_book_theme-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      365 2024-04-29 16:23:42.137320 sphinx_orange_book_theme-0.8.0/sphinx_orange_book_theme/__init__.py
--rw-r--r--   0        0        0     2691 2024-04-29 16:23:42.137320 sphinx_orange_book_theme-0.8.0/sphinx_orange_book_theme/static/styles/sphinx-orange-book-theme-colors.css
--rw-r--r--   0        0        0     1216 2024-04-29 16:23:42.137320 sphinx_orange_book_theme-0.8.0/sphinx_orange_book_theme/static/styles/sphinx-orange-book-theme.css
--rw-r--r--   0        0        0       85 2024-04-29 16:23:42.137320 sphinx_orange_book_theme-0.8.0/sphinx_orange_book_theme/theme.conf
--rw-r--r--   0        0        0     3065 1970-01-01 00:00:00.000000 sphinx_orange_book_theme-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-18 12:25:18.496177 sphinx_orange_book_theme-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     1812 2024-05-18 12:25:18.496177 sphinx_orange_book_theme-0.9.0/README.md
+-rw-r--r--   0        0        0     2008 2024-05-18 12:25:18.501177 sphinx_orange_book_theme-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      365 2024-05-18 12:25:18.501177 sphinx_orange_book_theme-0.9.0/sphinx_orange_book_theme/__init__.py
+-rw-r--r--   0        0        0     2695 2024-05-18 12:25:18.501177 sphinx_orange_book_theme-0.9.0/sphinx_orange_book_theme/static/styles/sphinx-orange-book-theme-colors.css
+-rw-r--r--   0        0        0     1216 2024-05-18 12:25:18.501177 sphinx_orange_book_theme-0.9.0/sphinx_orange_book_theme/static/styles/sphinx-orange-book-theme.css
+-rw-r--r--   0        0        0       85 2024-05-18 12:25:18.501177 sphinx_orange_book_theme-0.9.0/sphinx_orange_book_theme/theme.conf
+-rw-r--r--   0        0        0     3065 1970-01-01 00:00:00.000000 sphinx_orange_book_theme-0.9.0/PKG-INFO
```

### Comparing `sphinx_orange_book_theme-0.8.0/LICENSE.txt` & `sphinx_orange_book_theme-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sphinx_orange_book_theme-0.8.0/README.md` & `sphinx_orange_book_theme-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `sphinx_orange_book_theme-0.8.0/pyproject.toml` & `sphinx_orange_book_theme-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinx-orange-book-theme"
-version = "0.8.0"
+version = "0.9.0"
 description = "An orange version of sphinx-book-theme."
 authors = ["Kenta Kabashima <kenta_program37@hotmail.co.jp>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/MusicScience37Projects/utility-libraries/sphinx-orange-book-theme"
 documentation = "https://sphinx-orange-book-theme-musicscience37projects--1dc46f9ab80e60.gitlab.io/"
 repository = "https://gitlab.com/MusicScience37Projects/utility-libraries/sphinx-orange-book-theme.git"
```

### Comparing `sphinx_orange_book_theme-0.8.0/sphinx_orange_book_theme/static/styles/sphinx-orange-book-theme-colors.css` & `sphinx_orange_book_theme-0.9.0/sphinx_orange_book_theme/static/styles/sphinx-orange-book-theme-colors.css`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,20 @@
   /* violet in the original theme */
   --pst-color-secondary: #a68715;
   --pst-color-secondary-bg: #ffebbc;
   /* pink in the original theme */
   --pst-color-accent: #379f14;
   --pst-color-accent-bg: #e2f2d9;
   /* gray in the original theme */
-  --pst-color-background: white;
-  --pst-color-on-background: white;
+  --pst-color-background: #fefdfc;
+  --pst-color-on-background: #fefdfc;
   --pst-color-surface: #fef4ef;
   --pst-color-on-surface: #3f2213;
   --pst-color-text-base: #2d2826;
-  --pst-color-text-muted: #7e6d65;
+  --pst-color-text-muted: #61554f;
   --pst-color-border: #c6bab4;
   --pst-color-border-muted: #dad3cf;
   /* info, warning, success, danger */
   --pst-color-info: #379f14;
   --pst-color-info-bg: #e2f2d9;
   --pst-color-warning: #a68715;
   --pst-color-warning-bg: #ffebbc;
```

### Comparing `sphinx_orange_book_theme-0.8.0/sphinx_orange_book_theme/static/styles/sphinx-orange-book-theme.css` & `sphinx_orange_book_theme-0.9.0/sphinx_orange_book_theme/static/styles/sphinx-orange-book-theme.css`

 * *Files identical despite different names*

### Comparing `sphinx_orange_book_theme-0.8.0/PKG-INFO` & `sphinx_orange_book_theme-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-orange-book-theme
-Version: 0.8.0
+Version: 0.9.0
 Summary: An orange version of sphinx-book-theme.
 Home-page: https://gitlab.com/MusicScience37Projects/utility-libraries/sphinx-orange-book-theme
 License: MIT
 Keywords: sphinx
 Author: Kenta Kabashima
 Author-email: kenta_program37@hotmail.co.jp
 Requires-Python: >=3.10,<3.13
```

