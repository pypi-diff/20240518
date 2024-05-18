# Comparing `tmp/transmission_rpc-7.0.5.tar.gz` & `tmp/transmission_rpc-7.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transmission_rpc-7.0.5.tar", max compression
+gzip compressed data, was "transmission_rpc-7.0.6.tar", max compression
```

## Comparing `transmission_rpc-7.0.5.tar` & `transmission_rpc-7.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1127 2024-05-07 03:54:42.274685 transmission_rpc-7.0.5/LICENSE
--rw-r--r--   0        0        0     2277 2024-05-07 03:54:42.274685 transmission_rpc-7.0.5/README.md
--rw-r--r--   0        0        0     3107 2024-05-07 03:54:42.274685 transmission_rpc-7.0.5/pyproject.toml
--rw-r--r--   0        0        0     1893 2024-05-07 03:54:42.278685 transmission_rpc-7.0.5/transmission_rpc/__init__.py
--rw-r--r--   0        0        0    44327 2024-05-07 03:54:42.278685 transmission_rpc-7.0.5/transmission_rpc/client.py
--rw-r--r--   0        0        0    10069 2024-05-07 03:54:42.278685 transmission_rpc-7.0.5/transmission_rpc/constants.py
--rw-r--r--   0        0        0     1640 2024-05-07 03:54:42.278685 transmission_rpc-7.0.5/transmission_rpc/error.py
--rw-r--r--   0        0        0        0 2024-05-07 03:54:42.278685 transmission_rpc-7.0.5/transmission_rpc/py.typed
--rw-r--r--   0        0        0    12506 2024-05-07 03:54:42.278685 transmission_rpc-7.0.5/transmission_rpc/session.py
--rw-r--r--   0        0        0    23193 2024-05-07 03:54:42.278685 transmission_rpc-7.0.5/transmission_rpc/torrent.py
--rw-r--r--   0        0        0     1866 2024-05-07 03:54:42.278685 transmission_rpc-7.0.5/transmission_rpc/types.py
--rw-r--r--   0        0        0     2669 2024-05-07 03:54:42.278685 transmission_rpc-7.0.5/transmission_rpc/utils.py
--rw-r--r--   0        0        0     3412 1970-01-01 00:00:00.000000 transmission_rpc-7.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1127 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/LICENSE
+-rw-r--r--   0        0        0     2277 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/README.md
+-rw-r--r--   0        0        0     2981 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2230 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/transmission_rpc/__init__.py
+-rw-r--r--   0        0        0    45797 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/transmission_rpc/client.py
+-rw-r--r--   0        0        0    10069 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/transmission_rpc/constants.py
+-rw-r--r--   0        0        0     1640 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/transmission_rpc/error.py
+-rw-r--r--   0        0        0        0 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/transmission_rpc/py.typed
+-rw-r--r--   0        0        0    12505 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/transmission_rpc/session.py
+-rw-r--r--   0        0        0    23775 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/transmission_rpc/torrent.py
+-rw-r--r--   0        0        0     1873 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/transmission_rpc/types.py
+-rw-r--r--   0        0        0     2669 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/transmission_rpc/utils.py
+-rw-r--r--   0        0        0     3422 1970-01-01 00:00:00.000000 transmission_rpc-7.0.6/PKG-INFO
```

### Comparing `transmission_rpc-7.0.5/LICENSE` & `transmission_rpc-7.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.5/README.md` & `transmission_rpc-7.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 `transmission-rpc` is a python wrapper on top of [transmission](https://github.com/transmission/transmission) JSON RPC protocol,
 hosted on GitHub at [github.com/trim21/transmission-rpc](https://github.com/trim21/transmission-rpc)
 
 ## Introduction
 
 `transmission-rpc` is a python module implementing the json-rpc client protocol for the BitTorrent client Transmission.
 
-Support 14 <= rpc version <= 17 (2.40 <= transmission version <= 4.0.4),
+Support 14 <= rpc version <= 17 (2.40 <= transmission version <= 4.0.5),
 should works fine with newer rpc version but some new feature may be missing.
 
 ## versioning
 
 `transmission-rpc` follow [Semantic Versioning](https://semver.org/),
 report an issue if you found unexpected API break changes at same major version.
```

### Comparing `transmission_rpc-7.0.5/pyproject.toml` & `transmission_rpc-7.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "transmission-rpc"
-version = "7.0.5"
+version = "7.0.6"
 description = "Python module that implements the Transmission bittorent client JSON-RPC protocol"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'README.md'
 repository = 'https://github.com/Trim21/transmission-rpc'
 license = 'MIT'
 packages = [{ include = 'transmission_rpc' }]
 keywords = ['transmission', 'rpc']
@@ -26,54 +26,43 @@
     'Programming Language :: Python :: Implementation :: PyPy',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 # dependencies
 requests = "^2.23.0"
-typing-extensions = "*"
+typing-extensions = ">=4.5.0"
 
 [tool.poetry.group.docs.dependencies]
-sphinx = { version = "^7.0.0", python = "^3.9" }
+sphinx = { version = "^7.3.7", python = "^3.9" }
 furo = { version = "2024.5.6", python = "^3.9" }
+sphinx-copybutton = { version = "^0.5.2", python = "^3.9" }
+sphinx-github-style = {version = "^1.2.2", python = "^3.9"}
 
 [tool.poetry.group.dev.dependencies]
 yarl = "==1.9.4"
 # tests
 pytest = "==8.2.0"
 pytest-github-actions-annotate-failures = "==0.2.0"
 coverage = "==7.5.0"
 
 # linter and formatter
 pre-commit = { version = "==3.7.0", markers = "implementation_name != 'pypy'", python = "^3.9" }
 mypy = { version = "==1.10.0", markers = "implementation_name != 'pypy'", python = "^3.9" }
-ruff = "0.4.2"
 
 # stubs
 types-requests = "==2.31.0.20240406"
-
-[tool.poetry-plugin-bump]
-commit_msg = 'bump: v{version}'
-
-[tool.isort]
-default_section = 'THIRDPARTY'
-indent = '    '
-profile = 'black'
-known_first_party = 'transmission_rpc'
-length_sort = true
-line_length = 120
-no_lines_before = 'LOCALFOLDER'
-use_parentheses = true
-include_trailing_comma = true
+sphinx-autobuild = {version = "2024.4.16", python = "^3.9"}
 
 [tool.pytest.ini_options]
 addopts = '-rav -Werror'
 
 [tool.mypy]
 python_version = "3.8"
+strict = true
 disallow_untyped_defs = true
 ignore_missing_imports = true
 warn_return_any = false
 warn_unused_configs = true
 show_error_codes = true
 
 [tool.black]
@@ -134,15 +123,14 @@
     'S314',
     'S101',
     'N815',
     'S104',
     'C901',
     'ISC003',
     'PLR0913',
-    'I001',
     'RUF001',
     'SIM108',
     'TCH003',
     'RUF003',
     'RET504',
     'TRY300',
     'TRY003',
```

### Comparing `transmission_rpc-7.0.5/transmission_rpc/client.py` & `transmission_rpc-7.0.6/transmission_rpc/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import json
-import time
-import types
-import string
 import logging
 import pathlib
-import urllib.parse
-from typing import Any, Dict, List, Type, Tuple, Union, TypeVar, BinaryIO, Iterable, Optional
+import string
+import time
+import types
+from typing import Any, BinaryIO, Dict, Iterable, List, Optional, Tuple, Type, TypeVar, Union
 from urllib.parse import quote
 
 import requests
 import requests.auth
 import requests.exceptions
-from typing_extensions import Literal, TypedDict
+from typing_extensions import Literal, TypedDict, deprecated
 
+from transmission_rpc.constants import DEFAULT_TIMEOUT, LOGGER, RpcMethod
 from transmission_rpc.error import (
-    TransmissionError,
     TransmissionAuthError,
     TransmissionConnectError,
+    TransmissionError,
     TransmissionTimeoutError,
 )
-from transmission_rpc.types import Group, _Timeout
-from transmission_rpc.utils import _try_read_torrent, get_torrent_arguments
 from transmission_rpc.session import Session, SessionStats
 from transmission_rpc.torrent import Torrent
-from transmission_rpc.constants import LOGGER, DEFAULT_TIMEOUT, RpcMethod
+from transmission_rpc.types import Group, _Timeout
+from transmission_rpc.utils import _try_read_torrent, get_torrent_arguments
 
 valid_hash_char = string.digits + string.ascii_letters
 
 _TorrentID = Union[int, str]
 _TorrentIDs = Union[_TorrentID, List[_TorrentID], None]
 
+_header_session_id = "x-transmission-session-id"
+
 
 class ResponseData(TypedDict):
     arguments: Any
     tag: int
     result: str
 
 
@@ -71,41 +72,37 @@
         return [_parse_torrent_id(args)]
     if isinstance(args, (list, tuple)):
         return [_parse_torrent_id(item) for item in args]
     raise ValueError(f"Invalid torrent id {args}")
 
 
 class Client:
-    semver_version: Optional[str]  # available in transmission>=4.0.0
-
     def __init__(
         self,
         *,
         protocol: Literal["http", "https"] = "http",
         username: Optional[str] = None,
         password: Optional[str] = None,
         host: str = "127.0.0.1",
         port: int = 9091,
         path: str = "/transmission/rpc",
         timeout: float = DEFAULT_TIMEOUT,
         logger: logging.Logger = LOGGER,
     ):
         """
 
-        Parameters
-        ----------
-        protocol
-        username
-        password
-        host
-        port
-        path:
-          rpc request target path, default ``/transmission/rpc``
-        timeout
-        logger
+        Parameters:
+            protocol:
+            username:
+            password:
+            host:
+            port:
+            path: rpc request target path, default ``/transmission/rpc``
+            timeout:
+            logger:
         """
         if isinstance(logger, logging.Logger):
             self.logger = logger
         else:
             raise TypeError(
                 "logger must be instance of `logging.Logger`, default: logging.getLogger('transmission-rpc')"
             )
@@ -114,25 +111,50 @@
         username = quote(username or "", safe="$-_.+!*'(),;&=", encoding="utf8") if username else ""
         password = ":" + quote(password or "", safe="$-_.+!*'(),;&=", encoding="utf8") if password else ""
         auth = f"{username}{password}@" if (username or password) else ""
 
         if path == "/transmission/":
             path = "/transmission/rpc"
 
-        url = urllib.parse.urlunparse((protocol, f"{auth}{host}:{port}", path, None, None, None))
-        self.url = str(url)
-        self._sequence = 0
-        self.raw_session: Dict[str, Any] = {}
-        self.session_id = "0"
-        self.server_version: str = "(unknown)"
-        self.protocol_version: int = 17  # default 17
+        url = f"{protocol}://{auth}{host}:{port}{path}"
+        self._url = str(url)
+        self.__raw_session: Dict[str, Any] = {}
+        self.__session_id = "0"
+        self.__server_version: str = "(unknown)"
+        self.__protocol_version: int = 17  # default 17
         self._http_session = requests.Session()
         self._http_session.trust_env = False
+        self.__semver_version = None
         self.get_session()
-        self.torrent_get_arguments = get_torrent_arguments(self.rpc_version)
+        self.__torrent_get_arguments = get_torrent_arguments(self.__protocol_version)
+
+    @property
+    @deprecated("do not use internal property")
+    def url(self) -> str:
+        return self._url
+
+    @property
+    @deprecated("do not use internal property, use `get_torrent_arguments(rpc_version)` if you need")
+    def torrent_get_arguments(self) -> List[str]:
+        return self.__torrent_get_arguments
+
+    @property
+    @deprecated("do not use internal property, use `.get_session()` instead")
+    def raw_session(self) -> Dict[str, Any]:
+        return self.__raw_session
+
+    @property
+    @deprecated("do not use internal property")
+    def session_id(self) -> str:
+        return self.__session_id
+
+    @property
+    @deprecated("do not use internal property, use `.get_session().version` instead")
+    def server_version(self) -> str:
+        return self.__server_version
 
     @property
     def timeout(self) -> _Timeout:
         """
         Get current timeout for HTTP queries.
         """
         return self._query_timeout
@@ -159,63 +181,67 @@
         """
         Reset the HTTP query timeout to the default.
         """
         self._query_timeout = DEFAULT_TIMEOUT
 
     @property
     def _http_header(self) -> Dict[str, str]:
-        return {"x-transmission-session-id": self.session_id}
+        return {_header_session_id: self.__session_id}
 
-    def _http_query(self, query: dict, timeout: Optional[_Timeout] = None) -> str:
+    def _http_query(self, query: Dict[str, Any], timeout: Optional[_Timeout] = None) -> str:
         """
         Query Transmission through HTTP.
         """
         request_count = 0
         if timeout is None:
             timeout = self.timeout
         while True:
-            if request_count >= 10:
+            if request_count >= 3:
                 raise TransmissionError("too much request, try enable logger to see what happened")
             self.logger.debug(
                 {
-                    "url": self.url,
+                    "url": self._url,
                     "headers": self._http_header,
                     "data": query,
                     "timeout": timeout,
                 }
             )
+
             request_count += 1
             try:
                 r = self._http_session.post(
-                    self.url,
+                    self._url,
                     headers=self._http_header,
                     json=query,
                     timeout=timeout,
                 )
             except requests.exceptions.Timeout as e:
                 raise TransmissionTimeoutError("timeout when connection to transmission daemon") from e
             except requests.exceptions.ConnectionError as e:
                 raise TransmissionConnectError(f"can't connect to transmission daemon: {e!s}") from e
 
-            self.session_id = r.headers.get("X-Transmission-Session-Id", "0")
             self.logger.debug(r.text)
             if r.status_code in {401, 403}:
                 self.logger.debug(r.request.headers)
                 raise TransmissionAuthError("transmission daemon require auth", original=r)
+
+            if _header_session_id in r.headers:
+                self.__session_id = r.headers["x-transmission-session-id"]
+
             if r.status_code != 409:
                 return r.text
 
     def _request(
         self,
         method: RpcMethod,
         arguments: Optional[Dict[str, Any]] = None,
         ids: Optional[_TorrentIDs] = None,
         require_ids: bool = False,
         timeout: Optional[_Timeout] = None,
-    ) -> dict:
+    ) -> Dict[str, Any]:
         """
         Send json-rpc request to Transmission using http POST
         """
         if not isinstance(method, str):
             raise TypeError("request takes method as string")
         if arguments is None:
             arguments = {}
@@ -224,26 +250,27 @@
 
         ids = _parse_torrent_ids(ids)
         if len(ids) > 0:
             arguments["ids"] = ids
         elif require_ids:
             raise ValueError("request require ids")
 
-        query = {"tag": self._sequence, "method": method, "arguments": arguments}
+        query = {"method": method, "arguments": arguments}
 
-        self._sequence += 1
-        start = time.time()
-        http_data = self._http_query(query, timeout)
-        elapsed = time.time() - start
-        self.logger.info("http request took %.3f s", elapsed)
+        start = time.monotonic()
+        try:
+            http_data = self._http_query(query, timeout)
+        finally:
+            elapsed = time.monotonic() - start
+            self.logger.debug("http request took %.3f s", elapsed)
 
         try:
             data: ResponseData = json.loads(http_data)
-        except ValueError as error:
-            self.logger.exception("Error: %s")
+        except json.JSONDecodeError as error:
+            self.logger.exception("Error:")
             self.logger.exception('Request: "%s"', query)
             self.logger.exception('HTTP data: "%s"', http_data)
             raise TransmissionError(
                 "failed to parse response as json", method=method, argument=arguments, rawResponse=http_data
             ) from error
 
         self.logger.debug(json.dumps(data, indent=2))
@@ -283,15 +310,15 @@
                     "Invalid torrent-add response.",
                     method=method,
                     argument=arguments,
                     response=data,
                     rawResponse=http_data,
                 )
         elif method == RpcMethod.SessionGet:
-            self.raw_session.update(res)
+            self.__raw_session.update(res)
         elif method == RpcMethod.SessionStats:
             # older versions of T has the return data in "session-stats"
             if "session-stats" in res:
                 return res["session-stats"]
             return res
         elif method in (
             RpcMethod.PortTest,
@@ -303,31 +330,38 @@
         else:
             return res
 
         return results
 
     def _update_server_version(self) -> None:
         """Decode the Transmission version string, if available."""
-        self.semver_version = self.raw_session.get("rpc-version-semver")
-        self.server_version = self.raw_session["version"]
-        self.protocol_version = self.raw_session["rpc-version"]
+        self.__semver_version = self.__raw_session.get("rpc-version-semver")
+        self.__server_version = self.__raw_session["version"]
+        self.__protocol_version = self.__raw_session["rpc-version"]
 
     @property
+    @deprecated("use .get_session().rpc_version_semver instead")
+    def semver_version(self) -> Optional[int]:
+        """Get the Transmission daemon RPC version."""
+        return self.__semver_version
+
+    @property
+    @deprecated("use .get_session().rpc_version instead")
     def rpc_version(self) -> int:
         """Get the Transmission daemon RPC version."""
-        return self.protocol_version
+        return self.__protocol_version
 
     def _rpc_version_warning(self, required_version: int) -> None:
         """
         Add a warning to the log if the Transmission RPC version is lower then the provided version.
         """
-        if self.rpc_version < required_version:
+        if self.__protocol_version < required_version:
             self.logger.warning(
                 "Using feature not supported by server. RPC version for server %d, feature introduced in %d.",
-                self.rpc_version,
+                self.__protocol_version,
                 required_version,
             )
 
     def add_torrent(
         self,
         torrent: Union[BinaryIO, str, bytes, pathlib.Path],
         timeout: Optional[_Timeout] = None,
@@ -348,48 +382,46 @@
         Add torrent to transfers list. ``torrent`` can be:
 
         - ``http://``, ``https://`` or  ``magnet:`` URL
         - torrent file-like object in **binary mode**
         - bytes of torrent content
         - ``pathlib.Path`` for local torrent file, will be read and encoded as base64.
 
-        Warnings
-        --------
-        base64 string or ``file://`` protocol URL are not supported in v4.
-
-        Parameters
-        ----------
-        torrent:
-            torrent to add
-        timeout:
-            request timeout
-        bandwidthPriority:
-            Priority for this transfer.
-        cookies:
-            One or more HTTP cookie(s).
-        download_dir:
-            The directory where the downloaded contents will be saved in.
-        files_unwanted:
-            A list of file id's that shouldn't be downloaded.
-        files_wanted:
-            A list of file id's that should be downloaded.
-        paused:
-            If ``True``, does not start the transfer when added.
-            Magnet url will always start to downloading torrents.
-        peer_limit:
-            Maximum number of peers allowed.
-        priority_high:
-            A list of file id's that should have high priority.
-        priority_low:
-            A list of file id's that should have low priority.
-        priority_normal:
-            A list of file id's that should have normal priority.
-        labels:
-            Array of string labels.
-            Add in rpc 17.
+        Warnings:
+            base64 string or ``file://`` protocol URL are not supported in v4.
+
+        Parameters:
+            torrent:
+                torrent to add
+            timeout:
+                request timeout
+            bandwidthPriority:
+                Priority for this transfer.
+            cookies:
+                One or more HTTP cookie(s).
+            download_dir:
+                The directory where the downloaded contents will be saved in.
+            files_unwanted:
+                A list of file id's that shouldn't be downloaded.
+            files_wanted:
+                A list of file id's that should be downloaded.
+            paused:
+                If ``True``, does not start the transfer when added.
+                Magnet url will always start to downloading torrents.
+            peer_limit:
+                Maximum number of peers allowed.
+            priority_high:
+                A list of file id's that should have high priority.
+            priority_low:
+                A list of file id's that should have low priority.
+            priority_normal:
+                A list of file id's that should have normal priority.
+            labels:
+                Array of string labels.
+                Add in rpc 17.
         """
         if torrent is None:
             raise ValueError("add_torrent requires data or a URI.")
 
         if labels is not None:
             self._rpc_version_warning(17)
 
@@ -468,47 +500,47 @@
         self,
         torrent_id: _TorrentID,
         arguments: Optional[Iterable[str]] = None,
         timeout: Optional[_Timeout] = None,
     ) -> Torrent:
         """
         Get information for torrent with provided id.
-        ``arguments`` contains a list of field names to be returned, when None
+        ``arguments`` contains a list of field names to be returned, when ``arguments=None`` (default),
         all fields are requested. See the Torrent class for more information.
 
         new argument ``format`` in rpc_version 16 is unnecessarily
         and this lib can't handle table response, So it's unsupported.
 
         Returns a Torrent object with the requested fields.
 
+        Note:
+            It's recommended that you only fetch arguments you need,
+            this could improve response speed.
+
+            For example, fetch all fields from transmission daemon with 1500 torrents would take ~5s,
+            but is only ~0.2s if to fetch 6 fields.
+
+        Parameters:
+            torrent_id:
+                torrent id can be an int or a torrent ``info_hash`` (``hashString`` property of the ``Torrent`` object).
+
+            arguments:
+                fetched torrent arguments, in most cases you don't need to set this,
+                transmission-rpc will fetch all torrent fields it supported.
 
-        Note
-        ----
-        It's recommended that you use torrent's ``info_hash`` as torrent id. The torrent's ``info_hash`` will never change.
-
-        Parameters
-        ----------
-        torrent_id:
-            torrent id can be an int or a torrent ``info_hash`` (``hashString`` property of the ``Torrent`` object).
-
-        arguments:
-            fetched torrent arguments, in most cases you don't need to set this,
-            transmission-rpc will fetch all torrent fields it supported.
-
-        timeout:
-            requests timeout
-
-        Raises
-        ------
-        KeyError: torrent with given ``torrent_id`` not found
+            timeout:
+                requests timeout
+
+        Raises:
+            KeyError: torrent with given ``torrent_id`` not found
         """
         if arguments:
             arguments = list(set(arguments) | {"id", "hashString"})
         else:
-            arguments = self.torrent_get_arguments
+            arguments = self.__torrent_get_arguments
         torrent_id = _parse_torrent_id(torrent_id)
         if torrent_id is None:
             raise ValueError("Invalid id")
 
         result = self._request(
             RpcMethod.TorrentGet,
             {"fields": arguments},
@@ -532,38 +564,35 @@
         Get information for torrents with provided ids. For more information see :py:meth:`Client.get_torrent`.
 
         Returns a list of Torrent object.
         """
         if arguments:
             arguments = list(set(arguments) | {"id", "hashString"})
         else:
-            arguments = self.torrent_get_arguments
+            arguments = self.__torrent_get_arguments
         return [
             Torrent(fields=x)
             for x in self._request(RpcMethod.TorrentGet, {"fields": arguments}, ids, timeout=timeout)["torrents"]
         ]
 
     def get_recently_active_torrents(
         self, arguments: Optional[Iterable[str]] = None, timeout: Optional[_Timeout] = None
     ) -> Tuple[List[Torrent], List[int]]:
         """
         Get information for torrents for recently active torrent. If you want to get recently-removed
         torrents. you should use this method.
 
-        Returns
-        -------
-        active_torrents: List[Torrent]
-            List of recently active torrents
-        removed_torrents: List[int]
-            List of torrent-id of recently-removed torrents.
+        Returns:
+            active_torrents, removed_torrents
+                List of recently active torrents and list of torrent-id of recently-removed torrents.
         """
         if arguments:
             arguments = list(set(arguments) | {"id", "hashString"})
         else:
-            arguments = self.torrent_get_arguments
+            arguments = self.__torrent_get_arguments
 
         result = self._request(RpcMethod.TorrentGet, {"fields": arguments}, "recently-active", timeout=timeout)
 
         return [Torrent(fields=x) for x in result["torrents"]], result["removed"]
 
     def change_torrent(
         self,
@@ -594,101 +623,68 @@
         tracker_list: Optional[Iterable[Iterable[str]]] = None,
         tracker_replace: Optional[Iterable[Tuple[int, str]]] = None,
         tracker_remove: Optional[Iterable[int]] = None,
         **kwargs: Any,
     ) -> None:
         """Change torrent parameters for the torrent(s) with the supplied id's.
 
-        Parameters
-        ----------
-        ids
-            torrent(s) to change.
-        timeout
-            requesst timeout.
-        honors_session_limits
-            true if session upload limits are honored.
-        location
-            new location of the torrent's content
-        peer_limit
-            maximum number of peers
-        queue_position
-            position of this torrent in its queue [0...n)
-        files_wanted
-            Array of file id to download.
-        files_unwanted
-            Array of file id to not download.
-        download_limit
-            maximum download speed (KBps)
-        download_limited
-            true if ``download_limit`` is honored
-        upload_limit
-            maximum upload speed (KBps)
-        upload_limited
-            true if ``upload_limit`` is honored
-        bandwidth_priority
-            Priority for this transfer.
-        priority_high
-            list of file id to set high download priority
-        priority_low
-            list of file id to set low download priority
-        priority_normal
-            list of file id to set normal download priority
-        seed_ratio_limit
-            Seed inactivity limit in minutes.
-        seed_ratio_mode
-            Torrent seed ratio mode
-
-            Valid options are :py:class:`transmission_rpc.constants.RatioLimitMode`
-        seed_idle_limit
-            torrent-level seeding ratio
-        seed_idle_mode
-            Seed inactivity mode.
-
-            Valid options are :py:class:`transmission_rpc.constants.IdleMode`
-        labels
-            Array of string labels.
-            Add in rpc 16.
-        group
-            The name of this torrent's bandwidth group.
-            Add in rpc 17.
-
-        tracker_list
-            A ``Iterable[Iterable[str]]``, each ``Iterable[str]`` for a tracker tier.
-
-            Add in rpc 17.
-
-            Example: ``[['https://tracker1/announce', 'https://tracker2/announce'],
-            ['https://backup1.example.com/announce'], ['https://backup2.example.com/announce']]``.
-
-        tracker_add:
-            Array of string with announce URLs to add.
-
-            Warnings
-            --------
-            since transmission daemon 4.0.0, this argument is deprecated, use ``tracker_list`` instead.
-
-        tracker_remove:
-            Array of ids of trackers to remove.
-
-            Warnings
-            --------
-            since transmission daemon 4.0.0, this argument is deprecated, use ``tracker_list`` instead.
-
-        tracker_replace:
-            Array of (id, url) tuples where the announcement URL should be replaced.
-
-            Warnings
-            --------
-            since transmission daemon 4.0.0, this argument is deprecated, use ``tracker_list`` instead.
-
-        Warnings
-        ----
-        ``kwargs`` is for the future features not supported yet, it's not compatibility promising.
-
-        It will be bypassed to request arguments **as-is**, the underline in the key will not be replaced, so you should use kwargs like ``{'a-argument': 'value'}``
+        Parameters:
+            ids: torrent(s) to change.
+            timeout: requesst timeout.
+            honors_session_limits: true if session upload limits are honored.
+            location: new location of the torrent's content
+            peer_limit: maximum number of peers
+            queue_position: position of this torrent in its queue [0...n)
+            files_wanted: Array of file id to download.
+            files_unwanted: Array of file id to not download.
+            download_limit: maximum download speed (KBps)
+            download_limited: true if ``download_limit`` is honored
+            upload_limit: maximum upload speed (KBps)
+            upload_limited: true if ``upload_limit`` is honored
+            bandwidth_priority: Priority for this transfer.
+            priority_high: list of file id to set high download priority
+            priority_low: list of file id to set low download priority
+            priority_normal: list of file id to set normal download priority
+            seed_ratio_limit: Seed inactivity limit in minutes.
+            seed_ratio_mode: Torrent seed ratio mode
+                Valid options are :py:class:`transmission_rpc.RatioLimitMode`
+            seed_idle_limit: torrent-level seeding ratio
+            seed_idle_mode: Seed inactivity mode.
+                Valid options are :py:class:`transmission_rpc.IdleMode`
+            labels: Array of string labels. Add in rpc 16.
+            group: The name of this torrent's bandwidth group. Add in rpc 17.
+            tracker_list:
+                A ``Iterable[Iterable[str]]``, each ``Iterable[str]`` for a tracker tier.
+
+                Add in rpc 17.
+
+                Example: ``[['https://tracker1/announce', 'https://tracker2/announce'],
+                ['https://backup1.example.com/announce'], ['https://backup2.example.com/announce']]``.
+
+            tracker_add:
+                Array of string with announce URLs to add.
+
+                Warnings:
+                    since transmission daemon 4.0.0, this argument is deprecated, use ``tracker_list`` instead.
+
+            tracker_remove:
+                Array of ids of trackers to remove.
+
+                Warnings:
+                    since transmission daemon 4.0.0, this argument is deprecated, use ``tracker_list`` instead.
+
+            tracker_replace:
+                Array of (id, url) tuples where the announcement URL should be replaced.
+
+                Warning:
+                    since transmission daemon 4.0.0, this argument is deprecated, use ``tracker_list`` instead.
+
+        Warnings:
+            ``kwargs`` is for the future features not supported yet, it's not compatibility promising.
+            It will be bypassed to request arguments **as-is**, the underline in the key will not be replaced, so you should use kwargs like ``{'a-argument': 'value'}``
         """
         if labels is not None:
             self._rpc_version_warning(16)
 
         if tracker_list is not None:
             self._rpc_version_warning(17)
 
@@ -738,41 +734,36 @@
         timeout: Optional[_Timeout] = None,
         *,
         move: bool = True,
     ) -> None:
         """
         Move torrent data to the new location.
 
-        See Also
-        --------
-
-        `RPC Spec: moving-a-torrent <https://github.com/transmission/transmission/blob/main/docs/rpc-spec.md#36-moving-a-torrent>`_
+        See Also:
+            `RPC Spec: moving-a-torrent <https://github.com/transmission/transmission/blob/main/docs/rpc-spec.md#36-moving-a-torrent>`_
         """
         args = {"location": ensure_location_str(location), "move": bool(move)}
         self._request(RpcMethod.TorrentSetLocation, args, ids, True, timeout=timeout)
 
     def rename_torrent_path(
         self,
         torrent_id: _TorrentID,
         location: str,
         name: str,
         timeout: Optional[_Timeout] = None,
     ) -> Tuple[str, str]:
         """
-        Warnings
-        --------
-        This method can only be called on single torrent.
-
-        Warnings
-        --------
-        This is not the method to move torrent data directory,
-
-        See Also
-        --------
-        `RPC Spec: renaming-a-torrents-path <https://github.com/transmission/transmission/blob/main/docs/rpc-spec.md#37-renaming-a-torrents-path>`_
+        Warnings:
+            This method can only be called on single torrent.
+
+        Warnings:
+            This is not the method to move torrent data directory,
+
+        See Also:
+            `RPC Spec: renaming-a-torrents-path <https://github.com/transmission/transmission/blob/main/docs/rpc-spec.md#37-renaming-a-torrents-path>`_
         """
         self._rpc_version_warning(15)
         torrent_id = _parse_torrent_id(torrent_id)
 
         name = name.strip()  # https://github.com/trim21/transmission-rpc/issues/185
 
         result = self._request(
@@ -811,15 +802,15 @@
 
     def get_session(self, timeout: Optional[_Timeout] = None) -> Session:
         """
         Get session parameters. See the Session class for more information.
         """
         self._request(RpcMethod.SessionGet, timeout=timeout)
         self._update_server_version()
-        return Session(fields=self.raw_session)
+        return Session(fields=self.__raw_session)
 
     def set_session(
         self,
         timeout: Optional[_Timeout] = None,
         *,
         alt_speed_down: Optional[int] = None,
         alt_speed_enabled: Optional[bool] = None,
@@ -869,120 +860,117 @@
         script_torrent_added_enabled: Optional[bool] = None,
         script_torrent_added_filename: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
         """
         Set session parameters.
 
-        Parameters
-        ----------
-        timeout
-            request timeout
-        alt_speed_down:
-            max global download speed (KBps)
-        alt_speed_enabled:
-            true means use the alt speeds
-        alt_speed_time_begin:
-            Time when alternate speeds should be enabled. Minutes after midnight.
-        alt_speed_time_day:
-            Enables alternate speeds scheduling these days.
-        alt_speed_time_enabled:
-            Enables alternate speeds scheduling.
-        alt_speed_time_end:
-            Time when alternate speeds should be disabled. Minutes after midnight.
-        alt_speed_up:
-            Alternate session upload speed limit (in Kib/s).
-        blocklist_enabled:
-            Enables the block list
-        blocklist_url:
-            Location of the block list. Updated with blocklist-update.
-        cache_size_mb:
-            The maximum size of the disk cache in MB
-        default_trackers:
-            List of default trackers to use on public torrents.
-        dht_enabled:
-            Enables DHT.
-        download_dir:
-            Set the session download directory.
-        download_queue_enabled:
-            Enables download queue.
-        download_queue_size:
-            Number of slots in the download queue.
-        encryption:
-            Set the session encryption mode, one of ``required``, ``preferred`` or ``tolerated``.
-        idle_seeding_limit:
-            The default seed inactivity limit in minutes.
-        idle_seeding_limit_enabled:
-            Enables the default seed inactivity limit
-        incomplete_dir:
-            The path to the directory of incomplete transfer data.
-        incomplete_dir_enabled:
-            Enables the incomplete transfer data directory,
-            Otherwise data for incomplete transfers are stored in the download target.
-        lpd_enabled:
-            Enables local peer discovery for public torrents.
-        peer_limit_global:
-            Maximum number of peers.
-        peer_limit_per_torrent:
-            Maximum number of peers per transfer.
-        peer_port:
-            Peer port.
-        peer_port_random_on_start:
-            Enables randomized peer port on start of Transmission.
-        pex_enabled:
-            Allowing PEX in public torrents.
-        port_forwarding_enabled:
-            Enables port forwarding.
-        queue_stalled_enabled:
-            Enable tracking of stalled transfers.
-        queue_stalled_minutes:
-            Number of minutes of idle that marks a transfer as stalled.
-        rename_partial_files:
-            Appends ".part" to incomplete files
-
-        seed_queue_enabled:
-            Enables upload queue.
-        seed_queue_size:
-            Number of slots in the upload queue.
-        seed_ratio_limit:
-            Seed ratio limit. 1.0 means 1:1 download and upload ratio.
-        seed_ratio_limited:
-            Enables seed ration limit.
-        speed_limit_down:
-            Download speed limit (in Kib/s).
-        speed_limit_down_enabled:
-            Enables download speed limiting.
-        speed_limit_up:
-            Upload speed limit (in Kib/s).
-        speed_limit_up_enabled:
-            Enables upload speed limiting.
-        start_added_torrents:
-            Added torrents will be started right away.
-        trash_original_torrent_files:
-            The .torrent file of added torrents will be deleted.
-        utp_enabled:
-            Enables Micro Transport Protocol (UTP).
-        script_torrent_done_enabled:
-            Whether to call the "done" script.
-        script_torrent_done_filename:
-            Filename of the script to run when the transfer is done.
-        script_torrent_added_filename:
-            filename of the script to run
-        script_torrent_added_enabled:
-            whether or not to call the ``added`` script
-        script_torrent_done_seeding_enabled:
-            whether or not to call the ``seeding-done`` script
-        script_torrent_done_seeding_filename:
-            filename of the script to run
-
-        Warnings
-        ----
-        ``kwargs`` is pass the arguments not supported yet future, it's not compatibility promising.
-
-        transmission-rpc will merge ``kwargs`` in rpc arguments *as-is*
+        Parameters:
+            timeout
+                request timeout
+            alt_speed_down:
+                max global download speed (KBps)
+            alt_speed_enabled:
+                true means use the alt speeds
+            alt_speed_time_begin:
+                Time when alternate speeds should be enabled. Minutes after midnight.
+            alt_speed_time_day:
+                Enables alternate speeds scheduling these days.
+            alt_speed_time_enabled:
+                Enables alternate speeds scheduling.
+            alt_speed_time_end:
+                Time when alternate speeds should be disabled. Minutes after midnight.
+            alt_speed_up:
+                Alternate session upload speed limit (in Kib/s).
+            blocklist_enabled:
+                Enables the block list
+            blocklist_url:
+                Location of the block list. Updated with blocklist-update.
+            cache_size_mb:
+                The maximum size of the disk cache in MB
+            default_trackers:
+                List of default trackers to use on public torrents.
+            dht_enabled:
+                Enables DHT.
+            download_dir:
+                Set the session download directory.
+            download_queue_enabled:
+                Enables download queue.
+            download_queue_size:
+                Number of slots in the download queue.
+            encryption:
+                Set the session encryption mode, one of ``required``, ``preferred`` or ``tolerated``.
+            idle_seeding_limit:
+                The default seed inactivity limit in minutes.
+            idle_seeding_limit_enabled:
+                Enables the default seed inactivity limit
+            incomplete_dir:
+                The path to the directory of incomplete transfer data.
+            incomplete_dir_enabled:
+                Enables the incomplete transfer data directory,
+                Otherwise data for incomplete transfers are stored in the download target.
+            lpd_enabled:
+                Enables local peer discovery for public torrents.
+            peer_limit_global:
+                Maximum number of peers.
+            peer_limit_per_torrent:
+                Maximum number of peers per transfer.
+            peer_port:
+                Peer port.
+            peer_port_random_on_start:
+                Enables randomized peer port on start of Transmission.
+            pex_enabled:
+                Allowing PEX in public torrents.
+            port_forwarding_enabled:
+                Enables port forwarding.
+            queue_stalled_enabled:
+                Enable tracking of stalled transfers.
+            queue_stalled_minutes:
+                Number of minutes of idle that marks a transfer as stalled.
+            rename_partial_files:
+                Appends ".part" to incomplete files
+
+            seed_queue_enabled:
+                Enables upload queue.
+            seed_queue_size:
+                Number of slots in the upload queue.
+            seed_ratio_limit:
+                Seed ratio limit. 1.0 means 1:1 download and upload ratio.
+            seed_ratio_limited:
+                Enables seed ration limit.
+            speed_limit_down:
+                Download speed limit (in Kib/s).
+            speed_limit_down_enabled:
+                Enables download speed limiting.
+            speed_limit_up:
+                Upload speed limit (in Kib/s).
+            speed_limit_up_enabled:
+                Enables upload speed limiting.
+            start_added_torrents:
+                Added torrents will be started right away.
+            trash_original_torrent_files:
+                The .torrent file of added torrents will be deleted.
+            utp_enabled:
+                Enables Micro Transport Protocol (UTP).
+            script_torrent_done_enabled:
+                Whether to call the "done" script.
+            script_torrent_done_filename:
+                Filename of the script to run when the transfer is done.
+            script_torrent_added_filename:
+                filename of the script to run
+            script_torrent_added_enabled:
+                whether or not to call the ``added`` script
+            script_torrent_done_seeding_enabled:
+                whether or not to call the ``seeding-done`` script
+            script_torrent_done_seeding_filename:
+                filename of the script to run
+
+        Warnings:
+            ``kwargs`` is pass the arguments not supported yet future, it's not compatibility promising.
+            transmission-rpc will merge ``kwargs`` in rpc arguments **as-is**
         """
 
         if encryption is not None and encryption not in ["required", "preferred", "tolerated"]:
             raise ValueError("Invalid encryption value")
 
         if default_trackers is not None:
             self._rpc_version_warning(17)
```

### Comparing `transmission_rpc-7.0.5/transmission_rpc/constants.py` & `transmission_rpc-7.0.6/transmission_rpc/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) 2018-2022 Trim21 <i@trim21.me>
 # Copyright (c) 2008-2014 Erik Svensson <erik.public@gmail.com>
 # Licensed under the MIT license.
 import enum
 import logging
-from typing import Dict, Optional, NamedTuple
+from typing import Dict, NamedTuple, Optional
 
 LOGGER = logging.getLogger("transmission-rpc")
 LOGGER.setLevel(logging.ERROR)
 
 
 DEFAULT_TIMEOUT = 30.0
```

### Comparing `transmission_rpc-7.0.5/transmission_rpc/error.py` & `transmission_rpc-7.0.6/transmission_rpc/error.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.5/transmission_rpc/session.py` & `transmission_rpc-7.0.6/transmission_rpc/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,17 +107,16 @@
 
         session = Client().get_session()
 
         current = session.download_dir
 
     https://github.com/transmission/transmission/blob/main/docs/rpc-spec.md#41-session-arguments
 
-    Warnings
-    --------
-    setter on session's properties has been removed, please use ``Client().set_session()`` instead
+    Warnings:
+        setter on session's properties has been removed, please use :py:meth`Client.set_session` instead
     """
 
     @property
     def alt_speed_down(self) -> int:
         """max global download speed (KBps)"""
         return self.fields["alt-speed-down"]
 
@@ -357,15 +356,15 @@
 
     @property
     def version(self) -> str:
         """long version str `$version ($revision)`"""
         return self.fields["version"]
 
     @property
-    def default_trackers(self) -> Optional[list]:
+    def default_trackers(self) -> Optional[List[str]]:
         """
         list of default trackers to use on public torrents
         new at rpc-version 17
         """
         trackers = self.get("default-trackers")
         if trackers:
             return trackers.split("\n")
```

### Comparing `transmission_rpc-7.0.5/transmission_rpc/torrent.py` & `transmission_rpc-7.0.6/transmission_rpc/torrent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import enum
+from datetime import datetime, timedelta, timezone
 from typing import Any, Dict, List, Optional
-from datetime import datetime, timezone, timedelta
 
-from transmission_rpc.types import File, Container
-from transmission_rpc.utils import format_timedelta
 from transmission_rpc.constants import IdleMode, Priority, RatioLimitMode
+from transmission_rpc.types import Container, File
+from transmission_rpc.utils import format_timedelta
 
 _STATUS_NEW_MAPPING = {
     0: "stopped",
     1: "check pending",
     2: "checking",
     3: "download pending",
     4: "downloading",
@@ -31,59 +31,74 @@
     DOWNLOAD_PENDING = "download pending"
     DOWNLOADING = "downloading"
     SEED_PENDING = "seed pending"
     SEEDING = "seeding"
 
     @property
     def stopped(self) -> bool:
+        """if torrent stopped"""
         return self == "stopped"
 
     @property
     def check_pending(self) -> bool:
+        """if torrent check pending"""
         return self == "check pending"
 
     @property
     def checking(self) -> bool:
+        """if torrent checking"""
         return self == "checking"
 
     @property
     def download_pending(self) -> bool:
+        """if download pending"""
         return self == "download pending"
 
     @property
     def downloading(self) -> bool:
+        """if downloading"""
         return self == "downloading"
 
     @property
     def seed_pending(self) -> bool:
+        """if seed pending"""
         return self == "seed pending"
 
     @property
     def seeding(self) -> bool:
+        """if seeding"""
         return self == "seeding"
 
     def __str__(self) -> str:
         return self.value
 
 
 class FileStat(Container):
+    """
+    type for :py:meth:`Torrent.file_stats`
+    """
+
     @property
     def bytesCompleted(self) -> int:
         return self.fields["bytesCompleted"]
 
     @property
     def wanted(self) -> int:
         return self.fields["wanted"]
 
     @property
     def priority(self) -> int:
         return self.fields["priority"]
 
 
 class Tracker(Container):
+    """
+    type for :py:attr:`Torrent.trackers`
+    """
+
     @property
     def id(self) -> int:
         return self.fields["id"]
 
     @property
     def announce(self) -> str:
         return self.fields["announce"]
@@ -94,14 +109,18 @@
 
     @property
     def tier(self) -> int:
         return self.fields["tier"]
 
 
 class TrackerStats(Container):
+    """
+    type for :py:attr:`Torrent.tracker_stats`
+    """
+
     @property
     def id(self) -> int:
         return self.fields["id"]
 
     @property
     def announce_state(self) -> int:
         return self.fields["announceState"]
@@ -207,17 +226,16 @@
         return self.fields["tier"]
 
 
 class Torrent(Container):
     """
     Torrent is a class holding the data received from Transmission regarding a bittorrent transfer.
 
-    Warnings
-    --------
-    setter on Torrent's properties has been removed, please use ``Client().change_torrent()`` instead
+    Warnings:
+        setter on Torrent's properties has been removed, please use :py:meth:`Client.change_torrent` instead
     """
 
     def __init__(self, *, fields: Dict[str, Any]):
         if "id" not in fields:
             raise ValueError(
                 "Torrent object requires field 'id', "
                 "you need to add 'id' in your 'arguments' when calling 'get_torrent'"
@@ -362,27 +380,25 @@
     def file_count(self) -> Optional[int]:
         return self.fields["file-count"]
 
     def get_files(self) -> List[File]:
         """
         Get list of files for this torrent.
 
-        Note
-        ----
-
+        Note:
             The order of the files is guaranteed. The index of file object is the id of the file
-            when calling :py:meth:`transmission_rpc.client.Client.set_files`.
+            when calling :py:meth:`transmission_rpc.Client.change_torrent`
 
         .. code-block:: python
 
             from transmission_rpc import Client
 
             torrent = Client().get_torrent(0)
 
-            for file in enumerate(torrent.get_files()):
+            for file in torrent.get_files():
                 print(file.id)
 
         """
         result: List[File] = []
         if "files" in self.fields:
             files = self.fields["files"]
             indices = range(len(files))
@@ -400,14 +416,15 @@
                 for id, file, raw_priority, raw_selected in zip(indices, files, priorities, wanted)
             )
 
         return result
 
     @property
     def file_stats(self) -> List[FileStat]:
+        """file stats"""
         return [FileStat(fields=x) for x in self.fields["fileStats"]]
 
     @property
     def group(self) -> str:
         return self.get("group", "")
 
     @property
@@ -584,23 +601,25 @@
 
     @property
     def size_when_done(self) -> int:
         return self.fields["sizeWhenDone"]
 
     @property
     def trackers(self) -> List[Tracker]:
+        """trackers of torrent"""
         return [Tracker(fields=x) for x in self.fields["trackers"]]
 
     @property
     def tracker_list(self) -> List[str]:
         """list of str of announce URLs"""
         return [x for x in self.fields["trackerList"].splitlines() if x]
 
     @property
     def tracker_stats(self) -> List[TrackerStats]:
+        """tracker status, for example, announce success/failure status"""
         return [TrackerStats(fields=x) for x in self.fields["trackerStats"]]
 
     @property
     def total_size(self) -> int:
         return self.fields["totalSize"]
 
     @property
@@ -627,16 +646,16 @@
         return self.fields["uploadLimited"]
 
     @property
     def upload_ratio(self) -> float:
         return self.fields["uploadRatio"]
 
     @property
-    def wanted(self) -> List:
-        # TODO
+    def wanted(self) -> List[int]:
+        """if files are wanted, sorted by file index. 1 for wanted 0 for unwanted"""
         return self.fields["wanted"]
 
     @property
     def webseeds(self) -> List[str]:
         return self.fields["webseeds"]
 
     @property
```

### Comparing `transmission_rpc-7.0.5/transmission_rpc/types.py` & `transmission_rpc-7.0.6/transmission_rpc/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Any, Dict, Tuple, Union, TypeVar, Optional, NamedTuple
+from typing import Any, Dict, NamedTuple, Optional, Tuple, TypeVar, Union
 
 from transmission_rpc.constants import Priority
 
 _Number = Union[int, float]
 _Timeout = Optional[Union[_Number, Tuple[_Number, _Number]]]
 
 T = TypeVar("T")
 
 
 class Container:
-    fields: Dict[str, Any]  #: raw fields
+    fields: Dict[str, Any]  #: raw response data
 
     def __init__(self, *, fields: Dict[str, Any]):
         self.fields = fields
 
     def get(self, key: str, default: Optional[T] = None) -> Any:
         """get the raw value by the **raw rpc response key**"""
         return self.fields.get(key, default)
```

### Comparing `transmission_rpc-7.0.5/transmission_rpc/utils.py` & `transmission_rpc-7.0.6/transmission_rpc/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) 2018-2021 Trim21 <i@trim21.me>
 # Copyright (c) 2008-2014 Erik Svensson <erik.public@gmail.com>
 # Licensed under the MIT license.
 import base64
-import pathlib
 import datetime
-from typing import List, Tuple, Union, BinaryIO, Optional
+import pathlib
+from typing import BinaryIO, List, Optional, Tuple, Union
 from urllib.parse import urlparse
 
 from transmission_rpc import constants
 
 UNITS = ["B", "KiB", "MiB", "GiB", "TiB", "PiB", "EiB"]
```

### Comparing `transmission_rpc-7.0.5/PKG-INFO` & `transmission_rpc-7.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transmission-rpc
-Version: 7.0.5
+Version: 7.0.6
 Summary: Python module that implements the Transmission bittorent client JSON-RPC protocol
 Home-page: https://github.com/Trim21/transmission-rpc
 License: MIT
 Keywords: transmission,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.8,<4.0
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: requests (>=2.23.0,<3.0.0)
-Requires-Dist: typing-extensions
+Requires-Dist: typing-extensions (>=4.5.0)
 Project-URL: Repository, https://github.com/Trim21/transmission-rpc
 Description-Content-Type: text/markdown
 
 # Transmission-rpc Readme
 
 [![PyPI](https://img.shields.io/pypi/v/transmission-rpc)](https://pypi.org/project/transmission-rpc/)
 [![Documentation Status](https://readthedocs.org/projects/transmission-rpc/badge/)](https://transmission-rpc.readthedocs.io/)
@@ -36,15 +36,15 @@
 `transmission-rpc` is a python wrapper on top of [transmission](https://github.com/transmission/transmission) JSON RPC protocol,
 hosted on GitHub at [github.com/trim21/transmission-rpc](https://github.com/trim21/transmission-rpc)
 
 ## Introduction
 
 `transmission-rpc` is a python module implementing the json-rpc client protocol for the BitTorrent client Transmission.
 
-Support 14 <= rpc version <= 17 (2.40 <= transmission version <= 4.0.4),
+Support 14 <= rpc version <= 17 (2.40 <= transmission version <= 4.0.5),
 should works fine with newer rpc version but some new feature may be missing.
 
 ## versioning
 
 `transmission-rpc` follow [Semantic Versioning](https://semver.org/),
 report an issue if you found unexpected API break changes at same major version.
```

