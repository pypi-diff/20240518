# Comparing `tmp/deezer_oauth_cli-1.2.8.tar.gz` & `tmp/deezer_oauth_cli-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deezer_oauth_cli-1.2.8.tar", max compression
+gzip compressed data, was "deezer_oauth_cli-1.3.0.tar", max compression
```

## Comparing `deezer_oauth_cli-1.2.8.tar` & `deezer_oauth_cli-1.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1068 2024-05-07 16:55:14.204769 deezer_oauth_cli-1.2.8/LICENSE
--rw-r--r--   0        0        0     5506 2024-05-07 16:55:14.204769 deezer_oauth_cli-1.2.8/README.md
--rw-r--r--   0        0        0     3414 2024-05-07 16:55:17.216796 deezer_oauth_cli-1.2.8/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-07 16:55:17.216796 deezer_oauth_cli-1.2.8/src/deezer_oauth/__init__.py
--rw-r--r--   0        0        0       53 2024-05-07 16:55:14.204769 deezer_oauth_cli-1.2.8/src/deezer_oauth/__main__.py
--rw-r--r--   0        0        0     1833 2024-05-07 16:55:14.204769 deezer_oauth_cli-1.2.8/src/deezer_oauth/client.py
--rw-r--r--   0        0        0      115 2024-05-07 16:55:14.204769 deezer_oauth_cli-1.2.8/src/deezer_oauth/constants.py
--rw-r--r--   0        0        0     1003 2024-05-07 16:55:14.204769 deezer_oauth_cli-1.2.8/src/deezer_oauth/files.py
--rw-r--r--   0        0        0     1044 2024-05-07 16:55:14.204769 deezer_oauth_cli-1.2.8/src/deezer_oauth/main.py
--rw-r--r--   0        0        0        0 2024-05-07 16:55:14.204769 deezer_oauth_cli-1.2.8/src/deezer_oauth/py.typed
--rw-r--r--   0        0        0     3238 2024-05-07 16:55:14.204769 deezer_oauth_cli-1.2.8/src/deezer_oauth/server.py
--rw-r--r--   0        0        0     6976 1970-01-01 00:00:00.000000 deezer_oauth_cli-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-18 13:12:11.701326 deezer_oauth_cli-1.3.0/LICENSE
+-rw-r--r--   0        0        0     5506 2024-05-18 13:12:11.701326 deezer_oauth_cli-1.3.0/README.md
+-rw-r--r--   0        0        0     3409 2024-05-18 13:12:14.885320 deezer_oauth_cli-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-18 13:12:14.885320 deezer_oauth_cli-1.3.0/src/deezer_oauth/__init__.py
+-rw-r--r--   0        0        0       53 2024-05-18 13:12:11.701326 deezer_oauth_cli-1.3.0/src/deezer_oauth/__main__.py
+-rw-r--r--   0        0        0     1827 2024-05-18 13:12:11.701326 deezer_oauth_cli-1.3.0/src/deezer_oauth/client.py
+-rw-r--r--   0        0        0      115 2024-05-18 13:12:11.701326 deezer_oauth_cli-1.3.0/src/deezer_oauth/constants.py
+-rw-r--r--   0        0        0     1003 2024-05-18 13:12:11.701326 deezer_oauth_cli-1.3.0/src/deezer_oauth/files.py
+-rw-r--r--   0        0        0     1044 2024-05-18 13:12:11.701326 deezer_oauth_cli-1.3.0/src/deezer_oauth/main.py
+-rw-r--r--   0        0        0        0 2024-05-18 13:12:11.701326 deezer_oauth_cli-1.3.0/src/deezer_oauth/py.typed
+-rw-r--r--   0        0        0     3238 2024-05-18 13:12:11.701326 deezer_oauth_cli-1.3.0/src/deezer_oauth/server.py
+-rw-r--r--   0        0        0     6975 1970-01-01 00:00:00.000000 deezer_oauth_cli-1.3.0/PKG-INFO
```

### Comparing `deezer_oauth_cli-1.2.8/LICENSE` & `deezer_oauth_cli-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.2.8/README.md` & `deezer_oauth_cli-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.2.8/pyproject.toml` & `deezer_oauth_cli-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deezer-oauth-cli"
-version = "1.2.8"
+version = "1.3.0"
 description = "A small CLI to quickly obtain an API token for Deezer API."
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/browniebroke/deezer-oauth-cli"
 documentation = "https://github.com/browniebroke/deezer-oauth-cli/blob/main/README.md"
 classifiers = [
@@ -26,24 +26,24 @@
 "Mastodon" = "https://fosstodon.org/@browniebroke"
 
 [tool.poetry.scripts]
 deezer-oauth = "deezer_oauth.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-requests = ">=2.27"
+httpx = ">=0.27.0"
 rich = ">=10"
 typer = {extras = ["all"], version = ">=0.12.0"}
 
 [tool.poetry.group.dev.dependencies]
 pyfakefs = "^5.0"
 pytest = "^8.0.0"
 pytest-cov = "^5.0.0"
 pytest-mock = "^3.6"
-responses = "^0.25.0"
+respx = "^0.21.1"
 
 [tool.semantic_release]
 version_toml = ["pyproject.toml:tool.poetry.version"]
 version_variables = [
     "src/deezer_oauth/__init__.py:__version__",
 ]
 build_command = "pip install poetry && poetry build"
```

### Comparing `deezer_oauth_cli-1.2.8/src/deezer_oauth/client.py` & `deezer_oauth_cli-1.3.0/src/deezer_oauth/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from urllib.parse import parse_qsl, urlencode
 
-import requests
+import httpx
 
 from deezer_oauth.constants import HOST_NAME, OAUTH_RETURN_PATH, SERVER_PORT
 
 
 class OAuthDancer:
     """A class to help with completing the OAuth dance."""
 
@@ -45,12 +45,12 @@
             {
                 "app_id": self.app_id,
                 "secret": self.app_secret,
                 "code": code,
             }
         )
         url = f"{self.base_url}/oauth/access_token.php?{query}"
