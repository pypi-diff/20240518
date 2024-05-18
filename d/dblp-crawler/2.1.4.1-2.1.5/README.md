# Comparing `tmp/dblp_crawler-2.1.4.1.tar.gz` & `tmp/dblp_crawler-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dblp_crawler-2.1.4.1.tar", last modified: Mon Mar  4 03:44:16 2024, max compression
+gzip compressed data, was "dblp_crawler-2.1.5.tar", last modified: Sat May 18 03:55:55 2024, max compression
```

## Comparing `dblp_crawler-2.1.4.1.tar` & `dblp_crawler-2.1.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 03:44:16.863302 dblp_crawler-2.1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-03-04 03:44:16.863302 dblp_crawler-2.1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 03:44:16.859302 dblp_crawler-2.1.4.1/dblp_crawler/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/arg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 03:44:16.859302 dblp_crawler-2.1.4.1/dblp_crawler/data/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 03:44:16.859302 dblp_crawler-2.1.4.1/dblp_crawler/data/ccf/
--rw-r--r--   0 runner    (1001) docker     (127)     9544 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/data/ccf/CCF_A.py
--rw-r--r--   0 runner    (1001) docker     (127)    26883 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/data/ccf/CCF_B.py
--rw-r--r--   0 runner    (1001) docker     (127)    33160 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/data/ccf/CCF_C.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/data/ccf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/data/ccf/key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/data/ccf/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/data/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 03:44:16.863302 dblp_crawler-2.1.4.1/dblp_crawler/filter/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/filter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/filter/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/journal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 03:44:16.863302 dblp_crawler-2.1.4.1/dblp_crawler/keyword/
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/keyword/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/keyword/arg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 03:44:16.863302 dblp_crawler-2.1.4.1/dblp_crawler/summarizer/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/summarizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/summarizer/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/dblp_crawler/summarizer/networkx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 03:44:16.859302 dblp_crawler-2.1.4.1/dblp_crawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-03-04 03:44:16.000000 dblp_crawler-2.1.4.1/dblp_crawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-04 03:44:16.000000 dblp_crawler-2.1.4.1/dblp_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 03:44:16.000000 dblp_crawler-2.1.4.1/dblp_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-04 03:44:16.000000 dblp_crawler-2.1.4.1/dblp_crawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-04 03:44:16.000000 dblp_crawler-2.1.4.1/dblp_crawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 03:44:16.863302 dblp_crawler-2.1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-04 03:44:10.000000 dblp_crawler-2.1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 03:55:55.511183 dblp_crawler-2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-18 03:55:55.507183 dblp_crawler-2.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 03:55:55.507183 dblp_crawler-2.1.5/dblp_crawler/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/arg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 03:55:55.507183 dblp_crawler-2.1.5/dblp_crawler/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 03:55:55.507183 dblp_crawler-2.1.5/dblp_crawler/data/ccf/
+-rw-r--r--   0 runner    (1001) docker     (127)     9544 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/data/ccf/CCF_A.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26883 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/data/ccf/CCF_B.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33160 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/data/ccf/CCF_C.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/data/ccf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/data/ccf/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/data/ccf/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/data/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 03:55:55.507183 dblp_crawler-2.1.5/dblp_crawler/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/filter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/filter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/journal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 03:55:55.507183 dblp_crawler-2.1.5/dblp_crawler/keyword/
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/keyword/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/keyword/arg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 03:55:55.507183 dblp_crawler-2.1.5/dblp_crawler/summarizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/summarizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/summarizer/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/dblp_crawler/summarizer/networkx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 03:55:55.507183 dblp_crawler-2.1.5/dblp_crawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-18 03:55:55.000000 dblp_crawler-2.1.5/dblp_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-18 03:55:55.000000 dblp_crawler-2.1.5/dblp_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 03:55:55.000000 dblp_crawler-2.1.5/dblp_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-18 03:55:55.000000 dblp_crawler-2.1.5/dblp_crawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-18 03:55:55.000000 dblp_crawler-2.1.5/dblp_crawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 03:55:55.511183 dblp_crawler-2.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-18 03:55:47.000000 dblp_crawler-2.1.5/setup.py
```

### Comparing `dblp_crawler-2.1.4.1/LICENSE` & `dblp_crawler-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/PKG-INFO` & `dblp_crawler-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblp_crawler
-Version: 2.1.4.1
+Version: 2.1.5
 Summary: 异步高并发dblp爬虫，慎用
 Home-page: https://github.com/yindaheng98/dblp-crawler
 Author: yindaheng98
 Author-email: yindaheng98@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dblp_crawler-2.1.4.1/README.md` & `dblp_crawler-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler/__main__.py` & `dblp_crawler-2.1.5/dblp_crawler/__main__.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler/arg.py` & `dblp_crawler-2.1.5/dblp_crawler/arg.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler/data/ccf/CCF_A.py` & `dblp_crawler-2.1.5/dblp_crawler/data/ccf/CCF_A.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler/data/ccf/CCF_B.py` & `dblp_crawler-2.1.5/dblp_crawler/data/ccf/CCF_B.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler/data/ccf/CCF_C.py` & `dblp_crawler-2.1.5/dblp_crawler/data/ccf/CCF_C.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler/data/ccf/key.py` & `dblp_crawler-2.1.5/dblp_crawler/data/ccf/key.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler/data/ccf/parse.py` & `dblp_crawler-2.1.5/dblp_crawler/data/ccf/parse.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler/downloader.py` & `dblp_crawler-2.1.5/dblp_crawler/downloader.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler/filter/__init__.py` & `dblp_crawler-2.1.5/dblp_crawler/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler/filter/__main__.py` & `dblp_crawler-2.1.5/dblp_crawler/filter/__main__.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler/filter/utils.py` & `dblp_crawler-2.1.5/dblp_crawler/filter/utils.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler/gather.py` & `dblp_crawler-2.1.5/dblp_crawler/gather.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler/graph.py` & `dblp_crawler-2.1.5/dblp_crawler/graph.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler/journal.py` & `dblp_crawler-2.1.5/dblp_crawler/journal.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler/keyword/__init__.py` & `dblp_crawler-2.1.5/dblp_crawler/keyword/__init__.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler/keyword/arg.py` & `dblp_crawler-2.1.5/dblp_crawler/keyword/arg.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler/parser.py` & `dblp_crawler-2.1.5/dblp_crawler/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
     def title(self) -> str:
         for child in self.data:
             if child.tag == "title":
                 return " ".join(t for t in child.itertext())
 
     def title_hash(self) -> str:
