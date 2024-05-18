# Comparing `tmp/moesifasgi-1.0.2.tar.gz` & `tmp/moesifasgi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moesifasgi-1.0.2.tar", last modified: Thu May 16 22:48:35 2024, max compression
+gzip compressed data, was "moesifasgi-1.0.3.tar", last modified: Fri May 17 05:54:48 2024, max compression
```

## Comparing `moesifasgi-1.0.2.tar` & `moesifasgi-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-16 22:48:35.603078 moesifasgi-1.0.2/
--rw-r--r--   0 keyur      (501) staff       (20)    11908 2021-08-28 00:36:27.000000 moesifasgi-1.0.2/LICENSE
--rw-r--r--   0 keyur      (501) staff       (20)       61 2021-08-28 00:36:31.000000 moesifasgi-1.0.2/MANIFEST.in
--rw-r--r--   0 keyur      (501) staff       (20)    13688 2024-05-16 22:48:35.603284 moesifasgi-1.0.2/PKG-INFO
--rw-r--r--   0 keyur      (501) staff       (20)    12564 2024-01-10 01:16:32.000000 moesifasgi-1.0.2/README.md
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-16 22:48:35.600315 moesifasgi-1.0.2/moesifasgi/
--rw-r--r--   0 keyur      (501) staff       (20)       26 2024-04-15 15:48:48.000000 moesifasgi-1.0.2/moesifasgi/__init__.py
--rw-r--r--   0 keyur      (501) staff       (20)      301 2021-08-28 00:35:10.000000 moesifasgi-1.0.2/moesifasgi/async_iterator_wrapper.py
--rw-r--r--   0 keyur      (501) staff       (20)     4957 2024-05-16 22:46:04.000000 moesifasgi-1.0.2/moesifasgi/client_ip.py
--rw-r--r--   0 keyur      (501) staff       (20)     3592 2024-05-16 17:14:06.000000 moesifasgi-1.0.2/moesifasgi/event_mapper.py
--rw-r--r--   0 keyur      (501) staff       (20)     9087 2024-05-16 17:13:31.000000 moesifasgi-1.0.2/moesifasgi/logger_helper.py
--rw-r--r--   0 keyur      (501) staff       (20)    11096 2024-05-16 22:46:04.000000 moesifasgi-1.0.2/moesifasgi/middleware.py
--rw-r--r--   0 keyur      (501) staff       (20)     2218 2024-05-16 22:45:23.000000 moesifasgi-1.0.2/moesifasgi/send_batch_events.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-16 22:48:35.602766 moesifasgi-1.0.2/moesifasgi.egg-info/
--rw-r--r--   0 keyur      (501) staff       (20)    13688 2024-05-16 22:48:35.000000 moesifasgi-1.0.2/moesifasgi.egg-info/PKG-INFO
--rw-r--r--   0 keyur      (501) staff       (20)      413 2024-05-16 22:48:35.000000 moesifasgi-1.0.2/moesifasgi.egg-info/SOURCES.txt
--rw-r--r--   0 keyur      (501) staff       (20)        1 2024-05-16 22:48:35.000000 moesifasgi-1.0.2/moesifasgi.egg-info/dependency_links.txt
--rw-r--r--   0 keyur      (501) staff       (20)       82 2024-05-16 22:48:35.000000 moesifasgi-1.0.2/moesifasgi.egg-info/requires.txt
--rw-r--r--   0 keyur      (501) staff       (20)       11 2024-05-16 22:48:35.000000 moesifasgi-1.0.2/moesifasgi.egg-info/top_level.txt
--rw-r--r--   0 keyur      (501) staff       (20)       67 2024-05-16 22:48:35.604123 moesifasgi-1.0.2/setup.cfg
--rw-r--r--   0 keyur      (501) staff       (20)     3269 2024-05-16 22:46:04.000000 moesifasgi-1.0.2/setup.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-17 05:54:48.605944 moesifasgi-1.0.3/
+-rw-r--r--   0 keyur      (501) staff       (20)    11908 2021-08-28 00:36:27.000000 moesifasgi-1.0.3/LICENSE
+-rw-r--r--   0 keyur      (501) staff       (20)       61 2021-08-28 00:36:31.000000 moesifasgi-1.0.3/MANIFEST.in
+-rw-r--r--   0 keyur      (501) staff       (20)    13688 2024-05-17 05:54:48.606185 moesifasgi-1.0.3/PKG-INFO
+-rw-r--r--   0 keyur      (501) staff       (20)    12564 2024-01-10 01:16:32.000000 moesifasgi-1.0.3/README.md
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-17 05:54:48.602430 moesifasgi-1.0.3/moesifasgi/
+-rw-r--r--   0 keyur      (501) staff       (20)       26 2024-04-15 15:48:48.000000 moesifasgi-1.0.3/moesifasgi/__init__.py
+-rw-r--r--   0 keyur      (501) staff       (20)      301 2021-08-28 00:35:10.000000 moesifasgi-1.0.3/moesifasgi/async_iterator_wrapper.py
+-rw-r--r--   0 keyur      (501) staff       (20)     4957 2024-05-16 22:46:04.000000 moesifasgi-1.0.3/moesifasgi/client_ip.py
+-rw-r--r--   0 keyur      (501) staff       (20)     3592 2024-05-17 05:27:16.000000 moesifasgi-1.0.3/moesifasgi/event_mapper.py
+-rw-r--r--   0 keyur      (501) staff       (20)     9087 2024-05-16 17:13:31.000000 moesifasgi-1.0.3/moesifasgi/logger_helper.py
+-rw-r--r--   0 keyur      (501) staff       (20)    11687 2024-05-17 05:53:31.000000 moesifasgi-1.0.3/moesifasgi/middleware.py
+-rw-r--r--   0 keyur      (501) staff       (20)     2218 2024-05-17 05:30:06.000000 moesifasgi-1.0.3/moesifasgi/send_batch_events.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-17 05:54:48.605660 moesifasgi-1.0.3/moesifasgi.egg-info/
+-rw-r--r--   0 keyur      (501) staff       (20)    13688 2024-05-17 05:54:48.000000 moesifasgi-1.0.3/moesifasgi.egg-info/PKG-INFO
+-rw-r--r--   0 keyur      (501) staff       (20)      413 2024-05-17 05:54:48.000000 moesifasgi-1.0.3/moesifasgi.egg-info/SOURCES.txt
+-rw-r--r--   0 keyur      (501) staff       (20)        1 2024-05-17 05:54:48.000000 moesifasgi-1.0.3/moesifasgi.egg-info/dependency_links.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       82 2024-05-17 05:54:48.000000 moesifasgi-1.0.3/moesifasgi.egg-info/requires.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       11 2024-05-17 05:54:48.000000 moesifasgi-1.0.3/moesifasgi.egg-info/top_level.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       67 2024-05-17 05:54:48.606850 moesifasgi-1.0.3/setup.cfg
+-rw-r--r--   0 keyur      (501) staff       (20)     3269 2024-05-17 05:53:31.000000 moesifasgi-1.0.3/setup.py
```

### Comparing `moesifasgi-1.0.2/LICENSE` & `moesifasgi-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `moesifasgi-1.0.2/PKG-INFO` & `moesifasgi-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moesifasgi
-Version: 1.0.2
+Version: 1.0.3
 Summary: Moesif Middleware for Python ASGI based platforms (FastAPI & Others)
 Home-page: https://www.moesif.com/docs/server-integration/python-asgi/
 Author: Moesif, Inc
 Author-email: keyur@moesif.com
 License: Apache Software License
 Keywords: log analysis restful api development debug asgi fastapi http middleware
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moesifasgi-1.0.2/README.md` & `moesifasgi-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `moesifasgi-1.0.2/moesifasgi/client_ip.py` & `moesifasgi-1.0.3/moesifasgi/client_ip.py`

 * *Files identical despite different names*

### Comparing `moesifasgi-1.0.2/moesifasgi/event_mapper.py` & `moesifasgi-1.0.3/moesifasgi/event_mapper.py`

 * *Files identical despite different names*

### Comparing `moesifasgi-1.0.2/moesifasgi/logger_helper.py` & `moesifasgi-1.0.3/moesifasgi/logger_helper.py`

 * *Files identical despite different names*

### Comparing `moesifasgi-1.0.2/moesifasgi/middleware.py` & `moesifasgi-1.0.3/moesifasgi/middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .event_mapper import EventMapper
 from moesifapi.update_companies import Company
 from moesifapi.update_users import User
 from starlette.middleware.base import _StreamingResponse
 from moesifpythonrequest.start_capture.start_capture import StartCapture
 from moesifapi.config_manager import ConfigUpdateManager
 from moesifapi.workers import BatchedWorkerPool, ConfigJobScheduler
