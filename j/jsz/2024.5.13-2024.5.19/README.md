# Comparing `tmp/jsz-2024.5.13.tar.gz` & `tmp/jsz-2024.5.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsz-2024.5.13.tar", last modified: Fri May 10 16:46:22 2024, max compression
+gzip compressed data, was "jsz-2024.5.19.tar", last modified: Sat May 18 20:42:05 2024, max compression
```

## Comparing `jsz-2024.5.13.tar` & `jsz-2024.5.19.tar`

### file list

```diff
@@ -1,16 +1,6 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 16:46:22.878573 jsz-2024.5.13/
--rw-rw-rw-   0        0        0      884 2024-05-10 16:46:22.876560 jsz-2024.5.13/PKG-INFO
--rw-rw-rw-   0        0        0      128 2024-05-09 15:00:28.000000 jsz-2024.5.13/README.md
--rw-rw-rw-   0        0        0      675 2024-05-10 16:45:48.000000 jsz-2024.5.13/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-10 16:46:22.879644 jsz-2024.5.13/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-10 16:46:22.753969 jsz-2024.5.13/src/
-drwxrwxrwx   0        0        0        0 2024-05-10 16:46:22.842126 jsz-2024.5.13/src/jsz/
--rw-rw-rw-   0        0        0      304 2024-04-29 13:27:07.000000 jsz-2024.5.13/src/jsz/__init__.py
--rw-rw-rw-   0        0        0     4366 2024-04-21 16:16:14.000000 jsz-2024.5.13/src/jsz/newpool.py
--rw-rw-rw-   0        0        0    20010 2024-05-10 16:44:49.000000 jsz-2024.5.13/src/jsz/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-10 16:46:22.871239 jsz-2024.5.13/src/jsz.egg-info/
--rw-rw-rw-   0        0        0      884 2024-05-10 16:46:22.000000 jsz-2024.5.13/src/jsz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-05-10 16:46:22.000000 jsz-2024.5.13/src/jsz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 16:46:22.000000 jsz-2024.5.13/src/jsz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2024-05-10 16:46:22.000000 jsz-2024.5.13/src/jsz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-10 16:46:22.000000 jsz-2024.5.13/src/jsz.egg-info/top_level.txt
+-rw-r--r--   0        0        0      128 2024-05-09 15:00:28.691669 jsz-2024.5.19/README.md
+-rw-r--r--   0        0        0      734 2024-05-18 20:42:05.865001 jsz-2024.5.19/pyproject.toml
+-rw-r--r--   0        0        0      304 2024-05-18 20:33:48.507696 jsz-2024.5.19/src/jsz/__init__.py
+-rw-r--r--   0        0        0     4396 2024-05-18 20:33:49.720446 jsz-2024.5.19/src/jsz/newpool.py
+-rw-r--r--   0        0        0    21920 2024-05-18 20:33:50.819403 jsz-2024.5.19/src/jsz/tools.py
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 jsz-2024.5.19/PKG-INFO
```

### Comparing `jsz-2024.5.13/PKG-INFO` & `jsz-2024.5.19/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-Metadata-Version: 2.1
-Name: jsz
-Version: 2024.5.13
-Summary: 金手指
-Author: jiaosenvip
-Author-email: jiaosenvip <jiaosenvip@163.com>
-License: MIT
-Project-URL: Homepage, https://github.com/jiaosenvip/jsz
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-Requires-Dist: beautifulsoup4
-Requires-Dist: lxml
-Requires-Dist: rich
-Requires-Dist: oss2
-Requires-Dist: pymongo
-Requires-Dist: pypdf
-Requires-Dist: html2text
-Requires-Dist: faker
-Requires-Dist: python-dateutil
-Requires-Dist: dateparser; platform_machine != "aarch64"
-Requires-Dist: loguru
-Requires-Dist: grequests
-Requires-Dist: httpx
-Requires-Dist: jsonpath
-Requires-Dist: parsel
-Requires-Dist: ipython
-Requires-Dist: js2py
-Requires-Dist: pandas[excel]
-
-# jsz
-
-## 安装
-
-```sh
-pip install -U jsz
-```
-
-## 使用
-
-```py
-import jsz
-```
-
-## 功能
-
-```py
-dir(jsz)
-```
+Metadata-Version: 2.1
+Name: jsz
+Version: 2024.5.19
+Summary: 金手指
+Author: jiaosenvip
+Author-Email: jiaosenvip <jiaosenvip@163.com>
+License: MIT
+Project-URL: Homepage, https://github.com/jiaosenvip/jsz
+Requires-Python: >=3.11
+Requires-Dist: beautifulsoup4
+Requires-Dist: lxml
+Requires-Dist: rich
+Requires-Dist: oss2
+Requires-Dist: pymongo
+Requires-Dist: pypdf
+Requires-Dist: html2text
+Requires-Dist: faker
+Requires-Dist: python-dateutil
+Requires-Dist: dateparser; platform_machine != "aarch64"
+Requires-Dist: loguru
+Requires-Dist: grequests
+Requires-Dist: httpx
+Requires-Dist: jsonpath
+Requires-Dist: parsel
+Requires-Dist: ipython
+Requires-Dist: js2py
+Requires-Dist: pandas[excel]
+Description-Content-Type: text/markdown
+
+# jsz
+
+## 安装
+
+```sh
+pip install -U jsz
+```
+
+## 使用
+
+```py
+import jsz
+```
+
+## 功能
+
+```py
+dir(jsz)
+```
```

### Comparing `jsz-2024.5.13/pyproject.toml` & `jsz-2024.5.19/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,44 @@
-[project]
-name = "jsz"
-version = "2024.5.13"
-description = "金手指"
-authors = [
-    { name = "jiaosenvip" },
-    { name = "jiaosenvip", email = "jiaosenvip@163.com" },
-]
-dependencies = [
-    "beautifulsoup4",
-    "lxml",
-    "rich",
-    "oss2",
-    "pymongo",
-    "pypdf",
-    "html2text",
-    "faker",
-    "python-dateutil",
-    "dateparser; platform_machine != 'aarch64'",
-    "loguru",
-    "grequests",
-    "httpx",
-    "jsonpath",
-    "parsel",
-    "ipython",
-    "js2py",
-    "pandas[excel]",
-]
-requires-python = ">=3.11"
-readme = "README.md"
-license = { text = "MIT" }
-
-[project.urls]
-Homepage = "https://github.com/jiaosenvip/jsz"
+[build-system]
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
+
+[project]
+name = "jsz"
+version = "2024.5.19"
+description = "金手指"
+authors = [
+    { name = "jiaosenvip" },
+    { name = "jiaosenvip", email = "jiaosenvip@163.com" },
+]
+dependencies = [
+    "beautifulsoup4",
+    "lxml",
+    "rich",
+    "oss2",
+    "pymongo",
+    "pypdf",
+    "html2text",
+    "faker",
+    "python-dateutil",
+    "dateparser; platform_machine != 'aarch64'",
+    "loguru",
+    "grequests",
+    "httpx",
+    "jsonpath",
+    "parsel",
+    "ipython",
+    "js2py",
+    "pandas[excel]",
+]
+requires-python = ">=3.11"
+readme = "README.md"
+
+[project.license]
+text = "MIT"
+
+[project.urls]
+Homepage = "https://github.com/jiaosenvip/jsz"
+
+[tool]
```

### Comparing `jsz-2024.5.13/src/jsz/newpool.py` & `jsz-2024.5.19/src/jsz/newpool.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 from functools import wraps
 import time
 from rich.panel import Panel
 from rich import print
 
 
 class Pool:
