# Comparing `tmp/piligraphs-0.0.4.tar.gz` & `tmp/piligraphs-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piligraphs-0.0.4.tar", max compression
+gzip compressed data, was "piligraphs-0.0.5.tar", max compression
```

## Comparing `piligraphs-0.0.4.tar` & `piligraphs-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11558 2023-12-07 15:54:15.675037 piligraphs-0.0.4/LICENSE
--rw-r--r--   0        0        0      145 2024-05-14 13:21:11.131930 piligraphs-0.0.4/piligraphs/__init__.py
--rw-r--r--   0        0        0     6142 2024-05-15 09:43:37.430276 piligraphs-0.0.4/piligraphs/funcgraph.py
--rw-r--r--   0        0        0     1482 2024-05-14 13:20:33.858580 piligraphs-0.0.4/piligraphs/graph.py
--rw-r--r--   0        0        0     7231 2024-05-15 09:43:42.245524 piligraphs-0.0.4/piligraphs/linechart.py
--rw-r--r--   0        0        0     1119 2024-05-15 09:43:19.322384 piligraphs-0.0.4/piligraphs/node.py
--rw-r--r--   0        0        0     5703 2024-05-15 09:23:19.805282 piligraphs-0.0.4/piligraphs/piechart.py
--rw-r--r--   0        0        0     7555 2024-05-15 09:43:50.054767 piligraphs-0.0.4/piligraphs/radarchart.py
--rw-r--r--   0        0        0     3113 2024-05-16 08:53:49.165677 piligraphs-0.0.4/piligraphs/utils.py
--rw-r--r--   0        0        0      412 2024-05-12 15:23:19.816380 piligraphs-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1322 2024-05-16 08:52:26.375254 piligraphs-0.0.4/README.md
--rw-r--r--   0        0        0     1786 1970-01-01 00:00:00.000000 piligraphs-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-12-07 15:54:15.675037 piligraphs-0.0.5/LICENSE
+-rw-r--r--   0        0        0      145 2024-05-14 13:21:11.131930 piligraphs-0.0.5/piligraphs/__init__.py
+-rw-r--r--   0        0        0     6142 2024-05-15 09:43:37.430276 piligraphs-0.0.5/piligraphs/funcgraph.py
+-rw-r--r--   0        0        0     1482 2024-05-14 13:20:33.858580 piligraphs-0.0.5/piligraphs/graph.py
+-rw-r--r--   0        0        0     7231 2024-05-15 09:43:42.245524 piligraphs-0.0.5/piligraphs/linechart.py
+-rw-r--r--   0        0        0     1119 2024-05-15 09:43:19.322384 piligraphs-0.0.5/piligraphs/node.py
+-rw-r--r--   0        0        0     5703 2024-05-15 09:23:19.805282 piligraphs-0.0.5/piligraphs/piechart.py
+-rw-r--r--   0        0        0     7555 2024-05-15 09:43:50.054767 piligraphs-0.0.5/piligraphs/radarchart.py
+-rw-r--r--   0        0        0     3113 2024-05-16 08:53:49.165677 piligraphs-0.0.5/piligraphs/utils.py
+-rw-r--r--   0        0        0      489 2024-05-18 11:04:01.748179 piligraphs-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1468 2024-05-16 08:59:53.724586 piligraphs-0.0.5/README.md
+-rw-r--r--   0        0        0     2090 1970-01-01 00:00:00.000000 piligraphs-0.0.5/PKG-INFO
```

### Comparing `piligraphs-0.0.4/LICENSE` & `piligraphs-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `piligraphs-0.0.4/piligraphs/funcgraph.py` & `piligraphs-0.0.5/piligraphs/funcgraph.py`

 * *Files identical despite different names*

### Comparing `piligraphs-0.0.4/piligraphs/graph.py` & `piligraphs-0.0.5/piligraphs/graph.py`

 * *Files identical despite different names*

