# Comparing `tmp/drf_audit_trail-0.1.0.tar.gz` & `tmp/drf_audit_trail-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_audit_trail-0.1.0.tar", max compression
+gzip compressed data, was "drf_audit_trail-0.1.1.tar", max compression
```

## Comparing `drf_audit_trail-0.1.0.tar` & `drf_audit_trail-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       19 2024-05-09 11:24:11.563624 drf_audit_trail-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-08 01:49:41.058976 drf_audit_trail-0.1.0/drf_audit_trail/__init__.py
--rw-r--r--   0        0        0     1071 2024-05-09 19:43:15.712433 drf_audit_trail-0.1.0/drf_audit_trail/admin.py
--rw-r--r--   0        0        0      255 2024-05-10 20:28:23.293537 drf_audit_trail-0.1.0/drf_audit_trail/apps.py
--rw-r--r--   0        0        0        0 2024-05-08 23:42:25.366271 drf_audit_trail-0.1.0/drf_audit_trail/integrations/__init__.py
--rw-r--r--   0        0        0      958 2024-05-09 18:44:07.433037 drf_audit_trail-0.1.0/drf_audit_trail/integrations/rest_framework_simplejwt.py
--rw-r--r--   0        0        0      106 2024-05-09 18:15:40.126054 drf_audit_trail-0.1.0/drf_audit_trail/managers/__init__.py
--rw-r--r--   0        0        0     1301 2024-05-09 18:19:21.825227 drf_audit_trail-0.1.0/drf_audit_trail/managers/request_audit_event_manager.py
--rw-r--r--   0        0        0      120 2024-05-09 01:34:50.633399 drf_audit_trail-0.1.0/drf_audit_trail/middleware/__init__.py
--rw-r--r--   0        0        0     5270 2024-05-09 19:42:35.819785 drf_audit_trail-0.1.0/drf_audit_trail/middleware/request_login_audit_event.py
--rw-r--r--   0        0        0     5948 2024-05-09 19:40:49.994054 drf_audit_trail-0.1.0/drf_audit_trail/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-05-08 01:49:41.058976 drf_audit_trail-0.1.0/drf_audit_trail/migrations/__init__.py
--rw-r--r--   0        0        0      647 2024-05-09 19:26:04.213917 drf_audit_trail-0.1.0/drf_audit_trail/mixins.py
--rw-r--r--   0        0        0      150 2024-05-09 17:52:36.716410 drf_audit_trail-0.1.0/drf_audit_trail/models/__init__.py
--rw-r--r--   0        0        0      826 2024-05-09 19:29:58.942644 drf_audit_trail-0.1.0/drf_audit_trail/models/login_audit_event.py
--rw-r--r--   0        0        0     1737 2024-05-09 19:29:55.270574 drf_audit_trail-0.1.0/drf_audit_trail/models/request_audit_event.py
--rw-r--r--   0        0        0      700 2024-05-10 00:12:08.881038 drf_audit_trail-0.1.0/drf_audit_trail/settings.py
--rw-r--r--   0        0        0       60 2024-05-08 01:49:41.058976 drf_audit_trail-0.1.0/drf_audit_trail/tests.py
--rw-r--r--   0        0        0      709 2024-05-09 18:22:22.004405 drf_audit_trail-0.1.0/drf_audit_trail/utils.py
--rw-r--r--   0        0        0      516 2024-05-10 20:32:00.249692 drf_audit_trail-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 drf_audit_trail-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-05-09 11:24:11.563624 drf_audit_trail-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 01:49:41.058976 drf_audit_trail-0.1.1/drf_audit_trail/__init__.py
+-rw-r--r--   0        0        0     1071 2024-05-09 19:43:15.712433 drf_audit_trail-0.1.1/drf_audit_trail/admin.py
+-rw-r--r--   0        0        0      255 2024-05-10 20:28:23.293537 drf_audit_trail-0.1.1/drf_audit_trail/apps.py
+-rw-r--r--   0        0        0        0 2024-05-08 23:42:25.366271 drf_audit_trail-0.1.1/drf_audit_trail/integrations/__init__.py
+-rw-r--r--   0        0        0      958 2024-05-09 18:44:07.433037 drf_audit_trail-0.1.1/drf_audit_trail/integrations/rest_framework_simplejwt.py
+-rw-r--r--   0        0        0      106 2024-05-09 18:15:40.126054 drf_audit_trail-0.1.1/drf_audit_trail/managers/__init__.py
+-rw-r--r--   0        0        0     1301 2024-05-09 18:19:21.825227 drf_audit_trail-0.1.1/drf_audit_trail/managers/request_audit_event_manager.py
+-rw-r--r--   0        0        0      120 2024-05-09 01:34:50.633399 drf_audit_trail-0.1.1/drf_audit_trail/middleware/__init__.py
+-rw-r--r--   0        0        0     5256 2024-05-18 14:23:17.654457 drf_audit_trail-0.1.1/drf_audit_trail/middleware/request_login_audit_event.py
+-rw-r--r--   0        0        0     5948 2024-05-09 19:40:49.994054 drf_audit_trail-0.1.1/drf_audit_trail/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-08 01:49:41.058976 drf_audit_trail-0.1.1/drf_audit_trail/migrations/__init__.py
+-rw-r--r--   0        0        0      647 2024-05-09 19:26:04.213917 drf_audit_trail-0.1.1/drf_audit_trail/mixins.py
+-rw-r--r--   0        0        0      150 2024-05-09 17:52:36.716410 drf_audit_trail-0.1.1/drf_audit_trail/models/__init__.py
+-rw-r--r--   0        0        0      826 2024-05-09 19:29:58.942644 drf_audit_trail-0.1.1/drf_audit_trail/models/login_audit_event.py
+-rw-r--r--   0        0        0     1737 2024-05-09 19:29:55.270574 drf_audit_trail-0.1.1/drf_audit_trail/models/request_audit_event.py
+-rw-r--r--   0        0        0      700 2024-05-10 00:12:08.881038 drf_audit_trail-0.1.1/drf_audit_trail/settings.py
+-rw-r--r--   0        0        0       60 2024-05-08 01:49:41.058976 drf_audit_trail-0.1.1/drf_audit_trail/tests.py
+-rw-r--r--   0        0        0      709 2024-05-09 18:22:22.004405 drf_audit_trail-0.1.1/drf_audit_trail/utils.py
+-rw-r--r--   0        0        0      516 2024-05-18 14:24:33.979652 drf_audit_trail-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 drf_audit_trail-0.1.1/PKG-INFO
```

### Comparing `drf_audit_trail-0.1.0/drf_audit_trail/admin.py` & `drf_audit_trail-0.1.1/drf_audit_trail/admin.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.0/drf_audit_trail/integrations/rest_framework_simplejwt.py` & `drf_audit_trail-0.1.1/drf_audit_trail/integrations/rest_framework_simplejwt.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.0/drf_audit_trail/managers/request_audit_event_manager.py` & `drf_audit_trail-0.1.1/drf_audit_trail/managers/request_audit_event_manager.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.0/drf_audit_trail/middleware/request_login_audit_event.py` & `drf_audit_trail-0.1.1/drf_audit_trail/middleware/request_login_audit_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,14 @@
                 return LoginAuditEvent.SIGNIN
             else:
                 return LoginAuditEvent.FAILED
 
         return self.drf_login_audit_event.get("status")
 
     def __is_auth_url(self, request):
