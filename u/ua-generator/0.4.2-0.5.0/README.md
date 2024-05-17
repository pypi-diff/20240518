# Comparing `tmp/ua-generator-0.4.2.tar.gz` & `tmp/ua_generator-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ua-generator-0.4.2.tar", last modified: Wed Mar 13 23:02:19 2024, max compression
+gzip compressed data, was "ua_generator-0.5.0.tar", last modified: Fri May 17 22:19:40 2024, max compression
```

## Comparing `ua-generator-0.4.2.tar` & `ua_generator-0.5.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 23:02:19.597748 ua-generator-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-03-13 23:02:10.000000 ua-generator-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-03-13 23:02:19.597748 ua-generator-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-03-13 23:02:10.000000 ua-generator-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-13 23:02:10.000000 ua-generator-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-13 23:02:19.597748 ua-generator-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 23:02:19.589748 ua-generator-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 23:02:19.593748 ua-generator-0.4.2/src/ua_generator/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/client_hints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 23:02:19.593748 ua-generator-0.4.2/src/ua_generator/data/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 23:02:19.593748 ua-generator-0.4.2/src/ua_generator/data/browsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/data/browsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/data/browsers/chrome.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/data/browsers/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/data/browsers/firefox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/data/browsers/safari.py
--rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/data/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 23:02:19.593748 ua-generator-0.4.2/src/ua_generator/data/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/data/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 23:02:19.597748 ua-generator-0.4.2/src/ua_generator/data/platforms/android/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/data/platforms/android/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/data/platforms/android/android_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/data/platforms/android/android_pixel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11682 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/data/platforms/android/android_samsung.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/data/platforms/ios.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/data/platforms/linux.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/data/platforms/macos.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/data/platforms/windows.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/user_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-13 23:02:10.000000 ua-generator-0.4.2/src/ua_generator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 23:02:19.597748 ua-generator-0.4.2/src/ua_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-03-13 23:02:19.000000 ua-generator-0.4.2/src/ua_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-13 23:02:19.000000 ua-generator-0.4.2/src/ua_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 23:02:19.000000 ua-generator-0.4.2/src/ua_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-13 23:02:19.000000 ua-generator-0.4.2/src/ua_generator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 23:02:19.597748 ua-generator-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-03-13 23:02:10.000000 ua-generator-0.4.2/tests/test_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-03-13 23:02:10.000000 ua-generator-0.4.2/tests/test_client_hints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-03-13 23:02:10.000000 ua-generator-0.4.2/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-13 23:02:10.000000 ua-generator-0.4.2/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-03-13 23:02:10.000000 ua-generator-0.4.2/tests/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-13 23:02:10.000000 ua-generator-0.4.2/tests/test_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-13 23:02:10.000000 ua-generator-0.4.2/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-03-13 23:02:10.000000 ua-generator-0.4.2/tests/test_user_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-13 23:02:10.000000 ua-generator-0.4.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:19:40.284664 ua_generator-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-17 22:19:36.000000 ua_generator-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-17 22:19:40.284664 ua_generator-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-05-17 22:19:36.000000 ua_generator-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-17 22:19:36.000000 ua_generator-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-17 22:19:40.284664 ua_generator-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:19:40.276664 ua_generator-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:19:40.276664 ua_generator-0.5.0/src/ua_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/client_hints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:19:40.276664 ua_generator-0.5.0/src/ua_generator/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:19:40.280664 ua_generator-0.5.0/src/ua_generator/data/browsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/data/browsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/data/browsers/chrome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/data/browsers/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/data/browsers/firefox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/data/browsers/safari.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/data/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:19:40.280664 ua_generator-0.5.0/src/ua_generator/data/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/data/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:19:40.280664 ua_generator-0.5.0/src/ua_generator/data/platforms/android/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/data/platforms/android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/data/platforms/android/android_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/data/platforms/android/android_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11682 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/data/platforms/android/android_samsung.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/data/platforms/ios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/data/platforms/linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/data/platforms/macos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/data/platforms/windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/user_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-17 22:19:36.000000 ua_generator-0.5.0/src/ua_generator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:19:40.284664 ua_generator-0.5.0/src/ua_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-17 22:19:40.000000 ua_generator-0.5.0/src/ua_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-17 22:19:40.000000 ua_generator-0.5.0/src/ua_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:19:40.000000 ua_generator-0.5.0/src/ua_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 22:19:40.000000 ua_generator-0.5.0/src/ua_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:19:40.284664 ua_generator-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-17 22:19:36.000000 ua_generator-0.5.0/tests/test_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-05-17 22:19:36.000000 ua_generator-0.5.0/tests/test_client_hints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-17 22:19:36.000000 ua_generator-0.5.0/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-17 22:19:36.000000 ua_generator-0.5.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-17 22:19:36.000000 ua_generator-0.5.0/tests/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-17 22:19:36.000000 ua_generator-0.5.0/tests/test_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-17 22:19:36.000000 ua_generator-0.5.0/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-17 22:19:36.000000 ua_generator-0.5.0/tests/test_user_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-17 22:19:36.000000 ua_generator-0.5.0/tests/test_utils.py
```

### Comparing `ua-generator-0.4.2/LICENSE` & `ua_generator-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ua-generator-0.4.2/PKG-INFO` & `ua_generator-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ua-generator
-Version: 0.4.2
+Version: 0.5.0
 Summary: A random user-agent generator
 Home-page: https://github.com/iamdual/ua-generator
 Author: Ekin Karadeniz
 Author-email: iamdual@icloud.com
 Project-URL: Bug Tracker, https://github.com/iamdual/ua-generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ua-generator-0.4.2/README.md` & `ua_generator-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ua-generator-0.4.2/setup.cfg` & `ua_generator-0.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ua-generator