+from moesifapi.parse_body import ParseBody
 from starlette.types import Message
 from importlib.metadata import version
 from distutils.version import LooseVersion
 import math
 import random
 import logging
 
@@ -63,14 +64,15 @@
     def validate_settings(self):
         if self.settings is None or not self.settings.get("APPLICATION_ID", None):
             raise Exception("Moesif Application ID is required in settings")
     def initialize_counter(self):
         self.dropped_events = 0
         self.logger_helper = LoggerHelper()
         self.event_mapper = EventMapper()
+        self.parse_body = ParseBody()
 
     def initialize_client(self):
         self.api_version = self.settings.get("API_VERSION")
         self.client = MoesifAPIClient(self.settings.get("APPLICATION_ID"))
         self.api_client = self.client.api
 
     def schedule_config_job(self):
@@ -80,15 +82,15 @@
         except Exception as ex:
             self.is_config_job_scheduled = False
             if self.DEBUG:
                 logger.info(f'Error while starting the config scheduler job in background: {str(ex)}')
 
     def initialize_config(self):
         Configuration.BASE_URI = self.settings.get("BASE_URI", "https://api.moesif.net")
-        Configuration.version = 'moesifasgi-python/1.0.2'
+        Configuration.version = 'moesifasgi-python/1.0.3'
         self.LOG_BODY = self.settings.get("LOG_BODY", True)
 
         self.app_config = AppConfig()
         self.config = ConfigUpdateManager(self.api_client, self.app_config, self.DEBUG)
         self.schedule_config_job()
 
     def initialize_worker_pool(self):
