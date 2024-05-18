# Comparing `tmp/python-engineio-4.9.0.tar.gz` & `tmp/python_engineio-4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-engineio-4.9.0.tar", last modified: Mon Feb  5 15:06:29 2024, max compression
+gzip compressed data, was "python_engineio-4.9.1.tar", last modified: Sat May 18 16:09:38 2024, max compression
```

## Comparing `python-engineio-4.9.0.tar` & `python_engineio-4.9.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-02-05 15:06:29.026281 python-engineio-4.9.0/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1082 2023-07-05 12:32:34.000000 python-engineio-4.9.0/LICENSE
--rw-rw-r--   0 miguel    (1000) miguel    (1000)       72 2023-10-14 23:31:57.000000 python-engineio-4.9.0/MANIFEST.in
--rw-r--r--   0 miguel    (1000) miguel    (1000)     2236 2024-02-05 15:06:29.026281 python-engineio-4.9.0/PKG-INFO
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1277 2023-10-14 23:43:33.000000 python-engineio-4.9.0/README.md
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-02-05 15:06:29.022281 python-engineio-4.9.0/docs/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      580 2023-07-05 12:32:36.000000 python-engineio-4.9.0/docs/Makefile
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-02-05 15:06:29.022281 python-engineio-4.9.0/docs/_static/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)       51 2023-07-05 12:32:36.000000 python-engineio-4.9.0/docs/_static/README.md
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      441 2023-10-14 23:31:57.000000 python-engineio-4.9.0/docs/api.rst
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     5667 2023-07-05 12:32:51.000000 python-engineio-4.9.0/docs/client.rst
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     5535 2023-10-14 23:31:57.000000 python-engineio-4.9.0/docs/conf.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      540 2023-07-05 12:32:36.000000 python-engineio-4.9.0/docs/index.rst
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     5086 2023-10-14 23:31:57.000000 python-engineio-4.9.0/docs/intro.rst
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      787 2023-07-05 12:32:36.000000 python-engineio-4.9.0/docs/make.bat
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    24193 2023-10-14 23:31:57.000000 python-engineio-4.9.0/docs/server.rst
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1111 2024-02-05 15:06:25.000000 python-engineio-4.9.0/pyproject.toml
--rw-rw-r--   0 miguel    (1000) miguel    (1000)       38 2024-02-05 15:06:29.026281 python-engineio-4.9.0/setup.cfg
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-02-05 15:06:29.022281 python-engineio-4.9.0/src/
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-02-05 15:06:29.026281 python-engineio-4.9.0/src/engineio/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      481 2023-10-14 23:31:57.000000 python-engineio-4.9.0/src/engineio/__init__.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    27932 2024-02-05 00:13:30.000000 python-engineio-4.9.0/src/engineio/async_client.py
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-02-05 15:06:29.026281 python-engineio-4.9.0/src/engineio/async_drivers/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)        0 2023-10-14 23:31:57.000000 python-engineio-4.9.0/src/engineio/async_drivers/__init__.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      949 2023-10-14 23:31:57.000000 python-engineio-4.9.0/src/engineio/async_drivers/_websocket_wsgi.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     3768 2023-10-14 23:31:57.000000 python-engineio-4.9.0/src/engineio/async_drivers/aiohttp.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    10354 2023-12-28 20:23:59.000000 python-engineio-4.9.0/src/engineio/async_drivers/asgi.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1755 2023-12-28 20:20:06.000000 python-engineio-4.9.0/src/engineio/async_drivers/eventlet.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     2962 2023-10-14 23:31:57.000000 python-engineio-4.9.0/src/engineio/async_drivers/gevent.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     5962 2023-12-28 20:23:59.000000 python-engineio-4.9.0/src/engineio/async_drivers/gevent_uwsgi.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     4538 2023-12-28 20:23:59.000000 python-engineio-4.9.0/src/engineio/async_drivers/sanic.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      463 2023-10-14 23:31:57.000000 python-engineio-4.9.0/src/engineio/async_drivers/threading.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     5909 2023-12-28 19:46:51.000000 python-engineio-4.9.0/src/engineio/async_drivers/tornado.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    25061 2024-01-06 11:58:29.000000 python-engineio-4.9.0/src/engineio/async_server.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    10305 2023-12-28 20:23:59.000000 python-engineio-4.9.0/src/engineio/async_socket.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     4872 2023-10-14 23:31:57.000000 python-engineio-4.9.0/src/engineio/base_client.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    14013 2024-02-05 15:06:03.000000 python-engineio-4.9.0/src/engineio/base_server.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      400 2023-10-14 23:31:57.000000 python-engineio-4.9.0/src/engineio/base_socket.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    26291 2024-02-05 00:13:30.000000 python-engineio-4.9.0/src/engineio/client.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      292 2023-10-14 23:31:57.000000 python-engineio-4.9.0/src/engineio/exceptions.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      405 2023-10-14 23:31:57.000000 python-engineio-4.9.0/src/engineio/json.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     3766 2023-10-14 23:31:57.000000 python-engineio-4.9.0/src/engineio/middleware.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     3189 2024-01-17 00:14:09.000000 python-engineio-4.9.0/src/engineio/packet.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1547 2023-10-14 23:31:57.000000 python-engineio-4.9.0/src/engineio/payload.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    21558 2024-01-06 12:08:16.000000 python-engineio-4.9.0/src/engineio/server.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     9996 2023-12-28 20:23:59.000000 python-engineio-4.9.0/src/engineio/socket.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     2064 2023-10-14 23:31:57.000000 python-engineio-4.9.0/src/engineio/static_files.py
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-02-05 15:06:29.026281 python-engineio-4.9.0/src/python_engineio.egg-info/
--rw-r--r--   0 miguel    (1000) miguel    (1000)     2236 2024-02-05 15:06:29.000000 python-engineio-4.9.0/src/python_engineio.egg-info/PKG-INFO
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     2023 2024-02-05 15:06:29.000000 python-engineio-4.9.0/src/python_engineio.egg-info/SOURCES.txt
--rw-rw-r--   0 miguel    (1000) miguel    (1000)        1 2024-02-05 15:06:29.000000 python-engineio-4.9.0/src/python_engineio.egg-info/dependency_links.txt
--rw-rw-r--   0 miguel    (1000) miguel    (1000)        1 2023-10-11 19:17:59.000000 python-engineio-4.9.0/src/python_engineio.egg-info/not-zip-safe
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      123 2024-02-05 15:06:29.000000 python-engineio-4.9.0/src/python_engineio.egg-info/requires.txt
--rw-rw-r--   0 miguel    (1000) miguel    (1000)        9 2024-02-05 15:06:29.000000 python-engineio-4.9.0/src/python_engineio.egg-info/top_level.txt
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-02-05 15:06:29.026281 python-engineio-4.9.0/tests/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)        0 2023-07-05 12:32:34.000000 python-engineio-4.9.0/tests/__init__.py
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-02-05 15:06:29.026281 python-engineio-4.9.0/tests/async/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)        0 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/async/__init__.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)       14 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/async/index.html
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1902 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/async/test_aiohttp.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    17944 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/async/test_asgi.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    53900 2024-02-05 00:13:30.000000 python-engineio-4.9.0/tests/async/test_client.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)       70 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/async/test_sanic.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    45956 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/async/test_server.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    20010 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/async/test_socket.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     2287 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/async/test_tornado.py
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-02-05 15:06:29.026281 python-engineio-4.9.0/tests/common/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)        0 2023-07-05 12:32:36.000000 python-engineio-4.9.0/tests/common/__init__.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)       14 2023-07-05 12:32:36.000000 python-engineio-4.9.0/tests/common/index.html
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      942 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/common/test_async_eventlet.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    61260 2024-02-05 00:13:30.000000 python-engineio-4.9.0/tests/common/test_client.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     7559 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/common/test_middleware.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     5116 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/common/test_packet.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     2454 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/common/test_payload.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    44351 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/common/test_server.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    18637 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/common/test_socket.py
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-02-05 15:06:29.026281 python-engineio-4.9.0/tests/performance/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      115 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/performance/README.md
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      423 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/performance/binary_b64_packet.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      411 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/performance/binary_packet.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      413 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/performance/json_packet.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      459 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/performance/payload.py
--rwxrwxr-x   0 miguel    (1000) miguel    (1000)      151 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/performance/run.sh
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      962 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/performance/server_receive.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      408 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tests/performance/text_packet.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      691 2023-10-14 23:31:57.000000 python-engineio-4.9.0/tox.ini
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-05-18 16:09:38.079695 python_engineio-4.9.1/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1082 2023-07-05 12:32:34.000000 python_engineio-4.9.1/LICENSE
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       72 2023-10-14 23:31:57.000000 python_engineio-4.9.1/MANIFEST.in
+-rw-r--r--   0 miguel    (1000) miguel    (1000)     2236 2024-05-18 16:09:38.079695 python_engineio-4.9.1/PKG-INFO
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1277 2023-10-14 23:43:33.000000 python_engineio-4.9.1/README.md
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-05-18 16:09:38.075695 python_engineio-4.9.1/docs/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      580 2023-07-05 12:32:36.000000 python_engineio-4.9.1/docs/Makefile
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-05-18 16:09:38.075695 python_engineio-4.9.1/docs/_static/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       51 2023-07-05 12:32:36.000000 python_engineio-4.9.1/docs/_static/README.md
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      441 2023-10-14 23:31:57.000000 python_engineio-4.9.1/docs/api.rst
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     5667 2023-07-05 12:32:51.000000 python_engineio-4.9.1/docs/client.rst
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     5535 2023-10-14 23:31:57.000000 python_engineio-4.9.1/docs/conf.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      540 2023-07-05 12:32:36.000000 python_engineio-4.9.1/docs/index.rst
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     5086 2023-10-14 23:31:57.000000 python_engineio-4.9.1/docs/intro.rst
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      787 2023-07-05 12:32:36.000000 python_engineio-4.9.1/docs/make.bat
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    24193 2023-10-14 23:31:57.000000 python_engineio-4.9.1/docs/server.rst
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1111 2024-05-18 16:09:36.000000 python_engineio-4.9.1/pyproject.toml
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       38 2024-05-18 16:09:38.079695 python_engineio-4.9.1/setup.cfg
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-05-18 16:09:38.075695 python_engineio-4.9.1/src/
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-05-18 16:09:38.075695 python_engineio-4.9.1/src/engineio/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      481 2023-10-14 23:31:57.000000 python_engineio-4.9.1/src/engineio/__init__.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    27932 2024-02-05 00:13:30.000000 python_engineio-4.9.1/src/engineio/async_client.py
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-05-18 16:09:38.075695 python_engineio-4.9.1/src/engineio/async_drivers/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        0 2023-10-14 23:31:57.000000 python_engineio-4.9.1/src/engineio/async_drivers/__init__.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      949 2023-10-14 23:31:57.000000 python_engineio-4.9.1/src/engineio/async_drivers/_websocket_wsgi.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     3768 2023-10-14 23:31:57.000000 python_engineio-4.9.1/src/engineio/async_drivers/aiohttp.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    10837 2024-02-09 18:54:24.000000 python_engineio-4.9.1/src/engineio/async_drivers/asgi.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1755 2023-12-28 20:20:06.000000 python_engineio-4.9.1/src/engineio/async_drivers/eventlet.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2962 2023-10-14 23:31:57.000000 python_engineio-4.9.1/src/engineio/async_drivers/gevent.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     5962 2023-12-28 20:23:59.000000 python_engineio-4.9.1/src/engineio/async_drivers/gevent_uwsgi.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     4538 2023-12-28 20:23:59.000000 python_engineio-4.9.1/src/engineio/async_drivers/sanic.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      463 2023-10-14 23:31:57.000000 python_engineio-4.9.1/src/engineio/async_drivers/threading.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     5909 2023-12-28 19:46:51.000000 python_engineio-4.9.1/src/engineio/async_drivers/tornado.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    25098 2024-05-18 13:53:22.000000 python_engineio-4.9.1/src/engineio/async_server.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    10305 2023-12-28 20:23:59.000000 python_engineio-4.9.1/src/engineio/async_socket.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     4872 2023-10-14 23:31:57.000000 python_engineio-4.9.1/src/engineio/base_client.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    14013 2024-02-05 15:06:03.000000 python_engineio-4.9.1/src/engineio/base_server.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      400 2023-10-14 23:31:57.000000 python_engineio-4.9.1/src/engineio/base_socket.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    26317 2024-02-29 18:08:27.000000 python_engineio-4.9.1/src/engineio/client.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      292 2023-10-14 23:31:57.000000 python_engineio-4.9.1/src/engineio/exceptions.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      405 2023-10-14 23:31:57.000000 python_engineio-4.9.1/src/engineio/json.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     3766 2023-10-14 23:31:57.000000 python_engineio-4.9.1/src/engineio/middleware.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     3189 2024-01-17 00:14:09.000000 python_engineio-4.9.1/src/engineio/packet.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1547 2023-10-14 23:31:57.000000 python_engineio-4.9.1/src/engineio/payload.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    21558 2024-01-06 12:08:16.000000 python_engineio-4.9.1/src/engineio/server.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     9996 2023-12-28 20:23:59.000000 python_engineio-4.9.1/src/engineio/socket.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2064 2023-10-14 23:31:57.000000 python_engineio-4.9.1/src/engineio/static_files.py
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-05-18 16:09:38.079695 python_engineio-4.9.1/src/python_engineio.egg-info/
+-rw-r--r--   0 miguel    (1000) miguel    (1000)     2236 2024-05-18 16:09:38.000000 python_engineio-4.9.1/src/python_engineio.egg-info/PKG-INFO
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2023 2024-05-18 16:09:38.000000 python_engineio-4.9.1/src/python_engineio.egg-info/SOURCES.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        1 2024-05-18 16:09:38.000000 python_engineio-4.9.1/src/python_engineio.egg-info/dependency_links.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        1 2023-10-11 19:17:59.000000 python_engineio-4.9.1/src/python_engineio.egg-info/not-zip-safe
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      123 2024-05-18 16:09:38.000000 python_engineio-4.9.1/src/python_engineio.egg-info/requires.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        9 2024-05-18 16:09:38.000000 python_engineio-4.9.1/src/python_engineio.egg-info/top_level.txt
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-05-18 16:09:38.079695 python_engineio-4.9.1/tests/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        0 2023-07-05 12:32:34.000000 python_engineio-4.9.1/tests/__init__.py
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-05-18 16:09:38.079695 python_engineio-4.9.1/tests/async/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        0 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/async/__init__.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       14 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/async/index.html
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1902 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/async/test_aiohttp.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    19077 2024-02-09 18:54:58.000000 python_engineio-4.9.1/tests/async/test_asgi.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    53900 2024-02-05 00:13:30.000000 python_engineio-4.9.1/tests/async/test_client.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       70 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/async/test_sanic.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    45956 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/async/test_server.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    20010 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/async/test_socket.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2287 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/async/test_tornado.py
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-05-18 16:09:38.079695 python_engineio-4.9.1/tests/common/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        0 2023-07-05 12:32:36.000000 python_engineio-4.9.1/tests/common/__init__.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       14 2023-07-05 12:32:36.000000 python_engineio-4.9.1/tests/common/index.html
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      942 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/common/test_async_eventlet.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    61260 2024-02-05 00:13:30.000000 python_engineio-4.9.1/tests/common/test_client.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     7559 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/common/test_middleware.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     5116 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/common/test_packet.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2454 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/common/test_payload.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    44351 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/common/test_server.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    18637 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/common/test_socket.py
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2024-05-18 16:09:38.079695 python_engineio-4.9.1/tests/performance/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      115 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/performance/README.md
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      423 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/performance/binary_b64_packet.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      411 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/performance/binary_packet.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      413 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/performance/json_packet.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      459 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/performance/payload.py
+-rwxrwxr-x   0 miguel    (1000) miguel    (1000)      151 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/performance/run.sh
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      962 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/performance/server_receive.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      408 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tests/performance/text_packet.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      691 2023-10-14 23:31:57.000000 python_engineio-4.9.1/tox.ini
```

### Comparing `python-engineio-4.9.0/LICENSE` & `python_engineio-4.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/PKG-INFO` & `python_engineio-4.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-engineio
-Version: 4.9.0
+Version: 4.9.1
 Summary: Engine.IO server and client for Python
 Author-email: Miguel Grinberg <miguel.grinberg@gmail.com>
 Project-URL: Homepage, https://github.com/miguelgrinberg/python-engineio
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/python-engineio/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-engineio-4.9.0/README.md` & `python_engineio-4.9.1/README.md`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/docs/Makefile` & `python_engineio-4.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/docs/client.rst` & `python_engineio-4.9.1/docs/client.rst`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/docs/conf.py` & `python_engineio-4.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/docs/index.rst` & `python_engineio-4.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/docs/intro.rst` & `python_engineio-4.9.1/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/docs/make.bat` & `python_engineio-4.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/docs/server.rst` & `python_engineio-4.9.1/docs/server.rst`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/pyproject.toml` & `python_engineio-4.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-engineio"
-version = "4.9.0"
+version = "4.9.1"
 authors = [{name = "Miguel Grinberg", email = "miguel.grinberg@gmail.com"}]
 description = "Engine.IO server and client for Python"
 classifiers = [
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `python-engineio-4.9.0/src/engineio/async_client.py` & `python_engineio-4.9.1/src/engineio/async_client.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/src/engineio/async_drivers/_websocket_wsgi.py` & `python_engineio-4.9.1/src/engineio/async_drivers/_websocket_wsgi.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/src/engineio/async_drivers/aiohttp.py` & `python_engineio-4.9.1/src/engineio/async_drivers/aiohttp.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/src/engineio/async_drivers/asgi.py` & `python_engineio-4.9.1/src/engineio/async_drivers/asgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,20 @@
     :param engineio_server: The Engine.IO server. Must be an instance of the
                             ``engineio.AsyncServer`` class.
     :param static_files: A dictionary with static file mapping rules. See the
                          documentation for details on this argument.
     :param other_asgi_app: A separate ASGI app that receives all other traffic.
     :param engineio_path: The endpoint where the Engine.IO application should
                           be installed. The default value is appropriate for