-version = 0.4.2
+version = 0.5.0
 author = Ekin Karadeniz
 author_email = iamdual@icloud.com
 description = A random user-agent generator
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/iamdual/ua-generator
 project_urls =
```

### Comparing `ua-generator-0.4.2/src/ua_generator/client_hints.py` & `ua_generator-0.5.0/src/ua_generator/client_hints.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Random User-Agent
 Copyright: 2022-2024 Ekin Karadeniz (github.com/iamdual)
 License: Apache License 2.0
 """
-from . import formats, serialization, utils
+from random import Random
+
+from . import formats, serialization
 from .data import platforms_mobile
 from .data import generator
 
 
 # https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Sec-CH-UA
 # https://wicg.github.io/ua-client-hints/#http-ua-hints
 class ClientHints:
@@ -22,95 +24,101 @@
     model: str
     wow64: str
 
     def __init__(self, gen: generator.Generator):
         self.__generator = gen
         self.__cache = {}
 
-    def __mobile(self):
+    def get_mobile(self):
         return self.__generator.platform in platforms_mobile
 
-    def __platform(self):
+    def get_platform(self):
         platform = self.__generator.platform
 
         if platform == 'ios':
             platform = 'iOS'
         elif platform == 'macos':
             platform = 'macOS'
         else:
             platform = platform.title()
 
         return platform
 
-    def __platform_version(self):
+    def get_platform_version(self):
         if self.__generator.platform == 'windows' and formats.major_version(self.__generator.platform_version) == '10':
-            return utils.choice(('10.0.0', '13.0.0'))
+            _random = Random(self.__generator.user_agent)
+            return _random.choice(('10.0.0', '13.0.0'))
 
         return formats.version(self.__generator.platform_version)
 
-    def __brands(self, full_version_list: bool = False):
+    def get_brands(self, full_version_list: bool = False):
         brand_list = [{'brand': 'Not A(Brand', 'version': '99'}]
 
-        if full_version_list:
-            browser_version = formats.version(self.__generator.browser_version)
-        else:
-            browser_version = formats.major_version(self.__generator.browser_version)
-
         if self.__generator.browser == 'chrome':
+            browser_version = self.get_browser_version(full_version=full_version_list)
             brand_list.append({'brand': 'Chromium', 'version': browser_version})
             brand_list.append({'brand': 'Google Chrome', 'version': browser_version})
         elif self.__generator.browser == 'edge':
+            browser_version = self.get_browser_version(full_version=full_version_list)
             brand_list.append({'brand': 'Chromium', 'version': browser_version})
             brand_list.append({'brand': 'Microsoft Edge', 'version': browser_version})
 
         return brand_list
 
-    def __bitness(self):
+    def get_browser_version(self, full_version: bool = True):
+        if full_version:
+            return formats.version(self.__generator.browser_version)
+        else:
+            return formats.major_version(self.__generator.browser_version)
+
+    def get_bitness(self):
         if self.__generator.platform == 'android':
-            return utils.choice(('32', '64', '32', '32'))
+            _random = Random(self.__generator.user_agent)
+            return _random.choice(('32', '64', '32', '32'))
 
         return '64'
 
-    def __architecture(self):
+    def get_architecture(self):
         if self.__generator.platform == 'android' or self.__generator.platform == 'ios':
             return 'arm'
         elif self.__generator.platform == 'macos':
-            return utils.choice(('arm', 'x86', 'arm', 'arm'))
+            _random = Random(self.__generator.user_agent)
+            return _random.choice(('arm', 'x86', 'arm', 'arm'))
 
         return 'x86'
 
-    def __model(self):
+    def get_model(self):
         if 'platform_model' in self.__generator.platform_version:
             return self.__generator.platform_version['platform_model']
 
         return ''
 
-    def __wow64(self):
+    def get_wow64(self):
         return self.__generator.platform == 'windows'
 
     def __getattr__(self, name):
         if name in self.__cache:
             return self.__cache[name]
 
         if name == 'mobile':
-            self.__cache[name] = serialization.ch_bool(self.__mobile())
+            self.__cache[name] = serialization.ch_bool(self.get_mobile())
         elif name == 'platform':
-            self.__cache[name] = serialization.ch_string(self.__platform())
+            self.__cache[name] = serialization.ch_string(self.get_platform())
         elif name == 'platform_version':
-            self.__cache[name] = serialization.ch_string(self.__platform_version())
+            self.__cache[name] = serialization.ch_string(self.get_platform_version())
         elif name == 'brands':
-            self.__cache[name] = serialization.ch_brand_list(self.__brands())
+            self.__cache[name] = serialization.ch_brand_list(self.get_brands())
         elif name == 'brands_full_version_list':
-            self.__cache[name] = serialization.ch_brand_list(self.__brands(full_version_list=True))
+            self.__cache[name] = serialization.ch_brand_list(self.get_brands(full_version_list=True))
         elif name == 'bitness':
-            self.__cache[name] = serialization.ch_string(self.__bitness())
+            self.__cache[name] = serialization.ch_string(self.get_bitness())
         elif name == 'architecture':
-            self.__cache[name] = serialization.ch_string(self.__architecture())
+            self.__cache[name] = serialization.ch_string(self.get_architecture())
         elif name == 'model':
-            self.__cache[name] = serialization.ch_string(self.__model())
+            self.__cache[name] = serialization.ch_string(self.get_model())
         elif name == 'wow64':
-            self.__cache[name] = serialization.ch_bool(self.__wow64())
+            self.__cache[name] = serialization.ch_bool(self.get_wow64())
 
         return self.__cache[name]
 
     def __str__(self):
         return self.brands
```

### Comparing `ua-generator-0.4.2/src/ua_generator/data/browsers/chrome.py` & `ua_generator-0.5.0/src/ua_generator/data/browsers/chrome.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,17 @@
     '116.0.5845': {'minor_range': (0, 255), 'webkit': '537.36'},
     '117.0.5938': {'minor_range': (0, 255), 'webkit': '537.36'},
     '118.0.5993': {'minor_range': (0, 255), 'webkit': '537.36'},
     '119.0.6045': {'minor_range': (0, 255), 'webkit': '537.36'},
     '120.0.6099': {'minor_range': (0, 255), 'webkit': '537.36'},
     '121.0.6167': {'minor_range': (0, 255), 'webkit': '537.36'},
     '122.0.6261': {'minor_range': (0, 255), 'webkit': '537.36'},
+    '123.0.6312': {'minor_range': (0, 255), 'webkit': '537.36'},
+    '124.0.6367': {'minor_range': (0, 255), 'webkit': '537.36'},
+    '125.0.6422': {'minor_range': (0, 255), 'webkit': '537.36'},
 }
 
 
 def get_version():
     choice = random.randint(0, len(versions) - 1)
     i = 0
     for major, props in versions.items():
```

### Comparing `ua-generator-0.4.2/src/ua_generator/data/browsers/edge.py` & `ua_generator-0.5.0/src/ua_generator/data/browsers/edge.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,17 @@
     '116.0.1938': {'minor_range': (0, 99), 'webkit': '537.36'},
     '117.0.2045': {'minor_range': (0, 99), 'webkit': '537.36'},
     '118.0.2088': {'minor_range': (0, 99), 'webkit': '537.36'},
     '119.0.2151': {'minor_range': (0, 99), 'webkit': '537.36'},
     '120.0.2210': {'minor_range': (0, 99), 'webkit': '537.36'},
     '121.0.2277': {'minor_range': (0, 99), 'webkit': '537.36'},
     '122.0.2365': {'minor_range': (0, 99), 'webkit': '537.36'},
+    '123.0.2420': {'minor_range': (0, 99), 'webkit': '537.36'},
+    '124.0.2478': {'minor_range': (0, 99), 'webkit': '537.36'},
+    '125.0.2535': {'minor_range': (0, 99), 'webkit': '537.36'},
 }
 
 
 def get_version():
     choice = random.randint(0, len(versions) - 1)
     i = 0
     for major, props in versions.items():
```

### Comparing `ua-generator-0.4.2/src/ua_generator/data/browsers/firefox.py` & `ua_generator-0.5.0/src/ua_generator/data/browsers/firefox.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,18 @@
     '116.0': {'minor_range': (0, 3)},
     '117.0': {'minor_range': (0, 1)},
     '118.0': {'minor_range': (0, 2)},
     '119.0': {'minor_range': (0, 1)},
     '120.0': {'minor_range': (0, 1)},
     '121.0': {'minor_range': (0, 1)},
     '122.0': {'minor_range': (0, 1)},
-    '123.0': {'minor_range': (0, 0)},
+    '123.0': {'minor_range': (0, 1)},
+    '124.0': {'minor_range': (0, 2)},
+    '125.0': {'minor_range': (1, 3)},
+    '126.0': {'minor_range': (0, 0)},
 }
 
 
 def get_version():
     choice = random.randint(0, len(versions) - 1)
     i = 0
     for major, props in versions.items():
```

### Comparing `ua-generator-0.4.2/src/ua_generator/data/browsers/safari.py` & `ua_generator-0.5.0/src/ua_generator/data/browsers/safari.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     '10': {'minor_range': (0, 0), 'webkit': '602.4.8'},
     '11': {'minor_range': (0, 0), 'webkit': '604.1.38'},
     '12': {'minor_range': (0, 1), 'webkit': '605.1.15'},
     '13': {'minor_range': (0, 1), 'webkit': '605.1.15'},
     '14': {'minor_range': (0, 1), 'webkit': '605.1.15'},
     '15': {'minor_range': (0, 6), 'webkit': '605.1.15'},
     '16': {'minor_range': (0, 6), 'webkit': '605.1.15'},
-    '17': {'minor_range': (0, 3), 'webkit': '605.1.15'},
+    '17': {'minor_range': (0, 5), 'webkit': '605.1.15'},
 }
 
 
 def get_version():
     choice = random.randint(0, len(versions) - 1)
     i = 0
     for major, props in versions.items():
```

### Comparing `ua-generator-0.4.2/src/ua_generator/data/generator.py` & `ua_generator-0.5.0/src/ua_generator/data/generator.py`

 * *Files identical despite different names*

### Comparing `ua-generator-0.4.2/src/ua_generator/data/platforms/android/android_nexus.py` & `ua_generator-0.5.0/src/ua_generator/data/platforms/android/android_nexus.py`

 * *Files identical despite different names*

### Comparing `ua-generator-0.4.2/src/ua_generator/data/platforms/android/android_pixel.py` & `ua_generator-0.5.0/src/ua_generator/data/platforms/android/android_pixel.py`

 * *Files identical despite different names*

### Comparing `ua-generator-0.4.2/src/ua_generator/data/platforms/android/android_samsung.py` & `ua_generator-0.5.0/src/ua_generator/data/platforms/android/android_samsung.py`

 * *Files identical despite different names*

### Comparing `ua-generator-0.4.2/src/ua_generator/data/platforms/ios.py` & `ua_generator-0.5.0/src/ua_generator/data/platforms/ios.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     '16.4': {'minor_range': (0, 1)},
     '16.5': {'minor_range': (0, 2)},
     '16.6': {'minor_range': (0, 1)},
     '17.0': {'minor_range': (0, 3)},
     '17.1': {'minor_range': (0, 2)},
     '17.2': {'minor_range': (0, 1)},
     '17.3': {'minor_range': (0, 1)},
+    '17.4': {'minor_range': (0, 1)},
+    '17.5': {'minor_range': (0, 1)},
 }
 
 
 def get_version():
     choice = random.randint(0, len(versions) - 1)
     i = 0
     for major, props in versions.items():
```

### Comparing `ua-generator-0.4.2/src/ua_generator/data/platforms/linux.py` & `ua_generator-0.5.0/src/ua_generator/data/platforms/linux.py`

 * *Files identical despite different names*

### Comparing `ua-generator-0.4.2/src/ua_generator/data/platforms/macos.py` & `ua_generator-0.5.0/src/ua_generator/data/platforms/macos.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,24 +22,27 @@
     '11.6': {'minor_range': (0, 6)},
     '12.0': {'minor_range': (0, 1)},
     '12.2': {'minor_range': (0, 1)},
     '12.3': {'minor_range': (0, 1)},
     '12.4': {'minor_range': (0, 0)},
     '12.5': {'minor_range': (0, 1)},
     '12.6': {'minor_range': (0, 4)},
+    '12.7': {'minor_range': (0, 5)},
     '13.0': {'minor_range': (0, 1)},
     '13.1': {'minor_range': (0, 0)},
     '13.2': {'minor_range': (0, 1)},
     '13.3': {'minor_range': (0, 1)},
     '13.4': {'minor_range': (0, 1)},
     '13.5': {'minor_range': (0, 2)},
     '14.0': {'minor_range': (0, 1)},
     '14.1': {'minor_range': (0, 2)},
     '14.2': {'minor_range': (0, 1)},
     '14.3': {'minor_range': (0, 1)},
+    '14.4': {'minor_range': (0, 1)},
+    '14.5': {'minor_range': (0, 0)},
 }
 
 
 def get_version():
     choice = random.randint(0, len(versions) - 1)
     i = 0
     for major, props in versions.items():
```

### Comparing `ua-generator-0.4.2/src/ua_generator/headers.py` & `ua_generator-0.5.0/src/ua_generator/headers.py`

 * *Files identical despite different names*

### Comparing `ua-generator-0.4.2/src/ua_generator/user_agent.py` & `ua_generator-0.5.0/src/ua_generator/user_agent.py`

 * *Files identical despite different names*

### Comparing `ua-generator-0.4.2/src/ua_generator/utils.py` & `ua_generator-0.5.0/src/ua_generator/utils.py`

 * *Files identical despite different names*

### Comparing `ua-generator-0.4.2/src/ua_generator.egg-info/PKG-INFO` & `ua_generator-0.5.0/src/ua_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ua-generator
-Version: 0.4.2
+Version: 0.5.0
 Summary: A random user-agent generator
 Home-page: https://github.com/iamdual/ua-generator
 Author: Ekin Karadeniz
 Author-email: iamdual@icloud.com
 Project-URL: Bug Tracker, https://github.com/iamdual/ua-generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ua-generator-0.4.2/src/ua_generator.egg-info/SOURCES.txt` & `ua_generator-0.5.0/src/ua_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ua-generator-0.4.2/tests/test_browser.py` & `ua_generator-0.5.0/tests/test_browser.py`

 * *Files identical despite different names*

### Comparing `ua-generator-0.4.2/tests/test_client_hints.py` & `ua_generator-0.5.0/tests/test_client_hints.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,105 +2,139 @@
 Random User-Agent
 Copyright: 2022 Ekin Karadeniz (github.com/iamdual)
 License: Apache License 2.0 
 """
 import unittest
 
 import src.ua_generator as ua_generator
