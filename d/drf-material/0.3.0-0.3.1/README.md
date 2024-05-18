# Comparing `tmp/drf_material-0.3.0.tar.gz` & `tmp/drf_material-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_material-0.3.0.tar", max compression
+gzip compressed data, was "drf_material-0.3.1.tar", max compression
```

## Comparing `drf_material-0.3.0.tar` & `drf_material-0.3.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1074 2024-05-14 07:39:17.393466 drf_material-0.3.0/LICENSE
--rw-r--r--   0        0        0     3088 2024-05-14 07:39:17.393466 drf_material-0.3.0/README.md
--rw-r--r--   0        0        0       87 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/__init__.py
--rw-r--r--   0        0        0      235 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/apps.py
--rw-r--r--   0        0        0    24027 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/api.html
--rw-r--r--   0        0        0     1882 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      684 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      606 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0     1004 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1762 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1636 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1617 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1373 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1411 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0      962 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     1004 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/inline/checkbox.html
--rw-r--r--   0        0        0     1766 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/inline/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/inline/dict_field.html
--rw-r--r--   0        0        0      427 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/inline/fieldset.html
--rw-r--r--   0        0        0      150 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/inline/form.html
--rw-r--r--   0        0        0     1307 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/inline/input.html
--rw-r--r--   0        0        0      262 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/inline/list_field.html
--rw-r--r--   0        0        0      330 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/inline/list_fieldset.html
--rw-r--r--   0        0        0     1637 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/inline/radio.html
--rw-r--r--   0        0        0     1481 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/inline/select.html
--rw-r--r--   0        0        0     1411 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/inline/select_multiple.html
--rw-r--r--   0        0        0     1077 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/inline/textarea.html
--rw-r--r--   0        0        0     3631 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/login.html
--rw-r--r--   0        0        0     1912 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0     1272 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      298 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0     1004 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/vertical/checkbox.html
--rw-r--r--   0        0        0     1766 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/vertical/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/vertical/dict_field.html
--rw-r--r--   0        0        0      427 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/vertical/fieldset.html
--rw-r--r--   0        0        0      150 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/vertical/form.html
--rw-r--r--   0        0        0     1281 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/vertical/input.html
--rw-r--r--   0        0        0      262 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/vertical/list_field.html
--rw-r--r--   0        0        0      330 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/vertical/list_fieldset.html
--rw-r--r--   0        0        0     1637 2024-05-14 07:39:17.397466 drf_material-0.3.0/drf_material/templates/rest_framework/vertical/radio.html
--rw-r--r--   0        0        0     1455 2024-05-14 07:39:17.401466 drf_material-0.3.0/drf_material/templates/rest_framework/vertical/select.html
--rw-r--r--   0        0        0     1473 2024-05-14 07:39:17.401466 drf_material-0.3.0/drf_material/templates/rest_framework/vertical/select_multiple.html
--rw-r--r--   0        0        0     1051 2024-05-14 07:39:17.401466 drf_material-0.3.0/drf_material/templates/rest_framework/vertical/textarea.html
--rw-r--r--   0        0        0       51 2024-05-14 07:39:17.401466 drf_material-0.3.0/drf_material/templatetags/__init__.py
--rw-r--r--   0        0        0     1681 2024-05-14 07:39:17.401466 drf_material-0.3.0/drf_material/templatetags/rest_framework_material.py
--rw-r--r--   0        0        0      548 2024-05-14 07:39:17.401466 drf_material-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3943 1970-01-01 00:00:00.000000 drf_material-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-18 17:44:32.203850 drf_material-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3088 2024-05-18 17:44:32.203850 drf_material-0.3.1/README.md
+-rw-r--r--   0        0        0       87 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/__init__.py
+-rw-r--r--   0        0        0      235 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/apps.py
+-rw-r--r--   0        0        0    24397 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/api.html
+-rw-r--r--   0        0        0     1882 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      684 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      606 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0     1004 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1762 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1636 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1617 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1373 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1411 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0      962 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     1004 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/checkbox.html
+-rw-r--r--   0        0        0     1766 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/dict_field.html
+-rw-r--r--   0        0        0      427 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/fieldset.html
+-rw-r--r--   0        0        0      150 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/form.html
+-rw-r--r--   0        0        0     1307 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/input.html
+-rw-r--r--   0        0        0      262 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/list_field.html
+-rw-r--r--   0        0        0      330 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/list_fieldset.html
+-rw-r--r--   0        0        0     1637 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/radio.html
+-rw-r--r--   0        0        0     1481 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/select.html
+-rw-r--r--   0        0        0     1411 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/select_multiple.html
+-rw-r--r--   0        0        0     1077 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/textarea.html
+-rw-r--r--   0        0        0     3631 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     1912 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0     1272 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      298 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0     1004 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/checkbox.html
+-rw-r--r--   0        0        0     1766 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/dict_field.html
+-rw-r--r--   0        0        0      427 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/fieldset.html
+-rw-r--r--   0        0        0      150 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/form.html
+-rw-r--r--   0        0        0     1281 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/input.html
+-rw-r--r--   0        0        0      262 2024-05-18 17:44:32.211850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/list_field.html
+-rw-r--r--   0        0        0      330 2024-05-18 17:44:32.211850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/list_fieldset.html
+-rw-r--r--   0        0        0     1637 2024-05-18 17:44:32.211850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/radio.html
+-rw-r--r--   0        0        0     1455 2024-05-18 17:44:32.211850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/select.html
+-rw-r--r--   0        0        0     1473 2024-05-18 17:44:32.211850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/select_multiple.html
+-rw-r--r--   0        0        0     1051 2024-05-18 17:44:32.211850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/textarea.html
+-rw-r--r--   0        0        0       51 2024-05-18 17:44:32.211850 drf_material-0.3.1/drf_material/templatetags/__init__.py
+-rw-r--r--   0        0        0     1681 2024-05-18 17:44:32.211850 drf_material-0.3.1/drf_material/templatetags/rest_framework_material.py
+-rw-r--r--   0        0        0      548 2024-05-18 17:44:32.211850 drf_material-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3943 1970-01-01 00:00:00.000000 drf_material-0.3.1/PKG-INFO
```

### Comparing `drf_material-0.3.0/LICENSE` & `drf_material-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/README.md` & `drf_material-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/api.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/api.html`

 * *Files 2% similar despite different names*

```diff
@@ -509,8 +509,17 @@
 
 {% block script %}
   {{ block.super }}
   <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/mdb-ui-kit/6.4.2/mdb.min.js"></script>
   <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/highlight.min.js"></script>
   <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/languages/http.min.js"></script>
   <script>hljs.highlightAll()</script>
