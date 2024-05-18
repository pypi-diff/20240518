# Comparing `tmp/faceext-0.0.2.tar.gz` & `tmp/faceext-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\faceext-0.0.2.tar", last modified: Tue Jul 20 05:14:38 2021, max compression
+gzip compressed data, was "faceext-0.0.3.tar", last modified: Sat May 18 05:38:43 2024, max compression
```

## Comparing `faceext-0.0.2.tar` & `faceext-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2021-07-20 05:14:38.000000 faceext-0.0.2/
--rw-rw-rw-   0        0        0     2509 2021-07-20 05:14:38.000000 faceext-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1458 2021-07-18 09:34:50.000000 faceext-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2021-07-20 05:14:38.000000 faceext-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      901 2021-07-20 05:08:14.000000 faceext-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2021-07-20 05:14:38.000000 faceext-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2021-07-20 05:14:38.000000 faceext-0.0.2/src/faceext.egg-info/
--rw-rw-rw-   0        0        0     2509 2021-07-20 05:14:38.000000 faceext-0.0.2/src/faceext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2021-07-20 05:14:38.000000 faceext-0.0.2/src/faceext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-20 05:14:38.000000 faceext-0.0.2/src/faceext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2021-07-20 05:14:38.000000 faceext-0.0.2/src/faceext.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2021-07-20 05:14:38.000000 faceext-0.0.2/src/faceext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2465 2021-07-20 05:13:58.000000 faceext-0.0.2/src/faceext.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-05-18 05:38:43.978412 faceext-0.0.3/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     2156 2024-05-18 05:38:43.978412 faceext-0.0.3/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1607 2024-05-18 05:30:21.000000 faceext-0.0.3/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-05-18 05:38:43.978412 faceext-0.0.3/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      966 2024-05-18 05:38:20.000000 faceext-0.0.3/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-05-18 05:38:43.978412 faceext-0.0.3/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-05-18 05:38:43.978412 faceext-0.0.3/src/faceext.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     2156 2024-05-18 05:38:43.000000 faceext-0.0.3/src/faceext.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      211 2024-05-18 05:38:43.000000 faceext-0.0.3/src/faceext.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-05-18 05:38:43.000000 faceext-0.0.3/src/faceext.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       42 2024-05-18 05:38:43.000000 faceext-0.0.3/src/faceext.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        8 2024-05-18 05:38:43.000000 faceext-0.0.3/src/faceext.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     2465 2021-07-20 05:13:58.000000 faceext-0.0.3/src/faceext.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `faceext-0.0.2/README.md` & `faceext-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # faceext
+This is under review.
+
 This is a faceext Python software for hiding all of your clothes and 
 background except your face.
 faceext.py is based on two state-of-the-art libraries including 
 mediapipe library for segmenting a face from the original image and 
 opencv library for superimposing faces and monotonous backgrounds 
 (black, white, or gray). 
 
+faceext has been downloaded 7876 times worldwide.
+
 OBS studio can play a virtual camera so that the crafted image of extracted face
 with superimposed monotonous background can be fed to remote meeting applications.
 Remote meeting applicaions including Zoom, WebEx, and Google meet
 were successfully tested.
 
 Python3.7 or Python3.8 is recommended.
 
@@ -24,14 +28,16 @@
 
 $ pip install opencv-python
 
 Finally install faceext
 
 $ pip install faceext
 
+$ pip install faceext --force-reinstall --no-cache-dir --no-binary :all:
+
 # How to run faceext
 Run faceext.
 
 $ faceext
 
 Your face with gray color background will be popped on the screen.
 
@@ -54,7 +60,8 @@
 
 Run any remote meeting application and select OBS virtual camera in video source selection.
 
 That is all.
 
 
 
+
```

### Comparing `faceext-0.0.2/setup.py` & `faceext-0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="faceext",
-    version="0.0.2",
+    version="0.0.3",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
-    description="faceext",
+    description="faceext for hiding all of your clothes and background except your face",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ytakefuji/faceext",
+    url="https://github.com/y-takefuji/faceext",
     project_urls={
-        "Bug Tracker": "https://github.com/ytakefuji/faceext",
+        "Bug Tracker": "https://github.com/y-takefuji/faceext",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     py_modules=['faceext'],
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     entry_points = {
         'console_scripts': [
             'faceext = faceext:main'
         ]
     },
 )
```

### Comparing `faceext-0.0.2/src/faceext.py` & `faceext-0.0.3/src/faceext.py`

 * *Files identical despite different names*

