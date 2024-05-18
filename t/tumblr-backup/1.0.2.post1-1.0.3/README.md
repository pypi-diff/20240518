# Comparing `tmp/tumblr-backup-1.0.2.post1.tar.gz` & `tmp/tumblr_backup-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tumblr-backup-1.0.2.post1.tar", last modified: Fri Mar  8 04:58:03 2024, max compression
+gzip compressed data, was "tumblr_backup-1.0.3.tar", last modified: Sat May 18 17:05:59 2024, max compression
```

## Comparing `tumblr-backup-1.0.2.post1.tar` & `tumblr_backup-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2024-03-08 04:58:03.400759 tumblr-backup-1.0.2.post1/
--rw-r--r--   0 jared     (1000) jared     (1000)    32472 2018-12-11 04:10:23.000000 tumblr-backup-1.0.2.post1/LICENSE
--rw-r--r--   0 jared     (1000) jared     (1000)    16956 2024-03-08 04:58:03.399759 tumblr-backup-1.0.2.post1/PKG-INFO
--rw-r--r--   0 jared     (1000) jared     (1000)    15538 2024-03-08 02:15:04.000000 tumblr-backup-1.0.2.post1/README.md
--rw-r--r--   0 jared     (1000) jared     (1000)     1324 2024-03-08 04:57:18.000000 tumblr-backup-1.0.2.post1/pyproject.toml
--rw-r--r--   0 jared     (1000) jared     (1000)       38 2024-03-08 04:58:03.400759 tumblr-backup-1.0.2.post1/setup.cfg
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2024-03-08 04:58:03.398759 tumblr-backup-1.0.2.post1/tumblr_backup/
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2024-02-21 00:49:10.000000 tumblr-backup-1.0.2.post1/tumblr_backup/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)     4012 2024-02-21 00:49:10.000000 tumblr-backup-1.0.2.post1/tumblr_backup/is_reblog.py
--rw-r--r--   0 jared     (1000) jared     (1000)     2212 2024-02-21 00:49:10.000000 tumblr-backup-1.0.2.post1/tumblr_backup/login.py
--rw-r--r--   0 jared     (1000) jared     (1000)   101827 2024-03-08 04:46:40.000000 tumblr-backup-1.0.2.post1/tumblr_backup/main.py
--rw-r--r--   0 jared     (1000) jared     (1000)     9466 2024-02-21 00:49:10.000000 tumblr-backup-1.0.2.post1/tumblr_backup/note_scraper.py
--rw-r--r--   0 jared     (1000) jared     (1000)    13838 2024-02-21 00:49:10.000000 tumblr-backup-1.0.2.post1/tumblr_backup/util.py
--rw-r--r--   0 jared     (1000) jared     (1000)    31919 2024-03-08 04:15:58.000000 tumblr-backup-1.0.2.post1/tumblr_backup/wget.py
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2024-03-08 04:58:03.399759 tumblr-backup-1.0.2.post1/tumblr_backup.egg-info/
--rw-r--r--   0 jared     (1000) jared     (1000)    16956 2024-03-08 04:58:03.000000 tumblr-backup-1.0.2.post1/tumblr_backup.egg-info/PKG-INFO
--rw-r--r--   0 jared     (1000) jared     (1000)      428 2024-03-08 04:58:03.000000 tumblr-backup-1.0.2.post1/tumblr_backup.egg-info/SOURCES.txt
--rw-r--r--   0 jared     (1000) jared     (1000)        1 2024-03-08 04:58:03.000000 tumblr-backup-1.0.2.post1/tumblr_backup.egg-info/dependency_links.txt
--rw-r--r--   0 jared     (1000) jared     (1000)       94 2024-03-08 04:58:03.000000 tumblr-backup-1.0.2.post1/tumblr_backup.egg-info/entry_points.txt
--rw-r--r--   0 jared     (1000) jared     (1000)      207 2024-03-08 04:58:03.000000 tumblr-backup-1.0.2.post1/tumblr_backup.egg-info/requires.txt
--rw-r--r--   0 jared     (1000) jared     (1000)       14 2024-03-08 04:58:03.000000 tumblr-backup-1.0.2.post1/tumblr_backup.egg-info/top_level.txt
+drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2024-05-18 17:05:59.851087 tumblr_backup-1.0.3/
+-rw-r--r--   0 jared     (1000) jared     (1000)    32472 2018-12-11 04:10:23.000000 tumblr_backup-1.0.3/LICENSE
+-rw-r--r--   0 jared     (1000) jared     (1000)    17420 2024-05-18 17:05:59.850087 tumblr_backup-1.0.3/PKG-INFO
+-rw-r--r--   0 jared     (1000) jared     (1000)    15538 2024-03-17 18:05:25.000000 tumblr_backup-1.0.3/README.md
+-rw-r--r--   0 jared     (1000) jared     (1000)     2501 2024-05-08 01:23:39.000000 tumblr_backup-1.0.3/pyproject.toml
+-rw-r--r--   0 jared     (1000) jared     (1000)       38 2024-05-18 17:05:59.851087 tumblr_backup-1.0.3/setup.cfg
+drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2024-05-18 17:05:59.848087 tumblr_backup-1.0.3/tumblr_backup/
+-rw-r--r--   0 jared     (1000) jared     (1000)        0 2024-03-17 18:05:25.000000 tumblr_backup-1.0.3/tumblr_backup/__init__.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     4046 2024-05-08 01:23:39.000000 tumblr_backup-1.0.3/tumblr_backup/is_reblog.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     2248 2024-05-08 01:23:39.000000 tumblr_backup-1.0.3/tumblr_backup/login.py
+-rw-r--r--   0 jared     (1000) jared     (1000)   101822 2024-05-18 16:50:54.000000 tumblr_backup-1.0.3/tumblr_backup/main.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     9518 2024-05-08 01:23:39.000000 tumblr_backup-1.0.3/tumblr_backup/note_scraper.py
+-rw-r--r--   0 jared     (1000) jared     (1000)    13840 2024-05-08 01:23:39.000000 tumblr_backup-1.0.3/tumblr_backup/util.py
+-rw-r--r--   0 jared     (1000) jared     (1000)    31868 2024-05-08 01:23:39.000000 tumblr_backup-1.0.3/tumblr_backup/wget.py
+drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2024-05-18 17:05:59.849087 tumblr_backup-1.0.3/tumblr_backup.egg-info/
+-rw-r--r--   0 jared     (1000) jared     (1000)    17420 2024-05-18 17:05:59.000000 tumblr_backup-1.0.3/tumblr_backup.egg-info/PKG-INFO
+-rw-r--r--   0 jared     (1000) jared     (1000)      428 2024-05-18 17:05:59.000000 tumblr_backup-1.0.3/tumblr_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 jared     (1000) jared     (1000)        1 2024-05-18 17:05:59.000000 tumblr_backup-1.0.3/tumblr_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 jared     (1000) jared     (1000)       94 2024-05-18 17:05:59.000000 tumblr_backup-1.0.3/tumblr_backup.egg-info/entry_points.txt
+-rw-r--r--   0 jared     (1000) jared     (1000)      404 2024-05-18 17:05:59.000000 tumblr_backup-1.0.3/tumblr_backup.egg-info/requires.txt
+-rw-r--r--   0 jared     (1000) jared     (1000)       14 2024-05-18 17:05:59.000000 tumblr_backup-1.0.3/tumblr_backup.egg-info/top_level.txt
```

### Comparing `tumblr-backup-1.0.2.post1/LICENSE` & `tumblr_backup-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tumblr-backup-1.0.2.post1/PKG-INFO` & `tumblr_backup-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,7 @@
-Metadata-Version: 2.1
-Name: tumblr-backup
-Version: 1.0.2.post1
-Summary: An advanced tool for backing up Tumblr blogs.
-Project-URL: Homepage, https://github.com/cebtenzzre/tumblr-utils
-Project-URL: Bug Reports, https://github.com/cebtenzzre/tumblr-utils/issues
-Project-URL: Source, https://github.com/cebtenzzre/tumblr-utils
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: filetype~=1.2
-Requires-Dist: platformdirs~=4.2
-Requires-Dist: requests~=2.31
-Requires-Dist: urllib3~=2.2
-Provides-Extra: exif
-Requires-Dist: py3exiv2~=0.12; extra == "exif"
-Provides-Extra: jq
-Requires-Dist: jq~=1.6; extra == "jq"
-Provides-Extra: notes
-Requires-Dist: beautifulsoup4~=4.12; extra == "notes"
-Requires-Dist: lxml~=5.1; extra == "notes"
-Provides-Extra: video
-Requires-Dist: yt_dlp>=2023.12.30; extra == "video"
-Provides-Extra: all
-Requires-Dist: tumblr-backup[exif,jq,notes,video]; extra == "all"
-
 # tumblr-backup
 
 ### About this fork
 
 This is a fork of bbolli's
 [tumblr-utils](https://github.com/bbolli/tumblr-utils), with a focus on
 tumblr\_backup.py. It adds Python 3 compatibility, various bug fixes, a few
```

### Comparing `tumblr-backup-1.0.2.post1/README.md` & `tumblr_backup-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,52 @@
+Metadata-Version: 2.1
+Name: tumblr-backup
+Version: 1.0.3
+Summary: An advanced tool for backing up Tumblr blogs.
+Project-URL: Homepage, https://github.com/cebtenzzre/tumblr-utils
+Project-URL: Bug Reports, https://github.com/cebtenzzre/tumblr-utils/issues
+Project-URL: Source, https://github.com/cebtenzzre/tumblr-utils
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: filetype~=1.2
+Requires-Dist: platformdirs~=4.2
+Requires-Dist: requests~=2.31
+Requires-Dist: urllib3~=2.2
+Provides-Extra: exif
+Requires-Dist: py3exiv2~=0.12; extra == "exif"
+Provides-Extra: jq
+Requires-Dist: jq~=1.6; extra == "jq"
+Provides-Extra: notes
+Requires-Dist: beautifulsoup4~=4.12; extra == "notes"
+Requires-Dist: lxml~=5.1; extra == "notes"
+Provides-Extra: video
+Requires-Dist: yt_dlp>=2023.12.30; extra == "video"
+Provides-Extra: all
+Requires-Dist: tumblr-backup[exif,jq,notes,video]; extra == "all"
+Provides-Extra: dev
+Requires-Dist: tumblr-backup[all]; extra == "dev"
+Requires-Dist: flake8~=7.0; extra == "dev"
+Requires-Dist: mypy~=1.9; extra == "dev"
+Requires-Dist: pytype>=2024.2.27; extra == "dev"
+Requires-Dist: wemake-python-styleguide~=0.18; extra == "dev"
+Requires-Dist: lxml-stubs~=0.5; extra == "dev"
+Requires-Dist: pysocks~=1.7; extra == "dev"
+Requires-Dist: types-beautifulsoup4~=4.12; extra == "dev"
+Requires-Dist: types-requests~=2.31; extra == "dev"
+Requires-Dist: youtube_dl>=2021.12.17; extra == "dev"
+
 # tumblr-backup
 
 ### About this fork
 
 This is a fork of bbolli's
 [tumblr-utils](https://github.com/bbolli/tumblr-utils), with a focus on
 tumblr\_backup.py. It adds Python 3 compatibility, various bug fixes, a few
```

### Comparing `tumblr-backup-1.0.2.post1/tumblr_backup/is_reblog.py` & `tumblr_backup-1.0.3/tumblr_backup/is_reblog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
+from __future__ import annotations
+
 import re
-from typing import Any, Callable, Dict
+from typing import Any, Callable
 
 
-def _check_posted_note(doc: Dict[str, Any]) -> bool:
+def _check_posted_note(doc: dict[str, Any]) -> bool:
     notes = doc.get('notes')
     if not (notes and isinstance(notes, list)):
         return False  # no notes available
 
     n = notes[-1]
     return bool(
         n['type'] == 'posted'
         and n['timestamp'] < doc['timestamp']  # sometimes a later reblog is credited
-        and n['blog_uuid'] != doc['blog']['uuid']
+        and n['blog_uuid'] != doc['blog']['uuid'],
     )
 
 
-def _check_content(doc: Dict[str, Any], pred: Callable[[str], bool], name: str) -> bool:
+def _check_content(doc: dict[str, Any], pred: Callable[[str], bool], name: str) -> bool:
     reblog_info = doc.get('reblog', {})
 
     if doc.get('is_submission') and not reblog_info.get('tree_html'):
         return False  # prone to false-positives
     if 'post_html' in doc:
         return False  # post_html is messy and we have root_id anyway
 
@@ -27,15 +29,15 @@
     if 'source' in doc:
         return name == 'via' and pred(doc['source'])  # this key is more specific
 
     # reason: comment content
     return bool(
         reblog_info
         and (name == 'via' or not reblog_info['tree_html'])
-        and pred(reblog_info['comment'])
+        and pred(reblog_info['comment']),
     )
 
 
 BQ_RE = re.compile(
     r'('
       r'<(?!a[ >])[^<>]+>'
       r'|'
@@ -64,15 +66,15 @@
       r')"'
       r'|'
       r' [^\s</>"' "'" r'=]+(="[^"]*"|\b)'
     r')*'
     r'>'
       r'[^<>]*'  # poster-editable
     r'</a>:'
-    r'(?![^\S\n]*[^<\s])'
+    r'(?![^\S\n]*[^<\s])',
 )
 BQ_RE2 = re.compile(r'(<p>)+[a-z0-9-]+:</p>\n*<blockquote>')
 
 
 def bqpred(c: str) -> bool:
     if 'replied to your' in c:
         return False
@@ -80,19 +82,19 @@
         return True
     m = BQ_RE.match(c)
     if not m:
         return False
     return bool(
         'tumblr_blog' in (m.group('classes') or '').split(' ')
         or m.group('blogpost') or m.group('priv') or m.group('bname0')
-        or ((m.group('blogco') or m.group('bname1')) and re.search(r'<blockquote[ >]', c))
+        or ((m.group('blogco') or m.group('bname1')) and re.search(r'<blockquote[ >]', c)),
     )
 
 
-def post_is_reblog(doc: Dict[str, Any]) -> bool:
+def post_is_reblog(doc: dict[str, Any]) -> bool:
     # reason: reblogged_from_id
     # true for 84.9% of posts, 99.7% of reblogs
     if 'reblogged_from_id' in doc:
         return True
 
     # reason: root_id
     # false for all svc reblogs (let's say 14.3% of posts)
```

### Comparing `tumblr-backup-1.0.2.post1/tumblr_backup/login.py` & `tumblr_backup-1.0.3/tumblr_backup/login.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 """
 This script uses Tumblr's internal SVC API to access a hidden or explicit blog,
 and retrieves a JSON of very similar (but not quite identical) format to the
 normal API.
 """
 
+from __future__ import annotations
+
 import re
 import sys
 from getpass import getpass
 from http.cookiejar import MozillaCookieJar
 
 import requests
```

### Comparing `tumblr-backup-1.0.2.post1/tumblr_backup/main.py` & `tumblr_backup-1.0.3/tumblr_backup/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # builtin modules
+from __future__ import annotations
+
 import argparse
 import calendar
 import contextlib
 import errno
 import hashlib
 import http.client
 import itertools
@@ -10,72 +12,69 @@
 import locale
 import multiprocessing
 import os
 import re
 import shutil
 import signal
 import sys
+import textwrap
 import threading
 import time
 import traceback
 from argparse import Namespace
 from collections import defaultdict
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from multiprocessing.queues import SimpleQueue
 from os.path import join, split, splitext
 from pathlib import Path
 from posixpath import basename as urlbasename, join as urlpathjoin, splitext as urlsplitext
 from tempfile import NamedTemporaryFile
 from types import ModuleType
-from typing import (TYPE_CHECKING, Any, Callable, ContextManager, DefaultDict, Dict, Iterable, Iterator, List, Optional,
-                    Set, TextIO, Tuple, Type, Union, cast)
+from typing import TYPE_CHECKING, Any, Callable, ContextManager, Iterable, Iterator, Literal, TextIO, cast
 from urllib.parse import quote, urlencode, urlparse
 from xml.sax.saxutils import escape
 
 # third-party modules
 import filetype
 import platformdirs
 import requests
 
 # internal modules
-from .util import (AsyncCallable, ConnectionFile, FakeGenericMeta, LockedQueue, LogLevel, MultiCondition, copyfile,
-                   enospc, fdatasync, fsync, have_module, is_dns_working, make_requests_session, no_internet, opendir,
-                   to_bytes)
-from .wget import HTTPError, HTTP_TIMEOUT, Retry, WGError, WgetRetrieveWrapper, setup_wget, touch, urlopen
 from .is_reblog import post_is_reblog
+from .util import (AsyncCallable, ConnectionFile, LockedQueue, LogLevel, MultiCondition, copyfile, enospc, fdatasync,
+                   fsync, have_module, is_dns_working, make_requests_session, no_internet, opendir, to_bytes)
+from .wget import HTTP_TIMEOUT, HTTPError, Retry, WGError, WgetRetrieveWrapper, setup_wget, touch, urlopen
 
 if TYPE_CHECKING:
-    from typing_extensions import Literal
     from bs4 import Tag
+    from typing_extensions import TypeAlias
 else:
-    class Literal(metaclass=FakeGenericMeta):
-        pass
     Tag = None
 
-JSONDict = Dict[str, Any]
+JSONDict: TypeAlias = 'dict[str, Any]'
 
 # extra optional packages
 try:
     import pyexiv2
 except ImportError:
     if not TYPE_CHECKING:
         pyexiv2 = None
 
 try:
-    import jq
+    import jq  # type: ignore[import-not-found]
 except ImportError:
     if not TYPE_CHECKING:
         jq = None
 
 # Imported later if needed
-ytdl_module: Optional[ModuleType] = None
+ytdl_module: ModuleType | None = None
 
 # Format of displayed tags
-TAG_FMT = '#{}'
+TAG_FMT = '#{}'  # noqa: P103
 
 # Format of tag link URLs; set to None to suppress the links.
 # Named placeholders that will be replaced: domain, tag
 TAGLINK_FMT = 'https://{domain}/tagged/{tag}'
 
 # exit codes
 EXIT_SUCCESS    = 0
@@ -130,20 +129,20 @@
 MUST_MATCH_OPTIONS = PREV_MUST_MATCH_OPTIONS + MEDIA_PATH_OPTIONS
 BACKUP_CHANGING_OPTIONS = (
     'save_images', 'save_video', 'save_video_tumblr', 'save_audio', 'save_notes', 'copy_notes', 'notes_limit', 'json',
     'count', 'skip', 'period', 'request', 'filter', 'no_reblog', 'only_reblog', 'exif', 'prev_archives',
     'use_server_timestamps', 'user_agent', 'no_get', 'internet_archive', 'media_list', 'idents',
 )
 
-wget_retrieve: Optional[WgetRetrieveWrapper] = None
+wget_retrieve: WgetRetrieveWrapper | None = None
 main_thread_lock = threading.RLock()
 multicond = MultiCondition(main_thread_lock)
-disable_note_scraper: Set[str] = set()
+disable_note_scraper: set[str] = set()
 disablens_lock = threading.Lock()
-downloading_media: Set[str] = set()
+downloading_media: set[str] = set()
 downloading_media_cond = threading.Condition()
 
 
 def load_bs4(reason):
     sys.modules['soupsieve'] = ()  # type: ignore[assignment]
     try:
         from bs4 import BeautifulSoup
@@ -157,16 +156,16 @@
 
 
 class Logger:
     def __init__(self, quiet=False, file=sys.stdout):
         self.quiet = quiet
         self.file = file
         self.lock = threading.Lock()
-        self.backup_account: Optional[str] = None
-        self.status_msg: Optional[str] = None
+        self.backup_account: str | None = None
+        self.status_msg: str | None = None
 
     def log(self, level: LogLevel, msg: str, account: bool = False) -> None:
         if self.quiet and level < LogLevel.WARN:
             return
         with self.lock:
             for line in msg.splitlines(True):
                 self._print(line, account)
@@ -202,21 +201,21 @@
         pad = ' ' * (80 - len(msg))  # Pad to 80 chars
         print(msg + pad + term, end='', file=self.file)
 
 
 logger = Logger()
 
 
-def mkdir(dir, recursive=False):
-    if not os.path.exists(dir):
+def mkdir(dir_, recursive=False):
+    if not os.path.exists(dir_):
         try:
             if recursive:
-                os.makedirs(dir)
+                os.makedirs(dir_)
             else:
-                os.mkdir(dir)
+                os.mkdir(dir_)
         except FileExistsError:
             pass  # ignored
 
 
 def path_to(*parts):
     return join(save_folder, *parts)
 
@@ -277,20 +276,18 @@
 
 
 def get_api_url(account: str, likes: bool) -> str:
     """construct the tumblr API URL"""
     global blog_name
     blog_name = account
     if any(c in account for c in '/\\') or account in ('.', '..'):
-        raise ValueError('Invalid blog name: {!r}'.format(account))
+        raise ValueError(f'Invalid blog name: {account!r}')
     if '.' not in account:
         blog_name += '.tumblr.com'
-    return 'https://api.tumblr.com/v2/blog/%s/%s' % (
-        blog_name, 'likes' if likes else 'posts'
-    )
+    return f'https://api.tumblr.com/v2/blog/{blog_name}/{"likes" if likes else "posts"}'
 
 
 def parse_period_date(period):
     """Prepare the period start and end timestamps"""
     timefn: Callable[[Any], float] = time.mktime
     # UTC marker
     if period[-1] == 'Z':
@@ -318,30 +315,30 @@
 
 def get_posts_key(likes: bool) -> str:
     return 'liked_posts' if likes else 'posts'
 
 
 class ApiParser:
     TRY_LIMIT = 2
-    session: Optional[requests.Session] = None
-    api_key: Optional[str] = None
+    session: requests.Session | None = None
+    api_key: str | None = None
 
     def __init__(self, base: str, account: str, options: Namespace):
         self.base = base
         self.account = account
         self.options = options
-        self.prev_resps: Optional[List[str]] = None
-        self.dashboard_only_blog: Optional[bool] = None
-        self._prev_iter: Optional[Iterator[JSONDict]] = None
-        self._last_mode: Optional[str] = None
-        self._last_offset: Optional[int] = None
+        self.prev_resps: list[str] | None = None
+        self.dashboard_only_blog: bool | None = None
+        self._prev_iter: Iterator[JSONDict] | None = None
+        self._last_mode: str | None = None
+        self._last_offset: int | None = None
 
     @classmethod
     def setup(
-        cls, api_key: str, no_ssl_verify: bool, user_agent: str, cookiefile: Union[str, os.PathLike[str]],
+        cls, api_key: str, no_ssl_verify: bool, user_agent: str, cookiefile: str | os.PathLike[str],
     ) -> None:
         cls.api_key = api_key
         cls.session = make_requests_session(
             requests.Session, HTTP_RETRY, HTTP_TIMEOUT,
             not no_ssl_verify, user_agent, cookiefile,
         )
 
@@ -378,25 +375,15 @@
                 read_resp(p)['liked_timestamp'] if self.options.likes
                 else int(os.path.basename(p)[:-5])
             ),
             reverse=True,
         )
         return True
 
