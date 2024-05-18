# Comparing `tmp/edgarquery-0.0.60.tar.gz` & `tmp/edgarquery-0.0.61.tar.gz`

## Comparing `edgarquery-0.0.60.tar` & `edgarquery-0.0.61.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rwxr-xr-x   0        0        0      621 2020-02-02 00:00:00.000000 edgarquery-0.0.60/genusage.sh
--rw-r--r--   0        0        0    10698 2020-02-02 00:00:00.000000 edgarquery-0.0.60/notes.txt
--rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 edgarquery-0.0.60/scripts/edgarquery.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 edgarquery-0.0.60/scripts/edgartickerstocsv.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/__about__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/__init__.py
--rwxr-xr-x   0        0        0      218 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/concepts.sh
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/ebquery.py
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarcikperson.py
--rwxr-xr-x   0        0        0     5063 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarcompanyconcepttocsv.py
--rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarcompanyfactsshow.py
--rwxr-xr-x   0        0        0     5961 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarcompanyfactstocsv.py
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarcompanyfactsziptocsv.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarlatest10K.py
--rw-r--r--   0        0        0     7894 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarlatestsubmission.py
--rw-r--r--   0        0        0     9258 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarlatestsubmissions.py
--rwxr-xr-x   0        0        0    15138 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarquery.py
--rw-r--r--   0        0        0    13988 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarsubmissions.py
--rwxr-xr-x   0        0        0     5369 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarsubmissionsziptocsv.py
--rwxr-xr-x   0        0        0     3865 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgartickerstocsv.py
--rwxr-xr-x   0        0        0     4679 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarxbrlframestocsv.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/sedfile
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/tickerd.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 edgarquery-0.0.60/tests/__init__.py
--rwxr-xr-x   0        0        0     2760 2020-02-02 00:00:00.000000 edgarquery-0.0.60/tests/p.sh
--rwxr-xr-x   0        0        0      230 2020-02-02 00:00:00.000000 edgarquery-0.0.60/tests/s.sh
--rwxr-xr-x   0        0        0     2429 2020-02-02 00:00:00.000000 edgarquery-0.0.60/tests/x.sh
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 edgarquery-0.0.60/tests/y.sh
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 edgarquery-0.0.60/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 edgarquery-0.0.60/LICENSE.txt
--rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 edgarquery-0.0.60/README.md
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 edgarquery-0.0.60/pyproject.toml
--rw-r--r--   0        0        0    10241 2020-02-02 00:00:00.000000 edgarquery-0.0.60/PKG-INFO
+-rwxr-xr-x   0        0        0      621 2020-02-02 00:00:00.000000 edgarquery-0.0.61/genusage.sh
+-rw-r--r--   0        0        0    10698 2020-02-02 00:00:00.000000 edgarquery-0.0.61/notes.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 edgarquery-0.0.61/requirements.txt
+-rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 edgarquery-0.0.61/scripts/edgarquery.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 edgarquery-0.0.61/scripts/edgartickerstocsv.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/__about__.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/__init__.py
+-rwxr-xr-x   0        0        0      218 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/concepts.sh
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/ebquery.py
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarcikperson.py
+-rwxr-xr-x   0        0        0     5063 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarcompanyconcepttocsv.py
+-rw-r--r--   0        0        0     7504 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarcompanyfactsshow.py
+-rwxr-xr-x   0        0        0     6004 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarcompanyfactstocsv.py
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarcompanyfactsziptocsv.py
+-rw-r--r--   0        0        0     8589 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarlatest10K.py
+-rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarlatestsubmission.py
+-rw-r--r--   0        0        0     9269 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarlatestsubmissions.py
+-rwxr-xr-x   0        0        0    15167 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarquery.py
+-rw-r--r--   0        0        0    13998 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarsubmissions.py
+-rwxr-xr-x   0        0        0     5369 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarsubmissionsziptocsv.py
+-rwxr-xr-x   0        0        0     3865 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgartickerstocsv.py
+-rwxr-xr-x   0        0        0     4679 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarxbrlframestocsv.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/sedfile
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/tickerd.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 edgarquery-0.0.61/tests/__init__.py
+-rwxr-xr-x   0        0        0     2760 2020-02-02 00:00:00.000000 edgarquery-0.0.61/tests/p.sh
+-rwxr-xr-x   0        0        0      230 2020-02-02 00:00:00.000000 edgarquery-0.0.61/tests/s.sh
+-rwxr-xr-x   0        0        0     2429 2020-02-02 00:00:00.000000 edgarquery-0.0.61/tests/x.sh
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 edgarquery-0.0.61/tests/y.sh
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 edgarquery-0.0.61/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 edgarquery-0.0.61/LICENSE.txt
+-rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 edgarquery-0.0.61/README.md
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 edgarquery-0.0.61/pyproject.toml
+-rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 edgarquery-0.0.61/PKG-INFO
```

### Comparing `edgarquery-0.0.60/genusage.sh` & `edgarquery-0.0.61/genusage.sh`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.60/notes.txt` & `edgarquery-0.0.61/notes.txt`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.60/scripts/edgarquery.py` & `edgarquery-0.0.61/scripts/edgarquery.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.60/src/edgarquery/ebquery.py` & `edgarquery-0.0.61/src/edgarquery/ebquery.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.60/src/edgarquery/edgarcikperson.py` & `edgarquery-0.0.61/src/edgarquery/edgarcikperson.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.60/src/edgarquery/edgarcompanyconcepttocsv.py` & `edgarquery-0.0.61/src/edgarquery/edgarcompanyconcepttocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.60/src/edgarquery/edgarcompanyfactsshow.py` & `edgarquery-0.0.61/src/edgarquery/edgarcompanyfactsshow.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 import argparse
 import csv
 import json
 import re
 import urllib.request
 import webbrowser
 
