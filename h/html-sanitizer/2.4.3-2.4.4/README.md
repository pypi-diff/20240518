# Comparing `tmp/html_sanitizer-2.4.3.tar.gz` & `tmp/html_sanitizer-2.4.4.tar.gz`

## Comparing `html_sanitizer-2.4.3.tar` & `html_sanitizer-2.4.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/.editorconfig
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/CHANGELOG.rst
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/tox.ini
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/html_sanitizer/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/html_sanitizer/__main__.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/html_sanitizer/django.py
--rw-r--r--   0        0        0    13871 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/html_sanitizer/sanitizer.py
--rw-r--r--   0        0        0    25020 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/html_sanitizer/tests.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/.gitignore
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/LICENSE
--rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/README.rst
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/pyproject.toml
--rw-r--r--   0        0        0     7920 2020-02-02 00:00:00.000000 html_sanitizer-2.4.3/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 html_sanitizer-2.4.4/.editorconfig
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 html_sanitizer-2.4.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 html_sanitizer-2.4.4/CHANGELOG.rst
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 html_sanitizer-2.4.4/tox.ini
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 html_sanitizer-2.4.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 html_sanitizer-2.4.4/html_sanitizer/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 html_sanitizer-2.4.4/html_sanitizer/__main__.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 html_sanitizer-2.4.4/html_sanitizer/django.py
+-rw-r--r--   0        0        0    13913 2020-02-02 00:00:00.000000 html_sanitizer-2.4.4/html_sanitizer/sanitizer.py
+-rw-r--r--   0        0        0    25265 2020-02-02 00:00:00.000000 html_sanitizer-2.4.4/html_sanitizer/tests.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 html_sanitizer-2.4.4/.gitignore
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 html_sanitizer-2.4.4/LICENSE
+-rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 html_sanitizer-2.4.4/README.rst
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 html_sanitizer-2.4.4/pyproject.toml
+-rw-r--r--   0        0        0     7920 2020-02-02 00:00:00.000000 html_sanitizer-2.4.4/PKG-INFO
```

### Comparing `html_sanitizer-2.4.3/.pre-commit-config.yaml` & `html_sanitizer-2.4.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.3/CHANGELOG.rst` & `html_sanitizer-2.4.4/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.3/.github/workflows/test.yml` & `html_sanitizer-2.4.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.3/html_sanitizer/django.py` & `html_sanitizer-2.4.4/html_sanitizer/django.py`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.3/html_sanitizer/sanitizer.py` & `html_sanitizer-2.4.4/html_sanitizer/sanitizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,24 +111,27 @@
         element.attrib["name"] = element.attrib["id"]
     return element
 
 
 def normalize_whitespace_in_text_or_tail(
     element, *, whitespace_re=None, keep_typographic_whitespace=False
 ):
+    if keep_typographic_whitespace:
+        return element
+
     if whitespace_re is None:
         whitespace_re = re.compile(r"\s+")
-    if element.text and not keep_typographic_whitespace:
+    if element.text:
         while True:
             text = whitespace_re.sub(" ", element.text)
             if element.text == text:
                 break
             element.text = text
 
-    if element.tail and not keep_typographic_whitespace:
+    if element.tail:
         while True:
             text = whitespace_re.sub(" ", element.tail)
             if element.tail == text:
                 break
             element.tail = text
 
     return element
@@ -376,15 +379,16 @@
                                 element.text or "", element.tail or "", nx.text
                             )
 
                     for child in nx:
                         element.append(child)
 
                     # tail is merged with previous element.
-                    nx.drop_tree()
+                    element.tail = nx.tail
+                    nx.getparent().remove(nx)
 
                     # Process element again
                     backlog.append(element)
                     continue
 
             for processor in self.element_postprocessors:
                 element = processor(element)
```

### Comparing `html_sanitizer-2.4.3/html_sanitizer/tests.py` & `html_sanitizer-2.4.4/html_sanitizer/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         )
 
         self.run_tests(entries)
 
     def test_03_merge(self):
         entries = (
             ("<h2>foo</h2><h2>bar</h2>", "<h2>foobar</h2>"),
-            ("<h2>foo  </h2>   <h2>   bar</h2>", "<h2>foo bar</h2> "),
+            ("<h2>foo  </h2>   <h2>   bar</h2>", "<h2>foo bar</h2>"),
         )
 
         self.run_tests(entries)
 
     def test_no_space_between_same_tags(self):
         entries = [
             ("<strong>Hel</strong><strong>lo</strong>", "<strong>Hello</strong>")
@@ -663,20 +663,26 @@
                     "\uff1cimg src=x onerror=\uff02alert(window.location)\uff02\uff1e",
                     "",
                 ),
             ]
         )
 
     def test_typographic_whitespace_tags_merging(self):
-        html = "This is <strong>some</strong> <strong>text</strong> with adjacent tags."
         sanitizer = Sanitizer(
             {
                 "whitespace": set(),
                 "keep_typographic_whitespace": True,
             }
         )
         self.run_tests(
             [
-                (html, "This is <strong>some text</strong>  with adjacent tags."),
+                (
+                    "This is <strong>some</strong> <strong>text</strong> with adjacent tags.",
+                    "This is <strong>some text</strong> with adjacent tags.",
+                ),
+                (
+                    "This is <strong>some</strong> <strong>text</strong>with adjacent tags.",
+                    "This is <strong>some text</strong>with adjacent tags.",
+                ),
             ],
             sanitizer=sanitizer,
         )
```

### Comparing `html_sanitizer-2.4.3/LICENSE` & `html_sanitizer-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.3/README.rst` & `html_sanitizer-2.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.3/pyproject.toml` & `html_sanitizer-2.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.3/PKG-INFO` & `html_sanitizer-2.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: html-sanitizer
-Version: 2.4.3
+Version: 2.4.4
 Summary: HTML sanitizer
 Project-URL: Homepage, https://github.com/matthiask/html-sanitizer/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