@@ -145,17 +147,22 @@
 
     async def dispatch(self, request, call_next):
         # request time
         request_time = self.get_time()
         if self.DEBUG:
             logger.info(f"event request time: {str(request_time)}")
 
+        # Request headers
+        request_headers = dict(request.headers)
+        # Check if multipart/form-data payload
+        is_multi_part_request_upload = self.parse_body.is_multi_part_upload(request_headers)
+
         # Read Request Body
         request_body = None
-        if self.LOG_BODY:
+        if self.LOG_BODY and not is_multi_part_request_upload:
             request_body = await self.get_body(request)
 
         # Prepare Event Request Model
         event_req = self.event_mapper.to_request(request, request_time, request_body, self.api_version,
                                                  self.disable_transaction_id, self.DEBUG)
 
         governed_response = {}
@@ -186,17 +193,22 @@
         # Check if needs to skip the event
         skip = await self.logger_helper.should_skip(self.settings, request, response, self.DEBUG)
         if skip:
             if self.DEBUG:
                 logger.info("Skipped Event using should_skip configuration option")
             return response
 
+        # Response headers
+        response_headers = dict(response.headers)
+        # Check if multipart/form-data payload
+        is_multi_part_response_upload = self.parse_body.is_multi_part_upload(response_headers)
+
         # Read Response Body
         resp_body = None
-        if self.LOG_BODY:
+        if self.LOG_BODY and not is_multi_part_response_upload:
             # Consuming FastAPI response and grabbing body here
             resp_body = [section async for section in response.__dict__['body_iterator']]
             # Preparing FastAPI response
             response.__setattr__('body_iterator', async_iterator_wrapper(resp_body))
 
         # Prepare Event Response Model
         event_rsp = self.event_mapper.to_response(response, response_time, resp_body)
```

### Comparing `moesifasgi-1.0.2/moesifasgi/send_batch_events.py` & `moesifasgi-1.0.3/moesifasgi/send_batch_events.py`

 * *Files identical despite different names*

### Comparing `moesifasgi-1.0.2/moesifasgi.egg-info/PKG-INFO` & `moesifasgi-1.0.3/moesifasgi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moesifasgi
-Version: 1.0.2
+Version: 1.0.3
 Summary: Moesif Middleware for Python ASGI based platforms (FastAPI & Others)
 Home-page: https://www.moesif.com/docs/server-integration/python-asgi/
 Author: Moesif, Inc
 Author-email: keyur@moesif.com
 License: Apache Software License
 Keywords: log analysis restful api development debug asgi fastapi http middleware
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moesifasgi-1.0.2/setup.py` & `moesifasgi-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 setup(
     name='moesifasgi',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.2',
+    version='1.0.3',
 
     description='Moesif Middleware for Python ASGI based platforms (FastAPI & Others)',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://www.moesif.com/docs/server-integration/python-asgi/',
@@ -77,15 +77,15 @@
     # simple. Or you can use find_packages().
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
 
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['starlette>=0.16.0', 'moesifapi>=1.4.6', 'moesifpythonrequest>=0.3.3'],
+    install_requires=['starlette>=0.16.0', 'moesifapi>=1.4.7', 'moesifpythonrequest>=0.3.3'],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
     # $ pip install -e .[dev,test]
     extras_require={
         'dev': [],
```

