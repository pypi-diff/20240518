# Comparing `tmp/wheke_auth-0.0.1a1.tar.gz` & `tmp/wheke_auth-0.0.1a2.tar.gz`

## Comparing `wheke_auth-0.0.1a1.tar` & `wheke_auth-0.0.1a2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/.github/workflows/test-suite.yml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/src/wheke_auth/__about__.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/src/wheke_auth/__init__.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/src/wheke_auth/cli.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/src/wheke_auth/exceptions.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/src/wheke_auth/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/src/wheke_auth/py.typed
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/src/wheke_auth/repository.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/src/wheke_auth/routes.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/src/wheke_auth/security.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/src/wheke_auth/service.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/src/wheke_auth/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/tests/__init__.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/tests/conftest.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/tests/test_app.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/tests/example_app/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/LICENSE.txt
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/README.md
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/.github/workflows/test-suite.yml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/src/wheke_auth/__about__.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/src/wheke_auth/__init__.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/src/wheke_auth/cli.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/src/wheke_auth/exceptions.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/src/wheke_auth/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/src/wheke_auth/py.typed
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/src/wheke_auth/repository.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/src/wheke_auth/routes.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/src/wheke_auth/security.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/src/wheke_auth/service.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/src/wheke_auth/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/tests/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/tests/conftest.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/tests/test_app.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/tests/example_app/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/LICENSE.txt
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/README.md
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 wheke_auth-0.0.1a2/PKG-INFO
```

### Comparing `wheke_auth-0.0.1a1/.github/workflows/test-suite.yml` & `wheke_auth-0.0.1a2/.github/workflows/test-suite.yml`

 * *Files identical despite different names*

### Comparing `wheke_auth-0.0.1a1/src/wheke_auth/cli.py` & `wheke_auth-0.0.1a2/src/wheke_auth/cli.py`

 * *Files identical despite different names*

### Comparing `wheke_auth-0.0.1a1/src/wheke_auth/repository.py` & `wheke_auth-0.0.1a2/src/wheke_auth/repository.py`

 * *Files identical despite different names*

### Comparing `wheke_auth-0.0.1a1/src/wheke_auth/routes.py` & `wheke_auth-0.0.1a2/src/wheke_auth/routes.py`

 * *Files identical despite different names*

### Comparing `wheke_auth-0.0.1a1/src/wheke_auth/security.py` & `wheke_auth-0.0.1a2/src/wheke_auth/security.py`

 * *Files identical despite different names*

### Comparing `wheke_auth-0.0.1a1/src/wheke_auth/service.py` & `wheke_auth-0.0.1a2/src/wheke_auth/service.py`

 * *Files identical despite different names*

### Comparing `wheke_auth-0.0.1a1/tests/conftest.py` & `wheke_auth-0.0.1a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `wheke_auth-0.0.1a1/LICENSE.txt` & `wheke_auth-0.0.1a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wheke_auth-0.0.1a1/README.md` & `wheke_auth-0.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `wheke_auth-0.0.1a1/pyproject.toml` & `wheke_auth-0.0.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 dependencies = [
   "aiotinydb",
   "bcrypt==4.0.1",
   "email-validator",
   "passlib[bcrypt]",
   "python-jose[cryptography]",
   "python-multipart",
-  "wheke>=0.0.1a10",
+  "wheke>=0.1.1",
 ]
 
 [project.urls]
 Documentation = "https://github.com/humrochagf/wheke-auth#readme"
 Issues = "https://github.com/humrochagf/wheke-auth/issues"
 Source = "https://github.com/humrochagf/wheke-auth"
```

### Comparing `wheke_auth-0.0.1a1/PKG-INFO` & `wheke_auth-0.0.1a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: wheke-auth
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: A Pod that adds auth to Wheke
 Project-URL: Documentation, https://github.com/humrochagf/wheke-auth#readme
 Project-URL: Issues, https://github.com/humrochagf/wheke-auth/issues
 Project-URL: Source, https://github.com/humrochagf/wheke-auth
 Author-email: Humberto Rocha <humrochagf@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -18,15 +18,15 @@
 Requires-Python: >=3.10
 Requires-Dist: aiotinydb
 Requires-Dist: bcrypt==4.0.1
 Requires-Dist: email-validator
 Requires-Dist: passlib[bcrypt]
 Requires-Dist: python-jose[cryptography]
 Requires-Dist: python-multipart
-Requires-Dist: wheke>=0.0.1a10
+Requires-Dist: wheke>=0.1.1
 Description-Content-Type: text/markdown
 
 <h1 align="center" style="font-size: 3rem">
   wheke-auth
 </h1>
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: wheke-auth Version: 0.0.1a1 Summary: A Pod that
+Metadata-Version: 2.3 Name: wheke-auth Version: 0.0.1a2 Summary: A Pod that
 adds auth to Wheke Project-URL: Documentation, https://github.com/humrochagf/
 wheke-auth#readme Project-URL: Issues, https://github.com/humrochagf/wheke-
 auth/issues Project-URL: Source, https://github.com/humrochagf/wheke-auth
 Author-email: Humberto Rocha
 gmail.com> License-Expression: MIT License-File: LICENSE.txt Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
 Python: >=3.10 Requires-Dist: aiotinydb Requires-Dist: bcrypt==4.0.1 Requires-
 Dist: email-validator Requires-Dist: passlib[bcrypt] Requires-Dist: python-jose
-[cryptography] Requires-Dist: python-multipart Requires-Dist: wheke>=0.0.1a10
+[cryptography] Requires-Dist: python-multipart Requires-Dist: wheke>=0.1.1
 Description-Content-Type: text/markdown
                            ************ wwhheekkee--aauutthh ************
                          AA PPoodd tthhaatt aaddddss aauutthh ttoo WWhheekkee
               _[_T_e_s_t_ _S_u_i_t_e_]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]
 --- ## Installation ```console pip install wheke-auth ```
```