-        return bool(re.match(DRF_AUDIT_TRAIL_AUTH_URL, request.META.get("PATH_INFO")))
+        return DRF_AUDIT_TRAIL_AUTH_URL == request.META.get("PATH_INFO")
 
     def __get_authenticated_user(self, request):
         if self.__is_auth_url(request):
             return self.drf_login_audit_event.get("user")
 
         return get_authenticated_user_by_request(request)
```

### Comparing `drf_audit_trail-0.1.0/drf_audit_trail/migrations/0001_initial.py` & `drf_audit_trail-0.1.1/drf_audit_trail/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.0/drf_audit_trail/mixins.py` & `drf_audit_trail-0.1.1/drf_audit_trail/mixins.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.0/drf_audit_trail/models/login_audit_event.py` & `drf_audit_trail-0.1.1/drf_audit_trail/models/login_audit_event.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.0/drf_audit_trail/models/request_audit_event.py` & `drf_audit_trail-0.1.1/drf_audit_trail/models/request_audit_event.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.0/drf_audit_trail/settings.py` & `drf_audit_trail-0.1.1/drf_audit_trail/settings.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.0/drf_audit_trail/utils.py` & `drf_audit_trail-0.1.1/drf_audit_trail/utils.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.0/pyproject.toml` & `drf_audit_trail-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-audit-trail"
-version = "0.1.0"
+version = "0.1.1"
 description = "A reusable django [DRF] application that handles auditing of requests and logins"
 authors = ["Talismar Fernandes Costa <talismar788.una@gmail.com>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `drf_audit_trail-0.1.0/PKG-INFO` & `drf_audit_trail-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-audit-trail
-Version: 0.1.0
+Version: 0.1.1
 Summary: A reusable django [DRF] application that handles auditing of requests and logins
 Author: Talismar Fernandes Costa
 Author-email: talismar788.una@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