+  <script>
+    // Make all links in response section clickable
+    setTimeout(() =>
+      document.querySelectorAll('.response-info .language-json .hljs-string .str').forEach(e => {
+        if (e.innerHTML.startsWith('"http')) {
+          e.innerHTML = `<a href="${e.innerHTML.slice(1, e.innerHTML.length - 1)}">${e.innerHTML}</a>`
+        }
+      }), 100);
+  </script>
 {% endblock %}
```

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/filters/base.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/filters/base.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/filters/ordering.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/filters/ordering.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/filters/search.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/filters/search.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/horizontal/checkbox.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/horizontal/checkbox_multiple.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/horizontal/input.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/input.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/horizontal/radio.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/radio.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/horizontal/select.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/select.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/horizontal/select_multiple.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/horizontal/textarea.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/inline/checkbox.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/inline/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/inline/checkbox_multiple.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/inline/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/inline/input.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/inline/input.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/inline/radio.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/inline/radio.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/inline/select.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/inline/select.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/inline/select_multiple.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/inline/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/inline/textarea.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/inline/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/login.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/login.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/pagination/numbers.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/pagination/numbers.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/pagination/previous_and_next.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/pagination/previous_and_next.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/vertical/checkbox.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/vertical/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/vertical/checkbox_multiple.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/vertical/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/vertical/input.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/vertical/input.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/vertical/radio.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/vertical/radio.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/vertical/select.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/vertical/select.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/vertical/select_multiple.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/vertical/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templates/rest_framework/vertical/textarea.html` & `drf_material-0.3.1/drf_material/templates/rest_framework/vertical/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/drf_material/templatetags/rest_framework_material.py` & `drf_material-0.3.1/drf_material/templatetags/rest_framework_material.py`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.0/pyproject.toml` & `drf_material-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-material"
-version = "0.3.0"
+version = "0.3.1"
 description = "Material design for Django REST Framework API"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "drf_material"}]
 homepage = "https://github.com/youzarsiph/drf-material/"
 repository = "https://github.com/youzarsiph/drf-material/"
```

### Comparing `drf_material-0.3.0/PKG-INFO` & `drf_material-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-material
-Version: 0.3.0
+Version: 0.3.1
 Summary: Material design for Django REST Framework API
 Home-page: https://github.com/youzarsiph/drf-material/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

