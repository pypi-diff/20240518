# Comparing `tmp/quart_auth-0.9.0.tar.gz` & `tmp/quart_auth-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quart_auth-0.9.0.tar", max compression
+gzip compressed data, was "quart_auth-0.9.1.tar", max compression
```

## Comparing `quart_auth-0.9.0.tar` & `quart_auth-0.9.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1050 2023-07-02 14:33:53.627236 quart_auth-0.9.0/LICENSE
--rw-r--r--   0        0        0     4037 2023-07-02 14:33:53.627236 quart_auth-0.9.0/README.rst
--rw-r--r--   0        0        0     2150 2023-07-02 14:33:53.627236 quart_auth-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      587 2023-07-02 14:33:53.627236 quart_auth-0.9.0/src/quart_auth/__init__.py
--rw-r--r--   0        0        0     2539 2023-07-02 14:33:53.627236 quart_auth-0.9.0/src/quart_auth/basic_auth.py
--rw-r--r--   0        0        0    11462 2023-07-02 14:33:53.627236 quart_auth-0.9.0/src/quart_auth/extension.py
--rw-r--r--   0        0        0     3205 2023-07-02 14:33:53.627236 quart_auth-0.9.0/src/quart_auth/globals.py
--rw-r--r--   0        0        0        7 2023-07-02 14:33:53.627236 quart_auth-0.9.0/src/quart_auth/py.typed
--rw-r--r--   0        0        0     5281 1970-01-01 00:00:00.000000 quart_auth-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1050 2024-01-28 19:42:05.931214 quart_auth-0.9.1/LICENSE
+-rw-r--r--   0        0        0     4037 2024-01-28 19:42:05.931214 quart_auth-0.9.1/README.rst
+-rw-r--r--   0        0        0     2151 2024-01-28 19:42:05.931214 quart_auth-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      587 2024-01-28 19:42:05.931214 quart_auth-0.9.1/src/quart_auth/__init__.py
+-rw-r--r--   0        0        0     2536 2024-01-28 19:42:05.931214 quart_auth-0.9.1/src/quart_auth/basic_auth.py
+-rw-r--r--   0        0        0    11811 2024-01-28 19:42:05.931214 quart_auth-0.9.1/src/quart_auth/extension.py
+-rw-r--r--   0        0        0     3201 2024-01-28 19:42:05.931214 quart_auth-0.9.1/src/quart_auth/globals.py
+-rw-r--r--   0        0        0        7 2024-01-28 19:42:05.931214 quart_auth-0.9.1/src/quart_auth/py.typed
+-rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 quart_auth-0.9.1/PKG-INFO
```

### Comparing `quart_auth-0.9.0/LICENSE` & `quart_auth-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quart_auth-0.9.0/README.rst` & `quart_auth-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `quart_auth-0.9.0/pyproject.toml` & `quart_auth-0.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "quart-auth"
-version = "0.9.0"
+version = "0.9.1"
 description = "A Quart extension to provide secure cookie authentication"
 authors = ["pgjones <philip.graham.jones@googlemail.com>"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = ["src/quart_auth/py.typed"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/pgjones/quart-auth/"
 
 [tool.black]
 line-length = 100
-target-version = ["py37"]
+target-version = ["py38"]
 
 [tool.isort]
 combine_as_imports = true
 force_grid_wrap = 0
 include_trailing_comma = true
 known_first_party = "quart_auth, tests"
 line_length = 100
@@ -54,15 +54,15 @@
 warn_redundant_casts = true
 warn_return_any = false
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [tool.poetry.dependencies]
 pydata_sphinx_theme = { version = "*", optional = true }
-python = ">=3.7"
+python = ">=3.8"
 quart = ">=0.18"
 typing_extensions = { version = "*", python = "<3.10" }
 
 [tool.poetry.dev-dependencies]
 tox = "*"
 
 [tool.poetry.extras]
```

### Comparing `quart_auth-0.9.0/src/quart_auth/__init__.py` & `quart_auth-0.9.1/src/quart_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `quart_auth-0.9.0/src/quart_auth/basic_auth.py` & `quart_auth-0.9.1/src/quart_auth/basic_auth.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from functools import wraps
 from secrets import compare_digest
-from typing import Any, Callable, Coroutine, TypeVar
+from typing import Awaitable, Callable, TypeVar
 
 from quart import current_app, has_request_context, has_websocket_context, request, websocket
 from werkzeug.datastructures import WWWAuthenticate
 from werkzeug.exceptions import Unauthorized as WerkzeugUnauthorized
 
 try:
     from typing import ParamSpec
@@ -20,15 +20,15 @@
         www_authenticate = WWWAuthenticate("basic")
         super().__init__(www_authenticate=www_authenticate)
 
 
 def basic_auth_required(
     username_key: str = "QUART_AUTH_BASIC_USERNAME",
     password_key: str = "QUART_AUTH_BASIC_PASSWORD",
-) -> Callable[[Callable[P, T]], Callable[P, Coroutine[Any, Any, T]]]:
+) -> Callable[[Callable[P, Awaitable[T]]], Callable[P, Awaitable[T]]]:
     """A decorator to restrict route access to basic authenticated users.
 
     This should be used to wrap a route handler (or view function) to
     enforce that only basic authenticated requests can access it. The
     basic auth username and password are configurable via the app
     configuration with the QUART_AUTH_BASIC_USERNAME, and
     QUART_AUTH_BASIC_PASSWORD keys used by default. Note that it is
@@ -43,15 +43,15 @@
             ...
 
     If the request is not authenticated a
     `quart.exceptions.UnauthorizedBasicAuth` exception will be raised.
 
     """
 