+    """
+    线程池
+    """
     def __init__(self, n: int = None):
         """
         线程池
 
         n: 线程数。默认为CPU核心数，可以自定义线程数。
         """
         if n:
```

### Comparing `jsz-2024.5.13/src/jsz/tools.py` & `jsz-2024.5.19/src/jsz/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,88 +1,94 @@
 """
 工具库
 """
 
+import time
+import datetime
 import calendar
 import os
+import platform
 import json
-import httpx
 import random
+import re
+import hashlib
+import base64
 from functools import wraps
 from threading import Timer
-from loguru import logger
 from urllib.parse import (
     urljoin,
     urlparse,
     urlunparse,
     urlencode,
     urlsplit,
     urlunsplit,
     unquote,
     unquote_plus,
     unwrap,
     quote,
     parse_qs,
     parse_qsl,
 )
-from pypdf import PdfReader
+import httpx
+from loguru import logger
 from faker import Faker
-from rich import print, print_json
+from rich import print, print_json, inspect, load_ipython_extension
+from rich.console import Console, Group
 from rich.progress import Progress, track
-from rich.console import Console
+from rich.padding import Padding
 from rich.columns import Columns
 from rich.markdown import Markdown
 from rich.panel import Panel
 from rich.rule import Rule
 from rich.status import Status
 from rich.table import Table
 from rich.pretty import pprint