+import plotly
+from plotly.subplots import make_subplots
+import plotly.graph_objects as go
+
 try:
     from edgarquery import ebquery
     from edgarquery import tickerd
 except ImportError as e:
     import ebquery
     import tickerd
 
@@ -99,19 +103,42 @@
                 assert type(units) == type({}), \
                     'jsonfacts: units not a dictionary'
                 uka = (u for u in units.keys() )
                 for uk in uka:
                     self.units = uk
                     assert type(units[uk]) == type([]), \
                         'jasonfacts %s is not an array'
+                    fig = self.jsonfactplot(units[uk], label)
+                    fightml = fig.to_html()
+                    htmla.append(fightml)
                     tbl = self.jsonfacttable(units[uk], label)
                     htmla.extend(tbl)
         self.htmla.extend(htmla)
 
 
+    def jsonfactplot(self, recs, label):
+        """ jsonfactplot(self, recs, label)
+
+        plot the first two columns of the fact array
+        recs - company fact rows
+        label - label
+        """
+
+        dates = [recs[i]['end'] for i in range(len(recs))]
+        vals = [recs[i]['val'] for i in range(len(recs))]
+        for i in range(len(recs)):
+            if type(vals[i]) != type(0):
+                vals[i] = 0
+
+        fig = go.Figure(go.Scatter(
+            x = dates,
+            y = vals
+        ))
+        return fig
+
     def jsonfacttable(self, recs, label):
         """ jsonfacttable(recs)
 
         construct an html table from the rows of a company fact
         recs - company fact rows
         """
         htmla = []
@@ -180,15 +207,15 @@
         self.processjson(rstr)
 
         self.savefacthtml(directory)
 
 
 def main():
     argp = argparse.ArgumentParser(description='parse EDGAR company\
-    facts for a cik and display them in a browser')
+    facts for a ticker or cik and display them in a browser')
     argp.add_argument('--cik', help='Centralized Index Key for the company')
     argp.add_argument('--ticker', help='Ticker for the company')
     argp.add_argument('--directory', default='/tmp',
         help='where to store the html file to display')
 
     args = argp.parse_args()
     if not args.cik and not args.ticker:
