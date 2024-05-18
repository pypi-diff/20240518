# Comparing `tmp/mo_math-7.627.24136.tar.gz` & `tmp/mo_math-7.631.24139.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_math-7.627.24136.tar", last modified: Wed May 15 02:15:09 2024, max compression
+gzip compressed data, was "mo_math-7.631.24139.tar", last modified: Sat May 18 02:56:51 2024, max compression
```

## Comparing `mo_math-7.627.24136.tar` & `mo_math-7.631.24139.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 02:15:09.826274 mo_math-7.627.24136/
--rw-rw-rw-   0        0        0    16725 2019-11-12 19:25:00.000000 mo_math-7.627.24136/LICENSE
--rw-rw-rw-   0        0        0     3607 2024-05-15 02:15:09.826274 mo_math-7.627.24136/PKG-INFO
--rw-rw-rw-   0        0        0     2492 2024-03-02 21:24:19.000000 mo_math-7.627.24136/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 02:15:09.804596 mo_math-7.627.24136/mo_math/
--rw-rw-rw-   0        0        0     9717 2024-04-20 01:24:30.000000 mo_math-7.627.24136/mo_math/__init__.py
--rw-rw-rw-   0        0        0     2992 2024-01-28 14:34:02.000000 mo_math-7.627.24136/mo_math/aes_crypto.py
--rw-rw-rw-   0        0        0      299 2023-05-30 00:20:59.000000 mo_math-7.627.24136/mo_math/crypto.py
--rw-rw-rw-   0        0        0      527 2023-05-30 00:20:59.000000 mo_math-7.627.24136/mo_math/hashes.py
--rw-rw-rw-   0        0        0     1535 2023-05-30 00:20:59.000000 mo_math-7.627.24136/mo_math/randoms.py
--rw-rw-rw-   0        0        0     1938 2023-05-30 00:20:59.000000 mo_math-7.627.24136/mo_math/rsa_crypto.py
--rw-rw-rw-   0        0        0    10687 2024-02-15 02:34:15.000000 mo_math-7.627.24136/mo_math/stats.py
-drwxrwxrwx   0        0        0        0 2024-05-15 02:15:09.811543 mo_math-7.627.24136/mo_math/vendor/
--rw-rw-rw-   0        0        0        0 2019-09-12 20:40:04.000000 mo_math-7.627.24136/mo_math/vendor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 02:15:09.819335 mo_math-7.627.24136/mo_math/vendor/aespython/
--rw-rw-rw-   0        0        0        0 2019-09-12 20:40:04.000000 mo_math-7.627.24136/mo_math/vendor/aespython/__init__.py
--rw-rw-rw-   0        0        0     5568 2022-12-05 00:55:06.000000 mo_math-7.627.24136/mo_math/vendor/aespython/aes_cipher.py
--rw-rw-rw-   0        0        0    12043 2022-12-05 00:49:49.000000 mo_math-7.627.24136/mo_math/vendor/aespython/aes_tables.py
--rw-rw-rw-   0        0        0     1836 2022-12-05 00:49:49.000000 mo_math-7.627.24136/mo_math/vendor/aespython/cbc_mode.py
--rw-rw-rw-   0        0        0     1715 2022-12-05 00:49:49.000000 mo_math-7.627.24136/mo_math/vendor/aespython/cfb_mode.py
--rw-rw-rw-   0        0        0     1103 2022-12-05 00:55:06.000000 mo_math-7.627.24136/mo_math/vendor/aespython/cipher_mode.py
--rw-rw-rw-   0        0        0     5263 2022-12-05 00:49:49.000000 mo_math-7.627.24136/mo_math/vendor/aespython/key_expander.py
--rw-rw-rw-   0        0        0     1276 2022-12-05 00:49:49.000000 mo_math-7.627.24136/mo_math/vendor/aespython/mode_test.py
--rw-rw-rw-   0        0        0     1871 2022-12-05 00:49:49.000000 mo_math-7.627.24136/mo_math/vendor/aespython/ofb_mode.py
--rw-rw-rw-   0        0        0     8248 2022-12-05 00:49:49.000000 mo_math-7.627.24136/mo_math/vendor/aespython/test_keys.py
-drwxrwxrwx   0        0        0        0 2024-05-15 02:15:09.823044 mo_math-7.627.24136/mo_math/vendor/strangman/
--rw-rw-rw-   0        0        0        0 2019-09-12 20:40:06.000000 mo_math-7.627.24136/mo_math/vendor/strangman/__init__.py
--rw-rw-rw-   0        0        0     7191 2019-09-12 20:40:06.000000 mo_math-7.627.24136/mo_math/vendor/strangman/pstat.py
--rw-rw-rw-   0        0        0    55583 2022-12-04 23:23:18.000000 mo_math-7.627.24136/mo_math/vendor/strangman/stats.py
--rw-rw-rw-   0        0        0     5514 2022-12-05 00:49:49.000000 mo_math-7.627.24136/mo_math/vendor/strangman/statstest.py
-drwxrwxrwx   0        0        0        0 2024-05-15 02:15:09.824115 mo_math-7.627.24136/mo_math.egg-info/
--rw-rw-rw-   0        0        0     3607 2024-05-15 02:15:09.000000 mo_math-7.627.24136/mo_math.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      869 2024-05-15 02:15:09.000000 mo_math-7.627.24136/mo_math.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 02:15:09.000000 mo_math-7.627.24136/mo_math.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2024-05-15 02:15:09.000000 mo_math-7.627.24136/mo_math.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-15 02:15:09.000000 mo_math-7.627.24136/mo_math.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 02:15:09.827372 mo_math-7.627.24136/setup.cfg
--rw-rw-rw-   0        0        0     3701 2024-05-15 02:15:04.000000 mo_math-7.627.24136/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:56:51.844256 mo_math-7.631.24139/
+-rw-rw-rw-   0        0        0    16725 2019-11-12 19:25:00.000000 mo_math-7.631.24139/LICENSE
+-rw-rw-rw-   0        0        0     3607 2024-05-18 02:56:51.843172 mo_math-7.631.24139/PKG-INFO
+-rw-rw-rw-   0        0        0     2492 2024-03-02 21:24:19.000000 mo_math-7.631.24139/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 02:56:51.818277 mo_math-7.631.24139/mo_math/
+-rw-rw-rw-   0        0        0     9770 2024-05-18 02:56:43.000000 mo_math-7.631.24139/mo_math/__init__.py
+-rw-rw-rw-   0        0        0     2992 2024-01-28 14:34:02.000000 mo_math-7.631.24139/mo_math/aes_crypto.py
+-rw-rw-rw-   0        0        0      299 2023-05-30 00:20:59.000000 mo_math-7.631.24139/mo_math/crypto.py
+-rw-rw-rw-   0        0        0      527 2023-05-30 00:20:59.000000 mo_math-7.631.24139/mo_math/hashes.py
+-rw-rw-rw-   0        0        0     1535 2023-05-30 00:20:59.000000 mo_math-7.631.24139/mo_math/randoms.py
+-rw-rw-rw-   0        0        0     1938 2023-05-30 00:20:59.000000 mo_math-7.631.24139/mo_math/rsa_crypto.py
+-rw-rw-rw-   0        0        0    10687 2024-02-15 02:34:15.000000 mo_math-7.631.24139/mo_math/stats.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:56:51.827628 mo_math-7.631.24139/mo_math/vendor/
+-rw-rw-rw-   0        0        0        0 2019-09-12 20:40:04.000000 mo_math-7.631.24139/mo_math/vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:56:51.837204 mo_math-7.631.24139/mo_math/vendor/aespython/
+-rw-rw-rw-   0        0        0        0 2019-09-12 20:40:04.000000 mo_math-7.631.24139/mo_math/vendor/aespython/__init__.py
+-rw-rw-rw-   0        0        0     5568 2022-12-05 00:55:06.000000 mo_math-7.631.24139/mo_math/vendor/aespython/aes_cipher.py
+-rw-rw-rw-   0        0        0    12043 2022-12-05 00:49:49.000000 mo_math-7.631.24139/mo_math/vendor/aespython/aes_tables.py
+-rw-rw-rw-   0        0        0     1836 2022-12-05 00:49:49.000000 mo_math-7.631.24139/mo_math/vendor/aespython/cbc_mode.py
+-rw-rw-rw-   0        0        0     1715 2022-12-05 00:49:49.000000 mo_math-7.631.24139/mo_math/vendor/aespython/cfb_mode.py
+-rw-rw-rw-   0        0        0     1103 2022-12-05 00:55:06.000000 mo_math-7.631.24139/mo_math/vendor/aespython/cipher_mode.py
+-rw-rw-rw-   0        0        0     5263 2022-12-05 00:49:49.000000 mo_math-7.631.24139/mo_math/vendor/aespython/key_expander.py
+-rw-rw-rw-   0        0        0     1276 2022-12-05 00:49:49.000000 mo_math-7.631.24139/mo_math/vendor/aespython/mode_test.py
+-rw-rw-rw-   0        0        0     1871 2022-12-05 00:49:49.000000 mo_math-7.631.24139/mo_math/vendor/aespython/ofb_mode.py
+-rw-rw-rw-   0        0        0     8248 2022-12-05 00:49:49.000000 mo_math-7.631.24139/mo_math/vendor/aespython/test_keys.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:56:51.840455 mo_math-7.631.24139/mo_math/vendor/strangman/
+-rw-rw-rw-   0        0        0        0 2019-09-12 20:40:06.000000 mo_math-7.631.24139/mo_math/vendor/strangman/__init__.py
+-rw-rw-rw-   0        0        0     7191 2019-09-12 20:40:06.000000 mo_math-7.631.24139/mo_math/vendor/strangman/pstat.py
+-rw-rw-rw-   0        0        0    55583 2022-12-04 23:23:18.000000 mo_math-7.631.24139/mo_math/vendor/strangman/stats.py
+-rw-rw-rw-   0        0        0     5514 2022-12-05 00:49:49.000000 mo_math-7.631.24139/mo_math/vendor/strangman/statstest.py
+drwxrwxrwx   0        0        0        0 2024-05-18 02:56:51.842097 mo_math-7.631.24139/mo_math.egg-info/
+-rw-rw-rw-   0        0        0     3607 2024-05-18 02:56:51.000000 mo_math-7.631.24139/mo_math.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      869 2024-05-18 02:56:51.000000 mo_math-7.631.24139/mo_math.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 02:56:51.000000 mo_math-7.631.24139/mo_math.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2024-05-18 02:56:51.000000 mo_math-7.631.24139/mo_math.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-18 02:56:51.000000 mo_math-7.631.24139/mo_math.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 02:56:51.844256 mo_math-7.631.24139/setup.cfg
+-rw-rw-rw-   0        0        0     3701 2024-05-18 02:56:46.000000 mo_math-7.631.24139/setup.py
```

### Comparing `mo_math-7.627.24136/LICENSE` & `mo_math-7.631.24139/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_math-7.627.24136/PKG-INFO` & `mo_math-7.631.24139/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-math
-Version: 7.627.24136
+Version: 7.631.24139
 Summary: More Math! Many of the aggregates you are familiar with, but null-safe
 Home-page: https://github.com/klahnakoski/mo-math
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
@@ -13,19 +13,19 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==10.627.24136
+Requires-Dist: mo-dots==10.630.24136
 Requires-Dist: mo-future==7.584.24095
 Provides-Extra: tests
