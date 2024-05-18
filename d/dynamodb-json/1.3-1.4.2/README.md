# Comparing `tmp/dynamodb-json-1.3.tar.gz` & `tmp/dynamodb_json-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dynamodb-json-1.3.tar", last modified: Wed May  9 21:35:38 2018, max compression
+gzip compressed data, was "dynamodb_json-1.4.2.tar", last modified: Sat May 18 17:57:42 2024, max compression
```

## Comparing `dynamodb-json-1.3.tar` & `dynamodb_json-1.4.2.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2018-05-09 21:35:38.000000 dynamodb-json-1.3/
-drwxrwxrwx   0        0        0        0 2018-05-09 21:35:38.000000 dynamodb-json-1.3/dynamodb_json/
--rw-rw-rw-   0        0        0     3593 2018-02-06 17:27:59.000000 dynamodb-json-1.3/dynamodb_json/json_util.py
--rw-rw-rw-   0        0        0       72 2018-05-09 21:19:41.000000 dynamodb-json-1.3/dynamodb_json/__init__.py
-drwxrwxrwx   0        0        0        0 2018-05-09 21:35:38.000000 dynamodb-json-1.3/dynamodb_json.egg-info/
--rw-rw-rw-   0        0        0        1 2018-05-09 21:35:38.000000 dynamodb-json-1.3/dynamodb_json.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2017-04-22 14:10:36.000000 dynamodb-json-1.3/dynamodb_json.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4503 2018-05-09 21:35:38.000000 dynamodb-json-1.3/dynamodb_json.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       36 2018-05-09 21:35:38.000000 dynamodb-json-1.3/dynamodb_json.egg-info/requires.txt
--rw-rw-rw-   0        0        0      301 2018-05-09 21:35:38.000000 dynamodb-json-1.3/dynamodb_json.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       14 2018-05-09 21:35:38.000000 dynamodb-json-1.3/dynamodb_json.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4503 2018-05-09 21:35:38.000000 dynamodb-json-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2930 2017-04-22 15:53:44.000000 dynamodb-json-1.3/README.md
--rw-rw-rw-   0        0        0       68 2018-05-09 21:35:38.000000 dynamodb-json-1.3/setup.cfg
--rw-rw-rw-   0        0        0     1870 2018-05-09 21:35:32.000000 dynamodb-json-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:57:42.495669 dynamodb_json-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-18 17:57:38.000000 dynamodb_json-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-18 17:57:42.495669 dynamodb_json-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-18 17:57:38.000000 dynamodb_json-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:57:42.491669 dynamodb_json-1.4.2/dynamodb_json/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-18 17:57:38.000000 dynamodb_json-1.4.2/dynamodb_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-18 17:57:38.000000 dynamodb_json-1.4.2/dynamodb_json/json_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:57:42.491669 dynamodb_json-1.4.2/dynamodb_json.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-18 17:57:42.000000 dynamodb_json-1.4.2/dynamodb_json.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-18 17:57:42.000000 dynamodb_json-1.4.2/dynamodb_json.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 17:57:42.000000 dynamodb_json-1.4.2/dynamodb_json.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 17:57:42.000000 dynamodb_json-1.4.2/dynamodb_json.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-18 17:57:42.000000 dynamodb_json-1.4.2/dynamodb_json.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-18 17:57:42.000000 dynamodb_json-1.4.2/dynamodb_json.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-18 17:57:42.495669 dynamodb_json-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-18 17:57:38.000000 dynamodb_json-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:57:42.491669 dynamodb_json-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 17:57:38.000000 dynamodb_json-1.4.2/tests/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dynamodb-json-1.3/dynamodb_json/json_util.py` & `dynamodb_json-1.4.2/dynamodb_json/json_util.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,115 +1,117 @@
-import re
-import uuid
-from decimal import Decimal
-import six
-import sys
-from datetime import datetime
-import simplejson as json
-from boto3.dynamodb.types import TypeSerializer
-
-
-def json_serial(o):
-    if isinstance(o, datetime):
-        serial = o.strftime('%Y-%m-%dT%H:%M:%S.%f')
-    elif isinstance(o, Decimal):
-        if o % 1 > 0:
-            serial = float(o)
-        elif six.PY3:
-            serial = int(o)
-        elif o < sys.maxsize:
-            serial = int(o)
-        else:
-            serial = long(o)
-    elif isinstance(o, uuid.UUID):
-        serial = str(o.hex)
-    elif isinstance(o, set):
-        serial = list(o)
-    else:
-        serial = o
-    return serial
-
-
-def dumps(dct, as_dict=False, **kwargs):
-    """ Dump the dict to json in DynamoDB Format
-        You can use any other simplejson or json options
-        :param dct - the dict to dump
-        :param as_dict - returns the result as python dict (useful for DynamoDB boto3 library) or as json sting
-        :returns: DynamoDB json format.
-        """
-
-    result_ = TypeSerializer().serialize(json.loads(json.dumps(dct, default=json_serial),
-                                                    use_decimal=True))
-    if as_dict:
-        return next(six.iteritems(result_))[1]
-    else:
-        return json.dumps(next(six.iteritems(result_))[1], **kwargs)
-
-
-def object_hook(dct):
-    """ DynamoDB object hook to return python values """
-    try:
-        # First - Try to parse the dct as DynamoDB parsed
-        if 'BOOL' in dct:
-            return dct['BOOL']
-        if 'S' in dct:
-            val = dct['S']
-            try:
-                return datetime.strptime(val, '%Y-%m-%dT%H:%M:%S.%f')
-            except:
-                return str(val)
-        if 'SS' in dct:
-            return list(dct['SS'])
-        if 'N' in dct:
-            if re.match("^-?\d+?\.\d+?$", dct['N']) is not None:
-                return float(dct['N'])
-            else:
-                try:
-                    return int(dct['N'])
-                except:
-                    return int(dct['N'])
-        if 'B' in dct:
-            return str(dct['B'])
-        if 'NS' in dct:
-            return set(dct['NS'])
-        if 'BS' in dct:
-            return set(dct['BS'])
-        if 'M' in dct:
-            return dct['M']
-        if 'L' in dct:
-            return dct['L']
-        if 'NULL' in dct and dct['NULL'] is True:
-            return None
-    except:
-        return dct
-
-    # In a Case of returning a regular python dict
-    for key, val in six.iteritems(dct):
-        if isinstance(val, six.string_types):
-            try:
-                dct[key] = datetime.strptime(val, '%Y-%m-%dT%H:%M:%S.%f')
-            except:
-                # This is a regular Basestring object
-                pass
-
-        if isinstance(val, Decimal):
-            if val % 1 > 0:
-                dct[key] = float(val)
-            elif six.PY3:
-                dct[key] = int(val)
-            elif val < sys.maxsize:
-                dct[key] = int(val)
-            else:
-                dct[key] = long(val)
-
-    return dct
-
-
-def loads(s, as_dict=False, *args, **kwargs):
-    """ Loads dynamodb json format to a python dict.
-        :param s - the json string or dict (with the as_dict variable set to True) to convert
-        :returns python dict object
-    """
-    if as_dict or (not isinstance(s, six.string_types)):
-        s = json.dumps(s)
-    kwargs['object_hook'] = object_hook
-    return json.loads(s, *args, **kwargs)
+import re
+import uuid
+from decimal import Decimal
+import six
+import sys
+from datetime import datetime, date
+import simplejson as json
+from boto3.dynamodb.types import TypeSerializer
+
+
+def json_serial(o):
+    if isinstance(o, datetime):
+        serial = o.strftime('%Y-%m-%dT%H:%M:%S.%f')
+    elif isinstance(o, date):
+        serial = o.strftime('%Y-%m-%d')
+    elif isinstance(o, Decimal):
+        if o % 1 > 0:
+            serial = float(o)
+        elif six.PY3:
+            serial = int(o)
+        elif o < sys.maxsize:
+            serial = int(o)
+        else:
+            serial = long(o)
+    elif isinstance(o, uuid.UUID):
+        serial = str(o.hex)
+    elif isinstance(o, set):
+        serial = list(o)
+    else:
+        serial = o
+    return serial
+
+
+def dumps(dct, as_dict=False, **kwargs):
+    """ Dump the dict to json in DynamoDB Format
+        You can use any other simplejson or json options
+        :param dct - the dict to dump
+        :param as_dict - returns the result as python dict (useful for DynamoDB boto3 library) or as json sting
+        :returns: DynamoDB json format.
+        """
+
+    result_ = TypeSerializer().serialize(json.loads(json.dumps(dct, default=json_serial),
+                                                    use_decimal=True))
+    if as_dict:
+        return next(six.iteritems(result_))[1]
+    else:
+        return json.dumps(next(six.iteritems(result_))[1], **kwargs)
+
+
+def object_hook(dct):
+    """ DynamoDB object hook to return python values """
+    try:
+        # First - Try to parse the dct as DynamoDB parsed
+        if 'BOOL' in dct:
+            return dct['BOOL']
+        if 'S' in dct:
+            val = dct['S']
+            try:
+                return datetime.strptime(val, '%Y-%m-%dT%H:%M:%S.%f')
+            except:
+                return str(val)
+        if 'SS' in dct:
+            return list(dct['SS'])
+        if 'N' in dct:
+            if re.match(r"^-?\d+?\.\d+?$", dct['N']) is not None:
+                return float(dct['N'])
+            else:
+                try:
+                    return int(dct['N'])
+                except:
+                    return int(dct['N'])
+        if 'B' in dct:
+            return str(dct['B'])
+        if 'NS' in dct:
+            return set(dct['NS'])
+        if 'BS' in dct:
+            return set(dct['BS'])
+        if 'M' in dct:
+            return dct['M']
+        if 'L' in dct:
+            return dct['L']
+        if 'NULL' in dct and dct['NULL'] is True:
+            return None
+    except:
+        return dct
+
+    # In a Case of returning a regular python dict
+    for key, val in six.iteritems(dct):
+        if isinstance(val, six.string_types):
+            try:
+                dct[key] = datetime.strptime(val, '%Y-%m-%dT%H:%M:%S.%f')
+            except:
+                # This is a regular Basestring object
+                pass
+
+        if isinstance(val, Decimal):
+            if val % 1 > 0:
+                dct[key] = float(val)
+            elif six.PY3:
+                dct[key] = int(val)
+            elif val < sys.maxsize:
+                dct[key] = int(val)
+            else:
+                dct[key] = long(val)
+
+    return dct
+
+
+def loads(s, as_dict=False, *args, **kwargs):
+    """ Loads dynamodb json format to a python dict.
+        :param s - the json string or dict (with the as_dict variable set to True) to convert
+        :returns python dict object
+    """
+    if as_dict or (not isinstance(s, six.string_types)):
+        s = json.dumps(s)
+    kwargs['object_hook'] = object_hook
+    return json.loads(s, *args, **kwargs)
```

### Comparing `dynamodb-json-1.3/dynamodb_json.egg-info/PKG-INFO` & `dynamodb_json-1.4.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,106 +1,113 @@
-Metadata-Version: 1.1
-Name: dynamodb-json
-Version: 1.3
-Summary: A DynamoDB json util from and to python objects
-Home-page: https://github.com/Alonreznik/dynamodb-json
-Author: Alon Reznik
-Author-email: alonreznik@gmail.com
-License: Mozilla
-Description: # DynamoDB Json
-        DynamoDB json util to load and dump strings of Dynamodb json format to python object and vise-versa
-        
-        # Install
-        just use pip: 
-        ```
-        pip install dynamodb-json
-        ```
-        # Use
-        
-        The dynamodb-json util works the same as json loads and dumps functions:
-        ```python
-        import time
-        import uuid
-        from datetime import datetime
-        from decimal import Decimal
-        
-        from dynamodb_json import json_util as json
-        
-        json_ = {"MyString": "a",
-                 "num": 4,
-                 "MyBool": False,
-                 "my_dict": {"my_date": datetime.utcnow()},
-                 "MyNone": None,
-                 "MyZero": 0,
-                 "myDecimal": Decimal("19.2"),  # converts Decimal to float, load it as float
-                 "myLong": long(1938475658493),
-                 "MyNestedDict": {
-                     "my_other_nested": {
-                         "name": "John",
-                         "surname": "Lennon",
-                         "MyOtherNone": None,
-                         "floaty": float(29.4),
-                         "myList": [1, 3, 4, 5, 6, "This Is Sparta!"],
-                         "mySet": {1, 3, 4, 5, 6},  # converts set to list, returns as list
-                         "myUUID": uuid.uuid4(),  # converts uuid to string, loads it as string
-                         "time": time.time()  # converts it to seconds python float, loads it as float
-                     }
-                 }
-            }
-        
-        dynamodb_json = json.dumps(json_)
-        
-        # {
-        # "my_dict": {"M": {"my_date": {"S": "2017-04-22T14:41:35.780000"}}}, 
-        # "MyBool": {"BOOL": false}, "MyNone": {"NULL": true}, 
-        # "MyNestedDict": {
-        #   "M": {"my_other_nested": {
-        #       "M": {"myUUID": {"S": "2f4ad21e098f49b18e22ad209779048b"}, 
-        #             "surname": {"S": "Lennon"}, "name": {"S": "John"}, 
-        #             "mySet": {"L": [{"N": "1"}, {"N": "3"}, {"N": "4"}, {"N": "5"}, {"N": "6"}]}, 
-        #             "floaty": {"N": "29.4"}, "time": {"N": "1492872095.78"}, 
-        #             "myList": {"L": [{"N": "1"}, {"N": "3"}, {"N": "4"}, {"N": "5"}, {"N": "6"}, {"S": "This Is Sparta!"}]}, 
-        #             "MyOtherNone": {"NULL": true}}
-        #             }
-        #       }
-        #   }, 
-        # "myDecimal": {"N": "19.2"}, "num": {"N": "4"}, 
-        # "MyString": {"S": "a"}, 
-        # "myLong": {"N": "1938475658493"}, 
-        # "MyZero": {"N": "0"}
-        # }
-        
-        
-        json.loads(dynamodb_json)
-        
-        # {'my_dict': {'my_date': datetime.datetime(2017, 4, 22, 14, 41, 35, 780000)}, 'MyBool': False, 'MyNone': None,
-        #  'MyNestedDict': {
-        #      'my_other_nested': {'myUUID': '2f4ad21e098f49b18e22ad209779048b', 
-        #                          'surname': 'Lennon', 'name': 'John',
-        #                          'mySet': [1, 3, 4, 5, 6], 
-        #                          'floaty': 29.4, 
-        #                          'time': 1492872095.78,
-        #                          'myList': [1, 3, 4, 5, 6, 'This Is Sparta!'], 
-        #                          'MyOtherNone': None
-        #                          }
-        #              }, 
-        #  'myDecimal': 19.2,
-        #  'num': 4, 
-        #  'MyString': 'a', 
-        #  'myLong': 1938475658493L, 
-        #  'MyZero': 0
-        # }
-        ```
-        
-Keywords: python dynamodb amazon json aws
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Metadata-Version: 2.1
+Name: dynamodb-json
+Version: 1.4.2
+Summary: A DynamoDB json util from and to python objects
+Home-page: https://github.com/Alonreznik/dynamodb-json
+Author: Alon Reznik
+Author-email: alonreznik@gmail.com
+License: Mozilla
+Keywords: python dynamodb amazon json aws
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: simplejson>=3.10.0
+Requires-Dist: boto3>=1.4.0
+Requires-Dist: six
+
+# DynamoDB Json
+DynamoDB json util to load and dump strings of Dynamodb json format to python object and vise-versa
+
+# Install
+just use pip: 
+```
+pip install dynamodb-json
+```
+
+# Use
+
+The dynamodb-json util works the same as json loads and dumps functions:
+
+```python
+import time
+import uuid
+from datetime import datetime
+from decimal import Decimal
+
+from dynamodb_json import json_util as json
+
+json_ = {"MyString": "a",
+         "num": 4,
+         "MyBool": False,
+         "my_dict": {"my_date": datetime.utcnow()},
+         "MyNone": None,
+         "MyZero": 0,
+         "myDecimal": Decimal("19.2"),  # converts Decimal to float, load it as float
+         "myLong": long(1938475658493),
+         "MyNestedDict": {
+             "my_other_nested": {
+                 "name": "John",
+                 "surname": "Lennon",
+                 "MyOtherNone": None,
+                 "floaty": float(29.4),
+                 "myList": [1, 3, 4, 5, 6, "This Is Sparta!"],
+                 "mySet": {1, 3, 4, 5, 6},  # converts set to list, returns as list
+                 "myUUID": uuid.uuid4(),  # converts uuid to string, loads it as string
+                 "time": time.time()  # converts it to seconds python float, loads it as float
+             }
+         }
+    }
+
+dynamodb_json = json.dumps(json_)
+
+# {
+# "my_dict": {"M": {"my_date": {"S": "2017-04-22T14:41:35.780000"}}}, 
+# "MyBool": {"BOOL": false}, "MyNone": {"NULL": true}, 
+# "MyNestedDict": {
+#   "M": {"my_other_nested": {
+#       "M": {"myUUID": {"S": "2f4ad21e098f49b18e22ad209779048b"}, 
+#             "surname": {"S": "Lennon"}, "name": {"S": "John"}, 
+#             "mySet": {"L": [{"N": "1"}, {"N": "3"}, {"N": "4"}, {"N": "5"}, {"N": "6"}]}, 
+#             "floaty": {"N": "29.4"}, "time": {"N": "1492872095.78"}, 
+#             "myList": {"L": [{"N": "1"}, {"N": "3"}, {"N": "4"}, {"N": "5"}, {"N": "6"}, {"S": "This Is Sparta!"}]}, 
+#             "MyOtherNone": {"NULL": true}}
+#             }
+#       }
+#   }, 
+# "myDecimal": {"N": "19.2"}, "num": {"N": "4"}, 
+# "MyString": {"S": "a"}, 
+# "myLong": {"N": "1938475658493"}, 
+# "MyZero": {"N": "0"}
+# }
+
+
+json.loads(dynamodb_json)
+
+# {'my_dict': {'my_date': datetime.datetime(2017, 4, 22, 14, 41, 35, 780000)}, 'MyBool': False, 'MyNone': None,
+#  'MyNestedDict': {
+#      'my_other_nested': {'myUUID': '2f4ad21e098f49b18e22ad209779048b', 
+#                          'surname': 'Lennon', 'name': 'John',
+#                          'mySet': [1, 3, 4, 5, 6], 
+#                          'floaty': 29.4, 
+#                          'time': 1492872095.78,
+#                          'myList': [1, 3, 4, 5, 6, 'This Is Sparta!'], 
+#                          'MyOtherNone': None
+#                          }
+#              }, 
+#  'myDecimal': 19.2,
+#  'num': 4, 
+#  'MyString': 'a', 
+#  'myLong': 1938475658493L, 
+#  'MyZero': 0
+# }
+```
```

### Comparing `dynamodb-json-1.3/PKG-INFO` & `dynamodb_json-1.4.2/dynamodb_json.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,106 +1,113 @@
-Metadata-Version: 1.1
-Name: dynamodb-json
-Version: 1.3
-Summary: A DynamoDB json util from and to python objects
-Home-page: https://github.com/Alonreznik/dynamodb-json
-Author: Alon Reznik
-Author-email: alonreznik@gmail.com
-License: Mozilla
-Description: # DynamoDB Json
-        DynamoDB json util to load and dump strings of Dynamodb json format to python object and vise-versa
-        
-        # Install
-        just use pip: 
-        ```
-        pip install dynamodb-json
-        ```
-        # Use
-        
-        The dynamodb-json util works the same as json loads and dumps functions:
-        ```python
-        import time
-        import uuid
-        from datetime import datetime
-        from decimal import Decimal
-        
-        from dynamodb_json import json_util as json
-        
-        json_ = {"MyString": "a",
-                 "num": 4,
-                 "MyBool": False,
-                 "my_dict": {"my_date": datetime.utcnow()},
-                 "MyNone": None,
-                 "MyZero": 0,
-                 "myDecimal": Decimal("19.2"),  # converts Decimal to float, load it as float
-                 "myLong": long(1938475658493),
-                 "MyNestedDict": {
-                     "my_other_nested": {
-                         "name": "John",
-                         "surname": "Lennon",
-                         "MyOtherNone": None,
-                         "floaty": float(29.4),
-                         "myList": [1, 3, 4, 5, 6, "This Is Sparta!"],
-                         "mySet": {1, 3, 4, 5, 6},  # converts set to list, returns as list
-                         "myUUID": uuid.uuid4(),  # converts uuid to string, loads it as string
-                         "time": time.time()  # converts it to seconds python float, loads it as float
-                     }
-                 }
-            }
-        
-        dynamodb_json = json.dumps(json_)
-        
-        # {
-        # "my_dict": {"M": {"my_date": {"S": "2017-04-22T14:41:35.780000"}}}, 
-        # "MyBool": {"BOOL": false}, "MyNone": {"NULL": true}, 
-        # "MyNestedDict": {
-        #   "M": {"my_other_nested": {
-        #       "M": {"myUUID": {"S": "2f4ad21e098f49b18e22ad209779048b"}, 
-        #             "surname": {"S": "Lennon"}, "name": {"S": "John"}, 
-        #             "mySet": {"L": [{"N": "1"}, {"N": "3"}, {"N": "4"}, {"N": "5"}, {"N": "6"}]}, 
-        #             "floaty": {"N": "29.4"}, "time": {"N": "1492872095.78"}, 
-        #             "myList": {"L": [{"N": "1"}, {"N": "3"}, {"N": "4"}, {"N": "5"}, {"N": "6"}, {"S": "This Is Sparta!"}]}, 
-        #             "MyOtherNone": {"NULL": true}}
-        #             }
-        #       }
-        #   }, 
-        # "myDecimal": {"N": "19.2"}, "num": {"N": "4"}, 
-        # "MyString": {"S": "a"}, 
-        # "myLong": {"N": "1938475658493"}, 
-        # "MyZero": {"N": "0"}
-        # }
-        
-        
-        json.loads(dynamodb_json)
-        
-        # {'my_dict': {'my_date': datetime.datetime(2017, 4, 22, 14, 41, 35, 780000)}, 'MyBool': False, 'MyNone': None,
-        #  'MyNestedDict': {
-        #      'my_other_nested': {'myUUID': '2f4ad21e098f49b18e22ad209779048b', 
-        #                          'surname': 'Lennon', 'name': 'John',
-        #                          'mySet': [1, 3, 4, 5, 6], 
-        #                          'floaty': 29.4, 
-        #                          'time': 1492872095.78,
-        #                          'myList': [1, 3, 4, 5, 6, 'This Is Sparta!'], 
-        #                          'MyOtherNone': None
-        #                          }
-        #              }, 
-        #  'myDecimal': 19.2,
-        #  'num': 4, 
-        #  'MyString': 'a', 
-        #  'myLong': 1938475658493L, 
-        #  'MyZero': 0
-        # }
-        ```
-        
-Keywords: python dynamodb amazon json aws
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Metadata-Version: 2.1
+Name: dynamodb-json
+Version: 1.4.2
+Summary: A DynamoDB json util from and to python objects
+Home-page: https://github.com/Alonreznik/dynamodb-json
+Author: Alon Reznik
+Author-email: alonreznik@gmail.com
+License: Mozilla
+Keywords: python dynamodb amazon json aws
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: simplejson>=3.10.0
+Requires-Dist: boto3>=1.4.0
+Requires-Dist: six
+
+# DynamoDB Json
+DynamoDB json util to load and dump strings of Dynamodb json format to python object and vise-versa
+
+# Install
+just use pip: 
+```
+pip install dynamodb-json
+```
+
+# Use
+
+The dynamodb-json util works the same as json loads and dumps functions:
+
+```python
+import time
+import uuid
+from datetime import datetime
+from decimal import Decimal
+
+from dynamodb_json import json_util as json
+
+json_ = {"MyString": "a",
+         "num": 4,
+         "MyBool": False,
+         "my_dict": {"my_date": datetime.utcnow()},
+         "MyNone": None,
+         "MyZero": 0,
+         "myDecimal": Decimal("19.2"),  # converts Decimal to float, load it as float
+         "myLong": long(1938475658493),
+         "MyNestedDict": {
+             "my_other_nested": {
+                 "name": "John",
+                 "surname": "Lennon",
+                 "MyOtherNone": None,
+                 "floaty": float(29.4),
+                 "myList": [1, 3, 4, 5, 6, "This Is Sparta!"],
+                 "mySet": {1, 3, 4, 5, 6},  # converts set to list, returns as list
+                 "myUUID": uuid.uuid4(),  # converts uuid to string, loads it as string
+                 "time": time.time()  # converts it to seconds python float, loads it as float
+             }
+         }
+    }
+
+dynamodb_json = json.dumps(json_)
+
+# {
+# "my_dict": {"M": {"my_date": {"S": "2017-04-22T14:41:35.780000"}}}, 
+# "MyBool": {"BOOL": false}, "MyNone": {"NULL": true}, 
+# "MyNestedDict": {
+#   "M": {"my_other_nested": {
+#       "M": {"myUUID": {"S": "2f4ad21e098f49b18e22ad209779048b"}, 
+#             "surname": {"S": "Lennon"}, "name": {"S": "John"}, 
+#             "mySet": {"L": [{"N": "1"}, {"N": "3"}, {"N": "4"}, {"N": "5"}, {"N": "6"}]}, 
+#             "floaty": {"N": "29.4"}, "time": {"N": "1492872095.78"}, 
+#             "myList": {"L": [{"N": "1"}, {"N": "3"}, {"N": "4"}, {"N": "5"}, {"N": "6"}, {"S": "This Is Sparta!"}]}, 
+#             "MyOtherNone": {"NULL": true}}
+#             }
+#       }
+#   }, 
+# "myDecimal": {"N": "19.2"}, "num": {"N": "4"}, 
+# "MyString": {"S": "a"}, 
+# "myLong": {"N": "1938475658493"}, 
+# "MyZero": {"N": "0"}
+# }
+
+
+json.loads(dynamodb_json)
+
+# {'my_dict': {'my_date': datetime.datetime(2017, 4, 22, 14, 41, 35, 780000)}, 'MyBool': False, 'MyNone': None,
+#  'MyNestedDict': {
+#      'my_other_nested': {'myUUID': '2f4ad21e098f49b18e22ad209779048b', 
+#                          'surname': 'Lennon', 'name': 'John',
+#                          'mySet': [1, 3, 4, 5, 6], 
+#                          'floaty': 29.4, 
+#                          'time': 1492872095.78,
+#                          'myList': [1, 3, 4, 5, 6, 'This Is Sparta!'], 
+#                          'MyOtherNone': None
+#                          }
+#              }, 
+#  'myDecimal': 19.2,
+#  'num': 4, 
+#  'MyString': 'a', 
+#  'myLong': 1938475658493L, 
+#  'MyZero': 0
+# }
+```
```

### Comparing `dynamodb-json-1.3/README.md` & `dynamodb_json-1.4.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,86 @@
-# DynamoDB Json
-DynamoDB json util to load and dump strings of Dynamodb json format to python object and vise-versa
-
-# Install
-just use pip: 
-```
-pip install dynamodb-json
-```
-# Use
-
-The dynamodb-json util works the same as json loads and dumps functions:
-```python
-import time
-import uuid
-from datetime import datetime
-from decimal import Decimal
-
-from dynamodb_json import json_util as json
-
-json_ = {"MyString": "a",
-         "num": 4,
-         "MyBool": False,
-         "my_dict": {"my_date": datetime.utcnow()},
-         "MyNone": None,
-         "MyZero": 0,
-         "myDecimal": Decimal("19.2"),  # converts Decimal to float, load it as float
-         "myLong": long(1938475658493),
-         "MyNestedDict": {
-             "my_other_nested": {
-                 "name": "John",
-                 "surname": "Lennon",
-                 "MyOtherNone": None,
-                 "floaty": float(29.4),
-                 "myList": [1, 3, 4, 5, 6, "This Is Sparta!"],
-                 "mySet": {1, 3, 4, 5, 6},  # converts set to list, returns as list
-                 "myUUID": uuid.uuid4(),  # converts uuid to string, loads it as string
-                 "time": time.time()  # converts it to seconds python float, loads it as float
-             }
-         }
-    }
-
-dynamodb_json = json.dumps(json_)
-
-# {
-# "my_dict": {"M": {"my_date": {"S": "2017-04-22T14:41:35.780000"}}}, 
-# "MyBool": {"BOOL": false}, "MyNone": {"NULL": true}, 
-# "MyNestedDict": {
-#   "M": {"my_other_nested": {
-#       "M": {"myUUID": {"S": "2f4ad21e098f49b18e22ad209779048b"}, 
-#             "surname": {"S": "Lennon"}, "name": {"S": "John"}, 
-#             "mySet": {"L": [{"N": "1"}, {"N": "3"}, {"N": "4"}, {"N": "5"}, {"N": "6"}]}, 
-#             "floaty": {"N": "29.4"}, "time": {"N": "1492872095.78"}, 
-#             "myList": {"L": [{"N": "1"}, {"N": "3"}, {"N": "4"}, {"N": "5"}, {"N": "6"}, {"S": "This Is Sparta!"}]}, 
-#             "MyOtherNone": {"NULL": true}}
-#             }
-#       }
-#   }, 
-# "myDecimal": {"N": "19.2"}, "num": {"N": "4"}, 
-# "MyString": {"S": "a"}, 
-# "myLong": {"N": "1938475658493"}, 
-# "MyZero": {"N": "0"}
-# }
-
-
-json.loads(dynamodb_json)
-
-# {'my_dict': {'my_date': datetime.datetime(2017, 4, 22, 14, 41, 35, 780000)}, 'MyBool': False, 'MyNone': None,
-#  'MyNestedDict': {
-#      'my_other_nested': {'myUUID': '2f4ad21e098f49b18e22ad209779048b', 
-#                          'surname': 'Lennon', 'name': 'John',
-#                          'mySet': [1, 3, 4, 5, 6], 
-#                          'floaty': 29.4, 
-#                          'time': 1492872095.78,
-#                          'myList': [1, 3, 4, 5, 6, 'This Is Sparta!'], 
-#                          'MyOtherNone': None
-#                          }
-#              }, 
-#  'myDecimal': 19.2,
-#  'num': 4, 
-#  'MyString': 'a', 
-#  'myLong': 1938475658493L, 
-#  'MyZero': 0
-# }
-```
+# DynamoDB Json
+DynamoDB json util to load and dump strings of Dynamodb json format to python object and vise-versa
+
+# Install
+just use pip: 
+```
+pip install dynamodb-json
+```
+
+# Use
+
+The dynamodb-json util works the same as json loads and dumps functions:
+
+```python
+import time
+import uuid
+from datetime import datetime
+from decimal import Decimal
+
+from dynamodb_json import json_util as json
+
+json_ = {"MyString": "a",
+         "num": 4,
+         "MyBool": False,
+         "my_dict": {"my_date": datetime.utcnow()},
+         "MyNone": None,
+         "MyZero": 0,
+         "myDecimal": Decimal("19.2"),  # converts Decimal to float, load it as float
+         "myLong": long(1938475658493),
+         "MyNestedDict": {
+             "my_other_nested": {
+                 "name": "John",
+                 "surname": "Lennon",
+                 "MyOtherNone": None,
+                 "floaty": float(29.4),
+                 "myList": [1, 3, 4, 5, 6, "This Is Sparta!"],
+                 "mySet": {1, 3, 4, 5, 6},  # converts set to list, returns as list
+                 "myUUID": uuid.uuid4(),  # converts uuid to string, loads it as string
+                 "time": time.time()  # converts it to seconds python float, loads it as float
+             }
+         }
+    }
+
+dynamodb_json = json.dumps(json_)
+
+# {
+# "my_dict": {"M": {"my_date": {"S": "2017-04-22T14:41:35.780000"}}}, 
+# "MyBool": {"BOOL": false}, "MyNone": {"NULL": true}, 
+# "MyNestedDict": {
+#   "M": {"my_other_nested": {
+#       "M": {"myUUID": {"S": "2f4ad21e098f49b18e22ad209779048b"}, 
+#             "surname": {"S": "Lennon"}, "name": {"S": "John"}, 
+#             "mySet": {"L": [{"N": "1"}, {"N": "3"}, {"N": "4"}, {"N": "5"}, {"N": "6"}]}, 
+#             "floaty": {"N": "29.4"}, "time": {"N": "1492872095.78"}, 
+#             "myList": {"L": [{"N": "1"}, {"N": "3"}, {"N": "4"}, {"N": "5"}, {"N": "6"}, {"S": "This Is Sparta!"}]}, 
+#             "MyOtherNone": {"NULL": true}}
+#             }
+#       }
+#   }, 
+# "myDecimal": {"N": "19.2"}, "num": {"N": "4"}, 
+# "MyString": {"S": "a"}, 
+# "myLong": {"N": "1938475658493"}, 
+# "MyZero": {"N": "0"}
+# }
+
+
+json.loads(dynamodb_json)
+
+# {'my_dict': {'my_date': datetime.datetime(2017, 4, 22, 14, 41, 35, 780000)}, 'MyBool': False, 'MyNone': None,
+#  'MyNestedDict': {
+#      'my_other_nested': {'myUUID': '2f4ad21e098f49b18e22ad209779048b', 
+#                          'surname': 'Lennon', 'name': 'John',
+#                          'mySet': [1, 3, 4, 5, 6], 
+#                          'floaty': 29.4, 
+#                          'time': 1492872095.78,
+#                          'myList': [1, 3, 4, 5, 6, 'This Is Sparta!'], 
+#                          'MyOtherNone': None
+#                          }
+#              }, 
+#  'myDecimal': 19.2,
+#  'num': 4, 
+#  'MyString': 'a', 
+#  'myLong': 1938475658493L, 
+#  'MyZero': 0
+# }
+```
```

