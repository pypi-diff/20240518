# Comparing `tmp/zjuintl_assistant-0.0.2.tar.gz` & `tmp/zjuintl_assistant-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zjuintl_assistant-0.0.2.tar", last modified: Mon May 13 15:54:42 2024, max compression
+gzip compressed data, was "zjuintl_assistant-0.0.3.tar", last modified: Sat May 18 15:10:51 2024, max compression
```

## Comparing `zjuintl_assistant-0.0.2.tar` & `zjuintl_assistant-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:54:42.360705 zjuintl_assistant-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-13 15:54:38.000000 zjuintl_assistant-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-13 15:54:42.360705 zjuintl_assistant-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-13 15:54:38.000000 zjuintl_assistant-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:54:42.360705 zjuintl_assistant-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-13 15:54:38.000000 zjuintl_assistant-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:54:42.360705 zjuintl_assistant-0.0.2/zjuintl_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-13 15:54:38.000000 zjuintl_assistant-0.0.2/zjuintl_assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17598 2024-05-13 15:54:38.000000 zjuintl_assistant-0.0.2/zjuintl_assistant/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-13 15:54:38.000000 zjuintl_assistant-0.0.2/zjuintl_assistant/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-13 15:54:38.000000 zjuintl_assistant-0.0.2/zjuintl_assistant/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-13 15:54:38.000000 zjuintl_assistant-0.0.2/zjuintl_assistant/login_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:54:42.360705 zjuintl_assistant-0.0.2/zjuintl_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-13 15:54:42.000000 zjuintl_assistant-0.0.2/zjuintl_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-13 15:54:42.000000 zjuintl_assistant-0.0.2/zjuintl_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:54:42.000000 zjuintl_assistant-0.0.2/zjuintl_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:54:42.000000 zjuintl_assistant-0.0.2/zjuintl_assistant.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 15:54:42.000000 zjuintl_assistant-0.0.2/zjuintl_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 15:54:42.000000 zjuintl_assistant-0.0.2/zjuintl_assistant.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:10:51.344246 zjuintl_assistant-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-18 15:10:47.000000 zjuintl_assistant-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-18 15:10:51.344246 zjuintl_assistant-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-18 15:10:47.000000 zjuintl_assistant-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 15:10:51.344246 zjuintl_assistant-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-18 15:10:47.000000 zjuintl_assistant-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:10:51.344246 zjuintl_assistant-0.0.3/zjuintl_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-18 15:10:47.000000 zjuintl_assistant-0.0.3/zjuintl_assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18115 2024-05-18 15:10:47.000000 zjuintl_assistant-0.0.3/zjuintl_assistant/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-18 15:10:47.000000 zjuintl_assistant-0.0.3/zjuintl_assistant/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-18 15:10:47.000000 zjuintl_assistant-0.0.3/zjuintl_assistant/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-18 15:10:47.000000 zjuintl_assistant-0.0.3/zjuintl_assistant/login_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:10:51.344246 zjuintl_assistant-0.0.3/zjuintl_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-18 15:10:51.000000 zjuintl_assistant-0.0.3/zjuintl_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-18 15:10:51.000000 zjuintl_assistant-0.0.3/zjuintl_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:10:51.000000 zjuintl_assistant-0.0.3/zjuintl_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:10:51.000000 zjuintl_assistant-0.0.3/zjuintl_assistant.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-18 15:10:51.000000 zjuintl_assistant-0.0.3/zjuintl_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-18 15:10:51.000000 zjuintl_assistant-0.0.3/zjuintl_assistant.egg-info/top_level.txt
```

### Comparing `zjuintl_assistant-0.0.2/LICENSE` & `zjuintl_assistant-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zjuintl_assistant-0.0.2/PKG-INFO` & `zjuintl_assistant-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zjuintl_assistant
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python interface for getting data from different platforms of ZJU International College
 Home-page: https://github.com/ZJUIntl-share/zjuintl_assistant
 Author: ZJUIntl-share
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `zjuintl_assistant-0.0.2/README.md` & `zjuintl_assistant-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `zjuintl_assistant-0.0.2/setup.py` & `zjuintl_assistant-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='zjuintl_assistant',
-    version='0.0.2',
+    version='0.0.3',
     description='Python interface for getting data from different platforms of ZJU International College',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ZJUIntl-share/zjuintl_assistant',
     author='ZJUIntl-share',
     license='MIT',
     packages=['zjuintl_assistant'],
```

### Comparing `zjuintl_assistant-0.0.2/zjuintl_assistant/assistant.py` & `zjuintl_assistant-0.0.3/zjuintl_assistant/assistant.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,28 @@
                 logger.debug(f"{key} cookie jar not found, copying from {base}")
                 self.__cookie_jars[key] = self.__cookie_jars[base].copy()
         else:
             logger.debug(f"{key} cookie jar found")
         return self.__cookie_jars[key]
 
 
+    def remove_cookie_jar(self, key: str = None):
+        """
+        Remove cookie jar
+        """
+
+        if key is None:
+            key = inspect.currentframe().f_back.f_code.co_name
+        if key in self.__cookie_jars:
+            logger.debug(f"Removing {key} cookie jar")
+            self.__cookie_jars.pop(key)
+        else:
+            logger.debug(f"{key} cookie jar not found")
+
+
     def logout(self):
         """
         Logout by clearing cookies and set related flags to False
         """
 
         logger.debug("Start logout")
         self.__cookie_jars: dict[str, requests.cookies.RequestsCookieJar] = {}
@@ -288,14 +302,17 @@
                 grade=grade,
                 date=date
             ))
             cnt += 1
 
         logger.debug("Get BB grades success")
 
+        # remove cookie jar
+        self.remove_cookie_jar()
+
         return result
 
 
     def get_bb_announcements(self, count: int, full: bool = False) -> list[data_classes.Announcement]:
         """
         Get announcements from Blackboard
         """
@@ -360,14 +377,17 @@
                 date=date,
                 event_type=event_type
             ))
             cnt += 1
 
         logger.debug("Get BB announcements success")
 
+        # remove cookie jar
+        self.remove_cookie_jar()
+
         return result
 
 
     def login_myZJU(self):
         """
         Login to myZJU
         """
```

### Comparing `zjuintl_assistant-0.0.2/zjuintl_assistant/constants.py` & `zjuintl_assistant-0.0.3/zjuintl_assistant/constants.py`

 * *Files identical despite different names*

### Comparing `zjuintl_assistant-0.0.2/zjuintl_assistant/data_classes.py` & `zjuintl_assistant-0.0.3/zjuintl_assistant/data_classes.py`

 * *Files identical despite different names*

### Comparing `zjuintl_assistant-0.0.2/zjuintl_assistant/login_utils.py` & `zjuintl_assistant-0.0.3/zjuintl_assistant/login_utils.py`

 * *Files identical despite different names*

### Comparing `zjuintl_assistant-0.0.2/zjuintl_assistant.egg-info/PKG-INFO` & `zjuintl_assistant-0.0.3/zjuintl_assistant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zjuintl_assistant
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python interface for getting data from different platforms of ZJU International College
 Home-page: https://github.com/ZJUIntl-share/zjuintl_assistant
 Author: ZJUIntl-share
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

