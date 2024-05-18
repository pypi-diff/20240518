# Comparing `tmp/battlemetrics-1.0.6.tar.gz` & `tmp/battlemetrics-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "battlemetrics-1.0.6.tar", last modified: Sun Feb 25 13:29:10 2024, max compression
+gzip compressed data, was "battlemetrics-1.0.7.tar", last modified: Sat May 18 07:22:08 2024, max compression
```

## Comparing `battlemetrics-1.0.6.tar` & `battlemetrics-1.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-02-25 13:29:10.294645 battlemetrics-1.0.6/
--rw-rw-rw-   0        0        0     3650 2024-02-25 13:29:10.292642 battlemetrics-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2870 2024-02-18 07:17:58.000000 battlemetrics-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-02-25 13:29:10.213064 battlemetrics-1.0.6/battlemetrics/
--rw-rw-rw-   0        0        0     5446 2024-02-18 07:05:35.000000 battlemetrics-1.0.6/battlemetrics/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-25 13:29:10.288638 battlemetrics-1.0.6/battlemetrics/components/
--rw-rw-rw-   0        0        0    21143 2024-02-14 11:12:24.000000 battlemetrics-1.0.6/battlemetrics/components/banlist.py
--rw-rw-rw-   0        0        0     6054 2024-02-14 12:00:23.000000 battlemetrics-1.0.6/battlemetrics/components/bans.py
--rw-rw-rw-   0        0        0     4869 2024-02-13 09:08:30.000000 battlemetrics-1.0.6/battlemetrics/components/flags.py
--rw-rw-rw-   0        0        0     3074 2024-02-13 09:08:30.000000 battlemetrics-1.0.6/battlemetrics/components/gameinfo.py
--rw-rw-rw-   0        0        0    11447 2024-02-14 12:18:34.000000 battlemetrics-1.0.6/battlemetrics/components/helpers.py
--rw-rw-rw-   0        0        0     3962 2024-02-19 03:47:02.000000 battlemetrics-1.0.6/battlemetrics/components/notes.py
--rw-rw-rw-   0        0        0    12535 2024-02-25 13:13:36.000000 battlemetrics-1.0.6/battlemetrics/components/organization.py
--rw-rw-rw-   0        0        0    20573 2024-02-19 03:46:02.000000 battlemetrics-1.0.6/battlemetrics/components/player.py
--rw-rw-rw-   0        0        0    26895 2024-02-25 13:27:42.000000 battlemetrics-1.0.6/battlemetrics/components/server.py
--rw-rw-rw-   0        0        0     2505 2024-02-13 09:08:30.000000 battlemetrics-1.0.6/battlemetrics/components/session.py
-drwxrwxrwx   0        0        0        0 2024-02-25 13:29:10.291641 battlemetrics-1.0.6/battlemetrics.egg-info/
--rw-rw-rw-   0        0        0     3650 2024-02-25 13:29:10.000000 battlemetrics-1.0.6/battlemetrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      591 2024-02-25 13:29:10.000000 battlemetrics-1.0.6/battlemetrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-25 13:29:10.000000 battlemetrics-1.0.6/battlemetrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-02-25 13:29:10.000000 battlemetrics-1.0.6/battlemetrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-02-25 13:29:10.000000 battlemetrics-1.0.6/battlemetrics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      871 2024-02-25 13:28:05.000000 battlemetrics-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-25 13:29:10.294645 battlemetrics-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-18 07:22:08.355435 battlemetrics-1.0.7/
+-rw-rw-rw-   0        0        0     3650 2024-05-18 07:22:08.353432 battlemetrics-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2870 2024-02-18 07:17:58.000000 battlemetrics-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 07:22:08.268945 battlemetrics-1.0.7/battlemetrics/
+-rw-rw-rw-   0        0        0     5446 2024-02-18 07:05:35.000000 battlemetrics-1.0.7/battlemetrics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 07:22:08.348428 battlemetrics-1.0.7/battlemetrics/components/
+-rw-rw-rw-   0        0        0    21143 2024-02-14 11:12:24.000000 battlemetrics-1.0.7/battlemetrics/components/banlist.py
+-rw-rw-rw-   0        0        0     6054 2024-02-14 12:00:23.000000 battlemetrics-1.0.7/battlemetrics/components/bans.py
+-rw-rw-rw-   0        0        0     4869 2024-02-13 09:08:30.000000 battlemetrics-1.0.7/battlemetrics/components/flags.py
+-rw-rw-rw-   0        0        0     3074 2024-02-13 09:08:30.000000 battlemetrics-1.0.7/battlemetrics/components/gameinfo.py
+-rw-rw-rw-   0        0        0    11749 2024-02-25 13:58:26.000000 battlemetrics-1.0.7/battlemetrics/components/helpers.py
+-rw-rw-rw-   0        0        0     3962 2024-02-19 03:47:02.000000 battlemetrics-1.0.7/battlemetrics/components/notes.py
+-rw-rw-rw-   0        0        0    13151 2024-04-21 13:00:34.000000 battlemetrics-1.0.7/battlemetrics/components/organization.py
+-rw-rw-rw-   0        0        0    20573 2024-02-19 03:46:02.000000 battlemetrics-1.0.7/battlemetrics/components/player.py
+-rw-rw-rw-   0        0        0    27139 2024-05-18 07:20:36.000000 battlemetrics-1.0.7/battlemetrics/components/server.py
+-rw-rw-rw-   0        0        0     2505 2024-02-13 09:08:30.000000 battlemetrics-1.0.7/battlemetrics/components/session.py
+drwxrwxrwx   0        0        0        0 2024-05-18 07:22:08.351431 battlemetrics-1.0.7/battlemetrics.egg-info/
+-rw-rw-rw-   0        0        0     3650 2024-05-18 07:22:08.000000 battlemetrics-1.0.7/battlemetrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2024-05-18 07:22:08.000000 battlemetrics-1.0.7/battlemetrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 07:22:08.000000 battlemetrics-1.0.7/battlemetrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-18 07:22:08.000000 battlemetrics-1.0.7/battlemetrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-18 07:22:08.000000 battlemetrics-1.0.7/battlemetrics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      871 2024-05-18 07:21:24.000000 battlemetrics-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-18 07:22:08.356437 battlemetrics-1.0.7/setup.cfg
```

### Comparing `battlemetrics-1.0.6/PKG-INFO` & `battlemetrics-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: battlemetrics
-Version: 1.0.6
+Version: 1.0.7
 Summary: Battlemetrics API wrapper.
 Author-email: Gnomeslayer <declan.otten@live.com.au>
 Project-URL: Homepage, https://github.com/Gnomeslayer/battlemetrics
 Keywords: battlemetrics,battlemetricsapi,api,gaming
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `battlemetrics-1.0.6/README.md` & `battlemetrics-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.6/battlemetrics/__init__.py` & `battlemetrics-1.0.7/battlemetrics/__init__.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.6/battlemetrics/components/banlist.py` & `battlemetrics-1.0.7/battlemetrics/components/banlist.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.6/battlemetrics/components/bans.py` & `battlemetrics-1.0.7/battlemetrics/components/bans.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.6/battlemetrics/components/flags.py` & `battlemetrics-1.0.7/battlemetrics/components/flags.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.6/battlemetrics/components/gameinfo.py` & `battlemetrics-1.0.7/battlemetrics/components/gameinfo.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.6/battlemetrics/components/helpers.py` & `battlemetrics-1.0.7/battlemetrics/components/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,24 @@
                 
                 if response_status >= 400:
                     if response_status == 429:
                         print("You're being rate limited. Waiting 30 seconds and trying again.")
                         await asyncio.sleep(30)
                         return await self._make_request(method=method, url=url,params=params, json_dict=json_dict)
                     else:
-                        response = await r.json()
-                        if response.get('errors'):
-                            print(json.dumps(response, indent=4))
-                        return response
+                        try:
+                            response = await r.json()
+                            if response.get('errors'):
+                                print(json.dumps(response, indent=4))
+                            return response
+                        except Exception as e:
+                            print(e)
+                            response = await r.text()
+                            with open('errors.txt', 'w') as f:
+                                f.write(response)
                 
                 if 'json' in content_type:
                     try:
                         response = await r.json()
                     except Exception as e:
                         print(f"There's an issue with the respon json data.. Going to try and fix!\n<<Exception@Json>>\n{e}\n")
                         try:
```

