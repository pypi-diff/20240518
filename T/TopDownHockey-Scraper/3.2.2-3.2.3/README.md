# Comparing `tmp/topdownhockey_scraper-3.2.2.tar.gz` & `tmp/topdownhockey_scraper-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topdownhockey_scraper-3.2.2.tar", last modified: Wed Apr 24 03:59:37 2024, max compression
+gzip compressed data, was "topdownhockey_scraper-3.2.3.tar", last modified: Sat May 18 04:40:51 2024, max compression
```

## Comparing `topdownhockey_scraper-3.2.2.tar` & `topdownhockey_scraper-3.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-04-24 03:59:37.762847 topdownhockey_scraper-3.2.2/
--rw-rw-r--   0 patrickbacon   (501) staff       (20)     1073 2021-10-23 01:32:32.000000 topdownhockey_scraper-3.2.2/LICENSE
--rw-r--r--   0 patrickbacon   (501) staff       (20)     5462 2024-04-24 03:59:37.762773 topdownhockey_scraper-3.2.2/PKG-INFO
--rw-rw-r--   0 patrickbacon   (501) staff       (20)     4697 2023-11-09 21:19:28.000000 topdownhockey_scraper-3.2.2/README.md
--rw-rw-r--   0 patrickbacon   (501) staff       (20)      103 2021-10-23 01:32:32.000000 topdownhockey_scraper-3.2.2/pyproject.toml
--rw-rw-r--   0 patrickbacon   (501) staff       (20)      892 2024-04-24 03:59:37.763110 topdownhockey_scraper-3.2.2/setup.cfg
--rw-rw-r--   0 patrickbacon   (501) staff       (20)     1191 2024-04-24 03:58:55.000000 topdownhockey_scraper-3.2.2/setup.py
-drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-04-24 03:59:37.760746 topdownhockey_scraper-3.2.2/src/
-drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-04-24 03:59:37.761573 topdownhockey_scraper-3.2.2/src/TopDownHockey_Scraper/
--rw-rw-r--   0 patrickbacon   (501) staff       (20)    45380 2023-10-04 05:55:32.000000 topdownhockey_scraper-3.2.2/src/TopDownHockey_Scraper/TopDownHockey_EliteProspects_Scraper.py
--rw-rw-r--   0 patrickbacon   (501) staff       (20)   148476 2024-04-24 03:59:31.000000 topdownhockey_scraper-3.2.2/src/TopDownHockey_Scraper/TopDownHockey_NHL_Scraper.py
-drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-04-24 03:59:37.762421 topdownhockey_scraper-3.2.2/src/TopDownHockey_Scraper.egg-info/
--rw-r--r--   0 patrickbacon   (501) staff       (20)     5462 2024-04-24 03:59:37.000000 topdownhockey_scraper-3.2.2/src/TopDownHockey_Scraper.egg-info/PKG-INFO
--rw-r--r--   0 patrickbacon   (501) staff       (20)      416 2024-04-24 03:59:37.000000 topdownhockey_scraper-3.2.2/src/TopDownHockey_Scraper.egg-info/SOURCES.txt
--rw-r--r--   0 patrickbacon   (501) staff       (20)        1 2024-04-24 03:59:37.000000 topdownhockey_scraper-3.2.2/src/TopDownHockey_Scraper.egg-info/dependency_links.txt
--rw-r--r--   0 patrickbacon   (501) staff       (20)       68 2024-04-24 03:59:37.000000 topdownhockey_scraper-3.2.2/src/TopDownHockey_Scraper.egg-info/requires.txt
--rw-r--r--   0 patrickbacon   (501) staff       (20)       22 2024-04-24 03:59:37.000000 topdownhockey_scraper-3.2.2/src/TopDownHockey_Scraper.egg-info/top_level.txt
+drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-05-18 04:40:51.732455 topdownhockey_scraper-3.2.3/
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)     1073 2021-10-23 01:32:32.000000 topdownhockey_scraper-3.2.3/LICENSE
+-rw-r--r--   0 patrickbacon   (501) staff       (20)     5462 2024-05-18 04:40:51.732409 topdownhockey_scraper-3.2.3/PKG-INFO
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)     4697 2023-11-09 21:19:28.000000 topdownhockey_scraper-3.2.3/README.md
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)      103 2021-10-23 01:32:32.000000 topdownhockey_scraper-3.2.3/pyproject.toml
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)      892 2024-05-18 04:40:51.732734 topdownhockey_scraper-3.2.3/setup.cfg
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)     1191 2024-05-18 04:40:29.000000 topdownhockey_scraper-3.2.3/setup.py
+drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-05-18 04:40:51.730594 topdownhockey_scraper-3.2.3/src/
+drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-05-18 04:40:51.731376 topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper/
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)    45380 2023-10-04 05:55:32.000000 topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper/TopDownHockey_EliteProspects_Scraper.py
+-rw-rw-r--   0 patrickbacon   (501) staff       (20)   148269 2024-05-18 04:37:31.000000 topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper/TopDownHockey_NHL_Scraper.py
+drwxr-xr-x   0 patrickbacon   (501) staff       (20)        0 2024-05-18 04:40:51.732187 topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper.egg-info/
+-rw-r--r--   0 patrickbacon   (501) staff       (20)     5462 2024-05-18 04:40:51.000000 topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper.egg-info/PKG-INFO
+-rw-r--r--   0 patrickbacon   (501) staff       (20)      416 2024-05-18 04:40:51.000000 topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 patrickbacon   (501) staff       (20)        1 2024-05-18 04:40:51.000000 topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 patrickbacon   (501) staff       (20)       68 2024-05-18 04:40:51.000000 topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper.egg-info/requires.txt
+-rw-r--r--   0 patrickbacon   (501) staff       (20)       22 2024-05-18 04:40:51.000000 topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper.egg-info/top_level.txt
```

### Comparing `topdownhockey_scraper-3.2.2/LICENSE` & `topdownhockey_scraper-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `topdownhockey_scraper-3.2.2/PKG-INFO` & `topdownhockey_scraper-3.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TopDownHockey_Scraper
-Version: 3.2.2
+Version: 3.2.3
 Summary: The TopDownHockey Scraper
 Home-page: https://github.com/TopDownHockey/TopDownHockey_Scraper
 Author: Patrick Bacon
 Author-email: patrick.s.bacon@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/TopDownHockey/TopDownHockey_Scraper/issues
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TopDownHockey_Scraper Version: 3.2.2 Summary: The
+Metadata-Version: 2.1 Name: TopDownHockey_Scraper Version: 3.2.3 Summary: The
 TopDownHockey Scraper Home-page: https://github.com/TopDownHockey/
 TopDownHockey_Scraper Author: Patrick Bacon Author-email:
 patrick.s.bacon@gmail.com License: MIT Project-URL: Bug Tracker, https://
 github.com/TopDownHockey/TopDownHockey_Scraper/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

### Comparing `topdownhockey_scraper-3.2.2/README.md` & `topdownhockey_scraper-3.2.3/README.md`

 * *Files identical despite different names*

### Comparing `topdownhockey_scraper-3.2.2/setup.cfg` & `topdownhockey_scraper-3.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = TopDownHockey_Scraper
-version = 3.2.2
+version = 3.2.3
 author = Patrick Bacon
 author_email = patrick.s.bacon@gmail.com
 description = A package built for scraping hockey data from EliteProspects, the NHL's HTML/API reports, and ESPN's XML reports.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/TopDownHockey/TopDownHockeyScraper
 project_urls =