-    def _iter_prev(self) -> Iterator[JSONDict]:
-        assert self.prev_resps is not None
-        for path in self.prev_resps:
-            with open(path, encoding=FILE_ENCODING) as f:
-                try:
-                    yield json.load(f)
-                except ValueError as e:
-                    f.seek(0)
-                    logger.error('{}: {}\n{!r}\n'.format(e.__class__.__name__, e, f.read()))
-
-    def get_initial(self) -> Optional[JSONDict]:
+    def get_initial(self) -> JSONDict | None:
         if self.prev_resps is not None:
             try:
                 first_post = next(self._iter_prev())
             except StopIteration:
                 return None
             r = {get_posts_key(self.options.likes): [first_post], 'blog': first_post['blog'].copy()}
             if self.options.likes:
@@ -407,15 +394,15 @@
 
         resp = self.apiparse(1)
         if self.dashboard_only_blog and resp and resp['posts']:
             # svc API doesn't return blog info, steal it from the first post
             resp['blog'] = resp['posts'][0]['blog']
         return resp
 
-    def apiparse(self, count, start=0, before=None, ident=None) -> Optional[JSONDict]:
+    def apiparse(self, count, start=0, before=None, ident=None) -> JSONDict | None:
         assert self.api_key is not None
 
         if self.prev_resps is not None:
             if self._prev_iter is None:
                 self._prev_iter = self._iter_prev()
             if ident is not None:
                 assert self._last_mode in (None, 'ident')
