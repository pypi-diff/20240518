# Comparing `tmp/TrackingNet-0.0.7.tar.gz` & `tmp/TrackingNet-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrackingNet-0.0.7.tar", last modified: Sun Jan  9 09:10:21 2022, max compression
+gzip compressed data, was "TrackingNet-0.0.8.tar", last modified: Sat May 18 19:20:31 2024, max compression
```

## Comparing `TrackingNet-0.0.7.tar` & `TrackingNet-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 giancos  (47541975) KAUST\Domain Users (1840429327)        0 2022-01-09 09:10:21.762265 TrackingNet-0.0.7/
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)      493 2022-01-09 08:26:33.000000 TrackingNet-0.0.7/MANIFEST.in
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)     1944 2022-01-09 09:10:21.761855 TrackingNet-0.0.7/PKG-INFO
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)      857 2022-01-09 08:26:33.000000 TrackingNet-0.0.7/README.md
-drwxr-xr-x   0 giancos  (47541975) KAUST\Domain Users (1840429327)        0 2022-01-09 09:10:21.743738 TrackingNet-0.0.7/TrackingNet/
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)     5134 2022-01-09 09:08:25.000000 TrackingNet-0.0.7/TrackingNet/Downloader.py
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)     1257 2022-01-09 09:09:02.000000 TrackingNet-0.0.7/TrackingNet/__init__.py
-drwxr-xr-x   0 giancos  (47541975) KAUST\Domain Users (1840429327)        0 2022-01-09 09:10:21.760799 TrackingNet-0.0.7/TrackingNet/data/
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)    12834 2022-01-09 08:26:33.000000 TrackingNet-0.0.7/TrackingNet/data/TEST.json
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)    62869 2022-01-09 08:26:33.000000 TrackingNet-0.0.7/TrackingNet/data/TRAIN_0.json
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)    65360 2022-01-09 08:26:33.000000 TrackingNet-0.0.7/TrackingNet/data/TRAIN_1.json
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)    65363 2022-01-09 08:26:33.000000 TrackingNet-0.0.7/TrackingNet/data/TRAIN_10.json
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)    65364 2022-01-09 08:26:33.000000 TrackingNet-0.0.7/TrackingNet/data/TRAIN_11.json
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)    65364 2022-01-09 08:26:33.000000 TrackingNet-0.0.7/TrackingNet/data/TRAIN_2.json
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)    65366 2022-01-09 08:26:33.000000 TrackingNet-0.0.7/TrackingNet/data/TRAIN_3.json
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)    65359 2022-01-09 08:26:33.000000 TrackingNet-0.0.7/TrackingNet/data/TRAIN_4.json
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)    65362 2022-01-09 08:26:33.000000 TrackingNet-0.0.7/TrackingNet/data/TRAIN_5.json
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)    65359 2022-01-09 08:26:33.000000 TrackingNet-0.0.7/TrackingNet/data/TRAIN_6.json
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)    65372 2022-01-09 08:26:33.000000 TrackingNet-0.0.7/TrackingNet/data/TRAIN_7.json
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)    65369 2022-01-09 08:26:33.000000 TrackingNet-0.0.7/TrackingNet/data/TRAIN_8.json
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)    65360 2022-01-09 08:26:33.000000 TrackingNet-0.0.7/TrackingNet/data/TRAIN_9.json
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)     1543 2022-01-09 08:26:33.000000 TrackingNet-0.0.7/TrackingNet/utils.py
-drwxr-xr-x   0 giancos  (47541975) KAUST\Domain Users (1840429327)        0 2022-01-09 09:10:21.746183 TrackingNet-0.0.7/TrackingNet.egg-info/
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)     1944 2022-01-09 09:10:21.000000 TrackingNet-0.0.7/TrackingNet.egg-info/PKG-INFO
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)      664 2022-01-09 09:10:21.000000 TrackingNet-0.0.7/TrackingNet.egg-info/SOURCES.txt
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)        1 2022-01-09 09:10:21.000000 TrackingNet-0.0.7/TrackingNet.egg-info/dependency_links.txt
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)       46 2022-01-09 09:10:21.000000 TrackingNet-0.0.7/TrackingNet.egg-info/requires.txt
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)       12 2022-01-09 09:10:21.000000 TrackingNet-0.0.7/TrackingNet.egg-info/top_level.txt
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)       38 2022-01-09 09:10:21.762402 TrackingNet-0.0.7/setup.cfg
--rw-r--r--   0 giancos  (47541975) KAUST\Domain Users (1840429327)     3722 2022-01-09 09:08:54.000000 TrackingNet-0.0.7/setup.py
+drwxr-xr-x   0 giancos  (47541975) 1840429327        0 2024-05-18 19:20:31.736177 TrackingNet-0.0.8/
+-rw-r--r--   0 giancos  (47541975) 1840429327      493 2022-01-09 08:26:33.000000 TrackingNet-0.0.8/MANIFEST.in
+-rw-r--r--   0 giancos  (47541975) 1840429327     1944 2024-05-18 19:20:31.735774 TrackingNet-0.0.8/PKG-INFO
+-rw-r--r--   0 giancos  (47541975) 1840429327      857 2022-01-09 08:26:33.000000 TrackingNet-0.0.8/README.md
+drwxr-xr-x   0 giancos  (47541975) 1840429327        0 2024-05-18 19:20:31.707795 TrackingNet-0.0.8/TrackingNet/
+-rw-r--r--   0 giancos  (47541975) 1840429327     5123 2024-05-18 19:16:35.000000 TrackingNet-0.0.8/TrackingNet/Downloader.py
+-rw-r--r--   0 giancos  (47541975) 1840429327     1257 2024-05-18 19:16:45.000000 TrackingNet-0.0.8/TrackingNet/__init__.py
+drwxr-xr-x   0 giancos  (47541975) 1840429327        0 2024-05-18 19:20:31.734741 TrackingNet-0.0.8/TrackingNet/data/
+-rw-r--r--   0 giancos  (47541975) 1840429327    12834 2022-01-09 08:26:33.000000 TrackingNet-0.0.8/TrackingNet/data/TEST.json
+-rw-r--r--   0 giancos  (47541975) 1840429327    62869 2022-01-09 08:26:33.000000 TrackingNet-0.0.8/TrackingNet/data/TRAIN_0.json
+-rw-r--r--   0 giancos  (47541975) 1840429327    65360 2022-01-09 08:26:33.000000 TrackingNet-0.0.8/TrackingNet/data/TRAIN_1.json
+-rw-r--r--   0 giancos  (47541975) 1840429327    65363 2022-01-09 08:26:33.000000 TrackingNet-0.0.8/TrackingNet/data/TRAIN_10.json
+-rw-r--r--   0 giancos  (47541975) 1840429327    65364 2022-01-09 08:26:33.000000 TrackingNet-0.0.8/TrackingNet/data/TRAIN_11.json
+-rw-r--r--   0 giancos  (47541975) 1840429327    65364 2022-01-09 08:26:33.000000 TrackingNet-0.0.8/TrackingNet/data/TRAIN_2.json
+-rw-r--r--   0 giancos  (47541975) 1840429327    65366 2022-01-09 08:26:33.000000 TrackingNet-0.0.8/TrackingNet/data/TRAIN_3.json
+-rw-r--r--   0 giancos  (47541975) 1840429327    65359 2022-01-09 08:26:33.000000 TrackingNet-0.0.8/TrackingNet/data/TRAIN_4.json
+-rw-r--r--   0 giancos  (47541975) 1840429327    65362 2022-01-09 08:26:33.000000 TrackingNet-0.0.8/TrackingNet/data/TRAIN_5.json
+-rw-r--r--   0 giancos  (47541975) 1840429327    65359 2022-01-09 08:26:33.000000 TrackingNet-0.0.8/TrackingNet/data/TRAIN_6.json
+-rw-r--r--   0 giancos  (47541975) 1840429327    65372 2022-01-09 08:26:33.000000 TrackingNet-0.0.8/TrackingNet/data/TRAIN_7.json
+-rw-r--r--   0 giancos  (47541975) 1840429327    65369 2022-01-09 08:26:33.000000 TrackingNet-0.0.8/TrackingNet/data/TRAIN_8.json
+-rw-r--r--   0 giancos  (47541975) 1840429327    65360 2022-01-09 08:26:33.000000 TrackingNet-0.0.8/TrackingNet/data/TRAIN_9.json
+-rw-r--r--   0 giancos  (47541975) 1840429327     1543 2022-01-09 08:26:33.000000 TrackingNet-0.0.8/TrackingNet/utils.py
+drwxr-xr-x   0 giancos  (47541975) 1840429327        0 2024-05-18 19:20:31.713491 TrackingNet-0.0.8/TrackingNet.egg-info/
+-rw-r--r--   0 giancos  (47541975) 1840429327     1944 2024-05-18 19:20:31.000000 TrackingNet-0.0.8/TrackingNet.egg-info/PKG-INFO
+-rw-r--r--   0 giancos  (47541975) 1840429327      664 2024-05-18 19:20:31.000000 TrackingNet-0.0.8/TrackingNet.egg-info/SOURCES.txt
+-rw-r--r--   0 giancos  (47541975) 1840429327        1 2024-05-18 19:20:31.000000 TrackingNet-0.0.8/TrackingNet.egg-info/dependency_links.txt
+-rw-r--r--   0 giancos  (47541975) 1840429327       46 2024-05-18 19:20:31.000000 TrackingNet-0.0.8/TrackingNet.egg-info/requires.txt
+-rw-r--r--   0 giancos  (47541975) 1840429327       12 2024-05-18 19:20:31.000000 TrackingNet-0.0.8/TrackingNet.egg-info/top_level.txt
+-rw-r--r--   0 giancos  (47541975) 1840429327       38 2024-05-18 19:20:31.736342 TrackingNet-0.0.8/setup.cfg
+-rw-r--r--   0 giancos  (47541975) 1840429327     3722 2022-01-09 09:08:54.000000 TrackingNet-0.0.8/setup.py
```

### Comparing `TrackingNet-0.0.7/PKG-INFO` & `TrackingNet-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrackingNet
-Version: 0.0.7
+Version: 0.0.8
 Summary: TrackingNet SDK
 Home-page: https://github.com/SilvioGiancola/TrackingNet
 Author: Silvio Giancola
 Author-email: silvio.giancola@kaust.edu.sa
 License: MIT
 Keywords: TrackingNet,SDK,Tracking,Video
 Platform: UNKNOWN