```

### Comparing `topdownhockey_scraper-3.2.2/setup.py` & `topdownhockey_scraper-3.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="TopDownHockey_Scraper", # Replace with your own username
-    version="3.2.2",
+    version="3.2.3",
     author="Patrick Bacon",
     author_email="patrick.s.bacon@gmail.com",
     description="The TopDownHockey Scraper",
     long_description=long_description,
     license = 'MIT',
     long_description_content_type="text/markdown",
     url="https://github.com/TopDownHockey/TopDownHockey_Scraper",
```

### Comparing `topdownhockey_scraper-3.2.2/src/TopDownHockey_Scraper/TopDownHockey_EliteProspects_Scraper.py` & `topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper/TopDownHockey_EliteProspects_Scraper.py`

 * *Files identical despite different names*

### Comparing `topdownhockey_scraper-3.2.2/src/TopDownHockey_Scraper/TopDownHockey_NHL_Scraper.py` & `topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper/TopDownHockey_NHL_Scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1868,14 +1868,15 @@
 
     if drop_description == True:
         return espn_events.drop(columns = 'description')
     else:
         return espn_events
 
 def scrape_espn_ids_single_game(game_date, home_team, away_team):
+    
     gamedays = pd.DataFrame()
     
     if home_team == 'ATLANTA THRASHERS':
         home_team = 'WINNIPEG JETS'
     if away_team == 'ATLANTA THRASHERS':
         away_team = 'WINNIPEG JETS'
         
