# Comparing `tmp/mo_testing-8.629.24136.tar.gz` & `tmp/mo_testing-8.631.24139.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_testing-8.629.24136.tar", last modified: Wed May 15 03:16:48 2024, max compression
+gzip compressed data, was "mo_testing-8.631.24139.tar", last modified: Sat May 18 03:03:06 2024, max compression
```

## Comparing `mo_testing-8.629.24136.tar` & `mo_testing-8.631.24139.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 03:16:48.488889 mo_testing-8.629.24136/
--rw-rw-rw-   0        0        0    16725 2019-11-12 20:39:14.000000 mo_testing-8.629.24136/LICENSE
--rw-rw-rw-   0        0        0     2836 2024-05-15 03:16:48.487874 mo_testing-8.629.24136/PKG-INFO
--rw-rw-rw-   0        0        0     1630 2024-04-21 13:20:38.000000 mo_testing-8.629.24136/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 03:16:48.474901 mo_testing-8.629.24136/mo_testing/
--rw-rw-rw-   0        0        0      493 2024-04-28 20:32:37.000000 mo_testing-8.629.24136/mo_testing/__init__.py
--rw-rw-rw-   0        0        0    11952 2024-05-15 03:16:41.000000 mo_testing-8.629.24136/mo_testing/fuzzytestcase.py
-drwxrwxrwx   0        0        0        0 2024-05-15 03:16:48.486764 mo_testing-8.629.24136/mo_testing.egg-info/
--rw-rw-rw-   0        0        0     2836 2024-05-15 03:16:48.000000 mo_testing-8.629.24136/mo_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-05-15 03:16:48.000000 mo_testing-8.629.24136/mo_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 03:16:48.000000 mo_testing-8.629.24136/mo_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2024-05-15 03:16:48.000000 mo_testing-8.629.24136/mo_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-15 03:16:48.000000 mo_testing-8.629.24136/mo_testing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 03:16:48.488889 mo_testing-8.629.24136/setup.cfg
--rw-rw-rw-   0        0        0     2819 2024-05-15 03:16:44.000000 mo_testing-8.629.24136/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 03:03:06.021118 mo_testing-8.631.24139/
+-rw-rw-rw-   0        0        0    16725 2019-11-12 20:39:14.000000 mo_testing-8.631.24139/LICENSE
+-rw-rw-rw-   0        0        0     2836 2024-05-18 03:03:06.020068 mo_testing-8.631.24139/PKG-INFO
+-rw-rw-rw-   0        0        0     1630 2024-04-21 13:20:38.000000 mo_testing-8.631.24139/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 03:03:06.012676 mo_testing-8.631.24139/mo_testing/
+-rw-rw-rw-   0        0        0      493 2024-04-28 20:32:37.000000 mo_testing-8.631.24139/mo_testing/__init__.py
+-rw-rw-rw-   0        0        0    12795 2024-05-18 03:01:55.000000 mo_testing-8.631.24139/mo_testing/fuzzytestcase.py
+drwxrwxrwx   0        0        0        0 2024-05-18 03:03:06.019055 mo_testing-8.631.24139/mo_testing.egg-info/
+-rw-rw-rw-   0        0        0     2836 2024-05-18 03:03:05.000000 mo_testing-8.631.24139/mo_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-18 03:03:06.000000 mo_testing-8.631.24139/mo_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 03:03:05.000000 mo_testing-8.631.24139/mo_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2024-05-18 03:03:05.000000 mo_testing-8.631.24139/mo_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-18 03:03:05.000000 mo_testing-8.631.24139/mo_testing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 03:03:06.021118 mo_testing-8.631.24139/setup.cfg
+-rw-rw-rw-   0        0        0     2819 2024-05-18 03:03:01.000000 mo_testing-8.631.24139/setup.py
```

### Comparing `mo_testing-8.629.24136/LICENSE` & `mo_testing-8.631.24139/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_testing-8.629.24136/PKG-INFO` & `mo_testing-8.631.24139/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-testing
-Version: 8.629.24136
+Version: 8.631.24139
 Summary: More Testing! Extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons
 Home-page: https://github.com/klahnakoski/mo-testing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -13,19 +13,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==10.627.24136