-        return re.sub(r"[^0-9a-z]", "", self.title().lower())
+        return re.sub(r"[^0-9a-z\u4e00-\u9fa5]", "", self.title().lower())
 
     def journal(self) -> Optional[str]:
         tag = {
             'inproceedings': 'booktitle',
             'proceedings': 'booktitle',
             'article': 'journal',
             'incollection': 'booktitle',
```

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler/summarizer/neo4j.py` & `dblp_crawler-2.1.5/dblp_crawler/summarizer/neo4j.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler/summarizer/networkx.py` & `dblp_crawler-2.1.5/dblp_crawler/summarizer/networkx.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler.egg-info/PKG-INFO` & `dblp_crawler-2.1.5/dblp_crawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblp-crawler
-Version: 2.1.4.1
+Version: 2.1.5
 Summary: 异步高并发dblp爬虫，慎用
 Home-page: https://github.com/yindaheng98/dblp-crawler
 Author: yindaheng98
 Author-email: yindaheng98@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dblp_crawler-2.1.4.1/dblp_crawler.egg-info/SOURCES.txt` & `dblp_crawler-2.1.5/dblp_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dblp_crawler-2.1.4.1/setup.py` & `dblp_crawler-2.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     'dblp_crawler.data.ccf': 'dblp_crawler/data/ccf',
     'dblp_crawler.keyword': 'dblp_crawler/keyword',
     'dblp_crawler.summarizer': 'dblp_crawler/summarizer',
 }
 
 setup(
     name='dblp_crawler',
-    version='2.1.4.1',
+    version='2.1.5',
     author='yindaheng98',
     author_email='yindaheng98@gmail.com',
     url='https://github.com/yindaheng98/dblp-crawler',
     description=u'异步高并发dblp爬虫，慎用',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir=package_dir,
```