```

### Comparing `TrackingNet-0.0.7/README.md` & `TrackingNet-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `TrackingNet-0.0.7/TrackingNet/Downloader.py` & `TrackingNet-0.0.8/TrackingNet/Downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         report('UA-99166333-5', self.client_id, data)
 
         return 0
 
 
 class TrackingNetDownloader(OwnCloudDownloader):
     def __init__(self, LocalDirectory,
-                 OwnCloudServer="https://exrcsdrive.kaust.edu.sa/exrcsdrive/public.php/webdav/"):
+                 OwnCloudServer="https://exrcsdrive.kaust.edu.sa/public.php/webdav/"):
         super(TrackingNetDownloader, self).__init__(
             LocalDirectory, OwnCloudServer)
 
     def downloadZippedSPLIT(self, split):
 
         FileLocal = os.path.join(self.LocalDirectory, split+".zip")
         FileURL = os.path.join(self.OwnCloudServer,
```

### Comparing `TrackingNet-0.0.7/TrackingNet/__init__.py` & `TrackingNet-0.0.8/TrackingNet/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version_info__ = ('0', '0', '7')
+__version_info__ = ('0', '0', '8')
 __version__ = '.'.join(__version_info__)
 __authors__ = "Silvio Giancola"
 __authors_username__ = "giancos"
 __author_email__ = "silvio.giancola@kaust.edu.sa"
 __github__ = 'https://github.com/SilvioGiancola/TrackingNet'