### Comparing `battlemetrics-1.0.6/battlemetrics/components/notes.py` & `battlemetrics-1.0.7/battlemetrics/components/notes.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.6/battlemetrics/components/organization.py` & `battlemetrics-1.0.7/battlemetrics/components/organization.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,7 +245,27 @@
         url = f"{self.base_url}/organizations"
         data = {
             "page[size]": "100",
             "include": "organizationUser,banList,organizationStats"
         }
 
         return await self.helpers._make_request(method="GET", url=url, params=data)
+
+
+    async def auditlogs(self, organization_id:int):
+        """_summary_
+
+        Args:
+            organization_id (int): _description_
+
+        Returns:
+            _type_: _description_
+        """
+        
+        url = f"{self.base_url}/audit-log"
+        data = {
+            "filter[organizations]": organization_id,
+            
+            "page[size]": "100",
+            "include": "flagPlayer,playerFlag,identifier,player,playerCounter,activityMessage,server,organization,organizationUser"
+        }
+        return await self.helpers._make_request(method="GET", url=url, params=data)
```

### Comparing `battlemetrics-1.0.6/battlemetrics/components/player.py` & `battlemetrics-1.0.7/battlemetrics/components/player.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.6/battlemetrics/components/server.py` & `battlemetrics-1.0.7/battlemetrics/components/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,17 @@
                      group_size_min:int=None,
                      group_size_max:int=None,
                      map_size_min:int=None,
                      map_size_max:int=None,
                      blueprints:str="both",
                      pve:str="both",
                      kits:str="both",
