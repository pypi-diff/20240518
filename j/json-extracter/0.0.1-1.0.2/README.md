# Comparing `tmp/json_extracter-0.0.1.tar.gz` & `tmp/json_extracter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_extracter-0.0.1.tar", last modified: Tue May  7 04:19:11 2024, max compression
+gzip compressed data, was "json_extracter-1.0.2.tar", last modified: Fri May 17 22:56:25 2024, max compression
```

## Comparing `json_extracter-0.0.1.tar` & `json_extracter-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 edy       (1000) edy       (1000)        0 2024-05-07 04:19:11.225121 json_extracter-0.0.1/
--rw-rw-r--   0 edy       (1000) edy       (1000)     1073 2024-05-07 04:03:04.000000 json_extracter-0.0.1/LICENSE
--rw-r--r--   0 edy       (1000) edy       (1000)      502 2024-05-07 04:19:11.225121 json_extracter-0.0.1/PKG-INFO
--rw-rw-r--   0 edy       (1000) edy       (1000)        0 2024-05-07 04:02:18.000000 json_extracter-0.0.1/README.md
--rw-rw-r--   0 edy       (1000) edy       (1000)      484 2024-05-07 04:18:54.000000 json_extracter-0.0.1/pyproject.toml
--rw-rw-r--   0 edy       (1000) edy       (1000)       38 2024-05-07 04:19:11.225121 json_extracter-0.0.1/setup.cfg
-drwxrwxr-x   0 edy       (1000) edy       (1000)        0 2024-05-07 04:19:11.221121 json_extracter-0.0.1/src/
--rw-rw-r--   0 edy       (1000) edy       (1000)       55 2024-05-07 03:58:09.000000 json_extracter-0.0.1/src/__init__.py
-drwxrwxr-x   0 edy       (1000) edy       (1000)        0 2024-05-07 04:19:11.221121 json_extracter-0.0.1/src/json_extracter.egg-info/
--rw-r--r--   0 edy       (1000) edy       (1000)      502 2024-05-07 04:19:11.000000 json_extracter-0.0.1/src/json_extracter.egg-info/PKG-INFO
--rw-rw-r--   0 edy       (1000) edy       (1000)      258 2024-05-07 04:19:11.000000 json_extracter-0.0.1/src/json_extracter.egg-info/SOURCES.txt
--rw-rw-r--   0 edy       (1000) edy       (1000)        1 2024-05-07 04:19:11.000000 json_extracter-0.0.1/src/json_extracter.egg-info/dependency_links.txt
--rw-rw-r--   0 edy       (1000) edy       (1000)       15 2024-05-07 04:19:11.000000 json_extracter-0.0.1/src/json_extracter.egg-info/top_level.txt
-drwxrwxr-x   0 edy       (1000) edy       (1000)        0 2024-05-07 04:19:11.221121 json_extracter-0.0.1/src/jsonx/
--rw-rw-r--   0 edy       (1000) edy       (1000)        0 2024-05-07 03:57:52.000000 json_extracter-0.0.1/src/jsonx/__init__.py
--rw-rw-r--   0 edy       (1000) edy       (1000)     1457 2024-05-07 01:22:18.000000 json_extracter-0.0.1/src/jsonx/modulo.py
+drwxrwxr-x   0 edy       (1000) edy       (1000)        0 2024-05-17 22:56:25.753949 json_extracter-1.0.2/
+-rw-rw-r--   0 edy       (1000) edy       (1000)     1054 2024-05-17 22:46:04.000000 json_extracter-1.0.2/LICENSE
+-rw-r--r--   0 edy       (1000) edy       (1000)     1879 2024-05-17 22:56:25.753949 json_extracter-1.0.2/PKG-INFO
+-rw-rw-r--   0 edy       (1000) edy       (1000)     1375 2024-05-17 22:53:19.000000 json_extracter-1.0.2/README.md
+-rw-rw-r--   0 edy       (1000) edy       (1000)      484 2024-05-17 22:56:22.000000 json_extracter-1.0.2/pyproject.toml
+-rw-rw-r--   0 edy       (1000) edy       (1000)       38 2024-05-17 22:56:25.753949 json_extracter-1.0.2/setup.cfg
+drwxrwxr-x   0 edy       (1000) edy       (1000)        0 2024-05-17 22:56:25.753949 json_extracter-1.0.2/src/
+-rw-rw-r--   0 edy       (1000) edy       (1000)       60 2024-05-17 22:47:05.000000 json_extracter-1.0.2/src/__init__.py
+drwxrwxr-x   0 edy       (1000) edy       (1000)        0 2024-05-17 22:56:25.753949 json_extracter-1.0.2/src/json_extracter.egg-info/
+-rw-r--r--   0 edy       (1000) edy       (1000)     1879 2024-05-17 22:56:25.000000 json_extracter-1.0.2/src/json_extracter.egg-info/PKG-INFO
+-rw-rw-r--   0 edy       (1000) edy       (1000)      258 2024-05-17 22:56:25.000000 json_extracter-1.0.2/src/json_extracter.egg-info/SOURCES.txt
+-rw-rw-r--   0 edy       (1000) edy       (1000)        1 2024-05-17 22:56:25.000000 json_extracter-1.0.2/src/json_extracter.egg-info/dependency_links.txt
+-rw-rw-r--   0 edy       (1000) edy       (1000)       15 2024-05-17 22:56:25.000000 json_extracter-1.0.2/src/json_extracter.egg-info/top_level.txt
+drwxrwxr-x   0 edy       (1000) edy       (1000)        0 2024-05-17 22:56:25.753949 json_extracter-1.0.2/src/jsonx/
+-rw-rw-r--   0 edy       (1000) edy       (1000)        0 2024-05-07 03:57:52.000000 json_extracter-1.0.2/src/jsonx/__init__.py
+-rw-rw-r--   0 edy       (1000) edy       (1000)     1462 2024-05-17 22:46:57.000000 json_extracter-1.0.2/src/jsonx/modulo.py
```

### Comparing `json_extracter-0.0.1/LICENSE` & `json_extracter-1.0.2/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Copyright (c) 2018 The Python Packaging Authority
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+to use, copy, modify, merge, publish, and distribute copies of the Software,
+and to permit persons to whom the Software is furnished to do so, subject to
+the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
+
```

### Comparing `json_extracter-0.0.1/src/jsonx/modulo.py` & `json_extracter-1.0.2/src/jsonx/modulo.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     if key_close_bracket < key_close_square_bracket:
         return open_text_clean[:key_close_square_bracket] + open_text_clean[key_close_square_bracket]
 
     if key_close_bracket > key_close_square_bracket:
         return open_text_clean[:key_close_bracket] + open_text_clean[key_close_bracket]
 
 
-def jsonc(txt):
+def json_parse(txt):
     txt_2 = str(txt.replace("\n", ""))
     text = re.sub(r'\s+', '', txt_2)
 
     # when open is {
     key_open_bracket = text.find("{")
 
     # when open is [
```