```

### Comparing `edgarquery-0.0.60/src/edgarquery/edgarcompanyfactstocsv.py` & `edgarquery-0.0.61/src/edgarquery/edgarcompanyfactstocsv.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,16 +139,15 @@
         except Exception as e:
             print('%s %s: %s' % (self.jsonfile, fn, e), file=sys.stderr )
             sys.exit(1)
 
 def main():
     EP = EDGARCompanyFactstoCSV()
     argp = argparse.ArgumentParser(description="Parse an SEC EDGAR\
-        companyfacts json file after it has been altered to deal with its\
-    multipart character and generate CSV files from its content")
+        companyfacts json file after it has been altered to deal with its\ multipart character and generate CSV files from its content. I think that the SEC fixed the multi-json bug")
 
     argp.add_argument('--file', required=True,
                 help="json file to process")
     argp.add_argument('--directory', help="where to deposit the csv fileѕ",
                       default='/tmp')
 
     args = argp.parse_args()
```

### Comparing `edgarquery-0.0.60/src/edgarquery/edgarcompanyfactsziptocsv.py` & `edgarquery-0.0.61/src/edgarquery/edgarcompanyfactsziptocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.60/src/edgarquery/edgarlatest10K.py` & `edgarquery-0.0.61/src/edgarquery/edgarlatest10K.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
 
 
 # if __name__ == '__main__':
 def main():
     LT = EDGARLatest10K()
 
     argp = argparse.ArgumentParser(
-              description='find the most recent 10-K for cik')
+              description='find the most recent 10-K for ticker or cik')
     argp.add_argument("--cik", help="10-digit Central Index Key")
     argp.add_argument("--ticker", help="company ticker symbol")
     argp.add_argument("--link", action='store_true', default=False,
           help="return the url for the latest 10-K")
     argp.add_argument("--directory", default='/tmp',
          help="directory to store the output")
     argp.add_argument("--show", action='store_true', default=False,
```

### Comparing `edgarquery-0.0.60/src/edgarquery/edgarlatestsubmission.py` & `edgarquery-0.0.61/src/edgarquery/edgarlatestsubmission.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,15 @@
                     return
 
 # if __name__ == '__main__':
 def main():
     LT = EDGARLatestSubmission()
 
     argp = argparse.ArgumentParser(
-              description='find the most recent X-K for cik')
+              description='find the most recent submission for a ticker or cik for some common submissƣons.') 
     argp.add_argument("--cik", help="10-digit Central Index Key")
     argp.add_argument("--ticker", help="company ticker symbol")
     argp.add_argument("--submission", default='10-K',
         choices=['SC 13D', '13F-HR', 'DEF 14A', '8-K', '10-K', '10-Q'],
         help="X-K submission type")
 
     argp.add_argument("--link", action='store_true', default=False,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `edgarquery-0.0.60/src/edgarquery/edgarlatestsubmissions.py` & `edgarquery-0.0.61/src/edgarquery/edgarlatestsubmissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         return latest
 
 # if __name__ == '__main__':
 def main():
     LT = EDGARLatestsubmissions()
 
     argp = argparse.ArgumentParser(
-              description='find the most recent submissions for cik')
+             description='find the most recent submissions for a ticker or cik')
     argp.add_argument("--cik", help="10-digit Central Index Key")
     argp.add_argument("--ticker", help="company ticker symbol")
 
     argp.add_argument("--directory", default='/tmp',
         help="directory to store the output")
     argp.add_argument('--file', help="where to store the output")
```

### Comparing `edgarquery-0.0.60/src/edgarquery/edgarquery.py` & `edgarquery-0.0.61/src/edgarquery/edgarquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,14 +220,15 @@
         # resp=self.query(url)
         # self.storequery(resp, file)
 
 def main():
     EQ = EDGARquery()
 
     EQ.argp = argparse.ArgumentParser(description="query SEC EDGAR site\
+        for a ticker or cik\
         NOTE thæt EQEMAIL env variable is required and\
         must contain a valid User-Agent such as your email address")
 
     EQ.argp.add_argument("--cik", required=False,
         help="10-digit Central Index Key")
     EQ.argp.add_argument("--ticker", required=False,
         help="company stock ticker")
```

### Comparing `edgarquery-0.0.60/src/edgarquery/edgarsubmissions.py` & `edgarquery-0.0.61/src/edgarquery/edgarsubmissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,15 +332,15 @@
 def main():
     LS = EDGARSubmissions()
 
     now = datetime.datetime.now()
     year = now.year
 
     argp = argparse.ArgumentParser(
-              description='find the most recent submissions for cik')
+              description='find the most recent submissions for ticker or cik')
     argp.add_argument("--cik", help="10-digit Central Index Key")
     argp.add_argument("--ticker", help="company ticker symbol")
     argp.add_argument("--year", required=False,
         help="year to search for submissions if not current year")
 
     argp.add_argument("--file", required=False,
         help="store the output in this file")
