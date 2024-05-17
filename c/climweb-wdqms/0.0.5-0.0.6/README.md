# Comparing `tmp/climweb_wdqms-0.0.5.tar.gz` & `tmp/climweb_wdqms-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climweb_wdqms-0.0.5.tar", last modified: Wed May 15 11:55:07 2024, max compression
+gzip compressed data, was "climweb_wdqms-0.0.6.tar", last modified: Fri May 17 22:11:15 2024, max compression
```

## Comparing `climweb_wdqms-0.0.5.tar` & `climweb_wdqms-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:55:07.967765 climweb_wdqms-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-15 11:55:07.967765 climweb_wdqms-0.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:55:07.967765 climweb_wdqms-0.0.5/climweb_wdqms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:55:07.967765 climweb_wdqms-0.0.5/climweb_wdqms/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:55:07.967765 climweb_wdqms-0.0.5/climweb_wdqms/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10147 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/management/commands/fetch_transmissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:55:07.967765 climweb_wdqms-0.0.5/climweb_wdqms/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/climweb_wdqms/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:55:07.967765 climweb_wdqms-0.0.5/climweb_wdqms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-15 11:55:07.000000 climweb_wdqms-0.0.5/climweb_wdqms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-15 11:55:07.000000 climweb_wdqms-0.0.5/climweb_wdqms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:55:07.000000 climweb_wdqms-0.0.5/climweb_wdqms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-15 11:55:07.000000 climweb_wdqms-0.0.5/climweb_wdqms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 11:55:07.000000 climweb_wdqms-0.0.5/climweb_wdqms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-15 11:55:02.000000 climweb_wdqms-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-15 11:55:07.971765 climweb_wdqms-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:15.025694 climweb_wdqms-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-17 22:11:15.025694 climweb_wdqms-0.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:15.021694 climweb_wdqms-0.0.6/climweb_wdqms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:15.021694 climweb_wdqms-0.0.6/climweb_wdqms/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:15.025694 climweb_wdqms-0.0.6/climweb_wdqms/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10147 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/management/commands/fetch_transmissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:15.025694 climweb_wdqms-0.0.6/climweb_wdqms/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11030 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/climweb_wdqms/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:15.025694 climweb_wdqms-0.0.6/climweb_wdqms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-17 22:11:15.000000 climweb_wdqms-0.0.6/climweb_wdqms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-17 22:11:15.000000 climweb_wdqms-0.0.6/climweb_wdqms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:11:15.000000 climweb_wdqms-0.0.6/climweb_wdqms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-17 22:11:15.000000 climweb_wdqms-0.0.6/climweb_wdqms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 22:11:15.000000 climweb_wdqms-0.0.6/climweb_wdqms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-17 22:11:11.000000 climweb_wdqms-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-17 22:11:15.025694 climweb_wdqms-0.0.6/setup.cfg
```

### Comparing `climweb_wdqms-0.0.5/PKG-INFO` & `climweb_wdqms-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climweb-wdqms
-Version: 0.0.5
+Version: 0.0.6
 Summary: National level WDQMS Summary tool
 Home-page: https://github.com/wmo-raf/climweb-wdqms
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `climweb_wdqms-0.0.5/climweb_wdqms/management/commands/fetch_transmissions.py` & `climweb_wdqms-0.0.6/climweb_wdqms/management/commands/fetch_transmissions.py`

 * *Files identical despite different names*

### Comparing `climweb_wdqms-0.0.5/climweb_wdqms/migrations/0001_initial.py` & `climweb_wdqms-0.0.6/climweb_wdqms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `climweb_wdqms-0.0.5/climweb_wdqms/models.py` & `climweb_wdqms-0.0.6/climweb_wdqms/models.py`

 * *Files identical despite different names*

### Comparing `climweb_wdqms-0.0.5/climweb_wdqms/serializers.py` & `climweb_wdqms-0.0.6/climweb_wdqms/serializers.py`

 * *Files identical despite different names*

### Comparing `climweb_wdqms-0.0.5/climweb_wdqms/urls.py` & `climweb_wdqms-0.0.6/climweb_wdqms/urls.py`

 * *Files identical despite different names*

### Comparing `climweb_wdqms-0.0.5/climweb_wdqms/views.py` & `climweb_wdqms-0.0.6/climweb_wdqms/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from climweb_wdqms.serializers import StationSerializer
 from datetime import datetime
 from rest_framework.views import APIView
 from rest_framework.response import Response
 from django.db.models.functions import ExtractHour,ExtractMonth,ExtractYear
 from django.db.models import Avg, Func, F
 from django.db.models.functions import TruncMonth
+from django.utils.timezone import utc
+
 
 
 
 def validate_params(query_params, supported_params):
     # Check for unsupported parameters
     error_message = None
     unsupported_params = [param for param in query_params.keys() if param not in supported_params]
@@ -91,15 +93,15 @@
             elif frequency == 'daily_synop':
                 queryset = queryset.filter(received_date__date=received_date.date(), variable=variable).order_by('received_date__hour')
             elif frequency == 'yearly_synop':
                 queryset = queryset.filter(received_date__year = received_date.year, variable=variable).order_by('received_date__hour')
 
         # Extract the hour from the received_date and annotate the queryset
         queryset = queryset.annotate(
-            synop_hour=ExtractHour('received_date')
+            synop_hour=ExtractHour('received_date', tzinfo=utc)
         )
 
         # Aggregate the queryset to calculate the average received_rate for each synoptic hour
         queryset = queryset.values('synop_hour').annotate(
             avg_received_rate=Avg('received_rate'),
             avg_received=Avg('received'),
             avg_expected=Avg('expected'),
```

### Comparing `climweb_wdqms-0.0.5/climweb_wdqms.egg-info/PKG-INFO` & `climweb_wdqms-0.0.6/climweb_wdqms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climweb-wdqms
-Version: 0.0.5
+Version: 0.0.6
 Summary: National level WDQMS Summary tool
 Home-page: https://github.com/wmo-raf/climweb-wdqms
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `climweb_wdqms-0.0.5/climweb_wdqms.egg-info/SOURCES.txt` & `climweb_wdqms-0.0.6/climweb_wdqms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `climweb_wdqms-0.0.5/setup.cfg` & `climweb_wdqms-0.0.6/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = climweb-wdqms
-version = 0.0.5
+version = 0.0.6
 description = National level WDQMS Summary tool
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/climweb-wdqms
 author = Grace Amondi
 author_email = miswa.grace@gmail.com
 license = MIT
```