+from src.ua_generator import serialization
 from src.ua_generator.data import browsers_support_ch
 
 
 class TestClientHints(unittest.TestCase):
     def test_ch_platform(self):
         for i in range(0, 100):
             ua = ua_generator.generate(browser=browsers_support_ch, platform='macos')
             self.assertIsNotNone(ua.ch)
+            self.assertTrue(type(ua.ch.platform) is str)
             self.assertEqual(ua.ch.platform, '"macOS"')
+            self.assertEqual(ua.ch.get_platform(), 'macOS')
 
     def test_ch_platform_2(self):
         for i in range(0, 100):
             ua = ua_generator.generate(browser=browsers_support_ch, platform='linux')
             self.assertIsNotNone(ua.ch)
+            self.assertTrue(type(ua.ch.platform) is str)
             self.assertEqual(ua.ch.platform, '"Linux"')
+            self.assertEqual(ua.ch.get_platform(), 'Linux')
 
     def test_ch_platform_version(self):
         for i in range(0, 100):
             ua = ua_generator.generate(browser=browsers_support_ch)
             self.assertIsNotNone(ua.ch)
             self.assertTrue(type(ua.ch.platform_version) is str)
             self.assertTrue(len(ua.ch.platform_version) > 0)
+            self.assertEqual(ua.ch.platform_version, serialization.ch_string(ua.ch.get_platform_version()))
 
     def test_ch_platform_version_windows(self):
         for i in range(0, 100):
             ua = ua_generator.generate(platform='windows')
             self.assertIsNotNone(ua.ch)
             self.assertTrue(type(ua.ch.platform_version) is str)
             self.assertEqual(len(ua.ch.platform_version.split('.')), 3)