```

### Comparing `edgarquery-0.0.60/src/edgarquery/edgarsubmissionsziptocsv.py` & `edgarquery-0.0.61/src/edgarquery/edgarsubmissionsziptocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.60/src/edgarquery/edgartickerstocsv.py` & `edgarquery-0.0.61/src/edgarquery/edgartickerstocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.60/src/edgarquery/edgarxbrlframestocsv.py` & `edgarquery-0.0.61/src/edgarquery/edgarxbrlframestocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.60/src/edgarquery/tickerd.py` & `edgarquery-0.0.61/src/edgarquery/tickerd.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.60/tests/p.sh` & `edgarquery-0.0.61/tests/p.sh`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.60/tests/x.sh` & `edgarquery-0.0.61/tests/x.sh`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.60/LICENSE.txt` & `edgarquery-0.0.61/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.60/README.md` & `edgarquery-0.0.61/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 <br/>
 ##<br/>
 ## edgarcompanyfactsshow<br/>
 ##<br/>
 usage: edgarcompanyfactsshow [-h] [--cik CIK] [--ticker TICKER]<br/>
 [--directory DIRECTORY]<br/>
 <br/>
-parse EDGAR company facts for a cik and display them in a browser<br/>
+parse EDGAR company facts for a ticker or cik and display them in a browser<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --cik CIK             Centralized Index Key for the company<br/>
 --ticker TICKER       Ticker for the company<br/>
 --directory DIRECTORY<br/>
 where to store the html file to display<br/>
@@ -76,15 +76,16 @@
 <br/>
 ##<br/>
 ## edgarcompanyfactstocsv<br/>
 ##<br/>
 usage: edgarcompanyfactstocsv [-h] --file FILE [--directory DIRECTORY]<br/>
 <br/>
 Parse an SEC EDGAR companyfacts json file after it has been altered to deal<br/>
-with its multipart character and generate CSV files from its content<br/>
+with its multipart character and generate CSV files from its content. I think<br/>
+that the SEC fixed the multi-json bug<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --file FILE           json file to process<br/>
 --directory DIRECTORY<br/>
 where to deposit the csv fileѕ<br/>
 <br/>
@@ -110,15 +111,15 @@
 <br/>
 ##<br/>
 ## edgarlatest10K<br/>
 ##<br/>
 usage: edgarlatest10K [-h] [--cik CIK] [--ticker TICKER] [--link]<br/>
 [--directory DIRECTORY] [--show]<br/>
 <br/>
-find the most recent 10-K for cik<br/>
+find the most recent 10-K for ticker or cik<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --cik CIK             10-digit Central Index Key<br/>
 --ticker TICKER       company ticker symbol<br/>
 --link                return the url for the latest 10-K<br/>
 --directory DIRECTORY<br/>
@@ -129,15 +130,16 @@
 ##<br/>
 ## edgarlatestsubmission<br/>
 ##<br/>
 usage: edgarlatestsubmission [-h] [--cik CIK] [--ticker TICKER]<br/>
 [--submission {SC 13D,13F-HR,DEF 14A,8-K,10-K,10-Q}]<br/>
 [--link] [--directory DIRECTORY] [--show]<br/>
 <br/>
-find the most recent X-K for cik<br/>
+find the most recent submission for a ticker or cik for some common<br/>
+submissƣons.<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --cik CIK             10-digit Central Index Key<br/>
 --ticker TICKER       company ticker symbol<br/>
 --submission {SC 13D,13F-HR,DEF 14A,8-K,10-K,10-Q}<br/>
 X-K submission type<br/>
