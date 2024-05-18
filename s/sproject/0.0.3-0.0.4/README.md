# Comparing `tmp/sproject-0.0.3.tar.gz` & `tmp/sproject-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sproject-0.0.3.tar", last modified: Mon Apr 15 03:38:29 2024, max compression
+gzip compressed data, was "sproject-0.0.4.tar", last modified: Sat May 18 08:47:40 2024, max compression
```

## Comparing `sproject-0.0.3.tar` & `sproject-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwx------   0 root         (0) root         (0)        0 2024-04-15 03:38:29.000000 sproject-0.0.3/
--rw-------   0 root         (0) root         (0)     1070 2024-04-07 05:12:27.000000 sproject-0.0.3/LICENSE.txt
--rw-------   0 root         (0) root         (0)      150 2024-04-15 03:38:29.000000 sproject-0.0.3/PKG-INFO
--rw-------   0 root         (0) root         (0)     1425 2024-04-07 05:12:27.000000 sproject-0.0.3/README.md
--rw-------   0 root         (0) root         (0)       38 2024-04-15 03:38:29.000000 sproject-0.0.3/setup.cfg
--rw-------   0 root         (0) root         (0)      423 2024-04-15 03:37:10.000000 sproject-0.0.3/setup.py
-drwx------   0 root         (0) root         (0)        0 2024-04-15 03:38:29.000000 sproject-0.0.3/sproject/
--rw-------   0 root         (0) root         (0)        0 2024-04-07 05:12:28.000000 sproject-0.0.3/sproject/__init__.py
--rw-------   0 root         (0) root         (0)     6634 2024-04-15 03:23:29.000000 sproject-0.0.3/sproject/file_organizer.py
-drwx------   0 root         (0) root         (0)        0 2024-04-15 03:38:29.000000 sproject-0.0.3/sproject.egg-info/
--rw-------   0 root         (0) root         (0)      150 2024-04-15 03:38:29.000000 sproject-0.0.3/sproject.egg-info/PKG-INFO
--rw-------   0 root         (0) root         (0)      206 2024-04-15 03:38:29.000000 sproject-0.0.3/sproject.egg-info/SOURCES.txt
--rw-------   0 root         (0) root         (0)        1 2024-04-15 03:38:29.000000 sproject-0.0.3/sproject.egg-info/dependency_links.txt
--rw-------   0 root         (0) root         (0)        9 2024-04-15 03:38:29.000000 sproject-0.0.3/sproject.egg-info/top_level.txt
+drwx------   0 root         (0) root         (0)        0 2024-05-18 08:47:40.000000 sproject-0.0.4/
+-rw-------   0 root         (0) root         (0)     1070 2024-05-18 04:27:19.000000 sproject-0.0.4/LICENSE.txt
+-rw-------   0 root         (0) root         (0)      171 2024-05-18 08:47:40.000000 sproject-0.0.4/PKG-INFO
+-rw-------   0 root         (0) root         (0)     1684 2024-05-18 04:27:19.000000 sproject-0.0.4/README.md
+-rw-------   0 root         (0) root         (0)       38 2024-05-18 08:47:40.000000 sproject-0.0.4/setup.cfg
+-rw-------   0 root         (0) root         (0)      444 2024-05-18 08:47:21.000000 sproject-0.0.4/setup.py
+drwx------   0 root         (0) root         (0)        0 2024-05-18 08:47:40.000000 sproject-0.0.4/sproject/
+-rw-------   0 root         (0) root         (0)        0 2024-05-18 04:27:19.000000 sproject-0.0.4/sproject/__init__.py
+-rw-------   0 root         (0) root         (0)     7569 2024-05-18 08:43:21.000000 sproject-0.0.4/sproject/file_organizer.py
+drwx------   0 root         (0) root         (0)        0 2024-05-18 08:47:40.000000 sproject-0.0.4/sproject.egg-info/
+-rw-------   0 root         (0) root         (0)      171 2024-05-18 08:47:40.000000 sproject-0.0.4/sproject.egg-info/PKG-INFO
+-rw-------   0 root         (0) root         (0)      206 2024-05-18 08:47:40.000000 sproject-0.0.4/sproject.egg-info/SOURCES.txt
+-rw-------   0 root         (0) root         (0)        1 2024-05-18 08:47:40.000000 sproject-0.0.4/sproject.egg-info/dependency_links.txt
+-rw-------   0 root         (0) root         (0)        9 2024-05-18 08:47:40.000000 sproject-0.0.4/sproject.egg-info/top_level.txt
```

### Comparing `sproject-0.0.3/LICENSE.txt` & `sproject-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sproject-0.0.3/README.md` & `sproject-0.0.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # API for finding same type of files and copy in a specific path
 
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)                 
 [![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)   
 
 [Follow Doveloper](https://www.instagram.com/nicky_connects/?next=%2F)
-## Functionality of the Music Player
+## Functionality of the Library
 
-- Better Optimization
-- Pause/Play Supported
-- Add/Delete songs from Playlist
-- Previous/Next song function
-- Time duration of song / next song displays
-- List of all the songs.
-- Adjust Volume
+- Copy/Move Files Recursively.
+- zip/unzip Files Recursively.
+- List all the files and folders and subfolders of given path.
+- In google drive you cannot directly see the size of the folder which is possible with sproject.
+- count the number of files/folders and subfolders recursively.
+- Encrypt and Decrypt the files using AES algorithm.(Better results with Minimum of 8GB RAM)
+- You can Split and Merge the large file into Smaller Chunks and viceversa.
 - Automatically Playing in Queue
 - Play Selected song from Playlist
 
 ## Usage
 
 - Make sure you have Python installed in your system.
 - Run Following command in the CMD.
  ```
-  pip install NTools
+  pip install sproject
   ```
 ## Example
 
  ```
  #test.py
 from NTools import copy_files
```

