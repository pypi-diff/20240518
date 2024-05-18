# Comparing `tmp/battlemetrics-1.0.7.tar.gz` & `tmp/battlemetrics-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "battlemetrics-1.0.7.tar", last modified: Sat May 18 07:22:08 2024, max compression
+gzip compressed data, was "battlemetrics-1.0.8.tar", last modified: Sat May 18 07:57:09 2024, max compression
```

## Comparing `battlemetrics-1.0.7.tar` & `battlemetrics-1.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 07:22:08.355435 battlemetrics-1.0.7/
--rw-rw-rw-   0        0        0     3650 2024-05-18 07:22:08.353432 battlemetrics-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2870 2024-02-18 07:17:58.000000 battlemetrics-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 07:22:08.268945 battlemetrics-1.0.7/battlemetrics/
--rw-rw-rw-   0        0        0     5446 2024-02-18 07:05:35.000000 battlemetrics-1.0.7/battlemetrics/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 07:22:08.348428 battlemetrics-1.0.7/battlemetrics/components/
--rw-rw-rw-   0        0        0    21143 2024-02-14 11:12:24.000000 battlemetrics-1.0.7/battlemetrics/components/banlist.py
--rw-rw-rw-   0        0        0     6054 2024-02-14 12:00:23.000000 battlemetrics-1.0.7/battlemetrics/components/bans.py
--rw-rw-rw-   0        0        0     4869 2024-02-13 09:08:30.000000 battlemetrics-1.0.7/battlemetrics/components/flags.py
--rw-rw-rw-   0        0        0     3074 2024-02-13 09:08:30.000000 battlemetrics-1.0.7/battlemetrics/components/gameinfo.py
--rw-rw-rw-   0        0        0    11749 2024-02-25 13:58:26.000000 battlemetrics-1.0.7/battlemetrics/components/helpers.py
--rw-rw-rw-   0        0        0     3962 2024-02-19 03:47:02.000000 battlemetrics-1.0.7/battlemetrics/components/notes.py
--rw-rw-rw-   0        0        0    13151 2024-04-21 13:00:34.000000 battlemetrics-1.0.7/battlemetrics/components/organization.py
--rw-rw-rw-   0        0        0    20573 2024-02-19 03:46:02.000000 battlemetrics-1.0.7/battlemetrics/components/player.py
--rw-rw-rw-   0        0        0    27139 2024-05-18 07:20:36.000000 battlemetrics-1.0.7/battlemetrics/components/server.py
--rw-rw-rw-   0        0        0     2505 2024-02-13 09:08:30.000000 battlemetrics-1.0.7/battlemetrics/components/session.py
-drwxrwxrwx   0        0        0        0 2024-05-18 07:22:08.351431 battlemetrics-1.0.7/battlemetrics.egg-info/
--rw-rw-rw-   0        0        0     3650 2024-05-18 07:22:08.000000 battlemetrics-1.0.7/battlemetrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      591 2024-05-18 07:22:08.000000 battlemetrics-1.0.7/battlemetrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 07:22:08.000000 battlemetrics-1.0.7/battlemetrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-18 07:22:08.000000 battlemetrics-1.0.7/battlemetrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-18 07:22:08.000000 battlemetrics-1.0.7/battlemetrics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      871 2024-05-18 07:21:24.000000 battlemetrics-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-18 07:22:08.356437 battlemetrics-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-18 07:57:09.537258 battlemetrics-1.0.8/
+-rw-rw-rw-   0        0        0     3650 2024-05-18 07:57:09.536257 battlemetrics-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2870 2024-02-18 07:17:58.000000 battlemetrics-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 07:57:09.459813 battlemetrics-1.0.8/battlemetrics/
+-rw-rw-rw-   0        0        0     5446 2024-02-18 07:05:35.000000 battlemetrics-1.0.8/battlemetrics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 07:57:09.532166 battlemetrics-1.0.8/battlemetrics/components/
+-rw-rw-rw-   0        0        0    21143 2024-02-14 11:12:24.000000 battlemetrics-1.0.8/battlemetrics/components/banlist.py
+-rw-rw-rw-   0        0        0     6054 2024-02-14 12:00:23.000000 battlemetrics-1.0.8/battlemetrics/components/bans.py
+-rw-rw-rw-   0        0        0     4869 2024-02-13 09:08:30.000000 battlemetrics-1.0.8/battlemetrics/components/flags.py
+-rw-rw-rw-   0        0        0     3074 2024-02-13 09:08:30.000000 battlemetrics-1.0.8/battlemetrics/components/gameinfo.py
+-rw-rw-rw-   0        0        0    11749 2024-02-25 13:58:26.000000 battlemetrics-1.0.8/battlemetrics/components/helpers.py
+-rw-rw-rw-   0        0        0     3962 2024-02-19 03:47:02.000000 battlemetrics-1.0.8/battlemetrics/components/notes.py
+-rw-rw-rw-   0        0        0    13151 2024-04-21 13:00:34.000000 battlemetrics-1.0.8/battlemetrics/components/organization.py
+-rw-rw-rw-   0        0        0    20573 2024-02-19 03:46:02.000000 battlemetrics-1.0.8/battlemetrics/components/player.py
+-rw-rw-rw-   0        0        0    27132 2024-05-18 07:56:17.000000 battlemetrics-1.0.8/battlemetrics/components/server.py
+-rw-rw-rw-   0        0        0     2505 2024-02-13 09:08:30.000000 battlemetrics-1.0.8/battlemetrics/components/session.py
+drwxrwxrwx   0        0        0        0 2024-05-18 07:57:09.534257 battlemetrics-1.0.8/battlemetrics.egg-info/
+-rw-rw-rw-   0        0        0     3650 2024-05-18 07:57:09.000000 battlemetrics-1.0.8/battlemetrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2024-05-18 07:57:09.000000 battlemetrics-1.0.8/battlemetrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 07:57:09.000000 battlemetrics-1.0.8/battlemetrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-18 07:57:09.000000 battlemetrics-1.0.8/battlemetrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-18 07:57:09.000000 battlemetrics-1.0.8/battlemetrics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      871 2024-05-18 07:56:46.000000 battlemetrics-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-18 07:57:09.538262 battlemetrics-1.0.8/setup.cfg
```

### Comparing `battlemetrics-1.0.7/PKG-INFO` & `battlemetrics-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: battlemetrics
-Version: 1.0.7
+Version: 1.0.8
 Summary: Battlemetrics API wrapper.
 Author-email: Gnomeslayer <declan.otten@live.com.au>
 Project-URL: Homepage, https://github.com/Gnomeslayer/battlemetrics
 Keywords: battlemetrics,battlemetricsapi,api,gaming
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `battlemetrics-1.0.7/README.md` & `battlemetrics-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.7/battlemetrics/__init__.py` & `battlemetrics-1.0.8/battlemetrics/__init__.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.7/battlemetrics/components/banlist.py` & `battlemetrics-1.0.8/battlemetrics/components/banlist.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.7/battlemetrics/components/bans.py` & `battlemetrics-1.0.8/battlemetrics/components/bans.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.7/battlemetrics/components/flags.py` & `battlemetrics-1.0.8/battlemetrics/components/flags.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.7/battlemetrics/components/gameinfo.py` & `battlemetrics-1.0.8/battlemetrics/components/gameinfo.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.7/battlemetrics/components/helpers.py` & `battlemetrics-1.0.8/battlemetrics/components/helpers.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.7/battlemetrics/components/notes.py` & `battlemetrics-1.0.8/battlemetrics/components/notes.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.7/battlemetrics/components/organization.py` & `battlemetrics-1.0.8/battlemetrics/components/organization.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.7/battlemetrics/components/player.py` & `battlemetrics-1.0.8/battlemetrics/components/player.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.7/battlemetrics/components/server.py` & `battlemetrics-1.0.8/battlemetrics/components/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
             if features:
                 url += f"?{features}"
                 
         if sort_rank:
             data['sort']='rank'
         else:
             data['sort']='-rank'
-        print(data)
+            
         return await self.helpers._make_request(method="GET", url=url, params=data)
     
     async def create(self, server_ip: str, server_port: str, port_query: str, game: str, server_gsp: str = None, organization_id: int = None, banlist_id: str = None, server_group: str = None) -> dict:
         """Add a server to the system.
         Documentation: https://www.battlemetrics.com/developers/documentation#link-POST-server-/servers
         The documentation does not provide information on how to properly use the params after the "Game" param.
         Args:
```

### Comparing `battlemetrics-1.0.7/battlemetrics/components/session.py` & `battlemetrics-1.0.8/battlemetrics/components/session.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.7/battlemetrics.egg-info/PKG-INFO` & `battlemetrics-1.0.8/battlemetrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: battlemetrics
-Version: 1.0.7
+Version: 1.0.8
 Summary: Battlemetrics API wrapper.
 Author-email: Gnomeslayer <declan.otten@live.com.au>
 Project-URL: Homepage, https://github.com/Gnomeslayer/battlemetrics
 Keywords: battlemetrics,battlemetricsapi,api,gaming
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `battlemetrics-1.0.7/battlemetrics.egg-info/SOURCES.txt` & `battlemetrics-1.0.8/battlemetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.7/pyproject.toml` & `battlemetrics-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "battlemetrics"
 description = "Battlemetrics API wrapper."
-version = "1.0.7"
+version = "1.0.8"
 authors = [{ name = "Gnomeslayer", email = "declan.otten@live.com.au" }]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

