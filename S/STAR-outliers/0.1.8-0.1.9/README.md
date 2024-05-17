# Comparing `tmp/STAR_outliers-0.1.8.tar.gz` & `tmp/STAR_outliers-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\STAR_outliers-0.1.8.tar", last modified: Tue Jun 29 16:04:04 2021, max compression
+gzip compressed data, was "dist\STAR_outliers-0.1.9.tar", last modified: Tue Jun 29 17:19:00 2021, max compression
```

## Comparing `STAR_outliers-0.1.8.tar` & `STAR_outliers-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2021-06-29 16:04:04.525893 STAR_outliers-0.1.8/
--rw-rw-rw-   0        0        0      868 2021-06-29 16:04:04.525893 STAR_outliers-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2469 2021-06-24 19:02:24.000000 STAR_outliers-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2021-06-29 16:04:04.513927 STAR_outliers-0.1.8/STAR_outliers.egg-info/
--rw-rw-rw-   0        0        0      868 2021-06-29 16:04:04.000000 STAR_outliers-0.1.8/STAR_outliers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2021-06-29 16:04:04.000000 STAR_outliers-0.1.8/STAR_outliers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-29 16:04:04.000000 STAR_outliers-0.1.8/STAR_outliers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2021-06-29 16:04:04.000000 STAR_outliers-0.1.8/STAR_outliers.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2021-06-29 16:04:04.000000 STAR_outliers-0.1.8/STAR_outliers.egg-info/requires.txt
--rw-rw-rw-   0        0        0      129 2021-06-29 16:04:04.000000 STAR_outliers-0.1.8/STAR_outliers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2566 2021-06-24 20:35:00.000000 STAR_outliers-0.1.8/STAR_outliers.py
--rw-rw-rw-   0        0        0    12102 2021-06-29 15:32:49.000000 STAR_outliers-0.1.8/STAR_outliers_library.py
--rw-rw-rw-   0        0        0     6846 2021-06-28 20:52:25.000000 STAR_outliers-0.1.8/STAR_outliers_plotting_library.py
--rw-rw-rw-   0        0        0     7217 2021-06-24 19:02:24.000000 STAR_outliers-0.1.8/STAR_outliers_polishing_library.py
--rw-rw-rw-   0        0        0     3254 2021-06-24 19:02:24.000000 STAR_outliers-0.1.8/STAR_outliers_testing_library.py
--rw-rw-rw-   0        0        0       42 2021-06-29 16:04:04.525893 STAR_outliers-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1670 2021-06-29 15:58:21.000000 STAR_outliers-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-06-29 16:04:04.523898 STAR_outliers-0.1.8/test/
--rw-rw-rw-   0        0        0     1417 2021-06-08 21:33:34.000000 STAR_outliers-0.1.8/test/test_output.py
+drwxrwxrwx   0        0        0        0 2021-06-29 17:19:00.777513 STAR_outliers-0.1.9/
+-rw-rw-rw-   0        0        0      868 2021-06-29 17:19:00.776521 STAR_outliers-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2021-06-29 17:19:00.773524 STAR_outliers-0.1.9/STAR_outliers.egg-info/
+-rw-rw-rw-   0        0        0      868 2021-06-29 17:19:00.000000 STAR_outliers-0.1.9/STAR_outliers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2021-06-29 17:19:00.000000 STAR_outliers-0.1.9/STAR_outliers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-06-29 17:19:00.000000 STAR_outliers-0.1.9/STAR_outliers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2021-06-29 17:19:00.000000 STAR_outliers-0.1.9/STAR_outliers.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2021-06-29 17:19:00.000000 STAR_outliers-0.1.9/STAR_outliers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      129 2021-06-29 17:19:00.000000 STAR_outliers-0.1.9/STAR_outliers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2758 2021-06-29 16:59:46.000000 STAR_outliers-0.1.9/STAR_outliers.py
+-rw-rw-rw-   0        0        0    12102 2021-06-29 15:32:49.000000 STAR_outliers-0.1.9/STAR_outliers_library.py
+-rw-rw-rw-   0        0        0     6846 2021-06-28 20:52:25.000000 STAR_outliers-0.1.9/STAR_outliers_plotting_library.py
+-rw-rw-rw-   0        0        0     7217 2021-06-24 19:02:24.000000 STAR_outliers-0.1.9/STAR_outliers_polishing_library.py
+-rw-rw-rw-   0        0        0     3254 2021-06-24 19:02:24.000000 STAR_outliers-0.1.9/STAR_outliers_testing_library.py
+-rw-rw-rw-   0        0        0       42 2021-06-29 17:19:00.777513 STAR_outliers-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1670 2021-06-29 17:18:15.000000 STAR_outliers-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-06-29 17:19:00.774522 STAR_outliers-0.1.9/test/
+-rw-rw-rw-   0        0        0     1417 2021-06-08 21:33:34.000000 STAR_outliers-0.1.9/test/test_output.py
```

### Comparing `STAR_outliers-0.1.8/PKG-INFO` & `STAR_outliers-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: STAR_outliers
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: STAR_outliers (Skew and Tail-heaviness Adjusted Removal of outliers) is an open source python package that determines which points are outliers relative to their distributions shapes. An exponential tail fit is used to determine outlier status if the distribution behaves in a sufficiently exponential-like manner. Otherwise, the data is transformed and fitted to a four parameteter tukey distribution as described in the paper titled 'Outlier identification for skewed and/or heavy-tailed unimodal multivariate distributions'. 
         
         please visit the [github page](https://github.com/EpistasisLab/STAR_outliers) for more information.
 Platform: UNKNOWN
```

### Comparing `STAR_outliers-0.1.8/STAR_outliers.egg-info/PKG-INFO` & `STAR_outliers-0.1.9/STAR_outliers.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: STAR-outliers
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: STAR_outliers (Skew and Tail-heaviness Adjusted Removal of outliers) is an open source python package that determines which points are outliers relative to their distributions shapes. An exponential tail fit is used to determine outlier status if the distribution behaves in a sufficiently exponential-like manner. Otherwise, the data is transformed and fitted to a four parameteter tukey distribution as described in the paper titled 'Outlier identification for skewed and/or heavy-tailed unimodal multivariate distributions'. 
         
         please visit the [github page](https://github.com/EpistasisLab/STAR_outliers) for more information.
 Platform: UNKNOWN
```

### Comparing `STAR_outliers-0.1.8/STAR_outliers.py` & `STAR_outliers-0.1.9/STAR_outliers.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('--input ', type = str, action = "store", dest = "input")
     parser.add_argument('--index ', type = str, action = "store", dest = "index")
     parser.add_argument('--bound ', type = float, action = "store", dest = "bound")
     parser.add_argument('--pcutoff ', type = float, action = "store", dest = "pcutoff")
-
+    parser.add_argument('--seed ', type = float, action = "store", dest = "seed")
+    
+    seed = parser.parse_args().seed
+    if not seed is None:
+        np.random.seed(seed = int(seed))
     pcutoff = parser.parse_args().pcutoff
     if pcutoff is None:
         pcutoff = 0.993
     input_file_name = parser.parse_args().input
     index_name = parser.parse_args().index
     bound = parser.parse_args().bound
     split_name = input_file_name.split(".")
```

### Comparing `STAR_outliers-0.1.8/STAR_outliers_library.py` & `STAR_outliers-0.1.9/STAR_outliers_library.py`

 * *Files identical despite different names*

### Comparing `STAR_outliers-0.1.8/STAR_outliers_plotting_library.py` & `STAR_outliers-0.1.9/STAR_outliers_plotting_library.py`

 * *Files identical despite different names*

### Comparing `STAR_outliers-0.1.8/STAR_outliers_polishing_library.py` & `STAR_outliers-0.1.9/STAR_outliers_polishing_library.py`

 * *Files identical despite different names*

### Comparing `STAR_outliers-0.1.8/STAR_outliers_testing_library.py` & `STAR_outliers-0.1.9/STAR_outliers_testing_library.py`

 * *Files identical despite different names*

### Comparing `STAR_outliers-0.1.8/setup.py` & `STAR_outliers-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 summary += "Lab/STAR_outliers) for more information."
 
 ep_val = {"console_scripts": ["STAR_outliers = STAR_outliers:main"]}
 setup(
     long_description = summary,
     long_description_content_type = "text/markdown",
     packages = find_packages(),
-    version = "0.1.8",
+    version = "0.1.9",
     python_requires = ">=3.6,<=3.9",
     name = "STAR_outliers",
     entry_points = ep_val,
     py_modules=["STAR_outliers", "STAR_outliers_library",
                 "STAR_outliers_plotting_library",
                 "STAR_outliers_polishing_library",
                 "STAR_outliers_testing_library"],
```

### Comparing `STAR_outliers-0.1.8/test/test_output.py` & `STAR_outliers-0.1.9/test/test_output.py`

 * *Files identical despite different names*