### Comparing `piligraphs-0.0.4/piligraphs/linechart.py` & `piligraphs-0.0.5/piligraphs/linechart.py`

 * *Files identical despite different names*

### Comparing `piligraphs-0.0.4/piligraphs/node.py` & `piligraphs-0.0.5/piligraphs/node.py`

 * *Files identical despite different names*

### Comparing `piligraphs-0.0.4/piligraphs/piechart.py` & `piligraphs-0.0.5/piligraphs/piechart.py`

 * *Files identical despite different names*

### Comparing `piligraphs-0.0.4/piligraphs/radarchart.py` & `piligraphs-0.0.5/piligraphs/radarchart.py`

 * *Files identical despite different names*

### Comparing `piligraphs-0.0.4/piligraphs/utils.py` & `piligraphs-0.0.5/piligraphs/utils.py`

 * *Files identical despite different names*

### Comparing `piligraphs-0.0.4/README.md` & `piligraphs-0.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![pypi](https://img.shields.io/pypi/v/piligraphs)](https://pypi.org/project/piligraphs)
 [![python](https://img.shields.io/badge/python-3.10-blue)](https://www.python.org/downloads)
 [![CodeFactor](https://www.codefactor.io/repository/github/eeemoon/piligraphs/badge)](https://www.codefactor.io/repository/github/eeemoon/piligraphs)
 [![BuyMeACoffee](https://img.shields.io/badge/support-yellow)](https://www.buymeacoffee.com/eeemoon)
 
 A [Pillow](https://github.com/python-pillow/Pillow) extension for drawing graphs and charts.
 
-![](examples/images/allgraphs.png)
+![](https://github.com/eeemoon/piligraphs/raw/master/examples/images/allgraphs.png)
 
 ## Installation
 To install this module, run the following command:
 ```
 pip install piligraphs
 ```
 
@@ -41,10 +41,10 @@
 chart.add_nodes(*nodes)
 
 # draw the graph
 image = chart.draw()
 image.show()
 ```
 Result:
-![](examples/images/linegraph.png)
+![](https://github.com/eeemoon/piligraphs/raw/master/examples/images/linegraph.png)
 
-You can find more examples [here.](examples/)
+You can find more examples [here.](https://github.com/eeemoon/piligraphs/raw/master/examples)
```

### Comparing `piligraphs-0.0.4/PKG-INFO` & `piligraphs-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
 Name: piligraphs
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Pillow extension for drawing graphs and charts.
 Home-page: https://github.com/eeemoon/piligraphs
 License: MIT
 Author: EeeMoon
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: Pillow (>=10.3.0,<11.0.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: pinkie (>=0.0.1,<0.0.2)
+Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # piligraphs
 [![pypi](https://img.shields.io/pypi/v/piligraphs)](https://pypi.org/project/piligraphs)
 [![python](https://img.shields.io/badge/python-3.10-blue)](https://www.python.org/downloads)
 [![CodeFactor](https://www.codefactor.io/repository/github/eeemoon/piligraphs/badge)](https://www.codefactor.io/repository/github/eeemoon/piligraphs)
 [![BuyMeACoffee](https://img.shields.io/badge/support-yellow)](https://www.buymeacoffee.com/eeemoon)
 
 A [Pillow](https://github.com/python-pillow/Pillow) extension for drawing graphs and charts.
 
-![](examples/images/allgraphs.png)
+![](https://github.com/eeemoon/piligraphs/raw/master/examples/images/allgraphs.png)
 
 ## Installation
 To install this module, run the following command:
 ```
 pip install piligraphs
 ```
 
@@ -56,11 +60,11 @@
 chart.add_nodes(*nodes)
 
 # draw the graph
 image = chart.draw()
 image.show()
 ```
 Result:
-![](examples/images/linegraph.png)
+![](https://github.com/eeemoon/piligraphs/raw/master/examples/images/linegraph.png)
 
-You can find more examples [here.](examples/)
+You can find more examples [here.](https://github.com/eeemoon/piligraphs/raw/master/examples)
```