-Requires-Dist: mo-json>=6.609.24119; extra == "tests"
-Requires-Dist: mo-testing>=8.610.24119; extra == "tests"
+Requires-Dist: mo-json>=6.624.24125; extra == "tests"
+Requires-Dist: mo-testing>=8.623.24125; extra == "tests"
 
 
 # More Math!  
 
 Basic math functions that have been stabilized to act well over `Null`/`None`/`NaN`
```

### Comparing `mo_math-7.627.24136/README.md` & `mo_math-7.631.24139/README.md`

 * *Files identical despite different names*

### Comparing `mo_math-7.627.24136/mo_math/__init__.py` & `mo_math-7.631.24139/mo_math/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,59 +4,54 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
-
 import base64
 from math import (
     pow as math_pow,
     exp as math_exp,
     log as math_log,
     isnan as math_isnan,
     ceil as math_ceil,
     log10 as math_log10,
     floor as math_floor,
 )
 
 from mo_dots import Null, coalesce, is_container, exists
-from mo_future import round as math_round, text, __builtin__, binary_type
+from mo_future import round as math_round, __builtin__, binary_type
 from mo_imports import delay_import
 
 logger = delay_import("mo_logs.Log")
+math_abs = __builtin__.abs
+INFINITY = float("+inf")
+LOG10_2 = math_log10(2)
 
 
 """
 MATH FUNCTIONS THAT ASSUME None IMPLY *NOT APPLICABLE* RATHER THAN *MISSING*
 LET "." BE SOME OPERATOR (+, -, *, etc)
 a.None == None
 None.a == None
 .None == None
 func(None, *kwargs)) == None
 """
 