@@ -444,15 +431,15 @@
                 posts = list(itertools.islice(it, None, count))
             return {get_posts_key(self.options.likes): posts}
 
         if self.dashboard_only_blog:
             base = 'https://www.tumblr.com/svc/indash_blog'
             params = {'tumblelog_name_or_id': self.account, 'post_id': '', 'limit': count,
                       'should_bypass_safemode': 'true', 'should_bypass_tagfiltering': 'true'}
-            headers: Optional[Dict[str, str]] = {
+            headers: dict[str, str] | None = {
                 'Referer': 'https://www.tumblr.com/dashboard/blog/' + self.account,
                 'X-Requested-With': 'XMLHttpRequest',
             }
         else:
             base = self.base
             params = {'api_key': self.api_key, 'limit': count, 'reblog_info': 'true'}
             headers = None
@@ -503,14 +490,24 @@
                     logger.info('[Note Scraper] Dashboard-only blog - scraping disabled for {}\n'.format(self.account))
         elif self.dashboard_only_blog is None:
             # If the first API request succeeds, it's a public blog
             self.dashboard_only_blog = False
 
         return doc.get('response')
 
+    def _iter_prev(self) -> Iterator[JSONDict]:
+        assert self.prev_resps is not None
+        for path in self.prev_resps:
+            with open(path, encoding=FILE_ENCODING) as f:
+                try:
+                    yield json.load(f)
+                except ValueError as e:
+                    f.seek(0)
+                    logger.error('{}: {}\n{!r}\n'.format(e.__class__.__name__, e, f.read()))
+
     def _get_resp(self, base, params, headers):
         assert self.session is not None
         try_count = 0
         while True:
             try:
                 with self.session.get(base, params=params, headers=headers) as resp:
                     try_count += 1
@@ -542,21 +539,21 @@
     def _ratelimit_sleep(headers):
         # Daily ratelimit
         if headers.get('X-Ratelimit-Perday-Remaining') == '0':
             reset = headers.get('X-Ratelimit-Perday-Reset')
             try:
                 freset = float(reset)  # pytype: disable=wrong-arg-types
             except (TypeError, ValueError):
-                logger.error("Expected numerical X-Ratelimit-Perday-Reset, got {!r}\n".format(reset))
+                logger.error(f'Expected numerical X-Ratelimit-Perday-Reset, got {reset!r}\n')
                 msg = 'sometime tomorrow'
             else:
                 treset = datetime.now() + timedelta(seconds=freset)
                 msg = 'at {}'.format(treset.ctime())
             raise RuntimeError('{}: Daily API ratelimit exceeded. Resume with --continue after reset {}.\n'.format(
-                logger.backup_account, msg
+                logger.backup_account, msg,
             ))
 
         # Hourly ratelimit
         reset = headers.get('X-Ratelimit-Perhour-Reset')
         if reset is None:
             return False
 
@@ -580,15 +577,15 @@
             ))
 
         logger.warn('Hit hourly ratelimit, sleeping for {} as requested\n'.format(sleep_dur_str), account=True)
         time.sleep(sleep_dur + 1)  # +1 to be sure we're past the reset
         return True
 
 
-def add_exif(image_name: str, tags: Set[str], exif: Set[str]) -> None:
+def add_exif(image_name: str, tags: set[str], exif: set[str]) -> None:
     assert pyexiv2 is not None
     try:
         metadata = pyexiv2.ImageMetadata(image_name)
         metadata.read()
     except OSError as e:
         logger.error('Error reading metadata for image {!r}: {!r}\n'.format(image_name, e))
         return
@@ -605,28 +602,28 @@
         metadata.write()
     except OSError as e:
         logger.error('Writing metadata failed for tags {} in {!r}: {!r}\n'.format(tags, image_name, e))
 
 
 def save_style():
     with open_text(backup_css) as css:
-        css.write('''\
-@import url("override.css");
+        css.write(textwrap.dedent("""\
+            @import url("override.css");
 
-body { width: 720px; margin: 0 auto; }
-body > footer { padding: 1em 0; }
-header > img { float: right; }
-img { max-width: 720px; }
-blockquote { margin-left: 0; border-left: 8px #999 solid; padding: 0 24px; }
-.archive h1, .subtitle, article { padding-bottom: 0.75em; border-bottom: 1px #ccc dotted; }
-article[class^="liked-"] { background-color: #f0f0f8; }
-.post a.llink { display: none; }
-header a, footer a { text-decoration: none; }
-footer, article footer a { font-size: small; color: #999; }
-''')
+            body { width: 720px; margin: 0 auto; }
+            body > footer { padding: 1em 0; }
+            header > img { float: right; }
+            img { max-width: 720px; }
+            blockquote { margin-left: 0; border-left: 8px #999 solid; padding: 0 24px; }
+            .archive h1, .subtitle, article { padding-bottom: 0.75em; border-bottom: 1px #ccc dotted; }
+            article[class^="liked-"] { background-color: #f0f0f8; }
+            .post a.llink { display: none; }
+            header a, footer a { text-decoration: none; }
+            footer, article footer a { font-size: small; color: #999; }
+        """))
 
 
 def find_files(path, match=None):
     try:
         it = os.scandir(path)
     except FileNotFoundError:
         return  # ignore nonexistent dir
@@ -644,15 +641,15 @@
     yield from filter(os.path.exists, indexes)
 
 
 def match_avatar(name):
     return name.startswith(avatar_base + '.')
 
 
-def get_avatar(prev_archive: Union[str, os.PathLike[str]], no_get: bool) -> None:
+def get_avatar(prev_archive: str | os.PathLike[str], no_get: bool) -> None:
     if prev_archive is not None:
         # Copy old avatar, if present
         avatar_matches = find_files(join(prev_archive, theme_dir), match_avatar)
         src = next(avatar_matches, None)
         if src is not None:
             path_parts = (theme_dir, split(src)[-1])
             cpy_res = maybe_copy_media(prev_archive, path_parts)
@@ -680,15 +677,15 @@
     assert wget_retrieve is not None
     try:
         wget_retrieve(url, avatar_dest, adjust_basename=adj_bn)
     except WGError as e:
         e.log()
 
 
-def get_style(prev_archive: Union[str, os.PathLike[str]], no_get: bool, use_dns_check: bool) -> None:
+def get_style(prev_archive: str | os.PathLike[str], no_get: bool, use_dns_check: bool) -> None:
     """Get the blog's CSS by brute-forcing it from the home page.
     The v2 API has no method for getting the style directly.
     See https://groups.google.com/d/msg/tumblr-api/f-rRH6gOb6w/sAXZIeYx5AUJ"""
     if prev_archive is not None:
         # Copy old style, if present
         path_parts = (theme_dir, 'style.css')
         cpy_res = maybe_copy_media(prev_archive, path_parts)
@@ -765,28 +762,28 @@
 
     try:
         import yt_dlp
     except ImportError:
         pass
     else:
         ytdl_module = yt_dlp
-        return ytdl_module
+        return ytdl_module  # noqa: WPS331
 
     import youtube_dl
 
     ytdl_module = youtube_dl
-    return ytdl_module
+    return ytdl_module  # noqa: WPS331
 
 
 class Index:
-    index: DefaultDict[int, DefaultDict[int, List['LocalPost']]]
+    index: defaultdict[int, defaultdict[int, list[LocalPost]]]
 
     def __init__(
-        self, blog: 'TumblrBackup', posts_per_page: int, dirs: bool, reverse_month: bool, reverse_index: bool,
-        tag_index: bool, body_class: str = 'index'
+        self, blog: TumblrBackup, posts_per_page: int, dirs: bool, reverse_month: bool, reverse_index: bool,
+        tag_index: bool, body_class: str = 'index',
     ):
         self.blog = blog
         self.posts_per_page = posts_per_page
         self.dirs_option = dirs
         self.reverse_month = reverse_month
         self.reverse_index = reverse_index
         self.tag_index = tag_index
@@ -794,37 +791,37 @@
         self.index = defaultdict(lambda: defaultdict(list))
 
     def add_post(self, post):
         self.index[post.tm.tm_year][post.tm.tm_mon].append(post)
 
     def save_index(self, index_dir='.', title=None):
         archives = sorted(((y, m) for y in self.index for m in self.index[y]),
-            reverse=self.reverse_month
-        )
+                          reverse=self.reverse_month)
         subtitle = self.blog.title if title else self.blog.subtitle
         title = title or self.blog.title
         with open_text(index_dir, dir_index) as idx:
             idx.write(self.blog.header(title, self.body_class, subtitle, avatar=True))
             if self.tag_index and self.body_class == 'index':
                 idx.write('<p><a href={}>Tag index</a></p>\n'.format(
-                    urlpathjoin(tag_index_dir, dir_index)
+                    urlpathjoin(tag_index_dir, dir_index),
                 ))
             for year in sorted(self.index.keys(), reverse=self.reverse_index):
                 self.save_year(idx, archives, index_dir, year)
-            idx.write('<footer><p>Generated on %s by <a href=https://github.com/'
-                'bbolli/tumblr-utils>tumblr-utils</a>.</p></footer>\n' % strftime('%x %X')
+            idx.write(
+                f'<footer><p>Generated on {strftime("%x %X")} by <a href=https://github.com/'
+                f'bbolli/tumblr-utils>tumblr-utils</a>.</p></footer>\n',
             )
 
     def save_year(self, idx, archives, index_dir, year):
         idx.write('<h3>%s</h3>\n<ul>\n' % year)
         for month in sorted(self.index[year].keys(), reverse=self.reverse_index):
             tm = time.localtime(time.mktime((year, month, 3, 0, 0, 0, 0, 0, -1)))
             month_name = self.save_month(archives, index_dir, year, month, tm)
             idx.write('    <li><a href={} title="{} post(s)">{}</a></li>\n'.format(
-                urlpathjoin(archive_dir, month_name), len(self.index[year][month]), strftime('%B', tm)
+                urlpathjoin(archive_dir, month_name), len(self.index[year][month]), strftime('%B', tm),
             ))
         idx.write('</ul>\n\n')
 
     def save_month(self, archives, index_dir, year, month, tm):
         posts = sorted(self.index[year][month], key=lambda x: x.date, reverse=self.reverse_month)
         posts_month = len(posts)
         posts_page = self.posts_per_page if self.posts_per_page >= 1 else posts_month
@@ -838,15 +835,15 @@
             i += inc
             if 0 <= i < len(archives):
                 return archives[i]
             return 0, 0
 
         FILE_FMT = '%d-%02d-p%s%s'
         pages_month = pages_per_month(year, month)
-        first_file: Optional[str] = None
+        first_file: str | None = None
         for page, start in enumerate(range(0, posts_month, posts_page), start=1):
 
             archive = [self.blog.header(strftime('%B %Y', tm), body_class='archive')]
             archive.extend(p.get_post(self.body_class == 'tag-archive') for p in posts[start:start + posts_page])
 
             suffix = '/' if self.dirs_option else post_ext
             file_name = FILE_FMT % (year, month, page, suffix)
@@ -877,36 +874,36 @@
 
         assert first_file is not None
         return first_file
 
 
 class TagIndex(Index):
     def __init__(
-        self, name: str, blog: 'TumblrBackup', posts_per_page: int, dirs: bool, reverse_month: bool,
-        reverse_index: bool, tag_index: bool,
+        self, name: str, blog: TumblrBackup, posts_per_page: int, dirs: bool, reverse_month: bool, reverse_index: bool,
+        tag_index: bool,
     ):
         super().__init__(blog, posts_per_page, dirs=dirs, reverse_month=reverse_month, reverse_index=reverse_index,
                          tag_index=tag_index, body_class='tag-archive')
         self.name = name
 
 
 class Indices:
     def __init__(
-        self, blog: 'TumblrBackup', posts_per_page: int, dirs: bool, reverse_month: bool, reverse_index: bool,
+        self, blog: TumblrBackup, posts_per_page: int, dirs: bool, reverse_month: bool, reverse_index: bool,
         tag_index: bool,
     ):
         self.blog = blog
         self.posts_per_page = posts_per_page
         self.dirs_option = dirs
         self.reverse_month = reverse_month
         self.reverse_index = reverse_index
         self.tag_index = tag_index
         self.main_index = Index(blog, posts_per_page, dirs=dirs, reverse_month=reverse_month,
                                 reverse_index=reverse_index, tag_index=tag_index)
-        self.tags: Dict[str, TagIndex] = {}
+        self.tags: dict[str, TagIndex] = {}
 
     def build_index(self):
         posts = (LocalPost(p, self.tag_index) for p in find_post_files(self.dirs_option))
         for post in posts:
             self.main_index.add_post(post)
             if self.tag_index:
                 for tag, name in post.tags:
@@ -927,66 +924,66 @@
     def save_tag_index(self):
         global save_dir
         save_dir = '../../..'
         mkdir(path_to(tag_index_dir))
         tag_index = [self.blog.header('Tag index', 'tag-index', self.blog.title, avatar=True), '<ul>']
         for tag, index in sorted(self.tags.items(), key=lambda kv: kv[1].name):
             digest = hashlib.md5(to_bytes(tag)).hexdigest()
-            index.save_index(tag_index_dir + os.sep + digest,
-                "Tag ‛%s’" % index.name
-            )
+            index.save_index(tag_index_dir + os.sep + digest, f'Tag ‛{index.name}’')
             tag_index.append('    <li><a href={}>{}</a></li>'.format(
-                urlpathjoin(digest, dir_index), escape(index.name)
+                urlpathjoin(digest, dir_index), escape(index.name),
             ))
         tag_index.extend(['</ul>', ''])
         with open_text(tag_index_dir, dir_index) as f:
             f.write('\n'.join(tag_index))
 
 
 class TumblrBackup:
-    def __init__(self, options: Namespace, orig_options: Dict[str, Any], get_arg_default: Callable[[str], Any]):
+    def __init__(self, options: Namespace, orig_options: dict[str, Any], get_arg_default: Callable[[str], Any]):
         self.options = options
         self.orig_options = orig_options
         self.get_arg_default = get_arg_default
-        self.failed_blogs: List[str] = []
-        self.postfail_blogs: List[str] = []
+        self.failed_blogs: list[str] = []
+        self.postfail_blogs: list[str] = []
         self.total_count = 0
         self.post_count = 0
         self.filter_skipped = 0
-        self.title: Optional[str] = None
-        self.subtitle: Optional[str] = None
-        self.pa_options: Optional[JSONDict] = None
-        self.media_list_file: Optional[TextIO] = None
-        self.mlf_seen: Set[int] = set()
+        self.title: str | None = None
+        self.subtitle: str | None = None
+        self.pa_options: JSONDict | None = None
+        self.media_list_file: TextIO | None = None
+        self.mlf_seen: set[int] = set()
         self.mlf_lock = threading.Lock()
 
     def exit_code(self):
         if self.failed_blogs or self.postfail_blogs:
             return EXIT_ERRORS
         if self.total_count == 0 and not self.options.json_info:
             return EXIT_NOPOSTS
         return EXIT_SUCCESS
 
     def header(self, title='', body_class='', subtitle='', avatar=False):
         root_rel = {
-            'index': '', 'tag-index': '..', 'tag-archive': '../..'
+            'index': '', 'tag-index': '..', 'tag-archive': '../..',
         }.get(body_class, save_dir)
         css_rel = urlpathjoin(root_rel, custom_css if have_custom_css else backup_css)
         if body_class:
             body_class = ' class=' + body_class
-        h = '''<!DOCTYPE html>
+        h = textwrap.dedent("""\
+            <!DOCTYPE html>
 
-<meta charset=%s>
-<title>%s</title>
-<link rel=stylesheet href=%s>
+            <meta charset=%s>
+            <title>%s</title>
+            <link rel=stylesheet href=%s>
 
-<body%s>
+            <body%s>
 
-<header>
-''' % (FILE_ENCODING, self.title, css_rel, body_class)
+            <header>
+            """ % (FILE_ENCODING, self.title, css_rel, body_class),
+        )
         if avatar:
             avatar_matches = find_files(path_to(theme_dir), match_avatar)
             avatar_path = next(avatar_matches, None)
             if avatar_path is not None:
                 h += '<img src={} alt=Avatar>\n'.format(urlpathjoin(root_rel, theme_dir, split(avatar_path)[1]))
         if title:
             h += '<h1>%s</h1>\n' % title
@@ -1003,19 +1000,19 @@
             f += '| <a href={} rel=prev>Previous</a>\n'.format(urlpathjoin(base, previous_page))
         if next_page:
             f += '| <a href={} rel=next>Next</a>\n'.format(urlpathjoin(base, next_page))
         f += '</nav></footer>\n'
         return f
 
     @staticmethod
-    def get_post_timestamp(post, BeautifulSoup_):
+    def get_post_timestamp(post, bs4_class):
         if TYPE_CHECKING:
             from bs4 import BeautifulSoup
         else:
-            BeautifulSoup = BeautifulSoup_
+            BeautifulSoup = bs4_class
 
         with open(post, encoding=FILE_ENCODING) as pf:
             soup = BeautifulSoup(pf, 'lxml')
         postdate = cast(Tag, soup.find('time'))['datetime']
         # datetime.fromisoformat does not understand 'Z' suffix
         return int(datetime.strptime(cast(str, postdate), '%Y-%m-%dT%H:%M:%SZ').timestamp())
 
@@ -1025,16 +1022,16 @@
             with open(path_to('.first_run_options'), encoding=FILE_ENCODING) as f:
                 first_run_options = json.load(f)
         except FileNotFoundError:
             first_run_options = None
 
         @dataclass(frozen=True)
         class Options:
-            fro: Dict[str, Any]
-            orig: Dict[str, Any]
+            fro: dict[str, Any]
+            orig: dict[str, Any]
             def differs(self, opt): return opt not in self.fro or self.orig[opt] != self.fro[opt]
             def first(self, opts): return {opt: self.fro.get(opt, '<not present>') for opt in opts}
             def this(self, opts): return {opt: self.orig[opt] for opt in opts}
 
         # These options must always match
         backdiff_nondef = None
         if first_run_options is not None:
@@ -1124,15 +1121,15 @@
             # Fallback assumptions
             logger.warn('Warning: Unknown media path options for previous archive, assuming they match ours\n',
                         account=True)
             pa_options = {opt: getattr(self.options, opt) for opt in MEDIA_PATH_OPTIONS}
 
         return oldest_tstamp, pa_options, write_fro
 
-    def record_media(self, ident: int, urls: Set[str]) -> None:
+    def record_media(self, ident: int, urls: set[str]) -> None:
         with self.mlf_lock:
             if self.media_list_file is not None and ident not in self.mlf_seen:
                 json.dump(dict(post=ident, media=sorted(urls)), self.media_list_file, separators=(',', ':'))
                 self.media_list_file.write('\n')
                 self.mlf_seen.add(ident)
 
     def backup(self, account, prev_archive):
@@ -1144,15 +1141,15 @@
         global save_folder, media_folder, post_ext, post_dir, save_dir, have_custom_css
         if self.options.json_info:
             pass  # Not going to save anything
         elif self.options.blosxom:
             save_folder = root_folder
             post_ext = '.txt'
             post_dir = os.curdir
-            post_class: Type[TumblrPost] = BlosxomPost
+            post_class: type[TumblrPost] = BlosxomPost
         else:
             save_folder = join(root_folder, self.options.outdir or account)
             media_folder = path_to(media_dir)
             if self.options.dirs:
                 post_ext = ''
                 save_dir = '../..'
             post_class = TumblrPost
@@ -1243,15 +1240,15 @@
                 reverse_index=self.options.reverse_index, tag_index=self.options.tag_index,
             )
             ix.build_index()
             ix.save_index()
 
             if not (account in self.failed_blogs or os.path.exists(path_to('.complete'))):
                 # Make .complete file
-                sf: Optional[int]
+                sf: int | None
                 if os.name == 'posix':  # Opening directories and fdatasync are POSIX features
                     sf = opendir(save_folder, os.O_RDONLY)
                 else:
                     sf = None
                 try:
                     if sf is not None:
                         fdatasync(sf)
@@ -1344,20 +1341,20 @@
                 if self.options.count and self.post_count >= self.options.count:
                     logger.info('Stopping backup: Reached limit of {} posts\n'.format(self.options.count), account=True)
                     return False, oldest_date
             return True, oldest_date
 
         api_thread = AsyncCallable(main_thread_lock, api_parser.apiparse, 'API Thread')
 
-        next_ident: Optional[int] = None
+        next_ident: int | None = None
         if self.options.idents is not None:
             remaining_idents = self.options.idents.copy()
             count_estimate = len(remaining_idents)
 
-        mlf: Optional[ContextManager[TextIO]]
+        mlf: ContextManager[TextIO] | None
         if self.options.media_list:
             mlf = open_text('media.json', mode='r+')
             self.media_list_file = mlf.__enter__()
             self.mlf_seen.clear()
             for line in self.media_list_file:
                 doc = json.loads(line)
                 self.mlf_seen.add(doc['post'])
@@ -1456,25 +1453,25 @@
     post_header = ''  # set by TumblrBackup.backup()
 
     def __init__(
         self,
         post: JSONDict,
         options: Namespace,
         backup_account: str,
-        prev_archive: Optional[str],
-        pa_options: Optional[JSONDict],
-        record_media: Callable[[int, Set[str]], None],
+        prev_archive: str | None,
+        pa_options: JSONDict | None,
+        record_media: Callable[[int, set[str]], None],
     ) -> None:
         self.post = post
         self.options = options
         self.backup_account = backup_account
         self.prev_archive = prev_archive
         self.pa_options = pa_options
         self.record_media = record_media
-        self.post_media: Set[str] = set()
+        self.post_media: set[str] = set()
         self.creator = post.get('blog_name') or post['tumblelog']
         self.ident = str(post['id'])
         self.url = post['post_url']
         self.shorturl = post['short_url']
         self.typ = str(post['type'])
         self.date: float = post['liked_timestamp' if options.likes else 'timestamp']
         self.isodate = datetime.utcfromtimestamp(self.date).isoformat() + 'Z'
@@ -1501,33 +1498,30 @@
         post = self.post
         content = []
         self.post_media.clear()
 
         def append(s, fmt='%s'):
             content.append(fmt % s)
 
-        def get_try(elt) -> Union[Any, Literal['']]:
+        def get_try(elt) -> Any | Literal['']:
             return post.get(elt, '')
 
         def append_try(elt, fmt='%s'):
             elt = get_try(elt)
             if elt:
                 if self.options.save_images:
-                    elt = re.sub(r'''(?i)(<img\s(?:[^>]*\s)?src\s*=\s*["'])(.*?)(["'][^>]*>)''',
-                        self.get_inline_image, elt
-                    )
+                    elt = re.sub(r"""(?i)(<img\s(?:[^>]*\s)?src\s*=\s*["'])(.*?)(["'][^>]*>)""",
+                                 self.get_inline_image, elt)
                 if self.options.save_video or self.options.save_video_tumblr:
                     # Handle video element poster attribute
-                    elt = re.sub(r'''(?i)(<video\s(?:[^>]*\s)?poster\s*=\s*["'])(.*?)(["'][^>]*>)''',
-                        self.get_inline_video_poster, elt
-                    )
+                    elt = re.sub(r"""(?i)(<video\s(?:[^>]*\s)?poster\s*=\s*["'])(.*?)(["'][^>]*>)""",
+                                 self.get_inline_video_poster, elt)
                     # Handle video element's source sub-element's src attribute
-                    elt = re.sub(r'''(?i)(<source\s(?:[^>]*\s)?src\s*=\s*["'])(.*?)(["'][^>]*>)''',
-                        self.get_inline_video, elt
-                    )
+                    elt = re.sub(r"""(?i)(<source\s(?:[^>]*\s)?src\s*=\s*["'])(.*?)(["'][^>]*>)""",
+                                 self.get_inline_video, elt)
                 append(elt, fmt)
 
         if self.typ == 'text':
             self.title = get_try('title')
             append_try('body')
 
         elif self.typ == 'photo':
@@ -1553,38 +1547,41 @@
 
         elif self.typ == 'quote':
             append(post['text'], '<blockquote><p>%s</p></blockquote>')
             append_try('source', '<p>%s</p>')
 
         elif self.typ == 'video':
             src = ''
-            if (self.options.save_video or self.options.save_video_tumblr) \
-                    and post['video_type'] == 'tumblr':
+            if (
+                (self.options.save_video or self.options.save_video_tumblr)
+                and post['video_type'] == 'tumblr'
+            ):
                 src = self.get_media_url(post['video_url'], '.mp4')
             elif self.options.save_video:
                 src = self.get_youtube_url(self.url)
                 if not src:
                     logger.warn('Unable to download video in post #{}\n'.format(self.ident))
             if src:
                 append('<p><video controls><source src="%s" type=video/mp4>%s<br>\n<a href="%s">%s</a></video></p>' % (
-                    src, "Your browser does not support the video element.", src, "Video file"
+                    src, 'Your browser does not support the video element.', src, 'Video file',
                 ))
             else:
                 player = get_try('player')
                 if player:
                     append(player[-1]['embed_code'])
                 else:
                     append_try('video_url')
             append_try('caption')
 
         elif self.typ == 'audio':
-            def make_player(src_):
-                append('<p><audio controls><source src="{src}" type=audio/mpeg>{}<br>\n<a href="{src}">{}'
-                       '</a></audio></p>'
-                       .format('Your browser does not support the audio element.', 'Audio file', src=src_))
+            def make_player(src):
+                append(textwrap.dedent(
+                    f'<p><audio controls><source src="{src}" type=audio/mpeg>'
+                    f'Your browser does not support the audio element.<br>\n<a href="{src}">Audio file</a></audio></p>',
+                ))
 
             src = None
             audio_url = get_try('audio_url') or get_try('audio_source_url')
             if self.options.save_audio:
                 if post['audio_type'] == 'tumblr':
                     if audio_url.startswith('https://a.tumblr.com/'):
                         src = self.get_media_url(audio_url, '.mp3')
@@ -1606,28 +1603,28 @@
             self.title = post['question']
             append_try('answer')
 
         elif self.typ == 'chat':
             self.title = get_try('title')
             append(
                 '<br>\n'.join('%(label)s %(phrase)s' % d for d in post['dialogue']),
-                '<p>%s</p>'
+                '<p>%s</p>',
             )
 
         else:
             logger.warn("Unknown post type '{}' in post #{}\n".format(self.typ, self.ident))
             append(escape(self.get_json_content()), '<pre>%s</pre>')
 
         # Write URLs to media.json
         self.record_media(int(self.ident), self.post_media)
 
         content_str = '\n'.join(content)
 
         # fix wrongly nested HTML elements
-        for p in ('<p>(<({})>)', '(</({})>)</p>'):
+        for p in ('<p>(<({})>)', '(</({})>)</p>'):  # noqa: P103
             content_str = re.sub(p.format('p|ol|iframe[^>]*'), r'\1', content_str)
 
         return content_str
 
     def get_youtube_url(self, youtube_url):
         # determine the media file name
         filetmpl = '%(id)s_%(uploader_id)s_%(title)s.%(ext)s'
@@ -1682,46 +1679,43 @@
             if self.options.exif and saved_name.endswith('.jpg'):
                 add_exif(join(self.media_folder, saved_name), set(self.tags), self.options.exif)
             return urlpathjoin(self.media_url, saved_name)
         return image_url
 
     @staticmethod
     def maxsize_image_url(image_url):
-        if ".tumblr.com/" not in image_url or image_url.endswith('.gif'):
+        if '.tumblr.com/' not in image_url or image_url.endswith('.gif'):
             return image_url
         # change the image resolution to 1280
         return re.sub(r'_\d{2,4}(\.\w+)$', r'_1280\1', image_url)
 
     def get_inline_image(self, match):
         """Saves an inline image if not saved yet. Returns the new <img> tag or
         the original one in case of download errors."""
         image_url, image_filename = self._parse_url_match(match, transform=self.maxsize_image_url)
         if not image_filename or not image_url.startswith('http'):
             return match.group(0)
         saved_name = self.download_media(image_url, filename=image_filename)
         if saved_name is None:
             return match.group(0)
-        return '%s%s/%s%s' % (match.group(1), self.media_url,
-            saved_name, match.group(3)
-        )
+        return match.group(1) + self.media_url + '/' + saved_name + match.group(3)
 
     def get_inline_video_poster(self, match):
         """Saves an inline video poster if not saved yet. Returns the new
         <video> tag or the original one in case of download errors."""
         poster_url, poster_filename = self._parse_url_match(match)
         if not poster_filename or not poster_url.startswith('http'):
             return match.group(0)
         saved_name = self.download_media(poster_url, filename=poster_filename)
         if saved_name is None:
             return match.group(0)
         # get rid of autoplay and muted attributes to align with normal video
         # download behaviour
-        return ('%s%s/%s%s' % (match.group(1), self.media_url,
-            saved_name, match.group(3)
-        )).replace('autoplay="autoplay"', '').replace('muted="muted"', '')
+        el = '%s%s/%s%s' % (match.group(1), self.media_url, saved_name, match.group(3))
+        return el.replace('autoplay="autoplay"', '').replace('muted="muted"', '')
 
     def get_inline_video(self, match):
         """Saves an inline video if not saved yet. Returns the new <video> tag
         or the original one in case of download errors."""
         video_url, video_filename = self._parse_url_match(match)
         if not video_filename or not video_url.startswith('http'):
             return match.group(0)
@@ -1759,29 +1753,28 @@
         if parsed_url.scheme not in ('http', 'https') or not hostname:
             return None  # This URL does not follow our basic assumptions
 
         # Make a sane directory to represent the host
         try:
             hostname = hostname.encode('idna').decode('ascii')
         except UnicodeError:
-            hostname = hostname
+            pass
         if hostname in ('.', '..'):
             hostname = hostname.replace('.', '%2E')
         if parsed_url.port not in (None, (80 if parsed_url.scheme == 'http' else 443)):
             hostname += '{}{}'.format('+' if os.name == 'nt' else ':', parsed_url.port)
 
         def get_path(media_dir, image_names, hostdirs):
             if filename is not None:
                 fname = filename
             else:
                 fname = self.get_filename(parsed_url, image_names, offset)
                 if extension is not None:
                     fname = splitext(fname)[0] + extension
-            parts = (media_dir,) + ((hostname,) if hostdirs else ()) + (fname,)
-            return parts
+            return media_dir, *((hostname,) if hostdirs else ()), fname
 
         path_parts = get_path(self.media_dir, self.options.image_names, self.options.hostdirs)
         media_path = path_to(*path_parts)
 
         # prevent racing of existence check and download
         with downloading_media_cond:
             while media_path in downloading_media:
@@ -1791,49 +1784,14 @@
         try:
             return self._download_media_inner(url, get_path, path_parts, media_path)
         finally:
             with downloading_media_cond:
                 downloading_media.remove(media_path)
                 downloading_media_cond.notify_all()
 
-    def _download_media_inner(self, url, get_path, path_parts, media_path):
-        self.post_media.add(url)
-
-        if self.prev_archive is None:
-            cpy_res = False
-        else:
-            assert self.pa_options is not None
-            pa_path_parts = get_path(
-                join(post_dir, self.ident) if self.pa_options['dirs'] else media_dir,
-                self.pa_options['image_names'], self.pa_options['hostdirs'],
-            )
-            cpy_res = maybe_copy_media(self.prev_archive, path_parts, pa_path_parts)
-        file_exists = os.path.exists(media_path)
-        if not (cpy_res or file_exists):
-            if self.options.no_get:
-                return None
-            # We don't have the media and we want it
-            assert wget_retrieve is not None
-            dstpath = open_file(lambda f: f, path_parts)
-            try:
-                wget_retrieve(url, dstpath, post_id=self.ident, post_timestamp=self.post['timestamp'])
-            except WGError as e:
-                e.log()
-                return None
-        if file_exists:
-            try:
-                st = os.stat(media_path)
-            except FileNotFoundError:
-                pass  # skip
-            else:
-                if st.st_mtime > self.post['timestamp']:
-                    touch(media_path, self.post['timestamp'])
-
-        return path_parts[-1]
-
     def get_post(self):
         """returns this post in HTML"""
         typ = ('liked-' if self.options.likes else '') + self.typ
         post = self.post_header + '<article class=%s id=p-%s>\n' % (typ, self.ident)
         post += '<header>\n'
         if self.options.likes:
             post += '<p><a href=\"https://{0}.tumblr.com/\" class=\"tumblr_blog\">{0}</a>:</p>\n'.format(self.creator)
@@ -1849,17 +1807,15 @@
         if self.title:
             post += '<h2>%s</h2>\n' % self.title
         post += content
         foot = []
         if self.tags:
             foot.append(''.join(self.tag_link(t) for t in self.tags))
         if self.source_title and self.source_url:
-            foot.append('<a title=Source href=%s>%s</a>' %
-                (self.source_url, self.source_title)
-            )
+            foot.append(f'<a title=Source href={self.source_url}>{self.source_title}</a>')
 
         notes_html = ''
 
         if self.options.save_notes or self.options.copy_notes:
             if TYPE_CHECKING:
                 from bs4 import BeautifulSoup
             else:
@@ -1881,15 +1837,15 @@
 
         if self.options.save_notes and self.backup_account not in disable_note_scraper and not notes_html.strip():
             from . import note_scraper
 
             # Scrape and save notes
             while True:
                 ns_stdout_rd, ns_stdout_wr = multiprocessing.Pipe(duplex=False)
-                ns_msg_queue: SimpleQueue[Tuple[LogLevel, str]] = multiprocessing.SimpleQueue()
+                ns_msg_queue: SimpleQueue[tuple[LogLevel, str]] = multiprocessing.SimpleQueue()
                 try:
                     args = (
                         ns_stdout_wr, ns_msg_queue, self.url, self.ident, self.options.no_ssl_verify,
                         self.options.user_agent, self.options.cookiefile, self.options.notes_limit,
                         self.options.use_dns_check,
                     )
                     process = multiprocessing.Process(target=note_scraper.main, args=args)
@@ -1924,17 +1880,17 @@
                 if process.exitcode == 2:  # EXIT_SAFE_MODE
                     # Safe mode is blocking us, disable note scraping for this blog
                     notes_html = ''
                     with disablens_lock:
                         # Check if another thread already set this
                         if self.backup_account not in disable_note_scraper:
                             disable_note_scraper.add(self.backup_account)
-                            logger.info('[Note Scraper] Blocked by safe mode - scraping disabled for {}\n'.format(
-                                self.backup_account
-                            ))
+                            logger.info(
+                                f'[Note Scraper] Blocked by safe mode - scraping disabled for {self.backup_account}\n',
+                            )
                 elif process.exitcode == 3:  # EXIT_NO_INTERNET
                     no_internet.signal()
                     continue
                 break
 
         notes_str = '{} note{}'.format(self.note_count, 's'[self.note_count == 1:])
         if notes_html.strip():
@@ -1975,14 +1931,49 @@
             logger.error('Caught exception while saving post {}:\n{}'.format(self.ident, traceback.format_exc()))
             return False
         return True
 
     def get_json_content(self):
         return json.dumps(self.post, sort_keys=True, indent=4, separators=(',', ': '))
 
+    def _download_media_inner(self, url, get_path, path_parts, media_path):
+        self.post_media.add(url)
+
+        if self.prev_archive is None:
+            cpy_res = False
+        else:
+            assert self.pa_options is not None
+            pa_path_parts = get_path(
+                join(post_dir, self.ident) if self.pa_options['dirs'] else media_dir,
+                self.pa_options['image_names'], self.pa_options['hostdirs'],
+            )
+            cpy_res = maybe_copy_media(self.prev_archive, path_parts, pa_path_parts)
+        file_exists = os.path.exists(media_path)
+        if not (cpy_res or file_exists):
+            if self.options.no_get:
+                return None
+            # We don't have the media and we want it
+            assert wget_retrieve is not None
+            dstpath = open_file(lambda f: f, path_parts)
+            try:
+                wget_retrieve(url, dstpath, post_id=self.ident, post_timestamp=self.post['timestamp'])
+            except WGError as e:
+                e.log()
+                return None
+        if file_exists:
+            try:
+                st = os.stat(media_path)
+            except FileNotFoundError:
+                pass  # skip
+            else:
+                if st.st_mtime > self.post['timestamp']:
+                    touch(media_path, self.post['timestamp'])
+
+        return path_parts[-1]
+
     @staticmethod
     def _parse_url_match(match, transform=None):
         url = match.group(2)
         if url.startswith('//'):
             url = 'https:' + url
         if transform is not None:
             url = transform(url)
@@ -2006,15 +1997,15 @@
 class LocalPost:
     def __init__(self, post_file: str, tag_index: bool):
         self.post_file = post_file
         if tag_index:
             with open(post_file, encoding=FILE_ENCODING) as f:
                 post = f.read()
             # extract all URL-encoded tags
-            self.tags: List[Tuple[str, str]] = []
+            self.tags: list[tuple[str, str]] = []
             footer_pos = post.find('<footer>')
             if footer_pos > 0:
                 self.tags = re.findall(r'<a.+?/tagged/(.+?)>#(.+?)</a>', post[footer_pos:])
         parts = post_file.split(os.sep)
         if parts[-1] == dir_index:  # .../<post_id>/index.html
             self.file_name = join(*parts[-2:])
             self.ident = parts[-2]
@@ -2188,15 +2179,16 @@
         def __call__(self, parser, namespace, values, option_string=None):
             request = getattr(namespace, self.dest) or {}
             for req in values.lower().split(','):
                 parts = req.strip().split(':')
                 typ = parts.pop(0)
                 if typ != TYPE_ANY and typ not in POST_TYPES:
                     parser.error("{}: invalid post type '{}'".format(option_string, typ))
-                for typ in POST_TYPES if typ == TYPE_ANY else (typ,):
+                types = POST_TYPES if typ == TYPE_ANY else (typ,)
+                for typ in types:
                     if not parts:
                         request[typ] = [TAG_ANY]
                         continue
                     if typ not in request:
                         request[typ] = []
                     request[typ].extend(parts)
             setattr(namespace, self.dest, request)
@@ -2224,17 +2216,17 @@
                 period = time.strftime(pformat)
                 prange = parse_period_date(period)
             setattr(namespace, self.dest, prange)
 
     class IdFileCallback(argparse.Action):
         def __call__(self, parser, namespace, values, option_string=None):
             with open(values) as f:
+                lines = (l.rstrip('\n') for l in f)
                 setattr(namespace, self.dest, sorted(
-                    map(int, (line for line in map(lambda l: l.rstrip('\n'), f) if line)),
-                    reverse=True,
+                    (int(line) for line in lines if line), reverse=True,
                 ))
 
     parser = argparse.ArgumentParser(usage='%(prog)s [options] blog-name ...',
                                      description='Makes a local backup of Tumblr blogs.')
     postexist_group = parser.add_mutually_exclusive_group()
     reblog_group = parser.add_mutually_exclusive_group()
     parser.add_argument('-O', '--outdir', help='set the output directory (default: blog-name)')
@@ -2266,23 +2258,21 @@
     parser.add_argument('-n', '--count', type=int, help='save only COUNT posts')
     parser.add_argument('-s', '--skip', type=int, default=0, help='skip the first SKIP posts')
     parser.add_argument('-p', '--period', action=PeriodCallback,
                         help="limit the backup to PERIOD ('y', 'm', 'd', YYYY[MM[DD]][Z], or START,END)")
     parser.add_argument('-N', '--posts-per-page', type=int, default=50, metavar='COUNT',
                         help='set the number of posts per monthly page, 0 for unlimited')
     parser.add_argument('-Q', '--request', action=RequestCallback,
-                        help='save posts matching the request TYPE:TAG:TAG:…,TYPE:TAG:…,…. '
-                             'TYPE can be {} or {any}; TAGs can be omitted or a colon-separated list. '
-                             'Example: -Q {any}:personal,quote,photo:me:self'
-                             .format(', '.join(POST_TYPES), any=TYPE_ANY))
+                        help=f'save posts matching the request TYPE:TAG:TAG:…,TYPE:TAG:…,…. '
+                             f'TYPE can be {", ".join(POST_TYPES)} or {TYPE_ANY}; TAGs can be omitted or a '
+                             f'colon-separated list. Example: -Q {TYPE_ANY}:personal,quote,photo:me:self')
     parser.add_argument('-t', '--tags', action=TagsCallback, dest='request',
                         help='save only posts tagged TAGS (comma-separated values; case-insensitive)')
     parser.add_argument('-T', '--type', action=RequestCallback, dest='request',
-                        help='save only posts of type TYPE (comma-separated values from {})'
-                             .format(', '.join(POST_TYPES)))
+                        help=f'save only posts of type TYPE (comma-separated values from {", ".join(POST_TYPES)})')
     parser.add_argument('-F', '--filter', help='save posts matching a jq filter (needs jq module)')
     reblog_group.add_argument('--no-reblog', action='store_true', help="don't save reblogged posts")
     reblog_group.add_argument('--only-reblog', action='store_true', help='save only reblogged posts')
     parser.add_argument('-I', '--image-names', choices=('o', 'i', 'bi'), default='o', metavar='FMT',
                         help="image filename format ('o'=original, 'i'=<post-id>, 'bi'=<blog-name>_<post-id>)")
     parser.add_argument('-e', '--exif', action=CSVCallback, default=[], metavar='KW',
                         help='add EXIF keyword tags to each picture'
@@ -2334,17 +2324,17 @@
     if options.count == 0 and (options.incremental or options.auto is not None):
         parser.error('--count 0 conflicts with --incremental and --auto')
     if options.skip < 0:
         parser.error('--skip: skip must not be negative')
     if options.posts_per_page < 0:
         parser.error('--posts-per-page: posts per page must not be negative')
     if options.outdir and len(blogs) > 1:
-        parser.error("-O can only be used for a single blog-name")
+        parser.error('-O can only be used for a single blog-name')
     if options.dirs and options.tag_index:
-        parser.error("-D cannot be used with --tag-index")
+        parser.error('-D cannot be used with --tag-index')
     if options.cookiefile is not None and not os.access(options.cookiefile, os.R_OK):
         parser.error('--cookiefile: file cannot be read')
     if options.notes_limit is not None:
         if not options.save_notes:
             parser.error('--notes-limit requires --save-notes')
         if options.notes_limit < 1:
             parser.error('--notes-limit: Value must be at least 1')
@@ -2381,21 +2371,20 @@
 
     check_optional_modules(options)
 
     try:
         with open(config_file) as f:
             api_key = json.load(f)['oauth_consumer_key']
     except (FileNotFoundError, KeyError):
-        print(f"""\
-API key not set. To use tumblr-backup:
-1. Go to https://www.tumblr.com/oauth/apps and create an app if you don't have one already.
-2. Copy the "OAuth Consumer Key" from the app you created.
-3. Run `{Path(sys.argv[0]).name} --set-api-key API_KEY`, where API_KEY is the key that you just copied.""",
-            file=sys.stderr,
-        )
+        msg = f"""\
+            API key not set. To use tumblr-backup:
+            1. Go to https://www.tumblr.com/oauth/apps and create an app if you don't have one already.
+            2. Copy the "OAuth Consumer Key" from the app you created.
+            3. Run `{Path(sys.argv[0]).name} --set-api-key API_KEY`, where API_KEY is the key that you just copied."""
+        print(textwrap.dedent(msg), file=sys.stderr)
         return 1
 
     wget_retrieve = WgetRetrieveWrapper(logger.log, options)
     setup_wget(not options.no_ssl_verify, options.user_agent)
 
     ApiParser.setup(api_key, options.no_ssl_verify, options.user_agent, options.cookiefile)
     tb = TumblrBackup(options, orig_options, parser.get_default)
```

### Comparing `tumblr-backup-1.0.2.post1/tumblr_backup/note_scraper.py` & `tumblr_backup-1.0.3/tumblr_backup/note_scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from __future__ import annotations
+
 import re
 import sys
 import time
 import traceback
 import warnings
 from datetime import datetime
 from multiprocessing.queues import SimpleQueue
-from typing import List, Optional, Tuple, cast
+from typing import cast
 from urllib.parse import parse_qs, quote, urlencode, urljoin, urlparse, urlsplit, urlunsplit
 
 import requests
 from bs4 import BeautifulSoup, Tag
 from requests.exceptions import RequestException
 from urllib3 import Retry, Timeout
 from urllib3.exceptions import HTTPError, InsecureRequestWarning
@@ -26,15 +28,15 @@
 # Always retry on 503 or 504, but never on connect or 429, the latter handled specially
 HTTP_RETRY = Retry(3, connect=False, status_forcelist=frozenset((503, 504)))
 HTTP_RETRY.RETRY_AFTER_STATUS_CODES = frozenset((413,))  # type: ignore[misc]
 
 # Globals
 post_url = None
 ident = None
-msg_queue: Optional[SimpleQueue[Tuple[int, str]]] = None
+msg_queue: SimpleQueue[tuple[int, str]] | None = None
 
 
 def log(level, url, msg):
     assert msg_queue is not None
     url_msg = ", URL '{}'".format(url) if url != post_url else ''
     # see https://github.com/google/pytype/issues/1344#issuecomment-1553500779
     msg_queue.put(  # pytype: disable=attribute-error
@@ -124,19 +126,21 @@
         uri = self.iri_to_uri(iri)
 
         try_count = 0
         while True:
             with self.session.get(uri) as resp:
                 try_count += 1
                 parsed_uri = urlparse(resp.url)
-                if (re.match(r'(www\.)?tumblr\.com', parsed_uri.netloc)
+                if (
+                    re.match(r'(www\.)?tumblr\.com', parsed_uri.netloc)
                     and re.match(r'/safe-mode$|/[a-z0-9-]+/[0-9]+(/|$)', parsed_uri.path)
                 ):
                     sys.exit(EXIT_SAFE_MODE)
-                if (resp.status_code in (420, 429) and try_count < self.TRY_LIMIT
+                if (
+                    resp.status_code in (420, 429) and try_count < self.TRY_LIMIT
                     and self.ratelimit_sleep(resp.status_code, resp.headers)
                 ):
                     continue
                 if 200 <= resp.status_code < 300:
                     return resp.content.decode('utf-8', errors='ignore')
                 log(LogLevel.WARN, iri, 'Unexpected response status: HTTP {} {}{}'.format(
                     resp.status_code, resp.reason,
@@ -185,15 +189,15 @@
         return True
 
     def get_notes(self, post_url):
         parsed_uri = urlparse(post_url)
         base = '{uri.scheme}://{uri.netloc}'.format(uri=parsed_uri)
 
         notes_10k = 0
-        notes_list: List[str] = []
+        notes_list: list[str] = []
 
         notes_url = post_url
         while True:
             resp_str = self.urlopen(notes_url)
             if resp_str is None:
                 break
```

### Comparing `tumblr-backup-1.0.2.post1/tumblr_backup/util.py` & `tumblr_backup-1.0.3/tumblr_backup/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-import collections
+from __future__ import annotations
+
 import errno
 import os
 import queue
 import shutil
 import socket
 import sys
 import threading
 import time
 import warnings
+from abc import ABC, abstractmethod
+from collections import deque
 from enum import Enum
 from functools import total_ordering
 from http.cookiejar import MozillaCookieJar
 from importlib.machinery import PathFinder
-from typing import TYPE_CHECKING, Any, Deque, Dict, Generic, Optional, Tuple, TypeVar
+from typing import TYPE_CHECKING, Any, Deque, Generic, TypeVar
 
 from urllib3.exceptions import DependencyWarning
 
 if sys.platform == 'darwin':
     import fcntl
 
 if TYPE_CHECKING:
     import requests
+    from typing_extensions import TypeAlias
     swt_base = requests.Session
 
 
 def to_bytes(string, encoding='utf-8', errors='strict'):
     if isinstance(string, bytes):
         return string
     return string.encode(encoding, errors)
@@ -88,18 +92,18 @@
             sock.recvfrom(1)
     except OSError:
         return False
 
     return True
 
 
-class WaitOnMainThread:
+class WaitOnMainThread(ABC):
     def __init__(self):
-        self.cond: Optional[threading.Condition] = None
-        self.flag: Optional[bool] = False
+        self.cond: threading.Condition | None = None
+        self.flag: bool | None = False
 
     def setup(self, lock=None):
         self.cond = threading.Condition(lock)
 
     def signal(self):
         assert self.cond is not None
         if isinstance(threading.current_thread(), threading._MainThread):  # type: ignore[attr-defined]
@@ -153,14 +157,15 @@
         except:
             with self.cond:
                 self.flag = None  # Waiting never completed
                 self.cond.notify_all()
             raise
 
     @staticmethod
+    @abstractmethod
     def _wait():
         raise NotImplementedError
 
 
 class NoInternet(WaitOnMainThread):
     @staticmethod
     def _wait():
@@ -211,28 +216,28 @@
         else:
             securetransport.inject_into_urllib3()
             have_sni = True  # SNI always works
 
     # Inject PyOpenSSL if the linked OpenSSL has no SNI
     if not have_sni:
         try:
-            # TODO: remove attr-defined ignore once we support urllib3 2.x
-            from urllib3.contrib import pyopenssl  # type: ignore[attr-defined,no-redef]
+            from urllib3.contrib import pyopenssl
             pyopenssl.inject_into_urllib3()
         except ImportError as e:
             print('Warning: Failed to inject pyOpenSSL: {!r}'.format(e), file=sys.stderr)
         else:
             have_sni = True  # SNI always works
 
 
 def make_requests_session(session_type, retry, timeout, verify, user_agent, cookiefile):
     if TYPE_CHECKING:
         global swt_base
     else:
         swt_base = session_type  # type: ignore
+
     class SessionWithTimeout(swt_base):
         def request(self, method, url, *args, **kwargs):
             kwargs.setdefault('timeout', timeout)
             return super().request(method, url, *args, **kwargs)
 
     session = SessionWithTimeout()
     session.verify = verify
@@ -281,20 +286,14 @@
 
 def fdatasync(fd):
     if hasattr(os, 'fdatasync'):
         return os.fdatasync(fd)
     fsync(fd)
 
 
-if TYPE_CHECKING:
-    WaiterSeq = Deque[Any]
-else:
-    WaiterSeq = collections.deque
-
-
 # Minimal implementation of a sum of mutable sequences
 class MultiSeqProxy:
     def __init__(self, subseqs):
         self.subseqs = subseqs
 
     def append(self, value):
         for sub in self.subseqs:
@@ -302,37 +301,37 @@
 
     def remove(self, value):
         for sub in self.subseqs:
             sub.remove((value, self.subseqs))
 
 
 # Hooks into methods used by threading.Condition.notify
-class NotifierWaiters(WaiterSeq):
+class NotifierWaiters(Deque[Any]):
     def __iter__(self):
-        return (value[0] for value in super().__iter__())
+        return (value[0] for value in super(NotifierWaiters, self).__iter__())
 
     def __getitem__(self, index):
         item = super().__getitem__(index)
-        return WaiterSeq(v[0] for v in item) if isinstance(index, slice) else item[0]  # pytype: disable=not-callable
+        return deque(v[0] for v in item) if isinstance(index, slice) else item[0]  # pytype: disable=not-callable
 
     def remove(self, value):
         try:
-            match = next(x for x in super().__iter__() if x[0] == value)
+            match = next(x for x in super(NotifierWaiters, self).__iter__() if x[0] == value)
         except StopIteration:
             raise ValueError('deque.remove(x): x not in deque')
         for ref in match[1]:
             try:
                 super(NotifierWaiters, ref).remove(match)  # Remove waiter from known location
             except ValueError:
                 raise RuntimeError('Unexpected missing waiter!')
 
 
 # Supports waiting on multiple threading.Conditions objects simultaneously
 class MultiCondition(threading.Condition):
-    def __init__(self, lock):
+    def __init__(self, lock):  # noqa: WPS612
         super().__init__(lock)
 
     def wait(self, children, timeout=None):  # pytype: disable=signature-mismatch
         assert len(frozenset(id(c) for c in children)) == len(children), 'Children must be unique'
         assert all(c._lock is self._lock for c in children), 'All locks must be the same'  # type: ignore[attr-defined]
 
         # Modify children so their notify methods do cleanup
@@ -347,15 +346,15 @@
 
     def notify(self, n=1):
         raise NotImplementedError
 
     def notify_all(self):
         raise NotImplementedError
 
-    notifyAll = notify_all
+    notifyAll = notify_all  # noqa: N815
 
 
 def lock_is_owned(lock):
     try:
         return lock._is_owned()
     except AttributeError:
         if lock.acquire(0):
@@ -375,19 +374,19 @@
 def lock_acquire_restore(lock, state):
     try:
         lock._acquire_restore(state)  # pytype: disable=attribute-error
     except AttributeError:
         lock.acquire()  # Ignore saved state
 
 
-ACParams = Tuple[Tuple[Any, ...], Dict[str, Any]]  # (args, kwargs)
+ACParams: TypeAlias = 'tuple[tuple[Any, ...], dict[str, Any]]'  # (args, kwargs)
 
 
 class AsyncCallable:
-    request: LockedQueue[Optional[ACParams]]
+    request: LockedQueue[ACParams | None]
     response: LockedQueue[Any]
 
     def __init__(self, lock, fun, name=None):
         self.lock = lock
         self.fun = fun
         self.request = LockedQueue(lock, maxsize=1)
         self.response = LockedQueue(lock, maxsize=1)
```

### Comparing `tumblr-backup-1.0.2.post1/tumblr_backup/wget.py` & `tumblr_backup-1.0.3/tumblr_backup/wget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
+from __future__ import annotations
+
 import errno
 import functools
 import itertools
 import os
 import time
 import traceback
 import warnings
 from argparse import Namespace
 from collections import OrderedDict
 from email.utils import mktime_tz, parsedate_tz
 from enum import Enum
-from http.client import HTTPConnection as _HTTPConnection
-from http.client import ResponseNotReady
+from http.client import HTTPConnection as _HTTPConnection, ResponseNotReady
 from tempfile import NamedTemporaryFile
 from typing import Any, BinaryIO, Callable, Dict, Optional, Set
 from urllib.parse import urljoin, urlsplit
 
 from urllib3 import (BaseHTTPResponse, HTTPConnectionPool, HTTPHeaderDict, HTTPResponse, HTTPSConnectionPool,
-                     PoolManager)
-from urllib3 import Retry as Retry
-from urllib3 import Timeout, make_headers
-from urllib3.connection import HTTPConnection, HTTPSConnection, _url_from_connection
-from urllib3.exceptions import ConnectTimeoutError, HeaderParsingError
-from urllib3.exceptions import HTTPError as HTTPError
-from urllib3.exceptions import InsecureRequestWarning, MaxRetryError, PoolError
+                     PoolManager, Retry as Retry, Timeout, make_headers)
+from urllib3.connection import HTTPConnection, HTTPSConnection, _url_from_connection  # noqa: WPS450
+from urllib3.exceptions import (ConnectTimeoutError, HeaderParsingError, HTTPError as HTTPError, InsecureRequestWarning,
+                                MaxRetryError, PoolError)
 from urllib3.util.response import assert_header_parsing
 
 from .util import LogLevel, enospc, fsync, is_dns_working, no_internet, opendir, setup_urllib3_ssl, try_unlink
 
 setup_urllib3_ssl()
 
 HTTP_TIMEOUT = Timeout(90)
@@ -86,25 +84,16 @@
             self.part_file = self._make_part_file()
             self._make_part_file = None
 
 
 class WGHTTPResponse(HTTPResponse):
     REDIRECT_STATUSES = [300] + HTTPResponse.REDIRECT_STATUSES
 
-    # Make decoder public for saving and restoring the decoder state
-    @property
-    def decoder(self):
-        return self._decoder  # pytype: disable=attribute-error
-
-    @decoder.setter
-    def decoder(self, value):
-        self._decoder = value
-
     def __init__(
-        self, body="", headers=None, status=0, version=0, reason=None, preload_content=True, decode_content=True,
+        self, body='', headers=None, status=0, version=0, reason=None, preload_content=True, decode_content=True,
         original_response=None, pool=None, connection=None, msg=None, retries=None, enforce_content_length=False,
         request_method=None, request_url=None, auto_close=True,
     ):
         # Copy original Content-Length for _init_length
         if not isinstance(headers, HTTPHeaderDict):
             headers = HTTPHeaderDict(headers)
         if 'Content-Length' not in headers and 'X-Archive-Orig-Content-Length' in headers:
@@ -113,14 +102,23 @@
         self.bytes_to_skip = 0
         self.last_read_length = 0
         super().__init__(
             body, headers, status, version, reason, preload_content, decode_content, original_response, pool,
             connection, msg, retries, enforce_content_length, request_method, request_url, auto_close,
         )
 
+    # Make decoder public for saving and restoring the decoder state
+    @property
+    def decoder(self):
+        return self._decoder  # pytype: disable=attribute-error
+
+    @decoder.setter
+    def decoder(self, value):
+        self._decoder = value
+
     # Make _init_length publicly usable because its implementation is nice
     def get_content_length(self, meth):
         return self._init_length(meth)  # type: ignore[attr-defined]
 
     def _init_decoder(self) -> None:
         self.last_read_length = 0
         super()._init_decoder()
@@ -403,16 +401,18 @@
         hstat.restval = 0
         retry_counter.increment(url, hstat, 'Resume with Range failed, must start over')
         return UErr.RETRINCOMPLETE, doctype
 
     # The Range request was misunderstood. Bail out.
     # Unlike wget, we bail hard with no retry, because this indicates a broken or unreasonable server.
     if contrange not in (0, hstat.restval):
-        raise WGRangeError(logger, url, 'Server provided unexpected Content-Range: Requested {}, got {}'
-                           .format(hstat.restval, contrange))
+        raise WGRangeError(
+            logger, url,
+            f'Server provided unexpected Content-Range: Requested {hstat.restval}, got {contrange}',
+        )
     # HTTP 206 Partial Contents
     if hstat.statcode == 206 and hstat.restval > 0 and contrange == 0:
         if crange_header is None:
             crange_status = 'not provided'
         elif crange_parsed is None:
             crange_status = 'invalid'
         else:  # contrange explicitly zero
@@ -707,15 +707,16 @@
             continue
         except WGUnreachableHostError as e:
             # Set the logger for unreachable host errors thrown from WGHTTP(S)ConnectionPool
             if e.logger is None:
                 e.logger = logger
             raise
         except WGWrongCodeError as e:
-            if (use_internet_archive
+            if (
+                use_internet_archive
                 and not using_internet_archive
                 and hstat.statcode in (403, 404)
                 and urlsplit(orig_url).netloc.endswith('.tumblr.com')  # type: ignore[arg-type]
             ):
                 using_internet_archive = True
                 traceback.clear_frames(e.__traceback__)  # prevent reference cycle
                 ia_fallback_cause = e
@@ -760,23 +761,23 @@
         # NamedTemporaryFile is created 0600, set mode to the usual 0644
         if os.name == 'posix':
             os.fchmod(hstat.part_file.fileno(), 0o644)
         else:
             os.chmod(hstat.part_file.name, 0o644)
 
         if use_server_timestamps and hstat.remote_time is None:
-            logger.warn(url, 'Warning: Last-Modified header is {}'
-                       .format('missing' if hstat.last_modified is None
-                               else 'invalid: {}'.format(hstat.last_modified)))
+            status = 'missing' if hstat.last_modified is None else f'invalid: {hstat.last_modified}'
+            logger.warn(url, f'Warning: Last-Modified header is {status}')
 
         # Flush the userspace buffer so mtime isn't updated
         hstat.part_file.flush()
 
         # Set the timestamp on the local file
-        if (use_server_timestamps
+        if (
+            use_server_timestamps
             and (hstat.remote_time is not None or post_timestamp is not None)
             and hstat.contlen in (None, hstat.bytes_read)
         ):
             if hstat.remote_time is None:
                 tstamp = post_timestamp
             elif post_timestamp is None:
                 tstamp = hstat.remote_time
```

### Comparing `tumblr-backup-1.0.2.post1/tumblr_backup.egg-info/PKG-INFO` & `tumblr_backup-1.0.3/tumblr_backup.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: tumblr-backup
-Version: 1.0.2.post1
+Version: 1.0.3
 Summary: An advanced tool for backing up Tumblr blogs.
 Project-URL: Homepage, https://github.com/cebtenzzre/tumblr-utils
 Project-URL: Bug Reports, https://github.com/cebtenzzre/tumblr-utils/issues
 Project-URL: Source, https://github.com/cebtenzzre/tumblr-utils
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: filetype~=1.2
 Requires-Dist: platformdirs~=4.2
 Requires-Dist: requests~=2.31
 Requires-Dist: urllib3~=2.2
 Provides-Extra: exif
@@ -28,14 +27,25 @@
 Provides-Extra: notes
 Requires-Dist: beautifulsoup4~=4.12; extra == "notes"
 Requires-Dist: lxml~=5.1; extra == "notes"
 Provides-Extra: video
 Requires-Dist: yt_dlp>=2023.12.30; extra == "video"
 Provides-Extra: all
 Requires-Dist: tumblr-backup[exif,jq,notes,video]; extra == "all"
+Provides-Extra: dev
+Requires-Dist: tumblr-backup[all]; extra == "dev"
+Requires-Dist: flake8~=7.0; extra == "dev"
+Requires-Dist: mypy~=1.9; extra == "dev"
+Requires-Dist: pytype>=2024.2.27; extra == "dev"
+Requires-Dist: wemake-python-styleguide~=0.18; extra == "dev"
+Requires-Dist: lxml-stubs~=0.5; extra == "dev"
+Requires-Dist: pysocks~=1.7; extra == "dev"
+Requires-Dist: types-beautifulsoup4~=4.12; extra == "dev"
+Requires-Dist: types-requests~=2.31; extra == "dev"
+Requires-Dist: youtube_dl>=2021.12.17; extra == "dev"
 
 # tumblr-backup
 
 ### About this fork
 
 This is a fork of bbolli's
 [tumblr-utils](https://github.com/bbolli/tumblr-utils), with a focus on
```