-        response = requests.get(url, timeout=10)
+        response = httpx.get(url, timeout=10)
         content = response.content.decode()
         # The body looks like this: 'access_token=blah&expires=1234'
         # -> parse this as querystring and convert to a dictionary
         return dict(parse_qsl(content))
```

### Comparing `deezer_oauth_cli-1.2.8/src/deezer_oauth/files.py` & `deezer_oauth_cli-1.3.0/src/deezer_oauth/files.py`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.2.8/src/deezer_oauth/main.py` & `deezer_oauth_cli-1.3.0/src/deezer_oauth/main.py`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.2.8/src/deezer_oauth/server.py` & `deezer_oauth_cli-1.3.0/src/deezer_oauth/server.py`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.2.8/PKG-INFO` & `deezer_oauth_cli-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deezer-oauth-cli
-Version: 1.2.8
+Version: 1.3.0
 Summary: A small CLI to quickly obtain an API token for Deezer API.
 Home-page: https://github.com/browniebroke/deezer-oauth-cli
 License: MIT
 Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: requests (>=2.27)
+Requires-Dist: httpx (>=0.27.0)
 Requires-Dist: rich (>=10)
 Requires-Dist: typer[all] (>=0.12.0)
 Project-URL: Bug Tracker, https://github.com/browniebroke/deezer-oauth-cli/issues
 Project-URL: Changelog, https://github.com/browniebroke/deezer-oauth-cli/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/browniebroke/deezer-oauth-cli/blob/main/README.md
 Project-URL: Mastodon, https://fosstodon.org/@browniebroke
 Project-URL: Repository, https://github.com/browniebroke/deezer-oauth-cli
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: deezer-oauth-cli Version: 1.2.8 Summary: A small
+Metadata-Version: 2.1 Name: deezer-oauth-cli Version: 1.3.0 Summary: A small
 CLI to quickly obtain an API token for Deezer API. Home-page: https://
 github.com/browniebroke/deezer-oauth-cli License: MIT Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
-Topic :: Software Development :: Libraries Requires-Dist: requests (>=2.27)
+Topic :: Software Development :: Libraries Requires-Dist: httpx (>=0.27.0)
 Requires-Dist: rich (>=10) Requires-Dist: typer[all] (>=0.12.0) Project-URL:
 Bug Tracker, https://github.com/browniebroke/deezer-oauth-cli/issues Project-
 URL: Changelog, https://github.com/browniebroke/deezer-oauth-cli/blob/main/
 CHANGELOG.md Project-URL: Documentation, https://github.com/browniebroke/
 deezer-oauth-cli/blob/main/README.md Project-URL: Mastodon, https://
 fosstodon.org/@browniebroke Project-URL: Repository, https://github.com/
 browniebroke/deezer-oauth-cli Project-URL: Twitter, https://twitter.com/
```

