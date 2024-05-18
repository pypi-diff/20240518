# Comparing `tmp/fastapi_keycloak_middleware-0.4.1.tar.gz` & `tmp/fastapi_keycloak_middleware-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_keycloak_middleware-0.4.1.tar", max compression
+gzip compressed data, was "fastapi_keycloak_middleware-0.4.2.tar", max compression
```

## Comparing `fastapi_keycloak_middleware-0.4.1.tar` & `fastapi_keycloak_middleware-0.4.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1063 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/LICENSE
--rw-r--r--   0        0        0     4422 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/README.md
--rw-r--r--   0        0        0     1481 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/decorators/__init__.py
--rw-r--r--   0        0        0     5058 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/decorators/require_permission.py
--rw-r--r--   0        0        0      856 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/decorators/strip_request.py
--rw-r--r--   0        0        0      352 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/dependencies/__init__.py
--rw-r--r--   0        0        0      467 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/dependencies/get_authorization_result.py
--rw-r--r--   0        0        0      420 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/dependencies/get_user.py
--rw-r--r--   0        0        0      703 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/exceptions.py
--rw-r--r--   0        0        0     1042 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/fast_api_user.py
--rw-r--r--   0        0        0     7549 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/keycloak_backend.py
--rw-r--r--   0        0        0     8039 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/middleware.py
--rw-r--r--   0        0        0        0 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/schemas/__init__.py
--rw-r--r--   0        0        0      523 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/schemas/authorization_methods.py
--rw-r--r--   0        0        0     1257 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/schemas/authorization_result.py
--rw-r--r--   0        0        0      232 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/schemas/exception_response.py
--rw-r--r--   0        0        0     6460 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/schemas/keycloak_configuration.py
--rw-r--r--   0        0        0      581 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/schemas/match_strategy.py
--rw-r--r--   0        0        0     5761 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/setup.py
--rw-r--r--   0        0        0     1637 2024-04-30 17:31:31.417459 fastapi_keycloak_middleware-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     5421 1970-01-01 00:00:00.000000 fastapi_keycloak_middleware-0.4.1/setup.py
--rw-r--r--   0        0        0     5010 1970-01-01 00:00:00.000000 fastapi_keycloak_middleware-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4422 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/README.md
+-rw-r--r--   0        0        0     1481 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/decorators/__init__.py
+-rw-r--r--   0        0        0     5058 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/decorators/require_permission.py
+-rw-r--r--   0        0        0      856 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/decorators/strip_request.py
+-rw-r--r--   0        0        0      352 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/dependencies/__init__.py
+-rw-r--r--   0        0        0      467 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/dependencies/get_authorization_result.py
+-rw-r--r--   0        0        0      420 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/dependencies/get_user.py
+-rw-r--r--   0        0        0      703 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/exceptions.py
+-rw-r--r--   0        0        0     1042 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/fast_api_user.py
+-rw-r--r--   0        0        0     7932 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/keycloak_backend.py
+-rw-r--r--   0        0        0     8195 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/middleware.py
+-rw-r--r--   0        0        0        0 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/schemas/__init__.py
+-rw-r--r--   0        0        0      523 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/schemas/authorization_methods.py
+-rw-r--r--   0        0        0     1257 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/schemas/authorization_result.py
+-rw-r--r--   0        0        0      232 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/schemas/exception_response.py
+-rw-r--r--   0        0        0     7178 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/schemas/keycloak_configuration.py
+-rw-r--r--   0        0        0      581 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/schemas/match_strategy.py
+-rw-r--r--   0        0        0     5761 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/setup.py
+-rw-r--r--   0        0        0     1618 2024-05-18 10:18:49.385028 fastapi_keycloak_middleware-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     5393 1970-01-01 00:00:00.000000 fastapi_keycloak_middleware-0.4.2/setup.py
+-rw-r--r--   0        0        0     4970 1970-01-01 00:00:00.000000 fastapi_keycloak_middleware-0.4.2/PKG-INFO
```

### Comparing `fastapi_keycloak_middleware-0.4.1/LICENSE` & `fastapi_keycloak_middleware-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.1/README.md` & `fastapi_keycloak_middleware-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/__init__.py` & `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Middleware for FastAPI that supports authenticating users against Keycloak
 """
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 import logging
 
 from fastapi_keycloak_middleware.decorators.require_permission import require_permission
 from fastapi_keycloak_middleware.decorators.strip_request import strip_request
 from fastapi_keycloak_middleware.dependencies.get_authorization_result import (
     get_authorization_result,
```

### Comparing `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/decorators/require_permission.py` & `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/decorators/require_permission.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/decorators/strip_request.py` & `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/decorators/strip_request.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/exceptions.py` & `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/fast_api_user.py` & `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/fast_api_user.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/keycloak_backend.py` & `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/keycloak_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,19 +78,31 @@
         )
 
     async def authenticate(self, conn: HTTPConnection) -> tuple[AuthCredentials, BaseUser | None]:
         """
         The authenticate method is invoked each time a route is called that
         the middleware is applied to.
         """
-        if "Authorization" not in conn.headers:
+
+        auth_header = None
+
+        # If this is a websocket connection, we can extract the token
+        # from the cookies
+        if (
+            self.keycloak_configuration.enable_websocket_support
+            and conn.headers.get("upgrade") == "websocket"
+        ):
+            auth_header = conn.cookies.get(self.keycloak_configuration.websocket_cookie_name, None)
+        else:
+            auth_header = conn.headers.get("Authorization", None)
+
+        if not auth_header:
             raise AuthHeaderMissing
 
         # Check if token starts with the authentication scheme
-        auth_header = conn.headers["Authorization"]
         token = auth_header.split(" ")
         if len(token) != 2 or token[0] != self.keycloak_configuration.authentication_scheme:
             raise AuthInvalidToken
 
         token_info = None
 
         # Depending on the chosen method by the user, either
```

### Comparing `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/middleware.py` & `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         log.info("Initializing Keycloak Middleware")
         self.app = app
         self.backend: KeycloakBackend = KeycloakBackend(
             keycloak_configuration=keycloak_configuration,
             user_mapper=user_mapper,
         )
         self.scope_mapper = scope_mapper
+        self.inspect_websockets = keycloak_configuration.enable_websocket_support
         log.debug("Keycloak Middleware initialized")
 
         # Try to compile patterns
         self.exclude_paths = []
         if exclude_patterns and isinstance(exclude_patterns, list):
             for path in exclude_patterns:
                 try:
@@ -104,18 +105,19 @@
             if pattern.match(path):
                 return True
         return False
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send):
         log.debug("Keycloak Middleware is handling request")
 
-        if scope["type"] not in [
-            "http",
-            "websocket",
-        ]:  # pragma nocover # Filter for relevant requests
+        supported_protocols = ["http"]
+        if self.inspect_websockets:
+            supported_protocols.append("websocket")
+
+        if scope["type"] not in supported_protocols:  # Filter for relevant requests
             log.debug("Skipping non-HTTP request")
             await self.app(scope, receive, send)  # pragma nocover # Bypass
             return
 
         # Extract path from scope
         path = scope["path"]
         if await self._exclude_path(path):
```

### Comparing `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/schemas/authorization_methods.py` & `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/schemas/authorization_methods.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/schemas/authorization_result.py` & `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/schemas/authorization_result.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/schemas/keycloak_configuration.py` & `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/schemas/keycloak_configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,19 @@
     :type verify: Union[bool,str], optional
     :param decode_options: Defines options to be passed to `python-jose`'s `decode``
         function. Defaults to ``{"verify_signature": True, "verify_aud": True,
         "verify_exp": True}``. See the following project for an overview of
         acceptable options:
         https://github.com/mpdavis/python-jose/blob/4b0701b46a8d00988afcc5168c2b3a1fd60d15d8/jose/jwt.py#L81
     :type decode_options: Dict[str, Union[bool,int]], optional
+    :param enable_websocket_support: Whether to enable WebSocket support. Defaults to ``True``.
+    :type enable_websocket_support: bool, optional
+    :param websocket_cookie_name: Name of the cookie that contains the access token.
+        Defaults to ``access_token``.
+    :type websocket_cookie_name: str, optional
     """
 
     realm: str = Field(title="Realm", description="The realm to use.")
     url: str = Field(title="URL", description="The URL of the Keycloak server.")
     client_id: str = Field(title="Client ID", description="The client ID.")
     swagger_client_id: Optional[str] = Field(
         default=None, title="Swagger Client ID", description="The client ID for the swagger UI."
@@ -136,7 +141,17 @@
             "verify_signature": True,
             "verify_aud": True,
             "verify_exp": True,
         },
         title="JWT Decode Options",
         description="Decode options that are passed to python-jose decode function.",
     )
