# Comparing `tmp/PKDevTools-0.13.20240517.120.tar.gz` & `tmp/PKDevTools-0.13.20240518.121.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240517.120.tar", last modified: Fri May 17 17:27:24 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240518.121.tar", last modified: Sat May 18 01:21:57 2024, max compression
```

## Comparing `PKDevTools-0.13.20240517.120.tar` & `PKDevTools-0.13.20240518.121.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 17:27:24.661450 PKDevTools-0.13.20240517.120/
--rw-rw-rw-   0        0        0     1086 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-17 17:27:24.645833 PKDevTools-0.13.20240517.120/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 17:27:24.661450 PKDevTools-0.13.20240517.120/PKDevTools/classes/
--rw-rw-rw-   0        0        0     4960 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     5178 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6376 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0     2608 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/FunctionTimeouts.py
--rw-rw-rw-   0        0        0    11963 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0     2860 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/OutputControls.py
--rw-rw-rw-   0        0        0    14576 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     5243 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/PKJoinableQueue.py
--rw-rw-rw-   0        0        0    11651 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14334 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     2004 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11301 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-17 17:27:20.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16136 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     7430 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-05-17 17:27:24.645833 PKDevTools-0.13.20240517.120/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5204 2024-05-17 17:27:24.000000 PKDevTools-0.13.20240517.120/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1161 2024-05-17 17:27:24.000000 PKDevTools-0.13.20240517.120/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 17:27:24.000000 PKDevTools-0.13.20240517.120/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-05-17 17:27:24.000000 PKDevTools-0.13.20240517.120/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-17 17:27:18.000000 PKDevTools-0.13.20240517.120/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      176 2024-05-17 17:27:24.000000 PKDevTools-0.13.20240517.120/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-17 17:27:24.000000 PKDevTools-0.13.20240517.120/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5204 2024-05-17 17:27:24.661450 PKDevTools-0.13.20240517.120/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/README.md
--rw-rw-rw-   0        0        0       86 2024-05-17 17:27:24.661450 PKDevTools-0.13.20240517.120/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 01:21:57.922354 PKDevTools-0.13.20240518.121/
+-rw-rw-rw-   0        0        0     1086 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-18 01:21:57.906731 PKDevTools-0.13.20240518.121/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 01:21:57.922354 PKDevTools-0.13.20240518.121/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     4960 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     5178 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6376 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     2608 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/FunctionTimeouts.py
+-rw-rw-rw-   0        0        0    11963 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     2860 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/OutputControls.py
+-rw-rw-rw-   0        0        0    15558 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     5243 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/PKJoinableQueue.py
+-rw-rw-rw-   0        0        0    11651 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14334 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     2004 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11301 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-18 01:21:52.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16136 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     7430 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-05-18 01:21:57.906731 PKDevTools-0.13.20240518.121/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5204 2024-05-18 01:21:57.000000 PKDevTools-0.13.20240518.121/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1161 2024-05-18 01:21:57.000000 PKDevTools-0.13.20240518.121/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 01:21:57.000000 PKDevTools-0.13.20240518.121/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-05-18 01:21:57.000000 PKDevTools-0.13.20240518.121/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-18 01:21:51.000000 PKDevTools-0.13.20240518.121/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      176 2024-05-18 01:21:57.000000 PKDevTools-0.13.20240518.121/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-18 01:21:57.000000 PKDevTools-0.13.20240518.121/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5204 2024-05-18 01:21:57.922354 PKDevTools-0.13.20240518.121/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-18 01:21:57.922354 PKDevTools-0.13.20240518.121/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-05-18 01:20:30.000000 PKDevTools-0.13.20240518.121/setup.py
```

### Comparing `PKDevTools-0.13.20240517.120/LICENSE` & `PKDevTools-0.13.20240518.121/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/__init__.py` & `PKDevTools-0.13.20240518.121/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/ColorText.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/ColorText.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/CookieHelper.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/FunctionTimeouts.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/FunctionTimeouts.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/OutputControls.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/OutputControls.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/PKDateUtilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -170,21 +170,48 @@
         if "simulation" in os.environ.keys():
             simulatedEnvs = json.loads(os.environ["simulation"])
             if "isTrading" in simulatedEnvs.keys():
                 return simulatedEnvs["isTrading"]
         curr = PKDateUtilities.currentDateTime()
         openTime = curr.replace(hour=9, minute=15)
         closeTime = curr.replace(hour=15, minute=30)
-        return (openTime <= curr <= closeTime) and PKDateUtilities.isTradingWeekday()
+        return ((openTime <= curr <= closeTime) and PKDateUtilities.isTradingWeekday()) or str(PKDateUtilities.onlineTradingStatus()[0]) == "Open"
 
     def isTradingWeekday(checkDate=None):
         if checkDate is None:
             checkDate = PKDateUtilities.currentDateTime()
-        return 0 <= checkDate.weekday() <= 4
-
+        if 0 <= checkDate.weekday() <= 4:
+            return True
+        else:
+            tradeDate = PKDateUtilities.onlineTradingStatus()[1]
+            if tradeDate is not None:
+                return (tradeDate.date() == checkDate.date())
+        return False
+
+    def onlineTradingStatus():
+        url = "https://www.nseindia.com/api/marketStatus"
+        headers = {"user-agent": random_user_agent()}
+        f = fetcher()
+        try:
+            status = None
+            tradeDate = None
+            res = f.fetchURL(url, headers=headers, timeout=10)
+            if res is None or res.status_code != 200:
+                return None, None
+            marketResp = res.json()
+            marketStates = marketResp["marketState"]
+            for mktState in marketStates:
+                if mktState["market"].lower() == "capital market":
+                    status = mktState["marketStatus"]
+                    tradeDate = PKDateUtilities.dateFromdbYString(mktState["tradeDate"].split(" ")[0])
+                    break
+        except:
+            pass
+        return status, tradeDate
+        
     def nextWeekday(forDate=None):
         if forDate is None:
             forDate = PKDateUtilities.currentDateTime()
         nextWeekday = forDate + datetime.timedelta(days=1)
         while not PKDateUtilities.isTradingWeekday(nextWeekday):
             nextWeekday = nextWeekday + datetime.timedelta(days=1)
         return nextWeekday
@@ -307,10 +334,7 @@
                 ]
                 break
         return occasion is not None, occasion
     
     def isTodayHoliday():
         curr = datetime.datetime.now(pytz.timezone("Asia/Kolkata"))
         return PKDateUtilities.isHoliday(curr)
-
-# d1 = PKDateUtilities.firstTradingDateOfMonth(PKDateUtilities.currentDateTime())
-# d2 = PKDateUtilities.lastTradingDateOfMonth(PKDateUtilities.currentDateTime())
```

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/PKJoinableQueue.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/PKJoinableQueue.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/PKPickler.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/Telegram.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/log.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240518.121/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240518.121/PKDevTools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240517.120
+Version: 0.13.20240518.121
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240517.120.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240518.121.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240517.120/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240518.121/PKDevTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/PKG-INFO` & `PKDevTools-0.13.20240518.121/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240517.120
+Version: 0.13.20240518.121
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240517.120.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240518.121.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240517.120/README.md` & `PKDevTools-0.13.20240518.121/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.120/setup.py` & `PKDevTools-0.13.20240518.121/setup.py`

 * *Files identical despite different names*

