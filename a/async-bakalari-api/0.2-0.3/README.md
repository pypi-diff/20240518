# Comparing `tmp/async_bakalari_api-0.2.tar.gz` & `tmp/async_bakalari_api-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_bakalari_api-0.2.tar", last modified: Tue May 14 11:35:44 2024, max compression
+gzip compressed data, was "async_bakalari_api-0.3.tar", last modified: Sat May 18 15:17:48 2024, max compression
```

## Comparing `async_bakalari_api-0.2.tar` & `async_bakalari_api-0.3.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:35:44.124381 async_bakalari_api-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-14 11:35:39.000000 async_bakalari_api-0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-05-14 11:35:44.124381 async_bakalari_api-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-14 11:35:39.000000 async_bakalari_api-0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-05-14 11:35:39.000000 async_bakalari_api-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 11:35:44.124381 async_bakalari_api-0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:35:44.120381 async_bakalari_api-0.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:35:39.000000 async_bakalari_api-0.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:35:44.124381 async_bakalari_api-0.2/src/async_bakalari_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-05-14 11:35:44.000000 async_bakalari_api-0.2/src/async_bakalari_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-14 11:35:44.000000 async_bakalari_api-0.2/src/async_bakalari_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 11:35:44.000000 async_bakalari_api-0.2/src/async_bakalari_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 11:35:44.000000 async_bakalari_api-0.2/src/async_bakalari_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 11:35:43.000000 async_bakalari_api-0.2/src/async_bakalari_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-14 11:35:44.000000 async_bakalari_api-0.2/src/async_bakalari_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 11:35:44.000000 async_bakalari_api-0.2/src/async_bakalari_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:35:44.120381 async_bakalari_api-0.2/src/bakalari_api/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-14 11:35:39.000000 async_bakalari_api-0.2/src/bakalari_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 11:35:39.000000 async_bakalari_api-0.2/src/bakalari_api/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13055 2024-05-14 11:35:39.000000 async_bakalari_api-0.2/src/bakalari_api/bakalari.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-14 11:35:39.000000 async_bakalari_api-0.2/src/bakalari_api/bakalari_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-14 11:35:39.000000 async_bakalari_api-0.2/src/bakalari_api/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-14 11:35:39.000000 async_bakalari_api-0.2/src/bakalari_api/datastructure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-14 11:35:39.000000 async_bakalari_api-0.2/src/bakalari_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-14 11:35:39.000000 async_bakalari_api-0.2/src/bakalari_api/first_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-05-14 11:35:39.000000 async_bakalari_api-0.2/src/bakalari_api/komens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-14 11:35:39.000000 async_bakalari_api-0.2/src/bakalari_api/logger_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:17:48.688350 async_bakalari_api-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16070 2024-05-18 15:17:48.688350 async_bakalari_api-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 15:17:48.688350 async_bakalari_api-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:17:48.684350 async_bakalari_api-0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:17:48.688350 async_bakalari_api-0.3/src/async_bakalari_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16070 2024-05-18 15:17:48.000000 async_bakalari_api-0.3/src/async_bakalari_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-18 15:17:48.000000 async_bakalari_api-0.3/src/async_bakalari_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:17:48.000000 async_bakalari_api-0.3/src/async_bakalari_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-18 15:17:48.000000 async_bakalari_api-0.3/src/async_bakalari_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:17:48.000000 async_bakalari_api-0.3/src/async_bakalari_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-18 15:17:48.000000 async_bakalari_api-0.3/src/async_bakalari_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:17:48.688350 async_bakalari_api-0.3/src/bakalari_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/bakalari_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/bakalari_api/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14669 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/bakalari_api/bakalari.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/bakalari_api/bakalari_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/bakalari_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/bakalari_api/datastructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/bakalari_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/bakalari_api/first_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/bakalari_api/komens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/src/bakalari_api/logger_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:17:48.688350 async_bakalari_api-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    19347 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/tests/test_bakalari.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/tests/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/tests/test_datastructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6279 2024-05-18 15:17:43.000000 async_bakalari_api-0.3/tests/test_komens.py
```

### Comparing `async_bakalari_api-0.2/LICENSE.md` & `async_bakalari_api-0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `async_bakalari_api-0.2/PKG-INFO` & `async_bakalari_api-0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_bakalari_api
-Version: 0.2
+Version: 0.3
 Summary: Async API for Bakalari endpoint v3
 Author-email: "Lukas Svoboda (@schizza)" <opensource@schizza.cz>
 Maintainer-email: Lukas Svoboda <opensource@schizza.cz>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -204,72 +204,89 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/schizza/bakalari-api3
-Project-URL: Documentation, https://github.com/schizza/bakalari-api3
+Project-URL: Documentation, https://async-bakalari-api.schizza.cz
 Project-URL: Repository, https://github.com/schizza/bakalari-api3
 Project-URL: Bug Tracker, https://github.com/schizza/bakalari-api3/issues
 Project-URL: Changelog, https://github.com/schizza/bakalari-api3/blob/master/CHANGELOG.md
 Keywords: bakalari,async
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: asyncio
-Requires-Dist: typing
-Requires-Dist: aiohttp
-Requires-Dist: orjson
-Requires-Dist: async_timeout
-Requires-Dist: logger
-Requires-Dist: strenum
-Requires-Dist: pytest
 
 [![codecov](https://codecov.io/gh/schizza/async-bakalari-api3/graph/badge.svg?token=KC2WYAOLOP)](https://codecov.io/gh/schizza/async-bakalari-api3)
 
-# Python async client for Bakalari API v3
+# Changelog
 
-### 0.0.2
+All notable changes to this project will be documented in this file.
 
-## Added
+🇨🇿 Full documentation (czech) on [this site](https://async-bakalari-api.schizza.cz)
 
-* better exceptions handling and logging
-* class Komens
-  * count unread messages
-  * get all messages
+## [0.3]
 
-* tests and coverage
+### Added
 
-## Changed
+- `bakalari_demo.py` is now CLI application
+- `Komens` now support for downloading attachment - `get_attachment`
+- `send_auth_request` now supports extending EndPoints url wiht `extend` argument
+- `school_list` now supports variable `town` - fetch schools in the town to limit downloading full list of schools.
+- `Messages` class now have function `json` to return messages as JSON representative
+- `Messages` class have `__str__` function for better handling `str(Messages)`
 
-* async_schools_list moved to Bakalari class
-* Refactor login functions
-* Refactor token handling
+### Changed
 
-## Fixed
+- refactor of the code for speed and better reading of the code
+- `school_list` now fetching schools in concurency mode - improved speed form about 1:30 min to 20s
+- `mid` variable in the `MessageContainter` is now string instead of integer.
+- `async_school_list` renamed to `school_list` as all methods are async
+- `MessageContainter` returns JSON bytes on `as_json()` call instead of `orjson.Fragment`
+- `get_messsages()` renamed to `fetch_messages()`
 
-* Invalid refresh token
-* Refactor send_request to better maintenance
+### Removed
 
-### v0.1
+- `username` from `Credentials` - as we do not need to store it
 
-## Class School from `datastructure.py`
+## [0.2]
 
-Now supports to download list of schools with their API points.
+### Added
 
-* get_url by school name or index in list
-* search school by town
-* cache list of schools by saving and loading list in JSON format
+- better exceptions handling and logging
+- `class Komens`
+  - count unread messages
+  - get all messages
+  - tests and coverage
 
-## Class Bakalari
+### Changed
 
-* first login with username and password and stores access and refresh token
-* automaticaly refreshes access token with refresh token if refresh token is not expired
-* save access and refresh token localy to be cached
+- `async_schools_list` moved to `Bakalari` class
+- Refactor login functions
+- Refactor token handling
 
-## Class Komens
+### Fixed
 
-* count unread messages `count_unread_messages`
+- Invalid refresh token
+- Refactor send_request to better maintenance
+
+## [0.0.1]
+
+### Added
+
+- main `class Bakalari`
+
+  - supports saving `access token` and `refresh token` localy
+  - automatically refreshes access token with refresh token if refresh token is not expired
+
+- `class Schools` in `datastructures.py` lists all schools with their API points
+
+  - get_url by school name or index in list
+  - search school by town
+  - cache list of schools by saving and loading list in JSON format
+
+[unreleased]: https://github.com/schizza/bakalari-api3/compare/v0.0.1...HEAD
+[0.0.1]: https://github.com/schizza/bakalari-api3/releases/tag/v0.0.1
```