@@ -1892,41 +1893,37 @@
                              'AnchorLink Button Button--sm Button--anchorLink Button--alt mb4 w-100',
                             'AnchorLink Button Button--sm Button--anchorLink Button--alt mb4 w-100 mr2'], 'href':[re.compile("/nhl/team/_/name/"), re.compile("game/_")]})
     at = []
     ht = []
     gids = []
     fax = pd.DataFrame()
     #print(str(i))
-    for i in range (0, (int(len(soup_found)/3))):
-        away = soup_found[0 + (i * 3)]['href'].rsplit('/')[-2].upper()
-        home = soup_found[1 + (i * 3)]['href'].rsplit('/')[-2].upper()
-        espnid = soup_found[2 + (i * 3)]['href'].split('gameId/', 1)[1]
+    for i in range (0, ((len(soup_found)))):
+        away = soup_found[i]['href'].rsplit('/')[-1].split('-')[0].upper()
+        home = soup_found[i]['href'].rsplit('/')[-1].split('-')[1].upper()
+        espnid = soup_found[i]['href'].rsplit('/')[-2]
         at.append(away)
         ht.append(home)
         gids.append(espnid)
-
+    
     fax = fax.assign(
     away_team = at,
     home_team = ht,
     espn_id = gids,
     game_date = pd.to_datetime(this_date))
-
+    
     gamedays = gamedays._append(fax)
-
+    
     gamedays = gamedays.assign(
         home_team = np.where(gamedays.home_team=='ST LOUIS BLUES', 'ST. LOUIS BLUES', gamedays.home_team),
         away_team = np.where(gamedays.away_team=='ST LOUIS BLUES', 'ST. LOUIS BLUES', gamedays.away_team),
         espn_id = gamedays.espn_id.str.split('/').str[0].astype(int)
-
+    
     )
-    #gamedays = gamedays.assign(
-     #   home_team = np.where(gamedays.home_team=='WINNIPEG JETS', 'ATLANTA THRASHERS', gamedays.home_team),
-      #  away_team = np.where(gamedays.away_team=='WINNIPEG JETS', 'ATLANTA THRASHERS', gamedays.away_team),
-       # espn_id = gamedays.espn_id.astype(int))
-
+    
     gamedays = gamedays.assign(
         home_team = np.where(gamedays.home_team=='TB', 'TBL',
                     np.where(gamedays.home_team=='T.B', 'TBL',
                     np.where(gamedays.home_team=='L.A', 'LAK',
                     np.where(gamedays.home_team=='LA', 'LAK',
                     np.where(gamedays.home_team=='S.J', 'SJS',
                     np.where(gamedays.home_team=='SJ', 'SJS',
@@ -1940,15 +1937,17 @@
                     np.where(gamedays.away_team=='S.J', 'SJS',
                     np.where(gamedays.away_team=='SJ', 'SJS',
                     np.where(gamedays.away_team=='N.J', 'NJD',
                     np.where(gamedays.away_team=='NJ', 'NJD',
                     gamedays.away_team)))))))),
         espn_id = gamedays.espn_id.astype(int))
     
-    gamedays = gamedays[(gamedays.game_date==this_date) & (gamedays.home_team==home_team) & (gamedays.away_team==away_team)]
+    # Might need to fix later; don't have right home/away teams right now 
+    
+    #gamedays = gamedays[(gamedays.game_date==this_date) & (gamedays.home_team==home_team) & (gamedays.away_team==away_team)] 
         
     return(gamedays)
 
 def merge_and_prepare(events, shifts):
     
     season = str(int(str(events.game_id.iloc[0])[:4])) + str(int(str(events.game_id.iloc[0])[:4]) + 1)
     small_id = str(events.game_id.iloc[0])[5:]
```

### Comparing `topdownhockey_scraper-3.2.2/src/TopDownHockey_Scraper.egg-info/PKG-INFO` & `topdownhockey_scraper-3.2.3/src/TopDownHockey_Scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TopDownHockey_Scraper
-Version: 3.2.2
+Version: 3.2.3
 Summary: The TopDownHockey Scraper
 Home-page: https://github.com/TopDownHockey/TopDownHockey_Scraper
 Author: Patrick Bacon
 Author-email: patrick.s.bacon@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/TopDownHockey/TopDownHockey_Scraper/issues
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TopDownHockey_Scraper Version: 3.2.2 Summary: The
+Metadata-Version: 2.1 Name: TopDownHockey_Scraper Version: 3.2.3 Summary: The
 TopDownHockey Scraper Home-page: https://github.com/TopDownHockey/
 TopDownHockey_Scraper Author: Patrick Bacon Author-email:
 patrick.s.bacon@gmail.com License: MIT Project-URL: Bug Tracker, https://
 github.com/TopDownHockey/TopDownHockey_Scraper/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