@@ -149,15 +151,15 @@
 <br/>
 ##<br/>
 ## edgarlatestsubmissions<br/>
 ##<br/>
 usage: edgarlatestsubmissions [-h] [--cik CIK] [--ticker TICKER]<br/>
 [--directory DIRECTORY] [--file FILE]<br/>
 <br/>
-find the most recent submissions for cik<br/>
+find the most recent submissions for a ticker or cik<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --cik CIK             10-digit Central Index Key<br/>
 --ticker TICKER       company ticker symbol<br/>
 --directory DIRECTORY<br/>
 directory to store the output<br/>
@@ -170,16 +172,16 @@
 usage: edgarquery [-h] [--cik CIK] [--ticker TICKER] [--cy CY]<br/>
 [--frame FRAME] [--units UNITS] [--fact FACT]<br/>
 [--directory DIRECTORY] [--file FILE] [--companyconcept]<br/>
 [--companyfacts] [--xbrlframes]<br/>
 [--companyfactsarchivezip] [--submissionszip]<br/>
 [--financialstatementandnotesdataset]<br/>
 <br/>
-query SEC EDGAR site NOTE thæt EQEMAIL env variable is required and must<br/>
-contain a valid User-Agent such as your email address<br/>
+query SEC EDGAR site for a ticker or cik NOTE thæt EQEMAIL env variable is<br/>
+required and must contain a valid User-Agent such as your email address<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --cik CIK             10-digit Central Index Key<br/>
 --ticker TICKER       company stock ticker<br/>
 --cy CY               calendar year e.g. CY2023, CY2023Q1, CY2023Q4I<br/>
 --frame FRAME         reporting frame e.g us-gaap, ifrs-full, dei, srt<br/>
@@ -209,15 +211,15 @@
 <br/>
 ##<br/>
 ## edgarsubmissions<br/>
 ##<br/>
 usage: edgarsubmissions [-h] [--cik CIK] [--ticker TICKER] [--year YEAR]<br/>
 [--file FILE] [--directory DIRECTORY]<br/>
 <br/>
-find the most recent submissions for cik<br/>
+find the most recent submissions for ticker or cik<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --cik CIK             10-digit Central Index Key<br/>
 --ticker TICKER       company ticker symbol<br/>
 --year YEAR           year to search for submissions if not current year<br/>
 --file FILE           store the output in this file<br/>
```

### Comparing `edgarquery-0.0.60/pyproject.toml` & `edgarquery-0.0.61/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.60/PKG-INFO` & `edgarquery-0.0.61/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgarquery
-Version: 0.0.60
+Version: 0.0.61
 Summary: Downloads various SEC EDGAR files by CIK or ticker.  companyfactsshow displays company facts in your browser
 Project-URL: Documentation, https://github.com/dfwcnj/edgarquery#readme
 Project-URL: Issues, https://github.com/dfwcnj/edgarquery/issues
 Project-URL: Source, https://github.com/dfwcnj/edgarquery
 Author-email: Don Caldwell <dfwcnj@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -82,15 +82,15 @@
 <br/>
 ##<br/>
 ## edgarcompanyfactsshow<br/>
 ##<br/>
 usage: edgarcompanyfactsshow [-h] [--cik CIK] [--ticker TICKER]<br/>
 [--directory DIRECTORY]<br/>
 <br/>
-parse EDGAR company facts for a cik and display them in a browser<br/>
+parse EDGAR company facts for a ticker or cik and display them in a browser<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --cik CIK             Centralized Index Key for the company<br/>
 --ticker TICKER       Ticker for the company<br/>
 --directory DIRECTORY<br/>
 where to store the html file to display<br/>
@@ -98,15 +98,16 @@
 <br/>
 ##<br/>
 ## edgarcompanyfactstocsv<br/>
 ##<br/>
 usage: edgarcompanyfactstocsv [-h] --file FILE [--directory DIRECTORY]<br/>
 <br/>
 Parse an SEC EDGAR companyfacts json file after it has been altered to deal<br/>