-                     status:bool=True) -> dict:
+                     status:bool=True,
+                     sort_rank:bool=True,
+                     page_size:int=100) -> dict:
         
         """List, search and filter servers.
         Documentation: https://www.battlemetrics.com/developers/documentation#link-GET-server-/servers
         Args:
             search (str, optional): Search for specific server. Defaults to None.
             countries (list, optional): Server in a country. Defaults to None.
             game (str, optional): Specific game. Defaults to None.
@@ -109,27 +111,27 @@
         
         mapsize_uuid = "689d22c3-66f4-11ea-8764-5723d5d7cfba" #1:9999999
         grouplimit_uuid = "ce84a17e-a52b-11ee-a465-a3c586d9e374" #1:255
         gatherrate_uuid = "ce84a17f-a52b-11ee-a465-33d2d6d4f5ea" #1:255
 
     
         data = {}
-        data['page[size]'] = "100"
+        data['page[size]'] = f"{page_size}"
         data['include'] = "serverGroup"
         data['filter[rcon]'] = str(rcon).lower()
         
         if not status:
             data['filter[status]'] = "offline,dead,invalid"
         else:
-            data['filter[status]'] = "true"
+            data['filter[status]'] = "online"
             
         if search:
             data["filter[search]"] = search
         if countries:
-            data["filter[countries]"] = countries
+            data["filter[countries][or][0]"] = countries
         if game:
             data["filter[game]"] = game
         if blacklist:
             data["filter[ids][blacklist]"] = blacklist
         if whitelist:
             data["filter[ids][whitelist]"] = whitelist
         if organization:
@@ -149,15 +151,15 @@
             
         if pve.lower() == "true" or pve.lower() == "false":
             data[f"filter[features][{pve_uuid}]"] = f"{pve}"
             
         if kits.lower() == "true" or kits.lower() == "false":
             data[f"filter[features][{kits_uuid}]"] = f"{kits}"
         
-          
+        
         if server_type:
             count = 0
             features = None
             for ServerType in server_type:
                 if features:
                     features += f"&filter[features][{server_type_uuid}][or][{count}]={server_types[ServerType.lower]}"
                 else:
@@ -173,14 +175,20 @@
                 if features:
                     features += f"&filter[features][{gamemode_uuid}][or][{count}]={game_modes[mode.lower]}"
                 else:
                     features = f"filter[features][{gamemode_uuid}][or][{count}]={game_modes[mode.lower]}"
                 count += 1
             if features:
                 url += f"?{features}"
+                
+        if sort_rank:
+            data['sort']='rank'
+        else:
+            data['sort']='-rank'
+        print(data)
         return await self.helpers._make_request(method="GET", url=url, params=data)
     
     async def create(self, server_ip: str, server_port: str, port_query: str, game: str, server_gsp: str = None, organization_id: int = None, banlist_id: str = None, server_group: str = None) -> dict:
         """Add a server to the system.
         Documentation: https://www.battlemetrics.com/developers/documentation#link-POST-server-/servers
         The documentation does not provide information on how to properly use the params after the "Game" param.
         Args:
```

### Comparing `battlemetrics-1.0.6/battlemetrics/components/session.py` & `battlemetrics-1.0.7/battlemetrics/components/session.py`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.6/battlemetrics.egg-info/PKG-INFO` & `battlemetrics-1.0.7/battlemetrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: battlemetrics
-Version: 1.0.6
+Version: 1.0.7
 Summary: Battlemetrics API wrapper.
 Author-email: Gnomeslayer <declan.otten@live.com.au>
 Project-URL: Homepage, https://github.com/Gnomeslayer/battlemetrics
 Keywords: battlemetrics,battlemetricsapi,api,gaming
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `battlemetrics-1.0.6/battlemetrics.egg-info/SOURCES.txt` & `battlemetrics-1.0.7/battlemetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `battlemetrics-1.0.6/pyproject.toml` & `battlemetrics-1.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "battlemetrics"
 description = "Battlemetrics API wrapper."
-version = "1.0.6"
+version = "1.0.7"
 authors = [{ name = "Gnomeslayer", email = "declan.otten@live.com.au" }]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