+            self.assertEqual(ua.ch.platform_version, serialization.ch_string(ua.ch.get_platform_version()))
 
     def test_ch_mobile(self):
         for i in range(0, 100):
             ua = ua_generator.generate(browser=browsers_support_ch, platform='android')
             self.assertIsNotNone(ua.ch)
+            self.assertTrue(type(ua.ch.mobile) is str)
             self.assertEqual(ua.ch.mobile, '?1')
+            self.assertTrue(type(ua.ch.get_mobile()) is bool)
+            self.assertEqual(ua.ch.get_mobile(), True)
 
     def test_ch_non_mobile(self):
         for i in range(0, 100):
             ua = ua_generator.generate(browser=browsers_support_ch, platform='windows')
             self.assertIsNotNone(ua.ch)
+            self.assertTrue(type(ua.ch.mobile) is str)
             self.assertEqual(ua.ch.mobile, '?0')
+            self.assertTrue(type(ua.ch.get_mobile()) is bool)
+            self.assertEqual(ua.ch.get_mobile(), False)
 
     def test_ch_brands(self):
         for i in range(0, 100):
             ua = ua_generator.generate(browser='chrome', platform='windows')
             self.assertIsNotNone(ua.ch)
+            self.assertTrue(type(ua.ch.brands) is str)
             self.assertTrue(ua.ch.brands.startswith('"Not A(Brand";v="99"'))
             self.assertTrue('Chromium' in ua.ch.brands)
             self.assertTrue('Google Chrome' in ua.ch.brands)