+Requires-Dist: mo-dots==10.630.24136
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-logs==8.628.24136
-Requires-Dist: mo-math==7.627.24136
-Requires-Dist: mo-times==5.629.24136
+Requires-Dist: mo-logs==8.631.24139
+Requires-Dist: mo-math==7.631.24139
+Requires-Dist: mo-times==5.631.24139
 Provides-Extra: tests
 Requires-Dist: mo_times; extra == "tests"
 Requires-Dist: mo_logs; extra == "tests"
 
 # More Testing
```

### Comparing `mo_testing-8.629.24136/README.md` & `mo_testing-8.631.24139/README.md`

 * *Files identical despite different names*

### Comparing `mo_testing-8.629.24136/mo_testing/fuzzytestcase.py` & `mo_testing-8.631.24139/mo_testing/fuzzytestcase.py`

 * *Files 9% similar despite different names*

```diff
@@ -128,17 +128,32 @@
             Log.error(
                 "{test|json|limit(10000)} is expected to not exist",
                 test=test,
                 expected=expected,
             )
         elif is_list(expected) and len(expected)==1:
             return assertAlmostEqual(test, expected[0], msg=msg, digits=digits, places=places, delta=delta)
-        elif is_list(test) and len(test)==1 and is_many(test[0]) and is_many(expected):
+    except Exception as cause:
+        Log.error(
+            "{test|json|limit(10000)} does not match expected {expected|json|limit(10000)}",
+            test=test,
+            expected=expected,
+            cause=cause,
+        )
+
+
+    first_cause = None
+    if is_list(test) and len(test)==1 and is_many(test[0]) and is_many(expected):
+        try:
             return assertAlmostEqual(test[0], expected, msg=msg, digits=digits, places=places, delta=delta)
