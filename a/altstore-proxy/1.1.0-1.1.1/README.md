# Comparing `tmp/altstore_proxy-1.1.0.tar.gz` & `tmp/altstore_proxy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altstore_proxy-1.1.0.tar", last modified: Sat May 18 12:00:56 2024, max compression
+gzip compressed data, was "altstore_proxy-1.1.1.tar", last modified: Sat May 18 18:52:55 2024, max compression
```

## Comparing `altstore_proxy-1.1.0.tar` & `altstore_proxy-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:00:56.882261 altstore_proxy-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-18 12:00:56.882261 altstore_proxy-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-18 12:00:51.000000 altstore_proxy-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:00:56.878261 altstore_proxy-1.1.0/altstore_proxy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 12:00:51.000000 altstore_proxy-1.1.0/altstore_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:00:56.882261 altstore_proxy-1.1.0/altstore_proxy/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 12:00:51.000000 altstore_proxy-1.1.0/altstore_proxy/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-18 12:00:51.000000 altstore_proxy-1.1.0/altstore_proxy/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-18 12:00:51.000000 altstore_proxy-1.1.0/altstore_proxy/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-18 12:00:51.000000 altstore_proxy-1.1.0/altstore_proxy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:00:56.878261 altstore_proxy-1.1.0/altstore_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-18 12:00:56.000000 altstore_proxy-1.1.0/altstore_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-18 12:00:56.000000 altstore_proxy-1.1.0/altstore_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 12:00:56.000000 altstore_proxy-1.1.0/altstore_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-18 12:00:56.000000 altstore_proxy-1.1.0/altstore_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 12:00:56.000000 altstore_proxy-1.1.0/altstore_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 12:00:56.000000 altstore_proxy-1.1.0/altstore_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 12:00:56.000000 altstore_proxy-1.1.0/altstore_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 12:00:56.882261 altstore_proxy-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-18 12:00:51.000000 altstore_proxy-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:52:54.997084 altstore_proxy-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-18 18:52:54.997084 altstore_proxy-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-18 18:52:46.000000 altstore_proxy-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:52:54.997084 altstore_proxy-1.1.1/altstore_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 18:52:46.000000 altstore_proxy-1.1.1/altstore_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:52:54.997084 altstore_proxy-1.1.1/altstore_proxy/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 18:52:46.000000 altstore_proxy-1.1.1/altstore_proxy/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-18 18:52:46.000000 altstore_proxy-1.1.1/altstore_proxy/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-05-18 18:52:46.000000 altstore_proxy-1.1.1/altstore_proxy/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-18 18:52:46.000000 altstore_proxy-1.1.1/altstore_proxy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:52:54.997084 altstore_proxy-1.1.1/altstore_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-18 18:52:54.000000 altstore_proxy-1.1.1/altstore_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-18 18:52:54.000000 altstore_proxy-1.1.1/altstore_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 18:52:54.000000 altstore_proxy-1.1.1/altstore_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-18 18:52:54.000000 altstore_proxy-1.1.1/altstore_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 18:52:54.000000 altstore_proxy-1.1.1/altstore_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 18:52:54.000000 altstore_proxy-1.1.1/altstore_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 18:52:54.000000 altstore_proxy-1.1.1/altstore_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 18:52:54.997084 altstore_proxy-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-18 18:52:46.000000 altstore_proxy-1.1.1/setup.py
```

### Comparing `altstore_proxy-1.1.0/PKG-INFO` & `altstore_proxy-1.1.1/altstore_proxy.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: altstore_proxy
-Version: 1.1.0
+Name: altstore-proxy
+Version: 1.1.1
 Summary: A simple proxy for slow AltStore servers
 Home-page: https://github.com/rix1337/docker-altstore-proxy
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -29,9 +29,22 @@
 altstore_proxy
   --port=8080
   --baseurl=https://example.com/
   --cache=/tmp/altstore_cache
   --repos=https://fake.tld/apps.json,https://foo.bar/altstore.json
 ```
 
+# Docker
+```
+docker run -d \
+  --name="AltStore-Proxy" \
+  -p port:8080 \
+  -v /path/to/cache/:/cache:rw \
+  rix1337/docker-altstore-proxy
+  ```
+## Optional Environment Variables
+ - `-e BASEURL` Base URL for the AltStore-Proxy (for reverse proxy usage)
+ - `-e REPOS` Desired apps.json Repositories to Cache - comma separated
+
+
```

### Comparing `altstore_proxy-1.1.0/altstore_proxy/proxy.py` & `altstore_proxy-1.1.1/altstore_proxy/proxy.py`

 * *Files 24% similar despite different names*

```diff
@@ -167,15 +167,58 @@
             print("[AltStore-Proxy] No repositories provided, using default repositories: " + str(
                 shared_state.values["repos_to_cache"]))
 
         app = Bottle()
 
         @app.get("/")
         def status():
-            return "AltStore-Proxy is running! Add this URL + /apps.json to your AltStore."
+            repos_html = ''.join(
+                f'<li><a href="{repo}">{repo}</a></li>' for repo in shared_state.values["repos_to_cache"])
+            return f'''
+            <html>
+            <head>
+                <title>AltStore-Proxy</title>
+                <style>
+                    body {{
+                        background: linear-gradient(to right, #f9f9f9, #e0e0e0);
+                        font-family: Arial, sans-serif;
+                        padding: 20px;
+                        text-align: center;
+                    }}
+                    button {{
+                        font-size: 20px;
+                        padding: 10px 20px;
+                        margin-top: 20px;
+                        background-color: #4CAF50; /* Green */
+                        border: none;
+                        color: white;
+                        text-align: center;
+                        text-decoration: none;
+                        display: inline-block;
+                        font-size: 16px;
+                        transition-duration: 0.4s;
+                        cursor: pointer;
+                    }}
+                    button:hover {{
+                        background-color: #45a049;
+                    }}
+                </style>
+            </head>
+            <body>
+                <h1>AltStore-Proxy</h1>
+                <a href="/apps.json">View apps.json</a><br>
+                <a href="altstore://source?url={shared_state.values["baseurl"]}">
+                    <button>Add this source to AltStore to receive app updates</button>
+                </a>
+                <h2>Source Repositories</h2>
+                <ul>
+                    {repos_html}
+                </ul>
+            </body>
+            </html>'''
 
         @app.get('/cache/<filename:path>')
         def serve_file(filename):
             return static_file(filename, root=shared_state.values["cache"], download=filename)
 
         @app.get("/apps.json")
         def status():
@@ -188,15 +231,16 @@
         hourly_update = multiprocessing.Process(target=merge_jsons, args=(shared_state_dict, shared_state_lock,))
         hourly_update.start()
 
         while not shared_state.values["ready"]:
             time.sleep(1)
 
         print(
-            "[AltStore-Proxy] AltStores proxied at http://127.0.0.1:" + str(shared_state.values["port"]) + "/apps.json")
+            "[AltStore-Proxy] Add this source to AltStore by opening " + shared_state.values[
+                "baseurl"] + " on your mobile device.")
         try:
             Server(app, listen='0.0.0.0', port=shared_state.values["port"]).serve_forever()
         except KeyboardInterrupt:
             hourly_update.terminate()
             sys.exit(0)
```

### Comparing `altstore_proxy-1.1.0/setup.py` & `altstore_proxy-1.1.1/setup.py`

 * *Files identical despite different names*