+            self.assertTrue(type(ua.ch.get_brands()) is list)
+            self.assertEqual(ua.ch.brands, serialization.ch_brand_list(ua.ch.get_brands()))
 
     def test_ch_brands_full_version_list(self):
         for i in range(0, 100):
             ua = ua_generator.generate(browser='edge', platform='windows')
             self.assertIsNotNone(ua.ch)
+            self.assertTrue(type(ua.ch.brands_full_version_list) is str)
             self.assertTrue(ua.ch.brands_full_version_list.startswith('"Not A(Brand";v="99"'))
             self.assertTrue('Chromium' in ua.ch.brands_full_version_list)
             self.assertTrue('Microsoft Edge' in ua.ch.brands_full_version_list)
+            self.assertTrue(type(ua.ch.get_brands(full_version_list=True)) is list)
+            self.assertEqual(ua.ch.brands_full_version_list,
+                             serialization.ch_brand_list(ua.ch.get_brands(full_version_list=True)))
 
     def test_ch_bitness(self):
         for i in range(0, 100):
             ua = ua_generator.generate(browser=browsers_support_ch)
             self.assertIsNotNone(ua.ch)
+            self.assertTrue(type(ua.ch.bitness) is str)
             self.assertIn(ua.ch.bitness, ('"32"', '"64"'))
