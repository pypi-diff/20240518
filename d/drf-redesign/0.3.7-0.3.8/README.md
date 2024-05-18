# Comparing `tmp/drf_redesign-0.3.7.tar.gz` & `tmp/drf_redesign-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_redesign-0.3.7.tar", max compression
+gzip compressed data, was "drf_redesign-0.3.8.tar", max compression
```

## Comparing `drf_redesign-0.3.7.tar` & `drf_redesign-0.3.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1074 2024-05-14 07:32:28.375659 drf_redesign-0.3.7/LICENSE
--rw-r--r--   0        0        0     3571 2024-05-14 07:32:28.375659 drf_redesign-0.3.7/README.md
--rw-r--r--   0        0        0       91 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/__init__.py
--rw-r--r--   0        0        0      235 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/apps.py
--rw-r--r--   0        0        0    27870 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/api.html
--rw-r--r--   0        0        0     1884 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      684 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      585 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0     1004 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1762 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1636 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1617 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1398 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1433 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0     1006 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     1004 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/inline/checkbox.html
--rw-r--r--   0        0        0     1766 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/inline/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/inline/dict_field.html
--rw-r--r--   0        0        0      427 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/inline/fieldset.html
--rw-r--r--   0        0        0      150 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/inline/form.html
--rw-r--r--   0        0        0     1307 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/inline/input.html
--rw-r--r--   0        0        0      262 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/inline/list_field.html
--rw-r--r--   0        0        0      330 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/inline/list_fieldset.html
--rw-r--r--   0        0        0     1637 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/inline/radio.html
--rw-r--r--   0        0        0     1487 2024-05-14 07:32:28.379659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/inline/select.html
--rw-r--r--   0        0        0     1411 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/inline/select_multiple.html
--rw-r--r--   0        0        0     1054 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/inline/textarea.html
--rw-r--r--   0        0        0     5226 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/login.html
--rw-r--r--   0        0        0     2051 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0     1272 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      296 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0     1004 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/vertical/checkbox.html
--rw-r--r--   0        0        0     1766 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/vertical/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/vertical/dict_field.html
--rw-r--r--   0        0        0      427 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/vertical/fieldset.html
--rw-r--r--   0        0        0      150 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/vertical/form.html
--rw-r--r--   0        0        0     1281 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/vertical/input.html
--rw-r--r--   0        0        0      262 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/vertical/list_field.html
--rw-r--r--   0        0        0      330 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/vertical/list_fieldset.html
--rw-r--r--   0        0        0     1637 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/vertical/radio.html
--rw-r--r--   0        0        0     1461 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/vertical/select.html
--rw-r--r--   0        0        0     1474 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/vertical/select_multiple.html
--rw-r--r--   0        0        0     1051 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/drf_redesign/templates/rest_framework/vertical/textarea.html
--rw-r--r--   0        0        0       51 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/drf_redesign/templatetags/__init__.py
--rw-r--r--   0        0        0     1682 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/drf_redesign/templatetags/rest_framework_redesign.py
--rw-r--r--   0        0        0      576 2024-05-14 07:32:28.383659 drf_redesign-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     4454 1970-01-01 00:00:00.000000 drf_redesign-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-18 17:42:51.803383 drf_redesign-0.3.8/LICENSE
+-rw-r--r--   0        0        0     3571 2024-05-18 17:42:51.803383 drf_redesign-0.3.8/README.md
+-rw-r--r--   0        0        0       91 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/__init__.py
+-rw-r--r--   0        0        0      235 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/apps.py
+-rw-r--r--   0        0        0    28239 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/api.html
+-rw-r--r--   0        0        0     1884 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      684 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      585 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0     1004 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1762 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1636 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1617 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1398 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1433 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0     1006 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     1004 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/checkbox.html
+-rw-r--r--   0        0        0     1766 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/dict_field.html
+-rw-r--r--   0        0        0      427 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/fieldset.html
+-rw-r--r--   0        0        0      150 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/form.html
+-rw-r--r--   0        0        0     1307 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/input.html
+-rw-r--r--   0        0        0      262 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/list_field.html
+-rw-r--r--   0        0        0      330 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/list_fieldset.html
+-rw-r--r--   0        0        0     1637 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/radio.html
+-rw-r--r--   0        0        0     1487 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/select.html
+-rw-r--r--   0        0        0     1411 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/select_multiple.html
+-rw-r--r--   0        0        0     1054 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/textarea.html
+-rw-r--r--   0        0        0     5226 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     2051 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0     1272 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      296 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0     1004 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/checkbox.html
+-rw-r--r--   0        0        0     1766 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/dict_field.html
+-rw-r--r--   0        0        0      427 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/fieldset.html
+-rw-r--r--   0        0        0      150 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/form.html
+-rw-r--r--   0        0        0     1281 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/input.html
+-rw-r--r--   0        0        0      262 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/list_field.html
+-rw-r--r--   0        0        0      330 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/list_fieldset.html
+-rw-r--r--   0        0        0     1637 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/radio.html
+-rw-r--r--   0        0        0     1461 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/select.html
+-rw-r--r--   0        0        0     1474 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/select_multiple.html
+-rw-r--r--   0        0        0     1051 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/textarea.html
+-rw-r--r--   0        0        0       51 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templatetags/__init__.py
+-rw-r--r--   0        0        0     1682 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templatetags/rest_framework_redesign.py
+-rw-r--r--   0        0        0      576 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     4454 1970-01-01 00:00:00.000000 drf_redesign-0.3.8/PKG-INFO
```

### Comparing `drf_redesign-0.3.7/LICENSE` & `drf_redesign-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/README.md` & `drf_redesign-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/api.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/api.html`

 * *Files 1% similar despite different names*

```diff
@@ -584,13 +584,21 @@
 {% block script %}
   {{ block.super }}
   <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"
     integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>
   <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/highlight.min.js"></script>
   <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/languages/http.min.js"></script>
   <script>hljs.highlightAll()</script>
