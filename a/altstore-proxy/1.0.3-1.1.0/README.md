# Comparing `tmp/altstore_proxy-1.0.3.tar.gz` & `tmp/altstore_proxy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altstore_proxy-1.0.3.tar", last modified: Sat May 18 11:46:51 2024, max compression
+gzip compressed data, was "altstore_proxy-1.1.0.tar", last modified: Sat May 18 12:00:56 2024, max compression
```

## Comparing `altstore_proxy-1.0.3.tar` & `altstore_proxy-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:46:51.265813 altstore_proxy-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-18 11:46:51.265813 altstore_proxy-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-18 11:46:46.000000 altstore_proxy-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:46:51.265813 altstore_proxy-1.0.3/altstore_proxy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 11:46:46.000000 altstore_proxy-1.0.3/altstore_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:46:51.265813 altstore_proxy-1.0.3/altstore_proxy/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 11:46:46.000000 altstore_proxy-1.0.3/altstore_proxy/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-18 11:46:46.000000 altstore_proxy-1.0.3/altstore_proxy/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-05-18 11:46:46.000000 altstore_proxy-1.0.3/altstore_proxy/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-18 11:46:46.000000 altstore_proxy-1.0.3/altstore_proxy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:46:51.265813 altstore_proxy-1.0.3/altstore_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-18 11:46:51.000000 altstore_proxy-1.0.3/altstore_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-18 11:46:51.000000 altstore_proxy-1.0.3/altstore_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 11:46:51.000000 altstore_proxy-1.0.3/altstore_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-18 11:46:51.000000 altstore_proxy-1.0.3/altstore_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 11:46:51.000000 altstore_proxy-1.0.3/altstore_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 11:46:51.000000 altstore_proxy-1.0.3/altstore_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 11:46:51.000000 altstore_proxy-1.0.3/altstore_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 11:46:51.265813 altstore_proxy-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-18 11:46:46.000000 altstore_proxy-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:00:56.882261 altstore_proxy-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-18 12:00:56.882261 altstore_proxy-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-18 12:00:51.000000 altstore_proxy-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:00:56.878261 altstore_proxy-1.1.0/altstore_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 12:00:51.000000 altstore_proxy-1.1.0/altstore_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:00:56.882261 altstore_proxy-1.1.0/altstore_proxy/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 12:00:51.000000 altstore_proxy-1.1.0/altstore_proxy/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-18 12:00:51.000000 altstore_proxy-1.1.0/altstore_proxy/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-18 12:00:51.000000 altstore_proxy-1.1.0/altstore_proxy/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-18 12:00:51.000000 altstore_proxy-1.1.0/altstore_proxy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:00:56.878261 altstore_proxy-1.1.0/altstore_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-18 12:00:56.000000 altstore_proxy-1.1.0/altstore_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-18 12:00:56.000000 altstore_proxy-1.1.0/altstore_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 12:00:56.000000 altstore_proxy-1.1.0/altstore_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-18 12:00:56.000000 altstore_proxy-1.1.0/altstore_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 12:00:56.000000 altstore_proxy-1.1.0/altstore_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 12:00:56.000000 altstore_proxy-1.1.0/altstore_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 12:00:56.000000 altstore_proxy-1.1.0/altstore_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 12:00:56.882261 altstore_proxy-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-18 12:00:51.000000 altstore_proxy-1.1.0/setup.py
```

### Comparing `altstore_proxy-1.0.3/PKG-INFO` & `altstore_proxy-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altstore_proxy
-Version: 1.0.3
+Version: 1.1.0
 Summary: A simple proxy for slow AltStore servers
 Home-page: https://github.com/rix1337/docker-altstore-proxy
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `altstore_proxy-1.0.3/altstore_proxy/proxy.py` & `altstore_proxy-1.1.0/altstore_proxy/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,20 @@
 
 def merge_jsons(shared_state_dict, shared_state_lock):
     shared_state.set_state(shared_state_dict, shared_state_lock)
 
     try:
         while True:
             merged_json = {
-                "apps": []
+                "name": "AltStore-Proxy",
+                "subtitle": "A simple proxy for slow AltStore servers.",
+                "iconURL": "https://altstore.io/images/AltStore_AppIcon.png",
+                "website": "https://github.com/rix1337/AltStore-Proxy",
+                "apps": [],
+                "news": []
             }
 
             for repo in shared_state.values["repos_to_cache"]:
                 response = requests.get(repo)
                 data = response.json()
                 for app in data['apps']:
                     print("Found " + app['name'] + ", v." + app['version'])
```

### Comparing `altstore_proxy-1.0.3/altstore_proxy.egg-info/PKG-INFO` & `altstore_proxy-1.1.0/altstore_proxy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altstore-proxy
-Version: 1.0.3
+Version: 1.1.0
 Summary: A simple proxy for slow AltStore servers
 Home-page: https://github.com/rix1337/docker-altstore-proxy
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `altstore_proxy-1.0.3/setup.py` & `altstore_proxy-1.1.0/setup.py`

 * *Files identical despite different names*

