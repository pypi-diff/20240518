# Comparing `tmp/pop_sort-0.2.tar.gz` & `tmp/pop_sort-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop_sort-0.2.tar", last modified: Sat May 18 11:59:26 2024, max compression
+gzip compressed data, was "pop_sort-1.0.tar", last modified: Sat May 18 15:16:21 2024, max compression
```

## Comparing `pop_sort-0.2.tar` & `pop_sort-1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 martynas  (1000) martynas  (1000)        0 2024-05-18 11:59:26.357528 pop_sort-0.2/
--rw-rw-r--   0 martynas  (1000) martynas  (1000)     1074 2024-04-17 16:48:17.000000 pop_sort-0.2/LICENSE
--rw-r--r--   0 martynas  (1000) martynas  (1000)      577 2024-05-18 11:59:26.357528 pop_sort-0.2/PKG-INFO
--rw-rw-r--   0 martynas  (1000) martynas  (1000)      102 2024-04-17 16:46:55.000000 pop_sort-0.2/README.md
-drwxrwxr-x   0 martynas  (1000) martynas  (1000)        0 2024-05-18 11:59:26.357528 pop_sort-0.2/pop_sort/
--rw-rw-r--   0 martynas  (1000) martynas  (1000)      184 2024-05-13 18:03:28.000000 pop_sort-0.2/pop_sort/__init__.py
--rw-rw-r--   0 martynas  (1000) martynas  (1000)      391 2024-05-13 18:15:55.000000 pop_sort-0.2/pop_sort/bubble_sort.py
--rw-rw-r--   0 martynas  (1000) martynas  (1000)      846 2024-05-13 18:15:55.000000 pop_sort-0.2/pop_sort/bucket_sort.py
--rw-rw-r--   0 martynas  (1000) martynas  (1000)      243 2024-05-13 17:56:30.000000 pop_sort-0.2/pop_sort/decorators.py
--rw-rw-r--   0 martynas  (1000) martynas  (1000)      430 2024-05-13 18:15:55.000000 pop_sort-0.2/pop_sort/insertion_sort.py
--rw-rw-r--   0 martynas  (1000) martynas  (1000)     1144 2024-05-13 18:11:56.000000 pop_sort-0.2/pop_sort/merge_sort.py
--rw-rw-r--   0 martynas  (1000) martynas  (1000)     1023 2024-05-13 18:15:43.000000 pop_sort-0.2/pop_sort/quick_sort.py
--rw-rw-r--   0 martynas  (1000) martynas  (1000)      442 2024-05-13 18:15:43.000000 pop_sort-0.2/pop_sort/selection_sort.py
-drwxrwxr-x   0 martynas  (1000) martynas  (1000)        0 2024-05-18 11:59:26.357528 pop_sort-0.2/pop_sort.egg-info/
--rw-r--r--   0 martynas  (1000) martynas  (1000)      577 2024-05-18 11:59:26.000000 pop_sort-0.2/pop_sort.egg-info/PKG-INFO
--rw-rw-r--   0 martynas  (1000) martynas  (1000)      383 2024-05-18 11:59:26.000000 pop_sort-0.2/pop_sort.egg-info/SOURCES.txt
--rw-rw-r--   0 martynas  (1000) martynas  (1000)        1 2024-05-18 11:59:26.000000 pop_sort-0.2/pop_sort.egg-info/dependency_links.txt
--rw-rw-r--   0 martynas  (1000) martynas  (1000)       15 2024-05-18 11:59:26.000000 pop_sort-0.2/pop_sort.egg-info/top_level.txt
--rw-rw-r--   0 martynas  (1000) martynas  (1000)       38 2024-05-18 11:59:26.357528 pop_sort-0.2/setup.cfg
--rw-rw-r--   0 martynas  (1000) martynas  (1000)      644 2024-05-13 18:20:44.000000 pop_sort-0.2/setup.py
-drwxrwxr-x   0 martynas  (1000) martynas  (1000)        0 2024-05-18 11:59:26.357528 pop_sort-0.2/tests/
--rw-rw-r--   0 martynas  (1000) martynas  (1000)       23 2024-04-17 18:39:52.000000 pop_sort-0.2/tests/__init__.py
--rw-rw-r--   0 martynas  (1000) martynas  (1000)     1983 2024-05-13 18:17:50.000000 pop_sort-0.2/tests/test_sort.py
+drwxrwxr-x   0 martynas  (1000) martynas  (1000)        0 2024-05-18 15:16:21.568019 pop_sort-1.0/
+-rw-rw-r--   0 martynas  (1000) martynas  (1000)     1074 2024-04-17 16:48:17.000000 pop_sort-1.0/LICENSE
+-rw-r--r--   0 martynas  (1000) martynas  (1000)      577 2024-05-18 15:16:21.568019 pop_sort-1.0/PKG-INFO
+-rw-rw-r--   0 martynas  (1000) martynas  (1000)      102 2024-04-17 16:46:55.000000 pop_sort-1.0/README.md
+drwxrwxr-x   0 martynas  (1000) martynas  (1000)        0 2024-05-18 15:16:21.568019 pop_sort-1.0/pop_sort/
+-rw-rw-r--   0 martynas  (1000) martynas  (1000)      254 2024-05-18 15:09:34.000000 pop_sort-1.0/pop_sort/__init__.py
+-rw-rw-r--   0 martynas  (1000) martynas  (1000)      451 2024-05-18 15:04:22.000000 pop_sort-1.0/pop_sort/bubble_sort.py
+-rw-rw-r--   0 martynas  (1000) martynas  (1000)     1072 2024-05-18 15:04:29.000000 pop_sort-1.0/pop_sort/bucket_sort.py
+-rw-rw-r--   0 martynas  (1000) martynas  (1000)      243 2024-05-18 14:19:41.000000 pop_sort-1.0/pop_sort/decorators.py
+-rw-rw-r--   0 martynas  (1000) martynas  (1000)      490 2024-05-18 15:04:37.000000 pop_sort-1.0/pop_sort/insertion_sort.py
+-rw-rw-r--   0 martynas  (1000) martynas  (1000)     1204 2024-05-18 15:04:46.000000 pop_sort-1.0/pop_sort/merge_sort.py
+-rw-rw-r--   0 martynas  (1000) martynas  (1000)     1083 2024-05-18 15:04:40.000000 pop_sort-1.0/pop_sort/quick_sort.py
+-rw-rw-r--   0 martynas  (1000) martynas  (1000)      502 2024-05-18 15:04:43.000000 pop_sort-1.0/pop_sort/selection_sort.py
+drwxrwxr-x   0 martynas  (1000) martynas  (1000)        0 2024-05-18 15:16:21.568019 pop_sort-1.0/pop_sort.egg-info/
+-rw-r--r--   0 martynas  (1000) martynas  (1000)      577 2024-05-18 15:16:21.000000 pop_sort-1.0/pop_sort.egg-info/PKG-INFO
+-rw-rw-r--   0 martynas  (1000) martynas  (1000)      383 2024-05-18 15:16:21.000000 pop_sort-1.0/pop_sort.egg-info/SOURCES.txt
+-rw-rw-r--   0 martynas  (1000) martynas  (1000)        1 2024-05-18 15:16:21.000000 pop_sort-1.0/pop_sort.egg-info/dependency_links.txt
+-rw-rw-r--   0 martynas  (1000) martynas  (1000)       15 2024-05-18 15:16:21.000000 pop_sort-1.0/pop_sort.egg-info/top_level.txt
+-rw-rw-r--   0 martynas  (1000) martynas  (1000)       38 2024-05-18 15:16:21.568019 pop_sort-1.0/setup.cfg
+-rw-rw-r--   0 martynas  (1000) martynas  (1000)      644 2024-05-18 15:05:08.000000 pop_sort-1.0/setup.py
+drwxrwxr-x   0 martynas  (1000) martynas  (1000)        0 2024-05-18 15:16:21.568019 pop_sort-1.0/tests/
+-rw-rw-r--   0 martynas  (1000) martynas  (1000)       23 2024-04-17 18:39:52.000000 pop_sort-1.0/tests/__init__.py
+-rw-rw-r--   0 martynas  (1000) martynas  (1000)     1983 2024-05-18 15:02:31.000000 pop_sort-1.0/tests/test_sort.py
```

### Comparing `pop_sort-0.2/LICENSE` & `pop_sort-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pop_sort-0.2/PKG-INFO` & `pop_sort-1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop_sort
-Version: 0.2
+Version: 1.0
 Summary: Project for exploring popular sorting algorithms.
 Home-page: https://github.com/MartynasGr/pop_sort
 Author: Martynas Greičius
 Author-email: martynas.greicius@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pop_sort-0.2/pop_sort/merge_sort.py` & `pop_sort-1.0/pop_sort/merge_sort.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 @reverse_decorator
 def merge_sort(arr, **kwargs):
     """
     Implementation of merge sort algorithm
     :param arr: Array to be sorted
+    :param reverse: True if sorted array should be reversed
     :return: Sorted array
     """
     if len(arr) <= 1:
         return arr
     mid = len(arr) // 2
     left = merge_sort(arr[:mid])
     right = merge_sort(arr[mid:])
```

### Comparing `pop_sort-0.2/pop_sort.egg-info/PKG-INFO` & `pop_sort-1.0/pop_sort.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-sort
-Version: 0.2
+Version: 1.0
 Summary: Project for exploring popular sorting algorithms.
 Home-page: https://github.com/MartynasGr/pop_sort
 Author: Martynas Greičius
 Author-email: martynas.greicius@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pop_sort-0.2/setup.py` & `pop_sort-1.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pop_sort',
-    version='0.2',
+    version='1.0',
     description='Project for exploring popular sorting algorithms.',
     long_description=open('README.md', 'r').read(),
     long_description_content_type="text/markdown",
     url='https://github.com/MartynasGr/pop_sort',
     author='Martynas Greičius',
     author_email='martynas.greicius@gmail.com',
     license='MIT',
```

### Comparing `pop_sort-0.2/tests/test_sort.py` & `pop_sort-1.0/tests/test_sort.py`

 * *Files identical despite different names*