-                          most cases.
+                          most cases. With a value of ``None``, all incoming
+                          traffic is directed to the Engine.IO server, with the
+                          assumption that routing, if necessary, is handled by
+                          a different layer. When this option is set to
+                          ``None``, ``static_files`` and ``other_asgi_app`` are
+                          ignored.
     :param on_startup: function to be called on application startup; can be
                        coroutine
     :param on_shutdown: function to be called on application shutdown; can be
                         coroutine
 
     Example usage::
 
@@ -40,32 +45,34 @@
     """
     def __init__(self, engineio_server, other_asgi_app=None,
                  static_files=None, engineio_path='engine.io',
                  on_startup=None, on_shutdown=None):
         self.engineio_server = engineio_server
         self.other_asgi_app = other_asgi_app
         self.engineio_path = engineio_path
-        if not self.engineio_path.startswith('/'):
-            self.engineio_path = '/' + self.engineio_path
-        if not self.engineio_path.endswith('/'):
-            self.engineio_path += '/'
+        if self.engineio_path is not None:
+            if not self.engineio_path.startswith('/'):
+                self.engineio_path = '/' + self.engineio_path
+            if not self.engineio_path.endswith('/'):
+                self.engineio_path += '/'
         self.static_files = static_files or {}
         self.on_startup = on_startup
         self.on_shutdown = on_shutdown
 
     async def __call__(self, scope, receive, send):
-        if scope['type'] in ['http', 'websocket'] and \
-                scope['path'].startswith(self.engineio_path):
+        if scope['type'] == 'lifespan':
+            await self.lifespan(scope, receive, send)
+        elif scope['type'] in ['http', 'websocket'] and (
+                self.engineio_path is None
+                or scope['path'].startswith(self.engineio_path)):
             await self.engineio_server.handle_request(scope, receive, send)
         else:
             static_file = get_static_file(scope['path'], self.static_files) \
                 if scope['type'] == 'http' and self.static_files else None
-            if scope['type'] == 'lifespan':
-                await self.lifespan(scope, receive, send)
-            elif static_file and os.path.exists(static_file['filename']):
+            if static_file and os.path.exists(static_file['filename']):
                 await self.serve_static_file(static_file, receive, send)
             elif self.other_asgi_app is not None:
                 await self.other_asgi_app(scope, receive, send)
             else:
                 await self.not_found(receive, send)
 
     async def serve_static_file(self, static_file, receive,
```

### Comparing `python-engineio-4.9.0/src/engineio/async_drivers/eventlet.py` & `python_engineio-4.9.1/src/engineio/async_drivers/eventlet.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/src/engineio/async_drivers/gevent.py` & `python_engineio-4.9.1/src/engineio/async_drivers/gevent.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/src/engineio/async_drivers/gevent_uwsgi.py` & `python_engineio-4.9.1/src/engineio/async_drivers/gevent_uwsgi.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/src/engineio/async_drivers/sanic.py` & `python_engineio-4.9.1/src/engineio/async_drivers/sanic.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/src/engineio/async_drivers/tornado.py` & `python_engineio-4.9.1/src/engineio/async_drivers/tornado.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/src/engineio/async_server.py` & `python_engineio-4.9.1/src/engineio/async_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -520,17 +520,17 @@
         self.service_task_event = self.create_event()
         while not self.service_task_event.is_set():
             if len(self.sockets) == 0:
                 # nothing to do
                 try:
                     await asyncio.wait_for(self.service_task_event.wait(),
                                            timeout=self.ping_timeout)
-                except asyncio.TimeoutError:
                     break
-                continue
+                except asyncio.TimeoutError:
+                    continue
 
             # go through the entire client list in a ping interval cycle
             sleep_interval = self.ping_timeout / len(self.sockets)
 
             try:
                 # iterate over the current clients
                 for s in self.sockets.copy().values():
@@ -542,16 +542,17 @@
                             # the _get_socket() method from another thread
                             pass
                     elif not s.closing:
                         await s.check_ping_timeout()
                     try:
                         await asyncio.wait_for(self.service_task_event.wait(),
                                                timeout=sleep_interval)
-                    except asyncio.TimeoutError:
                         raise KeyboardInterrupt()
+                    except asyncio.TimeoutError:
+                        continue
             except (
                 SystemExit,
                 KeyboardInterrupt,
                 asyncio.CancelledError,
                 GeneratorExit,
             ):
                 self.logger.info('service task canceled')
```

### Comparing `python-engineio-4.9.0/src/engineio/async_socket.py` & `python_engineio-4.9.1/src/engineio/async_socket.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/src/engineio/base_client.py` & `python_engineio-4.9.1/src/engineio/base_client.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/src/engineio/base_server.py` & `python_engineio-4.9.1/src/engineio/base_server.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/src/engineio/client.py` & `python_engineio-4.9.1/src/engineio/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -490,15 +490,15 @@
 
     def _read_loop_websocket(self):
         """Read packets from the Engine.IO WebSocket connection."""
         while self.state == 'connected':
             p = None
             try:
                 p = self.ws.recv()
-                if len(p) == 0:  # pragma: no cover
+                if len(p) == 0 and not self.ws.connected:  # pragma: no cover
                     # websocket client can return an empty string after close
                     raise websocket.WebSocketConnectionClosedException()
             except websocket.WebSocketTimeoutException:
                 self.logger.warning(
                     'Server has stopped communicating, aborting')
                 self.queue.put(None)
                 break
```

### Comparing `python-engineio-4.9.0/src/engineio/middleware.py` & `python_engineio-4.9.1/src/engineio/middleware.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/src/engineio/packet.py` & `python_engineio-4.9.1/src/engineio/packet.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/src/engineio/payload.py` & `python_engineio-4.9.1/src/engineio/payload.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/src/engineio/server.py` & `python_engineio-4.9.1/src/engineio/server.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/src/engineio/socket.py` & `python_engineio-4.9.1/src/engineio/socket.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/src/engineio/static_files.py` & `python_engineio-4.9.1/src/engineio/static_files.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/src/python_engineio.egg-info/PKG-INFO` & `python_engineio-4.9.1/src/python_engineio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-engineio
-Version: 4.9.0
+Version: 4.9.1
 Summary: Engine.IO server and client for Python
 Author-email: Miguel Grinberg <miguel.grinberg@gmail.com>
 Project-URL: Homepage, https://github.com/miguelgrinberg/python-engineio
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/python-engineio/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-engineio-4.9.0/src/python_engineio.egg-info/SOURCES.txt` & `python_engineio-4.9.1/src/python_engineio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/tests/async/test_aiohttp.py` & `python_engineio-4.9.1/tests/async/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/tests/async/test_asgi.py` & `python_engineio-4.9.1/tests/async/test_asgi.py`

 * *Files 6% similar despite different names*

```diff
@@ -510,7 +510,34 @@
             async_asgi.make_response(
                 '401 UNAUTHORIZED', [('foo', 'bar')], None, environ
             )
         )
         environ['asgi.send'].mock.assert_called_with(
             {'type': 'websocket.close'}
         )
+
+    def test_sub_app_routing(self):
+
+        class ASGIDispatcher:
+            def __init__(self, routes):
+                self.routes = routes
+
+            async def __call__(self, scope, receive, send):
+                path = scope['path']
+                for prefix, app in self.routes.items():
+                    if path.startswith(prefix):
+                        await app(scope, receive, send)
+                        return
+                assert False, 'No route found'
+
+        other_app = AsyncMock()
+        mock_server = mock.MagicMock()
+        mock_server.handle_request = AsyncMock()
+        eio_app = async_asgi.ASGIApp(mock_server, engineio_path=None)
+        root_app = ASGIDispatcher({'/foo': other_app, '/eio': eio_app})
+        scope = {'type': 'http', 'path': '/foo/bar'}
+        _run(root_app(scope, 'receive', 'send'))
+        other_app.mock.assert_called_once_with(scope, 'receive', 'send')
+        scope = {'type': 'http', 'path': '/eio/'}
+        _run(root_app(scope, 'receive', 'send'))
+        eio_app.engineio_server.handle_request.mock.assert_called_once_with(
+            scope, 'receive', 'send')
```

### Comparing `python-engineio-4.9.0/tests/async/test_client.py` & `python_engineio-4.9.1/tests/async/test_client.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/tests/async/test_server.py` & `python_engineio-4.9.1/tests/async/test_server.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/tests/async/test_socket.py` & `python_engineio-4.9.1/tests/async/test_socket.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/tests/async/test_tornado.py` & `python_engineio-4.9.1/tests/async/test_tornado.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/tests/common/test_async_eventlet.py` & `python_engineio-4.9.1/tests/common/test_async_eventlet.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/tests/common/test_client.py` & `python_engineio-4.9.1/tests/common/test_client.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/tests/common/test_middleware.py` & `python_engineio-4.9.1/tests/common/test_middleware.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/tests/common/test_packet.py` & `python_engineio-4.9.1/tests/common/test_packet.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/tests/common/test_payload.py` & `python_engineio-4.9.1/tests/common/test_payload.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/tests/common/test_server.py` & `python_engineio-4.9.1/tests/common/test_server.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/tests/common/test_socket.py` & `python_engineio-4.9.1/tests/common/test_socket.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/tests/performance/server_receive.py` & `python_engineio-4.9.1/tests/performance/server_receive.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.9.0/tox.ini` & `python_engineio-4.9.1/tox.ini`

 * *Files identical despite different names*

