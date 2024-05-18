# Comparing `tmp/deltachat_rpc_client-1.139.0.tar.gz` & `tmp/deltachat_rpc_client-1.139.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltachat_rpc_client-1.139.0.tar", last modified: Sat May 18 19:50:26 2024, max compression
+gzip compressed data, was "deltachat_rpc_client-1.139.1.tar", last modified: Sat May 18 20:41:19 2024, max compression
```

## Comparing `deltachat_rpc_client-1.139.0.tar` & `deltachat_rpc_client-1.139.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:50:26.836506 deltachat_rpc_client-1.139.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-18 19:50:26.836506 deltachat_rpc_client-1.139.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 19:50:26.836506 deltachat_rpc_client-1.139.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:50:26.832506 deltachat_rpc_client-1.139.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:50:26.836506 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13369 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/deltachat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/direct_imap.py
--rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/message.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/pytestplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:50:26.836506 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-18 19:50:26.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-18 19:50:26.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 19:50:26.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-18 19:50:26.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-18 19:50:26.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 19:50:26.000000 deltachat_rpc_client-1.139.0/src/deltachat_rpc_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:50:26.836506 deltachat_rpc_client-1.139.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/tests/test_chatlist_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    24172 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/tests/test_securejoin.py
--rw-r--r--   0 runner    (1001) docker     (127)    22129 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/tests/test_something.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/tests/test_vcard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-18 19:50:17.000000 deltachat_rpc_client-1.139.0/tests/test_webxdc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:41:19.336498 deltachat_rpc_client-1.139.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-18 20:41:19.336498 deltachat_rpc_client-1.139.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 20:41:19.336498 deltachat_rpc_client-1.139.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:41:19.332498 deltachat_rpc_client-1.139.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:41:19.336498 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13369 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/deltachat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/direct_imap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/pytestplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:41:19.336498 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-18 20:41:19.000000 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-18 20:41:19.000000 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 20:41:19.000000 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-18 20:41:19.000000 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-18 20:41:19.000000 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 20:41:19.000000 deltachat_rpc_client-1.139.1/src/deltachat_rpc_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:41:19.336498 deltachat_rpc_client-1.139.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/tests/test_chatlist_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24172 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/tests/test_securejoin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22129 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/tests/test_something.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/tests/test_vcard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-18 20:41:13.000000 deltachat_rpc_client-1.139.1/tests/test_webxdc.py
```

### Comparing `deltachat_rpc_client-1.139.0/LICENSE` & `deltachat_rpc_client-1.139.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.0/PKG-INFO` & `deltachat_rpc_client-1.139.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat-rpc-client
-Version: 1.139.0
+Version: 1.139.1
 Summary: Python client for Delta Chat core JSON-RPC interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deltachat_rpc_client-1.139.0/README.md` & `deltachat_rpc_client-1.139.1/README.md`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.0/pyproject.toml` & `deltachat_rpc_client-1.139.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "deltachat-rpc-client"
-version = "1.139.0"
+version = "1.139.1"
 description = "Python client for Delta Chat core JSON-RPC interface"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
```

### Comparing `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/__init__.py` & `deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/_utils.py` & `deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/_utils.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/account.py` & `deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/account.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/chat.py` & `deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/chat.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/client.py` & `deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/client.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/const.py` & `deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/const.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/contact.py` & `deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/contact.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/deltachat.py` & `deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/deltachat.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/direct_imap.py` & `deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/direct_imap.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/events.py` & `deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/events.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/message.py` & `deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/message.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/pytestplugin.py` & `deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/pytestplugin.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client/rpc.py` & `deltachat_rpc_client-1.139.1/src/deltachat_rpc_client/rpc.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client.egg-info/PKG-INFO` & `deltachat_rpc_client-1.139.1/src/deltachat_rpc_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat-rpc-client
-Version: 1.139.0
+Version: 1.139.1
 Summary: Python client for Delta Chat core JSON-RPC interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deltachat_rpc_client-1.139.0/src/deltachat_rpc_client.egg-info/SOURCES.txt` & `deltachat_rpc_client-1.139.1/src/deltachat_rpc_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.0/tests/test_chatlist_events.py` & `deltachat_rpc_client-1.139.1/tests/test_chatlist_events.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.0/tests/test_securejoin.py` & `deltachat_rpc_client-1.139.1/tests/test_securejoin.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.0/tests/test_something.py` & `deltachat_rpc_client-1.139.1/tests/test_something.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.0/tests/test_vcard.py` & `deltachat_rpc_client-1.139.1/tests/test_vcard.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.0/tests/test_webxdc.py` & `deltachat_rpc_client-1.139.1/tests/test_webxdc.py`

 * *Files identical despite different names*