-
+  <script>
+    // Make all links in response section clickable
+    setTimeout(() =>
+      document.querySelectorAll('.response-info .language-json .hljs-string .str').forEach(e => {
+        if (e.innerHTML.startsWith('"http')) {
+          e.innerHTML = `<a href="${e.innerHTML.slice(1, e.innerHTML.length - 1)}">${e.innerHTML}</a>`
+        }
+      }), 100);
+  </script>
   <script>
     const tooltipTriggerList = document.querySelectorAll('[data-bs-toggle="tooltip"]')
     const tooltipList = [...tooltipTriggerList].map(tooltipTriggerEl => new bootstrap.Tooltip(tooltipTriggerEl))
   </script>
 {% endblock %}
```

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/filters/base.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/filters/base.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/filters/ordering.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/filters/ordering.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/filters/search.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/filters/search.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/horizontal/checkbox.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/horizontal/checkbox_multiple.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/horizontal/input.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/input.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/horizontal/radio.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/radio.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/horizontal/select.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/select.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/horizontal/select_multiple.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/horizontal/textarea.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/inline/checkbox.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/inline/checkbox_multiple.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/inline/input.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/input.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/inline/radio.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/radio.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/inline/select.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/select.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/inline/select_multiple.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/inline/textarea.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/login.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/login.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/pagination/numbers.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/pagination/numbers.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/pagination/previous_and_next.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/pagination/previous_and_next.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/vertical/checkbox.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/vertical/checkbox_multiple.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/vertical/input.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/input.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/vertical/radio.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/radio.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/vertical/select.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/select.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/vertical/select_multiple.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templates/rest_framework/vertical/textarea.html` & `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/drf_redesign/templatetags/rest_framework_redesign.py` & `drf_redesign-0.3.8/drf_redesign/templatetags/rest_framework_redesign.py`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.7/pyproject.toml` & `drf_redesign-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-redesign"
-version = "0.3.7"
+version = "0.3.8"
 description = "Redesign of the browse-able api of Django REST Framework with Bootstrap 5"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "drf_redesign"}]
 homepage = "https://github.com/youzarsiph/drf-redesign/"
 repository = "https://github.com/youzarsiph/drf-redesign/"
```

### Comparing `drf_redesign-0.3.7/PKG-INFO` & `drf_redesign-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-redesign
-Version: 0.3.7
+Version: 0.3.8
 Summary: Redesign of the browse-able api of Django REST Framework with Bootstrap 5
 Home-page: https://github.com/youzarsiph/drf-redesign/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

