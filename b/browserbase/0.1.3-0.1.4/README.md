# Comparing `tmp/browserbase-0.1.3.tar.gz` & `tmp/browserbase-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browserbase-0.1.3.tar", last modified: Thu May 16 14:17:32 2024, max compression
+gzip compressed data, was "browserbase-0.1.4.tar", last modified: Sat May 18 11:35:52 2024, max compression
```

## Comparing `browserbase-0.1.3.tar` & `browserbase-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-16 14:17:32.346690 browserbase-0.1.3/
--rw-r--r--   0 mish       (501) staff       (20)     1064 2024-04-09 17:45:47.000000 browserbase-0.1.3/LICENSE
--rw-r--r--   0 mish       (501) staff       (20)     1575 2024-05-16 14:17:32.346409 browserbase-0.1.3/PKG-INFO
--rw-r--r--   0 mish       (501) staff       (20)      933 2024-04-19 10:57:22.000000 browserbase-0.1.3/README.md
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-16 14:17:32.344583 browserbase-0.1.3/browserbase/
--rw-r--r--   0 mish       (501) staff       (20)    10720 2024-05-16 14:16:11.000000 browserbase-0.1.3/browserbase/__init__.py
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-16 14:17:32.345845 browserbase-0.1.3/browserbase/helpers/
--rw-r--r--   0 mish       (501) staff       (20)      301 2024-04-16 18:32:01.000000 browserbase-0.1.3/browserbase/helpers/anthropic.py
--rw-r--r--   0 mish       (501) staff       (20)      503 2024-04-15 12:54:51.000000 browserbase-0.1.3/browserbase/helpers/gpt4.py
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-16 14:17:32.346166 browserbase-0.1.3/browserbase.egg-info/
--rw-r--r--   0 mish       (501) staff       (20)     1575 2024-05-16 14:17:32.000000 browserbase-0.1.3/browserbase.egg-info/PKG-INFO
--rw-r--r--   0 mish       (501) staff       (20)      291 2024-05-16 14:17:32.000000 browserbase-0.1.3/browserbase.egg-info/SOURCES.txt
--rw-r--r--   0 mish       (501) staff       (20)        1 2024-05-16 14:17:32.000000 browserbase-0.1.3/browserbase.egg-info/dependency_links.txt
--rw-r--r--   0 mish       (501) staff       (20)       49 2024-05-16 14:17:32.000000 browserbase-0.1.3/browserbase.egg-info/requires.txt
--rw-r--r--   0 mish       (501) staff       (20)       12 2024-05-16 14:17:32.000000 browserbase-0.1.3/browserbase.egg-info/top_level.txt
--rw-r--r--   0 mish       (501) staff       (20)      697 2024-05-16 14:17:21.000000 browserbase-0.1.3/pyproject.toml
--rw-r--r--   0 mish       (501) staff       (20)       38 2024-05-16 14:17:32.346742 browserbase-0.1.3/setup.cfg
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-18 11:35:52.871099 browserbase-0.1.4/
+-rw-r--r--   0 mish       (501) staff       (20)     1064 2024-04-09 17:45:47.000000 browserbase-0.1.4/LICENSE
+-rw-r--r--   0 mish       (501) staff       (20)     1575 2024-05-18 11:35:52.870814 browserbase-0.1.4/PKG-INFO
+-rw-r--r--   0 mish       (501) staff       (20)      933 2024-04-19 10:57:22.000000 browserbase-0.1.4/README.md
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-18 11:35:52.868841 browserbase-0.1.4/browserbase/
+-rw-r--r--   0 mish       (501) staff       (20)    10500 2024-05-18 11:35:32.000000 browserbase-0.1.4/browserbase/__init__.py
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-18 11:35:52.870128 browserbase-0.1.4/browserbase/helpers/
+-rw-r--r--   0 mish       (501) staff       (20)      301 2024-04-16 18:32:01.000000 browserbase-0.1.4/browserbase/helpers/anthropic.py
+-rw-r--r--   0 mish       (501) staff       (20)      503 2024-04-15 12:54:51.000000 browserbase-0.1.4/browserbase/helpers/gpt4.py
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-18 11:35:52.870533 browserbase-0.1.4/browserbase.egg-info/
+-rw-r--r--   0 mish       (501) staff       (20)     1575 2024-05-18 11:35:52.000000 browserbase-0.1.4/browserbase.egg-info/PKG-INFO
+-rw-r--r--   0 mish       (501) staff       (20)      291 2024-05-18 11:35:52.000000 browserbase-0.1.4/browserbase.egg-info/SOURCES.txt
+-rw-r--r--   0 mish       (501) staff       (20)        1 2024-05-18 11:35:52.000000 browserbase-0.1.4/browserbase.egg-info/dependency_links.txt
+-rw-r--r--   0 mish       (501) staff       (20)       49 2024-05-18 11:35:52.000000 browserbase-0.1.4/browserbase.egg-info/requires.txt
+-rw-r--r--   0 mish       (501) staff       (20)       12 2024-05-18 11:35:52.000000 browserbase-0.1.4/browserbase.egg-info/top_level.txt
+-rw-r--r--   0 mish       (501) staff       (20)      697 2024-05-18 11:35:48.000000 browserbase-0.1.4/pyproject.toml
+-rw-r--r--   0 mish       (501) staff       (20)       38 2024-05-18 11:35:52.871156 browserbase-0.1.4/setup.cfg
```

### Comparing `browserbase-0.1.3/LICENSE` & `browserbase-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `browserbase-0.1.3/PKG-INFO` & `browserbase-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserbase
-Version: 0.1.3
+Version: 0.1.4
 Summary: Browserbase Python SDK
 Author-email: Browserbase <info@browserbase.com>
 Project-URL: Homepage, https://browserbase.com
 Project-URL: Source, https://github.com/browserbase/python-sdk
 Project-URL: Issues, https://github.com/browserbase/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `browserbase-0.1.3/README.md` & `browserbase-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `browserbase-0.1.3/browserbase/__init__.py` & `browserbase-0.1.4/browserbase/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,60 +1,38 @@
 import os
 import httpx
 import time
-from typing import Optional, Sequence, Union, List
+from typing import Optional, Sequence, Union, Literal
 from enum import Enum
-from pydantic import BaseModel, Field
+from pydantic import BaseModel
 from playwright.sync_api import sync_playwright
 
 
-class BrowserType(str, Enum):
-    CHROME = "chrome"
-    FIREFOX = "firefox"
-    EDGE = "edge"
-    SAFARI = "safari"
-
-
-class DeviceType(str, Enum):
-    DESKTOP = "desktop"
-    MOBILE = "mobile"
-
-
-class OperatingSystem(str, Enum):
-    WINDOWS = "windows"
-    MACOS = "macos"
-    LINUX = "linux"
-    IOS = "ios"
-    ANDROID = "android"
-
-
-class SessionStatus(str, Enum):
-    NEW = "NEW"
-    CREATED = "CREATED"
-    ERROR = "ERROR"
-    RUNNING = "RUNNING"
-    REQUEST_RELEASE = "REQUEST_RELEASE"
-    RELEASING = "RELEASING"
-    COMPLETED = "COMPLETED"
+BrowserType = Literal["chrome", "firefox", "edge", "safari"]
+DeviceType = Literal["desktop", "mobile"]
+OperatingSystem = Literal["windows", "macos", "linux", "ios", "android"]
+SessionStatus = Literal[
+    "NEW", "CREATED", "ERROR", "RUNNING", "REQUEST_RELEASE", "RELEASING", "COMPLETED"
+]
 
 
 class Screen(BaseModel):
     maxHeight: Optional[int] = None
     maxWidth: Optional[int] = None
     minHeight: Optional[int] = None
     minWidth: Optional[int] = None
 
 
 class Fingerprint(BaseModel):
     browserListQuery: Optional[str] = None
     httpVersion: Optional[int] = None
-    browsers: Optional[List[BrowserType]] = None
-    devices: Optional[List[DeviceType]] = None
-    locales: Optional[List[str]] = None
-    operatingSystems: Optional[List[OperatingSystem]] = None
+    browsers: Optional[list[BrowserType]] = None
+    devices: Optional[list[DeviceType]] = None
+    locales: Optional[list[str]] = None
+    operatingSystems: Optional[list[OperatingSystem]] = None
     screen: Optional[Screen] = None
 
 
 class CreateSessionOptions(BaseModel):
     projectId: Optional[str] = None
     extensionId: Optional[str] = None
     fingerprint: Optional[Fingerprint] = None
@@ -125,23 +103,25 @@
     ):
         """Create new Browserbase SDK client instance"""
         self.api_key = api_key or os.environ["BROWSERBASE_API_KEY"]
         self.project_id = project_id or os.environ["BROWSERBASE_PROJECT_ID"]
         self.connect_url = connect_url or "wss://connect.browserbase.com"
         self.api_url = api_url or "https://www.browserbase.com"
 
-    def get_connect_url(self, session_id=None, proxy=False):
+    def get_connect_url(
+        self, session_id: Optional[str] = None, proxy: Optional[bool] = None
+    ):
         base_url = f"{self.connect_url}?apiKey={self.api_key}"
         if session_id:
             base_url += f"&sessionId={session_id}"
         if proxy:
             base_url += "&enableProxy=true"
         return base_url
 
-    def list_sessions(self) -> List[Session]:
+    def list_sessions(self) -> list[Session]:
         response = httpx.get(
             f"{self.api_url}/v1/sessions",
             headers={
                 "x-bb-api-key": self.api_key,
                 "Content-Type": "application/json",
             },
         )
@@ -163,15 +143,15 @@
             },
             json=payload,
         )
 
         response.raise_for_status()
         return Session(**response.json())
 
-    def get_session(self, session_id: str) -> List[Session]:
+    def get_session(self, session_id: str) -> Session:
         response = httpx.get(
             f"{self.api_url}/v1/sessions/{session_id}",
             headers={
                 "x-bb-api-key": self.api_key,
                 "Content-Type": "application/json",
             },
         )
@@ -194,15 +174,15 @@
             },
             json=payload,
         )
 
         response.raise_for_status()
         return Session(**response.json())
 
-    def get_session_recording(self, session_id: str) -> List[SessionRecording]:
+    def get_session_recording(self, session_id: str) -> list[SessionRecording]:
         response = httpx.get(
             f"{self.api_url}/v1/sessions/{session_id}/recording",
             headers={
                 "x-bb-api-key": self.api_key,
                 "Content-Type": "application/json",
             },
         )
@@ -243,15 +223,15 @@
                 "Content-Type": "application/json",
             },
         )
 
         response.raise_for_status()
         return DebugConnectionURLs(**response.json())
 
-    def get_session_logs(self, session_id: str) -> List[SessionLog]:
+    def get_session_logs(self, session_id: str) -> list[SessionLog]:
         response = httpx.get(
             f"{self.api_url}/v1/sessions/{session_id}/logs",
             headers={
                 "x-bb-api-key": self.api_key,
                 "Content-Type": "application/json",
             },
         )
```

### Comparing `browserbase-0.1.3/browserbase.egg-info/PKG-INFO` & `browserbase-0.1.4/browserbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserbase
-Version: 0.1.3
+Version: 0.1.4
 Summary: Browserbase Python SDK
 Author-email: Browserbase <info@browserbase.com>
 Project-URL: Homepage, https://browserbase.com
 Project-URL: Source, https://github.com/browserbase/python-sdk
 Project-URL: Issues, https://github.com/browserbase/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `browserbase-0.1.3/pyproject.toml` & `browserbase-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "browserbase"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Browserbase", email="info@browserbase.com" },
 ]
 description = "Browserbase Python SDK"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