+            self.assertIn(ua.ch.get_bitness(), ('32', '64'))
 
     def test_ch_architecture(self):
         for i in range(0, 100):
             ua = ua_generator.generate(browser=browsers_support_ch)
             self.assertIsNotNone(ua.ch)
+            self.assertTrue(type(ua.ch.architecture) is str)
             self.assertIn(ua.ch.architecture, ('"arm"', '"x86"'))
+            self.assertIn(ua.ch.get_architecture(), ('arm', 'x86'))
 
     def test_ch_model(self):
         for i in range(0, 100):
             ua = ua_generator.generate(platform='android', browser='chrome')
             self.assertIsNotNone(ua.ch)
+            self.assertTrue(type(ua.ch.model) is str)
             self.assertTrue(ua.ch.model != '""')
             self.assertTrue(len(ua.ch.model) > 2)
+            self.assertEqual(ua.ch.model, serialization.ch_string(ua.ch.get_model()))
 
     def test_ch_model_2(self):
         for i in range(0, 100):
             ua = ua_generator.generate(platform='linux', browser='firefox')
             self.assertIsNotNone(ua.ch)
+            self.assertTrue(type(ua.ch.model) is str)
             self.assertTrue(ua.ch.model == '""')
+            self.assertEqual(ua.ch.model, serialization.ch_string(ua.ch.get_model()))
 
     def test_ch_wow64(self):
         for i in range(0, 100):
             ua = ua_generator.generate(platform='windows')
             self.assertIsNotNone(ua.ch)
