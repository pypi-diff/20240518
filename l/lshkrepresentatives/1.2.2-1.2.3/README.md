# Comparing `tmp/lshkrepresentatives-1.2.2.tar.gz` & `tmp/lshkrepresentatives-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lshkrepresentatives-1.2.2.tar", last modified: Thu Jan 25 08:17:09 2024, max compression
+gzip compressed data, was "lshkrepresentatives-1.2.3.tar", last modified: Sat May 18 07:03:42 2024, max compression
```

## Comparing `lshkrepresentatives-1.2.2.tar` & `lshkrepresentatives-1.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 08:17:09.358841 lshkrepresentatives-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-01-25 08:16:56.000000 lshkrepresentatives-1.2.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 08:17:09.354841 lshkrepresentatives-1.2.2/LSHkRepresentatives/
--rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-01-25 08:16:56.000000 lshkrepresentatives-1.2.2/LSHkRepresentatives/ClusteringAlgorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-01-25 08:16:56.000000 lshkrepresentatives-1.2.2/LSHkRepresentatives/DILCA.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-01-25 08:16:56.000000 lshkrepresentatives-1.2.2/LSHkRepresentatives/LSH.py
--rw-r--r--   0 runner    (1001) docker     (127)    14342 2024-01-25 08:16:56.000000 lshkrepresentatives-1.2.2/LSHkRepresentatives/LSHkPrototypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    19091 2024-01-25 08:16:56.000000 lshkrepresentatives-1.2.2/LSHkRepresentatives/LSHkRepresentatives.py
--rw-r--r--   0 runner    (1001) docker     (127)    19428 2024-01-25 08:16:56.000000 lshkrepresentatives-1.2.2/LSHkRepresentatives/LSHkRepresentatives_Full.py
--rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-01-25 08:16:56.000000 lshkrepresentatives-1.2.2/LSHkRepresentatives/MathUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-01-25 08:16:56.000000 lshkrepresentatives-1.2.2/LSHkRepresentatives/Measure.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-01-25 08:16:56.000000 lshkrepresentatives-1.2.2/LSHkRepresentatives/MeasureManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-01-25 08:16:56.000000 lshkrepresentatives-1.2.2/LSHkRepresentatives/SimpleHashing.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-25 08:16:56.000000 lshkrepresentatives-1.2.2/LSHkRepresentatives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-01-25 08:17:09.358841 lshkrepresentatives-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-01-25 08:16:56.000000 lshkrepresentatives-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 08:17:09.358841 lshkrepresentatives-1.2.2/lshkrepresentatives.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-01-25 08:17:09.000000 lshkrepresentatives-1.2.2/lshkrepresentatives.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-01-25 08:17:09.000000 lshkrepresentatives-1.2.2/lshkrepresentatives.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 08:17:09.000000 lshkrepresentatives-1.2.2/lshkrepresentatives.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-25 08:17:09.000000 lshkrepresentatives-1.2.2/lshkrepresentatives.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 08:17:09.358841 lshkrepresentatives-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-01-25 08:16:56.000000 lshkrepresentatives-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:03:42.627593 lshkrepresentatives-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-18 07:03:38.000000 lshkrepresentatives-1.2.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:03:42.627593 lshkrepresentatives-1.2.3/LSHkRepresentatives/
+-rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-05-18 07:03:38.000000 lshkrepresentatives-1.2.3/LSHkRepresentatives/ClusteringAlgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-18 07:03:38.000000 lshkrepresentatives-1.2.3/LSHkRepresentatives/DILCA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-18 07:03:38.000000 lshkrepresentatives-1.2.3/LSHkRepresentatives/LSH.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14346 2024-05-18 07:03:38.000000 lshkrepresentatives-1.2.3/LSHkRepresentatives/LSHkPrototypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19091 2024-05-18 07:03:38.000000 lshkrepresentatives-1.2.3/LSHkRepresentatives/LSHkRepresentatives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19428 2024-05-18 07:03:38.000000 lshkrepresentatives-1.2.3/LSHkRepresentatives/LSHkRepresentatives_Full.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-05-18 07:03:38.000000 lshkrepresentatives-1.2.3/LSHkRepresentatives/MathUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-18 07:03:38.000000 lshkrepresentatives-1.2.3/LSHkRepresentatives/Measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-18 07:03:38.000000 lshkrepresentatives-1.2.3/LSHkRepresentatives/MeasureManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-18 07:03:38.000000 lshkrepresentatives-1.2.3/LSHkRepresentatives/SimpleHashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-18 07:03:38.000000 lshkrepresentatives-1.2.3/LSHkRepresentatives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-18 07:03:42.627593 lshkrepresentatives-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-18 07:03:38.000000 lshkrepresentatives-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:03:42.627593 lshkrepresentatives-1.2.3/lshkrepresentatives.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-18 07:03:42.000000 lshkrepresentatives-1.2.3/lshkrepresentatives.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-18 07:03:42.000000 lshkrepresentatives-1.2.3/lshkrepresentatives.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 07:03:42.000000 lshkrepresentatives-1.2.3/lshkrepresentatives.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-18 07:03:42.000000 lshkrepresentatives-1.2.3/lshkrepresentatives.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 07:03:42.627593 lshkrepresentatives-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-18 07:03:38.000000 lshkrepresentatives-1.2.3/setup.py
```

### Comparing `lshkrepresentatives-1.2.2/LICENSE` & `lshkrepresentatives-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lshkrepresentatives-1.2.2/LSHkRepresentatives/ClusteringAlgorithm.py` & `lshkrepresentatives-1.2.3/LSHkRepresentatives/ClusteringAlgorithm.py`

 * *Files identical despite different names*

### Comparing `lshkrepresentatives-1.2.2/LSHkRepresentatives/DILCA.py` & `lshkrepresentatives-1.2.3/LSHkRepresentatives/DILCA.py`

 * *Files identical despite different names*

### Comparing `lshkrepresentatives-1.2.2/LSHkRepresentatives/LSH.py` & `lshkrepresentatives-1.2.3/LSHkRepresentatives/LSH.py`

 * *Files identical despite different names*

### Comparing `lshkrepresentatives-1.2.2/LSHkRepresentatives/LSHkPrototypes.py` & `lshkrepresentatives-1.2.3/LSHkRepresentatives/LSHkPrototypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,17 +74,17 @@
             representatives_count[from_id][ii][val]-=1
 
 
         means_count[to_id] += 1
         means_count[from_id] -= 1
 
         if  len(means_sum.shape)>1:
-            for ki in range(self.k):
-                means_sum[to_id][ki] += self.X_NUM[point_id][ki]
-                means_sum[from_id][ki] -= self.X_NUM[point_id][ki]
+            for di in range(self.d_NUM):
+                means_sum[to_id][di] += self.X_NUM[point_id][di]
+                means_sum[from_id][di] -= self.X_NUM[point_id][di]
 
     def CheckEmptyClusters(self,representatives, X,representatives_sum, representatives_count,membship,labels_matrix,means_count,means_sum,means):
         move =0
         big_cluster_id = -1
         for ki in range(self.k):
             if representatives_sum[ki] ==0 :
                 big_cluster_id = np.argmax([sum(mem_) for mem_ in membship])
```

### Comparing `lshkrepresentatives-1.2.2/LSHkRepresentatives/LSHkRepresentatives.py` & `lshkrepresentatives-1.2.3/LSHkRepresentatives/LSHkRepresentatives.py`

 * *Files identical despite different names*

### Comparing `lshkrepresentatives-1.2.2/LSHkRepresentatives/LSHkRepresentatives_Full.py` & `lshkrepresentatives-1.2.3/LSHkRepresentatives/LSHkRepresentatives_Full.py`

 * *Files identical despite different names*

### Comparing `lshkrepresentatives-1.2.2/LSHkRepresentatives/MathUtils.py` & `lshkrepresentatives-1.2.3/LSHkRepresentatives/MathUtils.py`

 * *Files identical despite different names*

### Comparing `lshkrepresentatives-1.2.2/LSHkRepresentatives/Measure.py` & `lshkrepresentatives-1.2.3/LSHkRepresentatives/Measure.py`

 * *Files identical despite different names*

### Comparing `lshkrepresentatives-1.2.2/LSHkRepresentatives/MeasureManager.py` & `lshkrepresentatives-1.2.3/LSHkRepresentatives/MeasureManager.py`

 * *Files identical despite different names*

### Comparing `lshkrepresentatives-1.2.2/LSHkRepresentatives/SimpleHashing.py` & `lshkrepresentatives-1.2.3/LSHkRepresentatives/SimpleHashing.py`

 * *Files identical despite different names*

### Comparing `lshkrepresentatives-1.2.2/PKG-INFO` & `lshkrepresentatives-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lshkrepresentatives
-Version: 1.2.2
+Version: 1.2.3
 Summary: LSH-k-Representatives: Mixed categorial and numerical (ordinal and nonordinal) data clustering algorithm algorithm
 Home-page: https://github.com/nmtoan91/lshkrepresentatives
 Author: nmtoan91
 Author-email: toan_stt@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lshkrepresentatives-1.2.2/README.md` & `lshkrepresentatives-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `lshkrepresentatives-1.2.2/lshkrepresentatives.egg-info/PKG-INFO` & `lshkrepresentatives-1.2.3/lshkrepresentatives.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lshkrepresentatives
-Version: 1.2.2
+Version: 1.2.3
 Summary: LSH-k-Representatives: Mixed categorial and numerical (ordinal and nonordinal) data clustering algorithm algorithm
 Home-page: https://github.com/nmtoan91/lshkrepresentatives
 Author: nmtoan91
 Author-email: toan_stt@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lshkrepresentatives-1.2.2/lshkrepresentatives.egg-info/SOURCES.txt` & `lshkrepresentatives-1.2.3/lshkrepresentatives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lshkrepresentatives-1.2.2/setup.py` & `lshkrepresentatives-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lshkrepresentatives", 
-    version="1.2.2",
+    version="1.2.3",
     author="nmtoan91",
     author_email="toan_stt@yahoo.com",
     description="LSH-k-Representatives: Mixed categorial and numerical (ordinal and nonordinal) data clustering algorithm algorithm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nmtoan91/lshkrepresentatives",
     packages=setuptools.find_packages(),
```

