# Comparing `tmp/PKNSETools-0.1.20240517.110.tar.gz` & `tmp/PKNSETools-0.1.20240518.111.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKNSETools-0.1.20240517.110.tar", last modified: Fri May 17 18:29:05 2024, max compression
+gzip compressed data, was "PKNSETools-0.1.20240518.111.tar", last modified: Sat May 18 00:31:01 2024, max compression
```

## Comparing `PKNSETools-0.1.20240517.110.tar` & `PKNSETools-0.1.20240518.111.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 18:29:05.412774 PKNSETools-0.1.20240517.110/
--rw-rw-rw-   0        0        0     2663 2024-05-17 18:29:05.412774 PKNSETools-0.1.20240517.110/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-17 18:29:05.412774 PKNSETools-0.1.20240517.110/PKNSETools/
-drwxrwxrwx   0        0        0        0 2024-05-17 18:29:05.412774 PKNSETools-0.1.20240517.110/PKNSETools/Benny/
--rw-rw-rw-   0        0        0    34274 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/Benny/NSE.py
--rw-rw-rw-   0        0        0     1198 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/Benny/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 18:29:05.412774 PKNSETools-0.1.20240517.110/PKNSETools/Nasdaq/
--rw-rw-rw-   0        0        0     3386 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/Nasdaq/PKNasdaqIndex.py
--rw-rw-rw-   0        0        0     1225 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/Nasdaq/__init__.py
--rw-rw-rw-   0        0        0     4806 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/PKAllStocks.py
--rw-rw-rw-   0        0        0    10770 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/PKCompanyGeneral.py
--rw-rw-rw-   0        0        0     3303 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/PKCompanyStock.py
--rw-rw-rw-   0        0        0     2635 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/PKConstants.py
--rw-rw-rw-   0        0        0    10388 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/PKIntraDay.py
--rw-rw-rw-   0        0        0    16561 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/PKNSEStockDataFetcher.py
--rw-rw-rw-   0        0        0       31 2024-05-17 18:29:00.000000 PKNSETools-0.1.20240517.110/PKNSETools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 18:29:05.412774 PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/
--rw-rw-rw-   0        0        0     1830 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/NSEStockDB.py
--rw-rw-rw-   0        0        0     1848 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/NSEStockFairValueDB.py
--rw-rw-rw-   0        0        0     1836 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/NSEStockMFIDB.py
--rw-rw-rw-   0        0        0    61961 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
--rw-rw-rw-   0        0        0     1378 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/__init__.py
--rw-rw-rw-   0        0        0     2000 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/error.py
--rw-rw-rw-   0        0        0    40060 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/funds.py
--rw-rw-rw-   0        0        0    22038 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/search.py
--rw-rw-rw-   0        0        0    13495 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/security.py
--rw-rw-rw-   0        0        0    29916 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/stock.py
--rw-rw-rw-   0        0        0    23246 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-17 18:29:05.412774 PKNSETools-0.1.20240517.110/PKNSETools.egg-info/
--rw-rw-rw-   0        0        0     2663 2024-05-17 18:29:05.000000 PKNSETools-0.1.20240517.110/PKNSETools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1004 2024-05-17 18:29:05.000000 PKNSETools-0.1.20240517.110/PKNSETools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 18:29:05.000000 PKNSETools-0.1.20240517.110/PKNSETools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-17 18:28:58.000000 PKNSETools-0.1.20240517.110/PKNSETools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       79 2024-05-17 18:29:05.000000 PKNSETools-0.1.20240517.110/PKNSETools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-17 18:29:05.000000 PKNSETools-0.1.20240517.110/PKNSETools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1884 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/README.md
--rw-rw-rw-   0        0        0       86 2024-05-17 18:29:05.412774 PKNSETools-0.1.20240517.110/setup.cfg
--rw-rw-rw-   0        0        0     3832 2024-05-17 18:27:02.000000 PKNSETools-0.1.20240517.110/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 00:31:01.182737 PKNSETools-0.1.20240518.111/
+-rw-rw-rw-   0        0        0     2663 2024-05-18 00:31:01.182737 PKNSETools-0.1.20240518.111/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-18 00:31:01.167109 PKNSETools-0.1.20240518.111/PKNSETools/
+drwxrwxrwx   0        0        0        0 2024-05-18 00:31:01.167109 PKNSETools-0.1.20240518.111/PKNSETools/Benny/
+-rw-rw-rw-   0        0        0    34274 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/Benny/NSE.py
+-rw-rw-rw-   0        0        0     1198 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/Benny/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 00:31:01.167109 PKNSETools-0.1.20240518.111/PKNSETools/Nasdaq/
+-rw-rw-rw-   0        0        0     3386 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/Nasdaq/PKNasdaqIndex.py
+-rw-rw-rw-   0        0        0     1225 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/Nasdaq/__init__.py
+-rw-rw-rw-   0        0        0     4806 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/PKAllStocks.py
+-rw-rw-rw-   0        0        0    10770 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/PKCompanyGeneral.py
+-rw-rw-rw-   0        0        0     3303 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/PKCompanyStock.py
+-rw-rw-rw-   0        0        0     2635 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/PKConstants.py
+-rw-rw-rw-   0        0        0    10388 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/PKIntraDay.py
+-rw-rw-rw-   0        0        0    17114 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/PKNSEStockDataFetcher.py
+-rw-rw-rw-   0        0        0       31 2024-05-18 00:30:56.000000 PKNSETools-0.1.20240518.111/PKNSETools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 00:31:01.182737 PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/
+-rw-rw-rw-   0        0        0     1830 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/NSEStockDB.py
+-rw-rw-rw-   0        0        0     1848 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/NSEStockFairValueDB.py
+-rw-rw-rw-   0        0        0     1836 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/NSEStockMFIDB.py
+-rw-rw-rw-   0        0        0    61961 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
+-rw-rw-rw-   0        0        0     1378 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/__init__.py
+-rw-rw-rw-   0        0        0     2000 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/error.py
+-rw-rw-rw-   0        0        0    40060 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/funds.py
+-rw-rw-rw-   0        0        0    22038 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/search.py
+-rw-rw-rw-   0        0        0    13495 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/security.py
+-rw-rw-rw-   0        0        0    29916 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/stock.py
+-rw-rw-rw-   0        0        0    23246 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-18 00:31:01.167109 PKNSETools-0.1.20240518.111/PKNSETools.egg-info/
+-rw-rw-rw-   0        0        0     2663 2024-05-18 00:31:01.000000 PKNSETools-0.1.20240518.111/PKNSETools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1004 2024-05-18 00:31:01.000000 PKNSETools-0.1.20240518.111/PKNSETools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 00:31:01.000000 PKNSETools-0.1.20240518.111/PKNSETools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-18 00:30:54.000000 PKNSETools-0.1.20240518.111/PKNSETools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       79 2024-05-18 00:31:01.000000 PKNSETools-0.1.20240518.111/PKNSETools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-18 00:31:01.000000 PKNSETools-0.1.20240518.111/PKNSETools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1884 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-18 00:31:01.182737 PKNSETools-0.1.20240518.111/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2024-05-18 00:29:09.000000 PKNSETools-0.1.20240518.111/setup.py
```

### Comparing `PKNSETools-0.1.20240517.110/PKG-INFO` & `PKNSETools-0.1.20240518.111/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240517.110
+Version: 0.1.20240518.111
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240517.110.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240518.111.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/Benny/NSE.py` & `PKNSETools-0.1.20240518.111/PKNSETools/Benny/NSE.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/Benny/__init__.py` & `PKNSETools-0.1.20240518.111/PKNSETools/Benny/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/Nasdaq/PKNasdaqIndex.py` & `PKNSETools-0.1.20240518.111/PKNSETools/Nasdaq/PKNasdaqIndex.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/Nasdaq/__init__.py` & `PKNSETools-0.1.20240518.111/PKNSETools/Nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/PKAllStocks.py` & `PKNSETools-0.1.20240518.111/PKNSETools/PKAllStocks.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/PKCompanyGeneral.py` & `PKNSETools-0.1.20240518.111/PKNSETools/PKCompanyGeneral.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/PKCompanyStock.py` & `PKNSETools-0.1.20240518.111/PKNSETools/PKCompanyStock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/PKConstants.py` & `PKNSETools-0.1.20240518.111/PKNSETools/PKConstants.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/PKIntraDay.py` & `PKNSETools-0.1.20240518.111/PKNSETools/PKIntraDay.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/PKNSEStockDataFetcher.py` & `PKNSETools-0.1.20240518.111/PKNSETools/PKNSEStockDataFetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
     AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
     LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
     OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
     SOFTWARE.
 
 """
+import os
 import csv
 import datetime
 import pytz
 import random
 import warnings
 from io import StringIO
 
@@ -52,36 +53,46 @@
     6: "https://archives.nseindia.com/content/indices/ind_niftysmallcap50list.csv",
     7: "https://archives.nseindia.com/content/indices/ind_niftysmallcap100list.csv",
     8: "https://archives.nseindia.com/content/indices/ind_niftysmallcap250list.csv",
     9: "https://archives.nseindia.com/content/indices/ind_niftymidcap50list.csv",
     10: "https://archives.nseindia.com/content/indices/ind_niftymidcap100list.csv",
     11: "https://archives.nseindia.com/content/indices/ind_niftymidcap150list.csv",
     12: "https://archives.nseindia.com/content/equities/EQUITY_L.csv",
-    14: "https://archives.nseindia.com/content/fo/fo_mktlots.csv",
+    14: "https://nsearchives.nseindia.com/content/fo/NSE_FO_SosScheme.csv",
 }
 REPO_INDEX_MAP = {
     1: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_nifty50list.csv",
     2: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_niftynext50list.csv",
     3: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_nifty100list.csv",
     4: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_nifty200list.csv",
     5: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_nifty500list.csv",
     6: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_niftysmallcap50list.csv",
     7: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_niftysmallcap100list.csv",
     8: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_niftysmallcap250list.csv",
     9: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_niftymidcap50list.csv",
     10: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_niftymidcap100list.csv",
     11: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/ind_niftymidcap150list.csv",
     12: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/EQUITY_L.csv",
-    14: "https://archives.nseindia.com/content/fo/fo_mktlots.csv",
+    14: "https://raw.githubusercontent.com/pkjmesra/PKScreener/main/results/NSE_FO_SosScheme.csv",
 }
 
 # This Class Handles Fetching of Stock Data over the internet from NSE/BSE
 
 class nseStockDataFetcher(fetcher):
 
+    def saveAllNSEIndices(self):
+        for tickerOption in NSE_INDEX_MAP.keys():
+            try:
+                url = NSE_INDEX_MAP.get(tickerOption)
+                fileName = url.split("/")[-1]
+                filePath = os.path.join(Archiver.get_user_outputs_dir(),fileName)
+                self.fetchFileFromHostServer(filePath,tickerOption,"")
+            except:
+                continue
+
     def savedFileContents(self, fileName=None):
         data, filePath, modifiedDateTime = Archiver.findFileInAppResultsDirectory(fileName=fileName)
         return data, filePath, modifiedDateTime
 
     def fetchFileFromHostServer(self,filePath,tickerOption,fileContents,indexMap=NSE_INDEX_MAP):
         try:
             url = indexMap.get(tickerOption)
@@ -119,18 +130,19 @@
                 return list(data["SYMBOL"].values)
             except Exception as e:
                 default_logger().debug(e, exc_info=True)
                 return listStockCodes
         try:
             cr = csv.reader(fileContents.strip().split("\n"))
             if tickerOption == 14:
-                for i in range(5):
-                    next(cr)  # skipping first line
+                for i in range(2):
+                    next(cr)  # skipping first two lines
                 for row in cr:
-                    listStockCodes.append(row[1])
+                    listStockCodes.append(row[0])
+                listStockCodes = sorted(list(filter(None,list(set(listStockCodes)))))
             else:
                 next(cr)  # skipping first line
                 for row in cr:
                     listStockCodes.append(row[2])
         except Exception as e:
             default_logger().debug(e, exc_info=True)
             pass
```

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/NSEStockDB.py` & `PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/NSEStockDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/NSEStockFairValueDB.py` & `PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/NSEStockFairValueDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/NSEStockMFIDB.py` & `PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/NSEStockMFIDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/PKMorningstarDataFetcher.py` & `PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/PKMorningstarDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/__init__.py` & `PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/error.py` & `PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/error.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/funds.py` & `PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/funds.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/search.py` & `PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/search.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/security.py` & `PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/security.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/stock.py` & `PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/stock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools/morningstartools/utils.py` & `PKNSETools-0.1.20240518.111/PKNSETools/morningstartools/utils.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools.egg-info/PKG-INFO` & `PKNSETools-0.1.20240518.111/PKNSETools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240517.110
+Version: 0.1.20240518.111
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240517.110.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240518.111.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240517.110/PKNSETools.egg-info/SOURCES.txt` & `PKNSETools-0.1.20240518.111/PKNSETools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/README.md` & `PKNSETools-0.1.20240518.111/README.md`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240517.110/setup.py` & `PKNSETools-0.1.20240518.111/setup.py`

 * *Files identical despite different names*