+            self.assertTrue(type(ua.ch.wow64) is str)
             self.assertEqual(ua.ch.wow64, '?1')
+            self.assertTrue(type(ua.ch.get_wow64()) is bool)
+            self.assertEqual(ua.ch.get_wow64(), True)
 
     def test_ch_wow64_2(self):
         for i in range(0, 100):
             ua = ua_generator.generate(platform='linux')
             self.assertIsNotNone(ua.ch)
+            self.assertTrue(type(ua.ch.wow64) is str)
             self.assertEqual(ua.ch.wow64, '?0')
+            self.assertTrue(type(ua.ch.get_wow64()) is bool)
+            self.assertEqual(ua.ch.get_wow64(), False)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ua-generator-0.4.2/tests/test_device.py` & `ua_generator-0.5.0/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `ua-generator-0.4.2/tests/test_exceptions.py` & `ua_generator-0.5.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `ua-generator-0.4.2/tests/test_headers.py` & `ua_generator-0.5.0/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `ua-generator-0.4.2/tests/test_platform.py` & `ua_generator-0.5.0/tests/test_platform.py`

 * *Files identical despite different names*

### Comparing `ua-generator-0.4.2/tests/test_serialization.py` & `ua_generator-0.5.0/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `ua-generator-0.4.2/tests/test_user_agent.py` & `ua_generator-0.5.0/tests/test_user_agent.py`

 * *Files identical despite different names*

### Comparing `ua-generator-0.4.2/tests/test_utils.py` & `ua_generator-0.5.0/tests/test_utils.py`

 * *Files identical despite different names*