-        elif is_list(test) and isinstance(expected, set):
+        except Exception as cause:
+            first_cause = cause
+
+    if is_list(test) and isinstance(expected, set):
+        try:
             test = set(to_data(t) for t in test)
             if len(test) != len(expected):
                 Log.error(
                     "Sets do not match, element count"
                     " different:\n{test|json|indent}\nexpecting{expectedtest|json|indent}",
                     test=test,
                     expected=expected,
@@ -154,15 +169,19 @@
                             assertAlmostEqual(t, e, msg=msg, digits=digits, places=places, delta=delta)
                             break
                         except Exception as _:
                             pass
                     else:
                         Log.error("Sets do not match. {value|json} not found in {test|json}", value=e, test=test)
             return  # ok
-        elif is_data(expected) and is_data(test):
+        except Exception as cause:
+            first_cause = first_cause or cause
+
+    if is_data(expected) and is_data(test):
+        try:
             for k, e in from_data(expected).items():
                 if is_missing(k):
                     k = Null
                 t = test.get(k)
                 try:
                     assertAlmostEqual(
                         t,
@@ -170,51 +189,69 @@
                         msg=coalesce(msg, "") + "key " + quote(k) + ": ",
                         digits=digits,
                         places=places,
                         delta=delta,
                     )
                 except Exception as cause:
                     Log.error("key {k}={t} does not match expected {k}={e}", k=k, t=t, e=e, cause=cause)
-        elif is_data(expected):
+            return
+        except Exception as cause:
+            first_cause = first_cause or cause
+
+    if is_data(expected):
+        try:
             if is_many(test):
                 test = list(test)
                 if len(test) != 1:
                     Log.error("Expecting data, not a list")
                 test = test[0]
             for k, e in expected.items():
                 t = get_attr(test, literal_field(k))
                 try:
                     assertAlmostEqual(t, e, msg=msg, digits=digits, places=places, delta=delta)
                 except Exception as cause:
                     Log.error("key {k}={t} does not match expected {k}={e}", k=k, t=t, e=e, cause=cause)
-        elif isinstance(expected, types.FunctionType):
+            return
+        except Exception as cause:
+            first_cause = first_cause or cause
+
+    if isinstance(expected, types.FunctionType):
+        try:
             return expected(test)
-        elif hasattr(test, "__iter__") and hasattr(expected, "__iter__"):
+        except Exception as cause:
+            first_cause = first_cause or cause
+
+    if hasattr(test, "__iter__") and hasattr(expected, "__iter__"):
+        try:
             if test.__class__.__name__ == "ndarray":  # numpy
                 test = test.tolist()
             elif test.__class__.__name__ == "DataFrame":  # pandas
                 test = test[test.columns[0]].values.tolist()
             elif test.__class__.__name__ == "Series":  # pandas
                 test = test.values.tolist()
 
             if not expected and test == None:
                 return
             if expected == None:
                 expected = []  # REPRESENT NOTHING
             for t, e in zip_longest(test, expected):
                 assertAlmostEqual(t, e, msg=msg, digits=digits, places=places, delta=delta)
-        else:
-            assertAlmostEqualValue(test, expected, msg=msg, digits=digits, places=places, delta=delta)
+        except Exception as cause:
+            first_cause = first_cause or cause
+    try:
+        return assertAlmostEqualValue(test, expected, msg=msg, digits=digits, places=places, delta=delta)
     except Exception as cause:
-        Log.error(
-            "{test|json|limit(10000)} does not match expected {expected|json|limit(10000)}",
-            test=test,
-            expected=expected,
-            cause=cause,
-        )
+        first_cause = first_cause or cause
+
+    Log.error(
+        "{test|json|limit(10000)} does not match expected {expected|json|limit(10000)}",
+        test=test,
+        expected=expected,
+        cause=first_cause,
+    )
 
 
 def assertAlmostEqualValue(test, expected, digits=None, places=None, msg=None, delta=None):
     """
     Snagged from unittest/case.py, then modified (Aug2014)
     """
     if test == expected:
```

### Comparing `mo_testing-8.629.24136/mo_testing.egg-info/PKG-INFO` & `mo_testing-8.631.24139/mo_testing.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-testing
-Version: 8.629.24136
+Version: 8.631.24139
 Summary: More Testing! Extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons
 Home-page: https://github.com/klahnakoski/mo-testing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -13,19 +13,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==10.627.24136
+Requires-Dist: mo-dots==10.630.24136
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-logs==8.628.24136
-Requires-Dist: mo-math==7.627.24136
-Requires-Dist: mo-times==5.629.24136
+Requires-Dist: mo-logs==8.631.24139
+Requires-Dist: mo-math==7.631.24139
+Requires-Dist: mo-times==5.631.24139
 Provides-Extra: tests
 Requires-Dist: mo_times; extra == "tests"
 Requires-Dist: mo_logs; extra == "tests"
 
 # More Testing
```

### Comparing `mo_testing-8.629.24136/setup.py` & `mo_testing-8.631.24139/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Programming Language :: Python :: 3.10","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='More Testing! Extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons',
     extras_require={"tests":["mo_times","mo_logs"]},
     include_package_data=True,
-    install_requires=["mo-dots==10.627.24136","mo-future==7.584.24095","mo-logs==8.628.24136","mo-math==7.627.24136","mo-times==5.629.24136"],
+    install_requires=["mo-dots==10.630.24136","mo-future==7.584.24095","mo-logs==8.631.24139","mo-math==7.631.24139","mo-times==5.631.24139"],
     license='MPL 2.0',
     long_description='# More Testing\n\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-testing.svg)](https://pypi.org/project/mo-testing/)\n[![Build Status](https://github.com/klahnakoski/mo-testing/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-testing/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-testing/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-testing?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-testing/month)](https://pepy.tech/project/mo-testing)\n\n\n`FuzzyTestCase` extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons; intended for use in test cases dealing with JSON.\n\n\n## Details\n\nThe primary method is the `assertAlmostEqual` method with the following arguments:\n\n* `test_value` - the value, or structure being tested\n* `expected` - the expected value or structure.  In the case of a number, the accuracy is controlled by the following parameters.  In the case of a structure, only the not-null parameters of `expected` are tested for existence.\n* `msg` - Detailed error message if there is no match\n\nKeyword arguments:\n* `digits` - number of decimal places of accuracy required to consider two values equal\n* `places` - number of significant digits used to compare values for accuracy\n* `delta` - maximum difference between values for them to be equal\n\nThis method `assertEqual` is recursive; it does a deep comparison; it can not handle cycles in the data structure.\n\n## Major Changes\n\n### Version 8\n\n* `digits`, `places`, and `delta` must be specified as keyword arguments\n',
     long_description_content_type='text/markdown',
     name='mo-testing',
     packages=["mo_testing"],
     url='https://github.com/klahnakoski/mo-testing',
-    version='8.629.24136'
+    version='8.631.24139'
 )
```