### Comparing `async_bakalari_api-0.2/pyproject.toml` & `async_bakalari_api-0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,16 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "async_bakalari_api"
-version = "0.2"
-dependencies = [
-  "asyncio",
-  "typing",
-  "aiohttp",
-  "orjson",
-  "async_timeout",
-  "logger",
-  "strenum",
-  "pytest",
-]
+version = "0.3"
+dynamic = ["dependencies"]
+
 
 requires-python = ">=3.12"
 authors = [
   {name = "Lukas Svoboda (@schizza)", email = "opensource@schizza.cz"}
 ]
 maintainers = [
   {name = "Lukas Svoboda", email = "opensource@schizza.cz"}
@@ -29,35 +21,44 @@
 license = {file = "LICENSE.md"}
 keywords = ["bakalari", "async"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python"
 ]
 
+[tool.setuptools.dynamic]
+dependencies = { file = ["requirements.in"] }
+
+[tool.setuptools]
+platforms = ["any"]
+zip-safe  = false
+include-package-data = true
+
 [project.urls]
 Homepage = "https://github.com/schizza/bakalari-api3"
-Documentation = "https://github.com/schizza/bakalari-api3"
+Documentation = "https://async-bakalari-api.schizza.cz"
 Repository = "https://github.com/schizza/bakalari-api3"
 "Bug Tracker" = "https://github.com/schizza/bakalari-api3/issues"
 Changelog = "https://github.com/schizza/bakalari-api3/blob/master/CHANGELOG.md"
 
 [project.scripts]
 bakalari = "bakalari_api:main"
 
-[tool.setuptools]
-platforms = ["any"]
-zip-safe  = false
-include-package-data = true
-
 [tool.pylint.MAIN]
 py-version = "3.12"
 ignore = [
     "tests"
 ]
 
+[tool.coverage.run]
+omit = [
+    "tests/*",
+    "src/bakalari_api/bakalari_demo.py"
+  ]
+
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 testpaths = [
     "tests"
 ]
 addopts = "--cov=bakalari_api --cov-report html"
```

### Comparing `async_bakalari_api-0.2/src/async_bakalari_api.egg-info/PKG-INFO` & `async_bakalari_api-0.3/src/async_bakalari_api.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_bakalari_api
-Version: 0.2
+Version: 0.3
 Summary: Async API for Bakalari endpoint v3
 Author-email: "Lukas Svoboda (@schizza)" <opensource@schizza.cz>
 Maintainer-email: Lukas Svoboda <opensource@schizza.cz>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -204,72 +204,89 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/schizza/bakalari-api3
-Project-URL: Documentation, https://github.com/schizza/bakalari-api3
+Project-URL: Documentation, https://async-bakalari-api.schizza.cz
 Project-URL: Repository, https://github.com/schizza/bakalari-api3
 Project-URL: Bug Tracker, https://github.com/schizza/bakalari-api3/issues
 Project-URL: Changelog, https://github.com/schizza/bakalari-api3/blob/master/CHANGELOG.md
 Keywords: bakalari,async
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: asyncio
-Requires-Dist: typing
-Requires-Dist: aiohttp
-Requires-Dist: orjson
-Requires-Dist: async_timeout
-Requires-Dist: logger
-Requires-Dist: strenum
-Requires-Dist: pytest
 
 [![codecov](https://codecov.io/gh/schizza/async-bakalari-api3/graph/badge.svg?token=KC2WYAOLOP)](https://codecov.io/gh/schizza/async-bakalari-api3)
 
-# Python async client for Bakalari API v3
+# Changelog
 
-### 0.0.2
+All notable changes to this project will be documented in this file.
 
-## Added
+🇨🇿 Full documentation (czech) on [this site](https://async-bakalari-api.schizza.cz)
 
-* better exceptions handling and logging
-* class Komens
-  * count unread messages
-  * get all messages
+## [0.3]
 
-* tests and coverage
+### Added
 
-## Changed
+- `bakalari_demo.py` is now CLI application
+- `Komens` now support for downloading attachment - `get_attachment`
+- `send_auth_request` now supports extending EndPoints url wiht `extend` argument
+- `school_list` now supports variable `town` - fetch schools in the town to limit downloading full list of schools.
+- `Messages` class now have function `json` to return messages as JSON representative
+- `Messages` class have `__str__` function for better handling `str(Messages)`
 
-* async_schools_list moved to Bakalari class
-* Refactor login functions
-* Refactor token handling
+### Changed
 
-## Fixed
+- refactor of the code for speed and better reading of the code
+- `school_list` now fetching schools in concurency mode - improved speed form about 1:30 min to 20s
+- `mid` variable in the `MessageContainter` is now string instead of integer.
+- `async_school_list` renamed to `school_list` as all methods are async
+- `MessageContainter` returns JSON bytes on `as_json()` call instead of `orjson.Fragment`
+- `get_messsages()` renamed to `fetch_messages()`
 
-* Invalid refresh token
-* Refactor send_request to better maintenance
+### Removed
 
-### v0.1
+- `username` from `Credentials` - as we do not need to store it
 
-## Class School from `datastructure.py`
+## [0.2]
 
-Now supports to download list of schools with their API points.
+### Added
 
-* get_url by school name or index in list
-* search school by town
-* cache list of schools by saving and loading list in JSON format
+- better exceptions handling and logging
+- `class Komens`
+  - count unread messages
+  - get all messages
+  - tests and coverage
 
-## Class Bakalari
+### Changed
 
-* first login with username and password and stores access and refresh token
-* automaticaly refreshes access token with refresh token if refresh token is not expired
-* save access and refresh token localy to be cached
+- `async_schools_list` moved to `Bakalari` class
+- Refactor login functions
+- Refactor token handling
 
-## Class Komens
+### Fixed
 
-* count unread messages `count_unread_messages`
+- Invalid refresh token
+- Refactor send_request to better maintenance
+
+## [0.0.1]
+
+### Added
+
+- main `class Bakalari`
+
+  - supports saving `access token` and `refresh token` localy
+  - automatically refreshes access token with refresh token if refresh token is not expired
+
+- `class Schools` in `datastructures.py` lists all schools with their API points
+
+  - get_url by school name or index in list
+  - search school by town
+  - cache list of schools by saving and loading list in JSON format
+
+[unreleased]: https://github.com/schizza/bakalari-api3/compare/v0.0.1...HEAD
+[0.0.1]: https://github.com/schizza/bakalari-api3/releases/tag/v0.0.1
```

### Comparing `async_bakalari_api-0.2/src/bakalari_api/bakalari.py` & `async_bakalari_api-0.3/src/bakalari_api/bakalari.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 log = api_logger("Bakalari API", loglevel=logging.ERROR).get()
 
 
 class Bakalari:
     """Root class of Bakalari."""
 
-    session: aiohttp.ClientSession | None = None
     response: None
     response_json: None
 
     _close_session = False
 
     def __init__(
         self,
@@ -47,22 +46,40 @@
         """
 
         self.server = server
         self.credentials = Credentials
         self.new_token = False
         self.auto_cache_credentials = auto_cache_credentials
         self.cache_filename = cache_filename
+        self.session = aiohttp.ClientSession()
 
         if self.auto_cache_credentials and not self.cache_filename:
             raise Ex.CacheError("Auto-cache is enabled, but no filename is provided!")
 
-    async def send_auth_request(self, request_endpoint: EndPoint, **kwargs):
+    def __del__(self):
+        """Destructor."""
+        # Close connection when this object is destroyed
+        try:
+            loop = asyncio.get_event_loop()
+            if loop.is_running():
+                return loop.create_task(self.session.close())
+            loop.run_until_complete(self.session.close())
+        finally:
+            pass
+
+    async def send_auth_request(
+        self, request_endpoint: EndPoint, extend: str | None = None, **kwargs
+    ):
         """Send authorized request with access token or refresh token."""
 
         request = self.get_request_url(request_endpoint)
+
+        if extend:
+            request += extend
+
         method = hdrs.METH_POST if "post" in request_endpoint.method else hdrs.METH_GET
 
         access_token_invalid = False
         result = None
 
         if not self.credentials.access_token and not self.credentials.refresh_token:
             raise Ex.TokenMissing("Access token or Refresh token is missing!")
@@ -88,15 +105,14 @@
                     continue
                 except Exception as ex:
                     raise ex from ex
                 else:
                     return result
 
             if access_token_invalid and self.refresh_access_token:
-                log.debug("Trying refresh token ...")
                 try:
                     await self.refresh_access_token()
                 except Ex.RefreshTokenExpired as ex:
                     log.error("Refresh token expired! Login with username/password")
                     raise ex from ex
                 except Exception as ex:
                     raise ex from ex
@@ -156,31 +172,42 @@
             Ex.RefreshTokenExpired: _description_
 
         Returns:
             str: response in json format
 
         """
 
-        if not self.session or self.session.closed:
-            self.session = aiohttp.ClientSession()
+        filedata = None
+        filename = None
+
+        if method == hdrs.METH_GET:
+            session = self.session.get
+        else:
+            session = self.session.post
 
         log.debug("Requesting URL %s, kwargs: %s", url, kwargs)
         try:
             async with asyncio.timeout(REQUEST_TIMEOUT):
-                async with self.session:
-                    if method == hdrs.METH_GET:
-                        response = await self.session.get(
-                            url, ssl=True, headers=headers, **kwargs
+
+                async with session(
+                    url, ssl=True, headers=headers, **kwargs
+                ) as response:
+
+                    if (
+                        response.headers.get(aiohttp.hdrs.CONTENT_TYPE)
+                        == "application/octet-stream"
+                    ):
+                        filedata = await response.read()
+                        filename = response.headers[aiohttp.hdrs.CONTENT_DISPOSITION]
+                        filename = parse.unquote(
+                            filename[filename.rindex("filename*=") + 17 :]
                         )
                     else:
-                        response = await self.session.post(
-                            url, ssl=True, headers=headers, **kwargs
-                        )
-                    response_json = await response.json()
-                    log.debug(f"Response: {response}")
+                        response_json = await response.json()
+                        log.debug(f"Response: {response_json}")
 
         except TimeoutError as err:
             raise Ex.TimeoutException(
                 f"Timeout occurred while connecting to server {url}"
             ) from err
         except aiohttp.ClientConnectionError as err:
             raise Ex.BadRequestException(f"Connection error: {url}") from err
@@ -212,87 +239,117 @@
                         raise Ex.RefreshTokenRedeemd("Refresh token already redeemd!")
                     case x if Errors.INVALID_REFRESH_TOKEN in x:
                         raise Ex.InvalidRefreshToken("Invalid refresh token!")
                     case _:
                         raise Ex.BadRequestException(
                             f"{url} with message: {response_json}"
                         )
+            case 404:
+                raise Ex.BadRequestException(f"Not found! ({url})")
             case 200:
-                return response_json
+                return [filename, filedata] if filedata else response_json
             case _:
                 raise Ex.BadRequestException(f"{url} with message: {response_json}")
 
-    async def async_schools_list(self) -> Schools:
+    async def schools_list(self, town: str | None = None) -> Schools:
         """Return list of schools with their API points."""
 
         _schools_list = Schools()
         headers = {"Accept": "application/json"}
 
-        log.debug("Gathering list of towns ...")
-        try:
-            towns_json = await self.send_unauth_request(EndPoint.SCHOOL_LIST, headers)
-        except Exception as exc:
-            log.error(f"Error while gathering schools endpoints. {exc}")
-            return None
+        if not town:
+            log.debug("Gathering list of towns ...")
+            try:
+                towns_json = await self.send_unauth_request(
+                    EndPoint.SCHOOL_LIST, headers
+                )
+            except Exception as exc:
+                log.error(f"Error while gathering schools endpoints. {exc}")
+                return None
+        else:
+            towns_json: dict = [{"name": f"{town}"}]
 
         schools: list = []
+        tasks = []
 
-        for town in towns_json:
-            town_name = str(town["name"])
-            if town_name == "":
+        for _town in towns_json:
+            town_name = str(_town["name"])
+            if town_name == "" or None:
                 continue
             if "." in town_name:
                 town_name = town_name[: town_name.find(".")]
 
             log.debug("Gathering schools for town: %s", town_name)
 
             endpoint = f"{EndPoint.SCHOOL_LIST.endpoint}/{parse.quote(town_name)}"
 
-            response_town = await self._send_request(endpoint, hdrs.METH_GET, headers)
+            task = asyncio.create_task(
+                self._send_request(endpoint, hdrs.METH_GET, headers), name=town_name
+            )
+            tasks.append(task)
+
+        responses = await asyncio.gather(*tasks)
+        for response_town in responses:
 
             schools: dict = response_town
             for _schools in schools.get("schools"):
                 _schools_list.append_school(
                     name=_schools.get("name"),
                     api_point=_schools.get("schoolUrl"),
-                    town=town_name,
+                    town=response_town.get("name"),
                 )
 
         return _schools_list
 
     async def first_login(self, username: str, password: str) -> Credentials:
         """First login.
 
         Create access and refresh tokens.
         """
 
-        login_url = f"client_id=ANDR&grant_type=password&username={username}&password={password}"
+        login_params = parse.urlencode(
+            {
+                "client_id": "ANDR",
+                "grant_type": "password",
+                "username": username,
+                "password": password,
+            }
+        )
+
         headers = {"Content-Type": "application/x-www-form-urlencoded"}
 
         try:
-            log.debug("Trying to login with username and password ...")
+            log.debug(f"Trying to login with username: {username}")
             _credentials = await self.send_unauth_request(
-                EndPoint.LOGIN, data=login_url, headers=headers
+                EndPoint.LOGIN, data=login_params, headers=headers
             )
         except Ex.InvalidLogin as ex:
             log.error("Invalid username / password provided.")
             raise ex from ex
         _credentials.update({"username": username})
         self.credentials = Credentials.create(_credentials)
 
+        log.info(f"Successfully logged in with username: {username}")
+
         if self.auto_cache_credentials:
             self.save_credentials()
         return self.credentials
 
     async def refresh_access_token(self):
         """Refresh access token using refresh token.
 
         returns new Credentials if success, else RefreshTokenExpired exception
         """
-        login_body = f"client_id=ANDR&grant_type=refresh_token&refresh_token={self.credentials.refresh_token}"
+        login_body = parse.urlencode(
+            {
+                "client_id": "ANDR",
+                "grant_type": "refresh_token",
+                "refresh_token": self.credentials.refresh_token,
+            }
+        )
         headers = {"Content-Type": "application/x-www-form-urlencoded"}
 
         try:
             log.debug("Trying refresh token ... ")
             _credentials = await self.send_unauth_request(
                 EndPoint.LOGIN, headers=headers, data=login_body
             )
@@ -315,14 +372,15 @@
         Raises:
             Ex.BadEndpointUrl: if no server is specified
 
         Returns:
             str: full url of endpoint
 
         """
+
         request = (
             request_endpoint.endpoint
             if request_endpoint.endpoint.lower().startswith(("http", "https"))
             else f"{self.server}{request_endpoint.endpoint}"
         )
 
         if not request.lower().startswith(("http", "https")):
@@ -332,36 +390,36 @@
 
     def save_credentials(self, filename: str | None = None) -> bool:
         """Save credentials to file in JSON format.
 
         If auto_save_credentials are enabled, parameters could be ommited.
         """
 
-        if not filename and self.auto_cache_credentials:
-            filename = self.cache_filename
+        filename = filename or self.cache_filename
         try:
             with open(filename, "wb") as file:
                 file.write(orjson.dumps(self.credentials, option=orjson.OPT_INDENT_2))
-            file.close()
-        except OSError:
+        except OSError as err:
+            log.error(f"Error while saving credentials to file {filename}. {str(err)}")
             return False
 
         return True
 
     def load_credentials(self, filename: str) -> Credentials | bool:
         """Load credentials from file."""
 
         try:
             with open(filename, "rb") as file:
                 data = orjson.loads(file.read())
-            file.close()
-        except OSError:
+        except (OSError, orjson.JSONDecodeError):
+            log.error(f"Error while loading credentials from file {filename}")
             return False
 
         self.credentials = Credentials.create_from_json(data)
+
         return self.credentials
 
     async def __aenter__(self) -> Self:
         """Async enter.
 
         Returns:
             Bakalari object.
```

### Comparing `async_bakalari_api-0.2/src/bakalari_api/const.py` & `async_bakalari_api-0.3/src/bakalari_api/const.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Constants."""
 
 from enum import Enum
 from typing import Any, Final
 
-from .logger_api import api_logger
 from strenum import StrEnum
 
+from .logger_api import api_logger
+
 log = api_logger("Bakalari API").get()
 
 REQUEST_TIMEOUT: int = 10
 
 
 class Errors(StrEnum):
     """Returned errors."""
@@ -37,14 +38,18 @@
         "endpoint": "/api/3/komens/messages/received",
         "method": "post",
     }
     KOMENS_UNREAD_COUNT: Final = {
         "endpoint": "/api/3/komens/messages/received/unread",
         "method": "get",
     }
+    KOMENS_ATTACHMENT = {
+        "endpoint": "/api/3/komens/attachment",
+        "method": "get",
+    }
 
     def get(self, key: str) -> Any:
         """Get key value."""
         if not (ret := self.value.get(key)):
             log.error(f"Requested key ({key}) is not valid. Check for spelling.")
             return False
         return ret
```

### Comparing `async_bakalari_api-0.2/src/bakalari_api/datastructure.py` & `async_bakalari_api-0.3/src/bakalari_api/datastructure.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Datastructure."""
 
 from __future__ import annotations
 
+from contextlib import suppress
 from dataclasses import dataclass
 from typing import Any
 
 import orjson
 
 from .const import Token
 from .logger_api import api_logger
@@ -26,26 +27,24 @@
     def create(cls, data: dict[str, Any]) -> Credentials:
         """Create class object form data."""
 
         return cls(
             user_id=data[Token.USER_ID],
             access_token=data[Token.ACCESS_TOKEN],
             refresh_token=data[Token.REFRESH_TOKEN],
-            username=data[Token.USERNAME],
         )
 
     @classmethod
     def create_from_json(cls, data: dict[str, Any]) -> Credentials:
         """Return class object from JSON dictionary."""
         return Credentials.create(
             {
                 Token.USER_ID: data["user_id"],
                 Token.ACCESS_TOKEN: data["access_token"],
                 Token.REFRESH_TOKEN: data["refresh_token"],
-                Token.USERNAME: data["username"],
             }
         )
 
 
 @dataclass
 class School:
     """Data structure for one school item."""
@@ -115,26 +114,20 @@
             except IndexError:
                 return False
 
         return False
 
     def get_schools_by_town(self, town: str | None = None) -> list[School]:
         """Get list of schools in town."""
-        _schools = []
-        for item in self.school_list:
-            _schools.append(item) if item.town in town else None
-        return _schools
+        return [item for item in self.school_list if item.town in town]
 
     def get_school_name_by_api_point(self, api_point: str) -> str | bool:
         """Get school name by its api point."""
-
-        for item in self.school_list:
-            if api_point == item.api_point:
-                return item.name
-        return False
+        with suppress(IndexError):
+            return [item for item in self.school_list if api_point == item.api_point][0].name
 
     def save_to_file(self, filename: str) -> bool:
         """Save loaded school list to file in JSON format."""
 
         schools = []
 
         for item in self.school_list:
@@ -143,17 +136,17 @@
                 "api_point": item.api_point,
                 "town": item.town,
             }
             schools.append(new_data)
 
         try:
             with open(filename, "wb") as file:
-                file.write(orjson.dumps(schools, option=orjson.OPT_INDENT_2))
-            file.close()
-        except OSError:
+                file.write(orjson.dumps(self.school_list, option=orjson.OPT_INDENT_2))
+        except (OSError, orjson.JSONEncodeError) as ex:
+            log.error(f"Unable to save schools list to file {filename}. Error: {str(ex)}")
             return False
 
         return True
 
     async def load_from_file(self, filename: str) -> Schools:
         """Load schools list from a file."""
```

### Comparing `async_bakalari_api-0.2/src/bakalari_api/exceptions.py` & `async_bakalari_api-0.3/src/bakalari_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `async_bakalari_api-0.2/src/bakalari_api/komens.py` & `async_bakalari_api-0.3/src/bakalari_api/komens.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,155 +1,187 @@
 """Module for working with Komens."""
 
 from datetime import datetime as dt
 from typing import Any
 
 import dateutil
+import dateutil.parser
 import orjson
 
 from .bakalari import Bakalari
 from .const import EndPoint
 from .logger_api import api_logger
 
 log = api_logger("Bakalari API").get()
 
 
 class MessageContainer:
     """Messages registry."""
 
-    mid: int
+    mid: str
     title: str
     text: str
-    sent: dt.date
+    sent: dt
     sender: dict[str, str]
     attachments: dict[str, str]
 
     def __init__(
         self,
         *,
-        mid: int,
+        mid: str,
         title: str,
         text: str,
         sent: dt,
         sender: dict[str, str],
         attachments: dict[str, str] | None = None,
     ):
         """Initialize MessagesContainer."""
 
         _setter = object.__setattr__
         _setter(self, "mid", mid)
         _setter(self, "title", title)
         _setter(self, "text", text)
-        _setter(self, "sent", sent)
+        _setter(self, "sent", sent.date())
         _setter(self, "sender", sender)
         _setter(self, "attachments", attachments)
 
     def __repr__(self) -> str:
         """Representation of MessageContainer."""
         return (
             f"<MessageContainer message_id={self.mid} "
             f"title={self.title} sender={self.sender}>"
         )
 
     def __setattr__(self, key: str, value: Any) -> None:
         """Set an attribute."""
         super().__setattr__(key, value)
 
-    def as_json(self) -> orjson.Fragment:
+    def as_json(self) -> bytes:
         """Return JSON fragment of message."""
         json_repr = {
             "mid": self.mid,
             "title": self.title,
             "text": self.text,
             "sent": self.sent,
             "sender": self.sender,
             "attachments": self.attachments,
         }
-        return orjson.Fragment(json_repr)
+        return orjson.dumps(json_repr)
 
     def __str__(self) -> str:
         """Return string representation of data."""
         return f"""Message id: {self.mid}
             title: {self.title}
             text: {self.text},
-            sent: {self.sent.date()},
+            sent: {self.sent},
             sender: {self.sender},
             attachments: {self.attachments}"""
 
 
 class Messages(list[MessageContainer]):
     """Messages class holds all messages."""
 
     def __init__(self) -> None:
         """Messages class holds all messages."""
         super().__init__()
 
-    def add_message(self, data: MessageContainer):
-        """Add new message to list."""
-        self.append([data])
+    def __str__(self) -> str:
+        """Print string representation."""
+
+        text = ""
+        for message in self:
+            text += message.__str__() + "\n"
+        return text
+
+    def json(self):
+        """Return json representation of Messages."""
 
-    def get_message_by_id(self, id: int) -> MessageContainer:
+        return [orjson.loads(m.as_json()) for m in self]
+
+    def get_message_by_id(self, id: str) -> MessageContainer:
         """Get message by id."""
         for i in self:
-            if i[0].mid == id:
-                return i[0]
+            if i.mid == id:
+                return i
 
     def get_messages_by_date(
         self, date: dt, to_date: dt | None = None
     ) -> list[MessageContainer]:
         """Get messages by date.
 
         If `to_date` is set, then returns list of range from `date` to `to_date`
         """
 
-        messages = []
+        to_date = to_date or date
 
-        for i in self:
-            if to_date:
-                if (i[0].sent.date() >= date) and (i[0].sent.date() <= to_date):
-                    messages.append(i[0])
-            elif i[0].sent.date() == date:
-                messages.append(i[0])
-        return None if len(messages) == 0 else messages
+        messages = [i for i in self if date <= i.sent <= to_date]
+
+        return messages if messages else None
 
     def count_messages(self) -> int:
         """Count messages."""
         return len(self)
 
 
 class Komens:
     """Class for working with Komens messages."""
 
     def __init__(self, bakalari: Bakalari):
         """Initialize class Komens."""
         self.bakalari = bakalari
         self.messages = Messages()
 
-    async def get_messages(self) -> Messages:
-        """Get unread messages."""
+    async def fetch_messages(self) -> Messages:
+        """Fetch unread messages.
+
+        Retrieve messages from the server and returns an instance of the Messages class
+        containing the messages.
+
+        Returns:
+            Messages: An instance of the Messages class containing the messages.
+
+        """
+        self.messages.clear()
         messages = await self.bakalari.send_auth_request(
             EndPoint.KOMENS_UNREAD,
         )
 
-        _messages = Messages()
-
-        # with open(".data", "rb") as f:
-        #     messages = orjson.loads(f.read())
-        #     f.close()
-
-        for msg in messages["Messages"]:
+        async def create_msg(msg):
             log.debug(f"Writing message: {msg}")
-            _message = MessageContainer(
+            return MessageContainer(
                 mid=msg["Id"],
                 title=msg["Title"],
                 text=msg["Text"],
                 sent=dateutil.parser.parse(msg["SentDate"]),
                 sender=msg["Sender"]["Name"],
                 attachments=msg["Attachments"],
             )
-            self.messages.add_message(_message)
 
-        return _messages
+        self.messages.extend([(await create_msg(msg)) for msg in messages["Messages"]])
+
+        return self.messages
 
     async def count_unread_messages(self) -> int:
         """Get count of unreaded messages."""
         return await self.bakalari.send_auth_request(EndPoint.KOMENS_UNREAD_COUNT)
+
+    async def get_attachment(self, id: str) -> Any:
+        """Get attachment.
+
+        Retrieves an attachment from the server based on the provided ID.
+
+        Args:
+            id (str): The ID of the attachment to retrieve.
+
+        Returns:
+            Tuple[str, Any]: A tuple containing the filename and file data of the attachment.
+
+        """
+        try:
+            filename, filedata = await self.bakalari.send_auth_request(
+                EndPoint.KOMENS_ATTACHMENT, extend=f"/{id}"
+            )
+        except Exception as ex:
+            log.error(f"Exception: {ex} has occurred.")
+            return False
+
+        return filename, filedata
```

### Comparing `async_bakalari_api-0.2/src/bakalari_api/logger_api.py` & `async_bakalari_api-0.3/src/bakalari_api/logger_api.py`

 * *Files identical despite different names*