-    def decorator(func: Callable[P, T]) -> Callable[P, Coroutine[Any, Any, T]]:
+    def decorator(func: Callable[P, Awaitable[T]]) -> Callable[P, Awaitable[T]]:
         @wraps(func)
         async def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
             if has_request_context():
                 auth = request.authorization
             elif has_websocket_context():
                 auth = websocket.authorization
             else:
```

### Comparing `quart_auth-0.9.0/src/quart_auth/extension.py` & `quart_auth-0.9.1/src/quart_auth/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
         if sum(ext.singleton for ext in app.extensions["QUART_AUTH"]) > 2:
             raise RuntimeError(
                 "Multiple singleton extensions, please see docs about multiple auth users"
             )
 
         app.after_request(self.after_request)
-        app.after_websocket(self.after_websocket)
+        app.after_websocket(self.after_websocket)  # type: ignore
         if self.singleton:
             app.context_processor(self._template_context)
 
     def resolve_user(self) -> AuthUser:
         if self.mode == "cookie":
             auth_id = self.load_cookie()
         else:
@@ -199,15 +199,15 @@
 
         serializer = self.serializer_class(app.secret_key, self.salt)
         try:
             return serializer.loads(token, max_age=self.duration)
         except (BadSignature, SignatureExpired):
             return None
 
-    def after_request(self, response: Response) -> Response:
+    async def after_request(self, response: Response) -> Response:
         user = self.load_user()
         if self.mode == "bearer":
             if user.action != Action.PASS:
                 warnings.warn("Login/logout/renew have no affect in bearer mode")
 
             return response
 
@@ -221,28 +221,34 @@
                 samesite=self.cookie_samesite,
             )
         elif user.action in {Action.WRITE, Action.WRITE_PERMANENT}:
             max_age = None
             if user.action == Action.WRITE_PERMANENT:
                 max_age = self.duration
 
+            if self.cookie_secure and not request.is_secure:
+                warnings.warn("Secure cookies will be ignored on insecure requests")
+
+            if self.cookie_samesite == "Strict" and 300 <= response.status_code < 400:
+                warnings.warn("Strict samesite cookies will be ignored on redirects")
+
             token = self.dump_token(user.auth_id)
             response.set_cookie(
                 self.cookie_name,
                 token,
                 domain=self.cookie_domain,
                 max_age=max_age,
                 httponly=cast(bool, self.cookie_http_only),
                 path=self.cookie_path,
                 secure=cast(bool, self.cookie_secure),
                 samesite=self.cookie_samesite,
             )
         return response
 
-    def after_websocket(self, response: Optional[Response]) -> Optional[Response]:
+    async def after_websocket(self, response: Optional[Response]) -> Optional[Response]:
         user = self.load_user()
         if self.mode == "bearer":
             if user.action != Action.PASS:
                 warnings.warn("Login/logout/renew have no affect in bearer mode")
 
             return response
```

### Comparing `quart_auth-0.9.0/src/quart_auth/globals.py` & `quart_auth-0.9.1/src/quart_auth/globals.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from contextlib import asynccontextmanager
 from functools import wraps
-from typing import Any, AsyncGenerator, Callable, Coroutine, Optional, TypeVar
+from typing import AsyncGenerator, Awaitable, Callable, Optional, TypeVar
 
 from quart import current_app, Quart
 from quart.typing import TestClientProtocol
 from werkzeug.local import LocalProxy
 
 from .extension import Action, AuthUser, QuartAuth, Unauthorized
 
@@ -32,15 +32,15 @@
         None,
     )
     if extension is None:
         raise RuntimeError("No singleton QuartAuth, please see docs about multiple auth users")
     return extension
 
 
-def login_required(func: Callable[P, T]) -> Callable[P, Coroutine[Any, Any, T]]:
+def login_required(func: Callable[P, Awaitable[T]]) -> Callable[P, Awaitable[T]]:
     """A decorator to restrict route access to authenticated users.
 
     This should be used to wrap a route handler (or view function) to
     enforce that only authenticated requests can access it. Note that
     it is important that this decorator be wrapped by the route
     decorator and not vice, versa, as below.
```

### Comparing `quart_auth-0.9.0/PKG-INFO` & `quart_auth-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: quart-auth
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Quart extension to provide secure cookie authentication
 Home-page: https://github.com/pgjones/quart-auth/
 License: MIT
 Author: pgjones
 Author-email: philip.graham.jones@googlemail.com
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 Requires-Dist: pydata_sphinx_theme ; extra == "docs"
 Requires-Dist: quart (>=0.18)
 Requires-Dist: typing_extensions ; python_version < "3.10"
 Project-URL: Repository, https://github.com/pgjones/quart-auth/
```