-import datetime
-import time
-import platform
+from bs4 import BeautifulSoup, element
+import html2text
+from pymongo import MongoClient
+from parsel import Selector
 from dateutil.parser import parse as timeparse
 
 if platform.machine() != "aarch64":
     from dateparser import parse as timeparse2
 else:
     timeparse2 = None
-from bs4 import BeautifulSoup, element
-import re
-import html2text
-import hashlib
-import base64
-from pymongo import MongoClient
-from parsel import Selector
 
 
 __all__ = [
     "base64_decode",
     "base64_encode",
     "bs_get_text",
     "bs_get_text2",
     "bs_html",
+    "console",
     "clear",
     "Columns",
     "connect_to_mongodb",
     "date_next",
     "fake",
     "fromtimestamp",
+    "get_proxies",
+    "Group",
     "hashlib",
     "html2md",
+    "inspect",
     "httpx",
     "listdir",
     "logger",
+    "load_ipython_extension",
     "Markdown",
     "md5",
     "now",
     "os",
     "oss2_find_file",
     "Panel",
     "parse_qs",
     "parse_qsl",
+    "Padding",
     "pdf2text",
     "pprint",
     "print",
     "print_json",
     "print_exception",
     "printx",
     "Progress",
@@ -199,15 +205,14 @@
     "tbody",
     "tfoot",
     "form",
 ]
 
 fake = Faker()
 fake.zh = Faker("zh")
-
 console = Console()
 print_exception = console.print_exception
 
 
 def clear():
     """
     清屏
@@ -497,20 +502,20 @@
     filename=None,
     encoding="utf-8",
     ensure_ascii: bool = False,
     indent: int = None,
     separators: tuple = None,
 ):
     """
-    JSON 序列化,将Python 对象写入文件或转换为字符串。
+    JSON 序列化, 将Python 对象写入文件或转换为字符串。
 
     filename: JSON 文件路径
     indent: 缩进
     ensure_ascii: 默认不转为unicode
-    separators: 默认为 (", ", ": ")
+    separators: 分隔符, 默认为 (", ", ": ")
     """
     if not filename:
         return json.dumps(
             obj,
             indent=indent,
             ensure_ascii=ensure_ascii,
             separators=separators,
@@ -657,49 +662,94 @@
     return wrap
 
 
 def send_bot(
     content: str = "测试",
     bot_key: str = "",
     msgtype: str = "markdown",
-    filepath=None,
+    filepath: str = None,
+    mentioned_list: list = [],
 ):
     """
     企业微信群机器人, 基础的 Mardkown 语法。
 
     <font color="info">绿色</font>
     <font color="comment">灰色</font>
     <font color="warning">橙红色</font>
 