+    enable_websocket_support: bool = Field(
+        default=True,
+        title="Enable WebSocket Support",
+        description="if enabled, websocket connections are also checked for valid tokens.",
+    )
+    websocket_cookie_name: str = Field(
+        default="access_token",
+        title="WebSocket Cookie Name",
+        description="The name of the cookie that contains the access token.",
+    )
```

### Comparing `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/schemas/match_strategy.py` & `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/schemas/match_strategy.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.1/fastapi_keycloak_middleware/setup.py` & `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/setup.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.1/pyproject.toml` & `fastapi_keycloak_middleware-0.4.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [tool.poetry]
 name = "fastapi-keycloak-middleware"
-version = "0.4.1"
+version = "0.4.2"
 description = "Middleware for FastAPI to authenticate a user against keycloak"
 authors = ["Daniel Herrmann <daniel.herrmann1@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "fastapi_keycloak_middleware" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 fastapi = ">=0.73.0"
-install = "^1.3.5"
 python-keycloak = ">2.14.0,<3.9.1"
 ruff = "^0.4.2"
 
 
 [tool.poetry.group.dev.dependencies]
 sphinx = "^6.1.3"
 sphinx-rtd-theme = "^1.2.0"
```

### Comparing `fastapi_keycloak_middleware-0.4.1/setup.py` & `fastapi_keycloak_middleware-0.4.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,22 +7,19 @@
  'fastapi_keycloak_middleware.dependencies',
  'fastapi_keycloak_middleware.schemas']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['fastapi>=0.73.0',
- 'install>=1.3.5,<2.0.0',
- 'python-keycloak>2.14.0,<3.9.1',
- 'ruff>=0.4.2,<0.5.0']
+['fastapi>=0.73.0', 'python-keycloak>2.14.0,<3.9.1', 'ruff>=0.4.2,<0.5.0']
 
 setup_kwargs = {
     'name': 'fastapi-keycloak-middleware',
-    'version': '0.4.1',
+    'version': '0.4.2',
     'description': 'Middleware for FastAPI to authenticate a user against keycloak',
     'long_description': '[![Documentation Status](https://readthedocs.org/projects/fastapi-keycloak-middleware/badge/?version=latest)](https://fastapi-keycloak-middleware.readthedocs.io/en/latest/?badge=latest)\n[![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)\n![GitHub issues](https://img.shields.io/github/issues/waza-ari/fastapi-keycloak-middleware)\n![GitHub release (latest by date)](https://img.shields.io/github/v/release/waza-ari/fastapi-keycloak-middleware)\n![GitHub top language](https://img.shields.io/github/languages/top/waza-ari/fastapi-keycloak-middleware)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/waza-ari/fastapi-keycloak-middleware/development.svg)](https://results.pre-commit.ci/latest/github/waza-ari/fastapi-keycloak-middleware/development)\n\n\n# FastAPI Keycloak Middleware\n\n**Full documentation** is [available at Read The Docs](https://fastapi-keycloak-middleware.readthedocs.io/en/latest/)\n\nThis package provides a middleware for [FastAPI](http://fastapi.tiangolo.com)  that\nsimplifies integrating with [Keycloak](http://keycloak.org) for\nauthentication and authorization. It supports OIDC and supports validating access\ntokens, reading roles and basic authentication. In addition it provides several\ndecorators and dependencies to easily integrate into your FastAPI application.\n\nIt relies on the [python-keycloak](http://python-keycloak.readthedocs.io) package,\nwhich is the only dependency outside of the FastAPI ecosystem which would be installed\nanyway. Shoutout to the author of [fastapi-auth-middleware](https://github.com/code-specialist/fastapi-auth-middleware)\nwhich served as inspiration for this package and some of its code.\n\nIn the future, I plan to add support for fine grained authorization using Keycloak\nAuthorization services.\n\n## Motivation\n\nUsing FastAPI and Keycloak quite a lot, and keeping to repeat myself quite a lot when\nit comes to authentiating users, I decided to create this library to help with this.\n\nThere is a clear separation between the authentication and authorization:\n\n- **Authentication** is about verifying the identity of the user\n  (who they are). This is done by an authentication backend\n  that verifies the users access token obtained from the\n  identity provider (Keycloak in this case).\n- **Authorization** is about deciding which resources can be\n  accessed. This package providers convenience decoraters to\n  enforce certain roles or permissions on FastAPI endpoints.\n\n## Installation\n\nInstall the package using poetry:\n\n```bash\npoetry add fastapi-keycloak-middleware\n```\n\nor `pip`:\n\n```bash\npip install fastapi-keycloak-middleware\n```\n\n## Features\n\nThe package helps with:\n\n* An easy to use middleware that validates the request for an access token\n* Validation can done in one of two ways:\n   * Validate locally using the public key obtained from Keycloak\n   * Validate using the Keycloak token introspection endpoint\n* Using Starlette authentication mechanisms to store both the user object as well as the authorization scopes in the Request object\n* Ability to provide custom callback functions to retrieve the user object (e.g. from your database) and to provide an arbitrary mapping to authentication scopes (e.g. roles to permissions)\n* A decorator to use previously stored information to enforce certain roles or permissions on FastAPI endpoints\n* Convenience dependencies to retrieve the user object or the authorization result after evaluation within the FastAPI endpoint\n\n## Acknowledgements\n\nThis package is heavily inspired by [fastapi-auth-middleware](https://github.com/code-specialist/fastapi-auth-middleware)\nwhich provides some of the same functionality but without the direct integration\ninto Keycloak. Thanks for writing and providing this great piece of software!\n\n## Contributing\n\nThe client is written in pure Python.\nAny changes or pull requests are more than welcome, but please adhere to the code style.\n\nRuff is used both for code formatting and linting. Before committing, please run the following command to ensure\nthat your code is properly formatted:\n\n```bash\nruff check .\nruff format .\n```\n\nA pre-commit hook configuration is supplied as part of the project.\n\n## Development\n\nThis project is using [Act](https://github.com/nektos/act) to handle local development tasks. It is used\nto work locally and also to test Github actions before deploying them.\n',
     'author': 'Daniel Herrmann',
     'author_email': 'daniel.herrmann1@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fastapi_keycloak_middleware-0.4.1/PKG-INFO` & `fastapi_keycloak_middleware-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: fastapi-keycloak-middleware
-Version: 0.4.1
+Version: 0.4.2
 Summary: Middleware for FastAPI to authenticate a user against keycloak
 Author: Daniel Herrmann
 Author-email: daniel.herrmann1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.73.0)
-Requires-Dist: install (>=1.3.5,<2.0.0)
 Requires-Dist: python-keycloak (>2.14.0,<3.9.1)
 Requires-Dist: ruff (>=0.4.2,<0.5.0)
 Description-Content-Type: text/markdown
 
 [![Documentation Status](https://readthedocs.org/projects/fastapi-keycloak-middleware/badge/?version=latest)](https://fastapi-keycloak-middleware.readthedocs.io/en/latest/?badge=latest)
 [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)
 ![GitHub issues](https://img.shields.io/github/issues/waza-ari/fastapi-keycloak-middleware)
```