-with its multipart character and generate CSV files from its content<br/>
+with its multipart character and generate CSV files from its content. I think<br/>
+that the SEC fixed the multi-json bug<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --file FILE           json file to process<br/>
 --directory DIRECTORY<br/>
 where to deposit the csv fileѕ<br/>
 <br/>
@@ -132,15 +133,15 @@
 <br/>
 ##<br/>
 ## edgarlatest10K<br/>
 ##<br/>
 usage: edgarlatest10K [-h] [--cik CIK] [--ticker TICKER] [--link]<br/>
 [--directory DIRECTORY] [--show]<br/>
 <br/>
-find the most recent 10-K for cik<br/>
+find the most recent 10-K for ticker or cik<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --cik CIK             10-digit Central Index Key<br/>
 --ticker TICKER       company ticker symbol<br/>
 --link                return the url for the latest 10-K<br/>
 --directory DIRECTORY<br/>
@@ -151,15 +152,16 @@
 ##<br/>
 ## edgarlatestsubmission<br/>
 ##<br/>
 usage: edgarlatestsubmission [-h] [--cik CIK] [--ticker TICKER]<br/>
 [--submission {SC 13D,13F-HR,DEF 14A,8-K,10-K,10-Q}]<br/>
 [--link] [--directory DIRECTORY] [--show]<br/>
 <br/>
-find the most recent X-K for cik<br/>
+find the most recent submission for a ticker or cik for some common<br/>
+submissƣons.<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --cik CIK             10-digit Central Index Key<br/>
 --ticker TICKER       company ticker symbol<br/>
 --submission {SC 13D,13F-HR,DEF 14A,8-K,10-K,10-Q}<br/>
 X-K submission type<br/>
@@ -171,15 +173,15 @@
 <br/>
 ##<br/>
 ## edgarlatestsubmissions<br/>
 ##<br/>
 usage: edgarlatestsubmissions [-h] [--cik CIK] [--ticker TICKER]<br/>
 [--directory DIRECTORY] [--file FILE]<br/>
 <br/>
-find the most recent submissions for cik<br/>
+find the most recent submissions for a ticker or cik<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --cik CIK             10-digit Central Index Key<br/>
 --ticker TICKER       company ticker symbol<br/>
 --directory DIRECTORY<br/>
 directory to store the output<br/>
@@ -192,16 +194,16 @@
 usage: edgarquery [-h] [--cik CIK] [--ticker TICKER] [--cy CY]<br/>
 [--frame FRAME] [--units UNITS] [--fact FACT]<br/>
 [--directory DIRECTORY] [--file FILE] [--companyconcept]<br/>
 [--companyfacts] [--xbrlframes]<br/>
 [--companyfactsarchivezip] [--submissionszip]<br/>
 [--financialstatementandnotesdataset]<br/>
 <br/>
-query SEC EDGAR site NOTE thæt EQEMAIL env variable is required and must<br/>
-contain a valid User-Agent such as your email address<br/>
+query SEC EDGAR site for a ticker or cik NOTE thæt EQEMAIL env variable is<br/>
+required and must contain a valid User-Agent such as your email address<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --cik CIK             10-digit Central Index Key<br/>
 --ticker TICKER       company stock ticker<br/>
 --cy CY               calendar year e.g. CY2023, CY2023Q1, CY2023Q4I<br/>
 --frame FRAME         reporting frame e.g us-gaap, ifrs-full, dei, srt<br/>
@@ -231,15 +233,15 @@
 <br/>
 ##<br/>
 ## edgarsubmissions<br/>
 ##<br/>
 usage: edgarsubmissions [-h] [--cik CIK] [--ticker TICKER] [--year YEAR]<br/>
 [--file FILE] [--directory DIRECTORY]<br/>
 <br/>
-find the most recent submissions for cik<br/>
+find the most recent submissions for ticker or cik<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --cik CIK             10-digit Central Index Key<br/>
 --ticker TICKER       company ticker symbol<br/>
 --year YEAR           year to search for submissions if not current year<br/>
 --file FILE           store the output in this file<br/>
```