-    msgtype: 类型, 包括 markdown, text, file, voice
+    content: 文本
+    bot_key: 微信机器人key, 也可以设置环境变量 BOT_KEY 自动读取, 参数权重高于环境变量。
+    msgtype: 类型, 包括 markdown, text, file, voice, image
+    filepath: 文件路径，非文本类型使用。
+    mentioned_list: 提醒用户列表, 填入手机号或 "@all", 仅支持 text 类型。
     """
+    if msgtype not in ["markdown", "text", "file", "voice", "image"]:
+        raise NameError('类型仅支持 "markdown", "text", "file", "voice", "image"')
     if not bot_key:
-        raise Exception("请填写 bot_key")
+        bot_key = os.environ.get("BOT_KEY")
+        if not bot_key:
+            print("未全局配置 BOT_KEY，也未填写参数 bot_key")
+            raise Exception("请填写 bot_key")
+    if "key=" in bot_key:
+        raise Exception("bot_key 只需要填入 `key=` 后面的部分")
     if msgtype == "file" or msgtype == "voice":
         file_upload_url = f"https://qyapi.weixin.qq.com/cgi-bin/webhook/upload_media?key={bot_key}&type=file"
         files = {filepath.rsplit(".", 1)[0]: open(filepath, "rb")}
         resp = httpx.post(file_upload_url, files=files)
         msg = {"media_id": resp.json().get("media_id")}
+    elif msgtype == "image":
+        content = open(filepath, "rb").read()
+        msg = {"base64": base64_encode(content), "md5": md5(content)}
+    elif msgtype == "text":
+        msg = {"content": content, "mentioned_mobile_list": mentioned_list}
     else:
         msg = {"content": content}
     url = f"https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key={bot_key}"
     json_data = {
         "msgtype": msgtype,
         msgtype: msg,
     }
     response = httpx.post(url, json=json_data)
     return response
 
 
+def get_proxies(n: int = 1, httpx: bool = False):
+    """
+    ## 随机返回代理
+
+    需要先配置环境变量 HTTP_PROXY_DICT,  使用 to_json 将 HTTP_PROXY_DICT 转换成 json
+
+    n: 代理选择，数字或对应的字符串
+    """
+    http_proxy_dict_str = os.environ.get("HTTP_PROXY_DICT")
+    if not http_proxy_dict_str:
+        print("未配置 HTTP_PROXY_DICT")
+        raise Exception()
+    proxyurl = random.choice(read_json(http_proxy_dict_str).get(str(n)))
+    if httpx:
+        proxies = {
+            "http://": proxyurl,
+            "https://": proxyurl,
+        }
+    else:
+        proxies = {
+            "http": proxyurl,
+            "https": proxyurl,
+        }
+    return proxies
+
+
 def pdf2text(filepath):
     """
     从 pdf 提取文本内容
 
     filepath: 文件路径
     """
+    from pypdf import PdfReader
+
     reader = PdfReader(filepath)
     content = "".join([i.extract_text() for i in reader.pages])
     return content
 
 
 def listdir(path=None, key=None, reverse: bool = False):
     """
@@ -741,15 +791,18 @@
         parse_only=parse_only,
         from_encoding=from_encoding,
         exclude_encodings=exclude_encodings,
         element_classes=element_classes,
     )
 
 
-def bs_get_text(soup, strip_tags: list = ["style", "script", "code"]) -> str:
+def bs_get_text(
+    soup,
+    strip_tags: list = ["style", "script", "code"],
+) -> str:
     """
     基于 BeautifulSoup 提取网页文本v1
 
     soup: BeautifulSoup 对象或html文本
     strip_tags: 需要删除的节点
     """
     if isinstance(soup, str):
@@ -758,15 +811,18 @@
         node.extract()
     for node in soup.find_all():
         if node.name not in NON_BREAKING_ELEMENTS:
             node.append("\n") if node.name == "br" else node.append("\n\n")
     return re.sub("\n\n+", "\n\n", soup.get_text()).strip()
 
 
-def bs_get_text2(soup, strip_tags: list = ["style", "script", "code"]):
+def bs_get_text2(
+    soup,
+    strip_tags: list = ["style", "script", "code"],
+):
     """
     基于 BeautifulSoup 提取网页文本v2
 
     soup: BeautifulSoup 对象或html文本
     """
     if isinstance(soup, str):
         soup = bs_html(soup)
```