-math_abs = __builtin__.abs
-
-
-INFINITY = float("+inf")
-
 
 def bayesian_add(*args):
     a = args[0]
     if a >= 1 or a <= 0:
-
         logger.error("Only allowed values *between* zero and one")
 
     for b in args[1:]:
         if b == None:
             continue
         if b >= 1 or b <= 0:
-
             logger.error("Only allowed values *between* zero and one")
         a = a * b / (a * b + (1 - a) * (1 - b))
 
     return a
 
 
 def bayesian_subtract(a, b):
@@ -313,15 +308,14 @@
     DECISIVE MAX
     :param values:
     :param others:
     :return:
     """
 
     if others:
-
         logger.warning("Calling wrong")
         return MAX([values] + list(others))
 
     output = Null
     for v in values:
         if v == None:
             continue
@@ -344,15 +338,14 @@
             continue
         output += v
     return output
 
 
 def PRODUCT(values, *others):
     if len(others) > 0:
-
         logger.error("no longer accepting args, use a single list")
 
     output = Null
     for v in values:
         if v == None:
             continue
         if isinstance(v, float) and math_isnan(v):
@@ -362,41 +355,38 @@
             continue
         output *= v
     return output
 
 
 def AND(values, *others):
     if len(others) > 0:
-
         logger.error("no longer accepting args, use a single list")
 
     for v in values:
         if v == None:
             continue
         if not v:
             return False
     return True
 
 
 def OR(values, *others):
     if len(others) > 0:
-
         logger.error("no longer accepting args, use a single list")
 
     for v in values:
         if v == None:
             continue
         if v:
             return True
     return False
 
 
 def UNION(values, *others):
     if len(others) > 0:
-
         logger.error("no longer accepting args, use a single list")
 
     output = set()
     for v in values:
         if v == None:
             continue
         if is_container(v):
@@ -416,15 +406,14 @@
         return not math_isnan(s)
     except Exception:
         return False
 
 
 def INTERSECT(values, *others):
     if len(others) > 0:
-
         logger.error("no longer accepting args, use a single list")
 
     output = set(values[0])
     for v in values[1:]:
         output -= set(v)
         if not output:
             return output  # EXIT EARLY
@@ -435,23 +424,24 @@
     try:
         if first == second:
             return True
 
         if delta is not None:
             if abs(first - second) <= delta:
                 return True
-        else:
-            places = coalesce(places, digits, 18)
-            diff = math_log10(abs(first - second))
-            if diff < ceiling(math_log10(first)) - places:
-                return True
+            return False
 
-        return False
-    except Exception as e:
+        if first == 0:
+            first, second = second, first
 
+        places = coalesce(places, digits, 18)
+        factor = ceiling(log10(abs(first)))
+        diff = log10(abs(first - second))
+        return diff < factor - places - LOG10_2
+    except Exception as e:
         logger.error("problem comparing", cause=e)
 
 
 def bytes2base64(value):
     if isinstance(value, bytearray):
         value = binary_type(value)
     return base64.b64encode(value).decode("latin1")
```

### Comparing `mo_math-7.627.24136/mo_math/aes_crypto.py` & `mo_math-7.631.24139/mo_math/aes_crypto.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.627.24136/mo_math/hashes.py` & `mo_math-7.631.24139/mo_math/hashes.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.627.24136/mo_math/randoms.py` & `mo_math-7.631.24139/mo_math/randoms.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.627.24136/mo_math/rsa_crypto.py` & `mo_math-7.631.24139/mo_math/rsa_crypto.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.627.24136/mo_math/stats.py` & `mo_math-7.631.24139/mo_math/stats.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.627.24136/mo_math/vendor/aespython/aes_cipher.py` & `mo_math-7.631.24139/mo_math/vendor/aespython/aes_cipher.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.627.24136/mo_math/vendor/aespython/aes_tables.py` & `mo_math-7.631.24139/mo_math/vendor/aespython/aes_tables.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.627.24136/mo_math/vendor/aespython/cbc_mode.py` & `mo_math-7.631.24139/mo_math/vendor/aespython/cbc_mode.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.627.24136/mo_math/vendor/aespython/cfb_mode.py` & `mo_math-7.631.24139/mo_math/vendor/aespython/cfb_mode.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.627.24136/mo_math/vendor/aespython/cipher_mode.py` & `mo_math-7.631.24139/mo_math/vendor/aespython/cipher_mode.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.627.24136/mo_math/vendor/aespython/key_expander.py` & `mo_math-7.631.24139/mo_math/vendor/aespython/key_expander.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.627.24136/mo_math/vendor/aespython/mode_test.py` & `mo_math-7.631.24139/mo_math/vendor/aespython/mode_test.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.627.24136/mo_math/vendor/aespython/ofb_mode.py` & `mo_math-7.631.24139/mo_math/vendor/aespython/ofb_mode.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.627.24136/mo_math/vendor/aespython/test_keys.py` & `mo_math-7.631.24139/mo_math/vendor/aespython/test_keys.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.627.24136/mo_math/vendor/strangman/pstat.py` & `mo_math-7.631.24139/mo_math/vendor/strangman/pstat.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.627.24136/mo_math/vendor/strangman/stats.py` & `mo_math-7.631.24139/mo_math/vendor/strangman/stats.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.627.24136/mo_math/vendor/strangman/statstest.py` & `mo_math-7.631.24139/mo_math/vendor/strangman/statstest.py`

 * *Files identical despite different names*

### Comparing `mo_math-7.627.24136/mo_math.egg-info/PKG-INFO` & `mo_math-7.631.24139/mo_math.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-math
-Version: 7.627.24136
+Version: 7.631.24139
 Summary: More Math! Many of the aggregates you are familiar with, but null-safe
 Home-page: https://github.com/klahnakoski/mo-math
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
@@ -13,19 +13,19 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==10.627.24136
+Requires-Dist: mo-dots==10.630.24136
 Requires-Dist: mo-future==7.584.24095
 Provides-Extra: tests
-Requires-Dist: mo-json>=6.609.24119; extra == "tests"
-Requires-Dist: mo-testing>=8.610.24119; extra == "tests"
+Requires-Dist: mo-json>=6.624.24125; extra == "tests"
+Requires-Dist: mo-testing>=8.623.24125; extra == "tests"
 
 
 # More Math!  
 
 Basic math functions that have been stabilized to act well over `Null`/`None`/`NaN`
```

### Comparing `mo_math-7.627.24136/mo_math.egg-info/SOURCES.txt` & `mo_math-7.631.24139/mo_math.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mo_math-7.627.24136/setup.py` & `mo_math-7.631.24139/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # THIS FILE IS AUTOGENERATED!
 from setuptools import setup
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.10","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='More Math! Many of the aggregates you are familiar with, but null-safe',
-    extras_require={"tests":["mo-json>=6.609.24119","mo-testing>=8.610.24119"]},
+    extras_require={"tests":["mo-json>=6.624.24125","mo-testing>=8.623.24125"]},
     include_package_data=True,
-    install_requires=["mo-dots==10.627.24136","mo-future==7.584.24095"],
+    install_requires=["mo-dots==10.630.24136","mo-future==7.584.24095"],
     license='MPL 2.0',
     long_description="\n# More Math!  \n\nBasic math functions that have been stabilized to act well over `Null`/`None`/`NaN`\n\n\n|Branch      |Status   |\n|------------|---------|\n|master      |  [![Build Status](https://github.com/klahnakoski/mo-math/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-math/actions/workflows/build.yml) |\n|dev         | [![Build Status](https://app.travis-ci.com/klahnakoski/mo-math.svg?branch=dev)](https://travis-ci.com/github/klahnakoski/mo-math)    |\n\n\n\n## Overview\n\nMany of the basic math functions you know and love, with the additional benefit \nthat they do not throw exceptions and do not return `NaN`. \n\nThese functions are all module methods. Be sure you call the functions \nwith `mo_math.` prefix, like \n\n    import mo_math\n\tmo_math.abs(-42)\n\nor rename the functions\n\n    from mo_math import abs as mo_abs\n    mo_abs(-42)\n\nThis prevents confusion with the `__builtin__` functions by the same name   \n\n\n## Functions\n\nFunctions are generally [conservative](https://github.com/mozilla/ActiveData/blob/dev/docs/jx_decisive_operators.md#definitions) in the face of nulls: Specifically, they return `Null` if any of their operands are not a number.\n\nMost functions need no introduction, but some are interesting:\n\n- `round(value, decimal=7, digits=None)` - Rounds to 7 decimal points, unless specified differently.  Rounding to `decimal=0` will return an `int`. The useful parameter here is `digits`, which rounds to a specified number of significant digits.\n- `floor(value, mod=1)` - The `mod`ulo parameter is used to specify the granularity of the floor function.\n- `ceiling(value, mod=1)` - Return the smallest value, that's equal or larger than `value`, with suitable granularity.\n- `mod(value, mod=1)` - Works on floats\n- `approx_str(value)` - Round values, and return `text` (`unicode` in py2, `str` in py3) \n- `sign(v)` - Missing from the Python library \n\n\nThe all-caps aggregate functions accept only one parameter; an iterable. They are [decisive](https://github.com/mozilla/ActiveData/blob/dev/docs/jx_decisive_operators.md#definitions) operators: Non-numbers are ignored, if no values are numbers then the aggregate will return `Null`.\n\n- `COUNT(values)`\n- `SUM(values)` \n- `PRODUCT(values)` \n- `MIN(values)` \n- `MAX(values)` \n\n## Crypto\n\nThe AES and RSA crypto functions provide structured input/output on top of `cryptography` library. The intent is to reveal the signed/encrypted structures so third parties can decode the data.\n",
     long_description_content_type='text/markdown',
     name='mo-math',
     packages=["mo_math.vendor.aespython","mo_math.vendor.strangman","mo_math.vendor","mo_math"],
     url='https://github.com/klahnakoski/mo-math',
-    version='7.627.24136'
+    version='7.631.24139'
 )
```