```

### Comparing `TrackingNet-0.0.7/TrackingNet/data/TEST.json` & `TrackingNet-0.0.8/TrackingNet/data/TEST.json`

 * *Files identical despite different names*

### Comparing `TrackingNet-0.0.7/TrackingNet/data/TRAIN_0.json` & `TrackingNet-0.0.8/TrackingNet/data/TRAIN_0.json`

 * *Files identical despite different names*

### Comparing `TrackingNet-0.0.7/TrackingNet/data/TRAIN_1.json` & `TrackingNet-0.0.8/TrackingNet/data/TRAIN_1.json`

 * *Files identical despite different names*

### Comparing `TrackingNet-0.0.7/TrackingNet/data/TRAIN_10.json` & `TrackingNet-0.0.8/TrackingNet/data/TRAIN_10.json`

 * *Files identical despite different names*

### Comparing `TrackingNet-0.0.7/TrackingNet/data/TRAIN_11.json` & `TrackingNet-0.0.8/TrackingNet/data/TRAIN_11.json`

 * *Files identical despite different names*

### Comparing `TrackingNet-0.0.7/TrackingNet/data/TRAIN_2.json` & `TrackingNet-0.0.8/TrackingNet/data/TRAIN_2.json`

 * *Files identical despite different names*

### Comparing `TrackingNet-0.0.7/TrackingNet/data/TRAIN_3.json` & `TrackingNet-0.0.8/TrackingNet/data/TRAIN_3.json`

 * *Files identical despite different names*

### Comparing `TrackingNet-0.0.7/TrackingNet/data/TRAIN_4.json` & `TrackingNet-0.0.8/TrackingNet/data/TRAIN_4.json`

 * *Files identical despite different names*

### Comparing `TrackingNet-0.0.7/TrackingNet/data/TRAIN_5.json` & `TrackingNet-0.0.8/TrackingNet/data/TRAIN_5.json`

 * *Files identical despite different names*

### Comparing `TrackingNet-0.0.7/TrackingNet/data/TRAIN_6.json` & `TrackingNet-0.0.8/TrackingNet/data/TRAIN_6.json`

 * *Files identical despite different names*

### Comparing `TrackingNet-0.0.7/TrackingNet/data/TRAIN_7.json` & `TrackingNet-0.0.8/TrackingNet/data/TRAIN_7.json`

 * *Files identical despite different names*

### Comparing `TrackingNet-0.0.7/TrackingNet/data/TRAIN_8.json` & `TrackingNet-0.0.8/TrackingNet/data/TRAIN_8.json`

 * *Files identical despite different names*

### Comparing `TrackingNet-0.0.7/TrackingNet/data/TRAIN_9.json` & `TrackingNet-0.0.8/TrackingNet/data/TRAIN_9.json`

 * *Files identical despite different names*

### Comparing `TrackingNet-0.0.7/TrackingNet/utils.py` & `TrackingNet-0.0.8/TrackingNet/utils.py`

 * *Files identical despite different names*

### Comparing `TrackingNet-0.0.7/TrackingNet.egg-info/PKG-INFO` & `TrackingNet-0.0.8/TrackingNet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrackingNet
-Version: 0.0.7
+Version: 0.0.8
 Summary: TrackingNet SDK
 Home-page: https://github.com/SilvioGiancola/TrackingNet
 Author: Silvio Giancola
 Author-email: silvio.giancola@kaust.edu.sa
 License: MIT
 Keywords: TrackingNet,SDK,Tracking,Video
 Platform: UNKNOWN
```

### Comparing `TrackingNet-0.0.7/TrackingNet.egg-info/SOURCES.txt` & `TrackingNet-0.0.8/TrackingNet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TrackingNet-0.0.7/setup.py` & `TrackingNet-0.0.8/setup.py`

 * *Files identical despite different names*

