# Comparing `tmp/youtube_video_analyzer-0.1.1.tar.gz` & `tmp/youtube_video_analyzer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtube_video_analyzer-0.1.1.tar", last modified: Sat May 18 08:37:01 2024, max compression
+gzip compressed data, was "youtube_video_analyzer-0.1.2.tar", last modified: Sat May 18 08:48:39 2024, max compression
```

## Comparing `youtube_video_analyzer-0.1.1.tar` & `youtube_video_analyzer-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-18 08:37:01.371179 youtube_video_analyzer-0.1.1/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     2589 2024-05-18 08:37:01.370935 youtube_video_analyzer-0.1.1/PKG-INFO
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       38 2024-05-18 08:37:01.371225 youtube_video_analyzer-0.1.1/setup.cfg
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      900 2024-05-18 08:35:36.000000 youtube_video_analyzer-0.1.1/setup.py
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-18 08:37:01.369760 youtube_video_analyzer-0.1.1/youtube_video_analyzer/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      181 2024-05-18 07:54:47.000000 youtube_video_analyzer-0.1.1/youtube_video_analyzer/__init__.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     2286 2024-05-18 08:03:45.000000 youtube_video_analyzer-0.1.1/youtube_video_analyzer/frame_extract.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     1288 2024-05-18 08:02:32.000000 youtube_video_analyzer-0.1.1/youtube_video_analyzer/sound_extract.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     3479 2024-05-18 08:01:14.000000 youtube_video_analyzer-0.1.1/youtube_video_analyzer/sound_intervals.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     2125 2024-05-18 08:01:36.000000 youtube_video_analyzer-0.1.1/youtube_video_analyzer/video_downloader.py
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-18 08:37:01.370706 youtube_video_analyzer-0.1.1/youtube_video_analyzer.egg-info/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     2589 2024-05-18 08:37:01.000000 youtube_video_analyzer-0.1.1/youtube_video_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      437 2024-05-18 08:37:01.000000 youtube_video_analyzer-0.1.1/youtube_video_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)        1 2024-05-18 08:37:01.000000 youtube_video_analyzer-0.1.1/youtube_video_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       37 2024-05-18 08:37:01.000000 youtube_video_analyzer-0.1.1/youtube_video_analyzer.egg-info/requires.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       23 2024-05-18 08:37:01.000000 youtube_video_analyzer-0.1.1/youtube_video_analyzer.egg-info/top_level.txt
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-18 08:48:39.041738 youtube_video_analyzer-0.1.2/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     2609 2024-05-18 08:48:39.041494 youtube_video_analyzer-0.1.2/PKG-INFO
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       38 2024-05-18 08:48:39.041950 youtube_video_analyzer-0.1.2/setup.cfg
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      900 2024-05-18 08:48:01.000000 youtube_video_analyzer-0.1.2/setup.py
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-18 08:48:39.039643 youtube_video_analyzer-0.1.2/youtube_video_analyzer/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      181 2024-05-18 07:54:47.000000 youtube_video_analyzer-0.1.2/youtube_video_analyzer/__init__.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     2286 2024-05-18 08:03:45.000000 youtube_video_analyzer-0.1.2/youtube_video_analyzer/frame_extract.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     1288 2024-05-18 08:02:32.000000 youtube_video_analyzer-0.1.2/youtube_video_analyzer/sound_extract.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     3479 2024-05-18 08:01:14.000000 youtube_video_analyzer-0.1.2/youtube_video_analyzer/sound_intervals.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     2125 2024-05-18 08:01:36.000000 youtube_video_analyzer-0.1.2/youtube_video_analyzer/video_downloader.py
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-18 08:48:39.041072 youtube_video_analyzer-0.1.2/youtube_video_analyzer.egg-info/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     2609 2024-05-18 08:48:38.000000 youtube_video_analyzer-0.1.2/youtube_video_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      437 2024-05-18 08:48:39.000000 youtube_video_analyzer-0.1.2/youtube_video_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)        1 2024-05-18 08:48:38.000000 youtube_video_analyzer-0.1.2/youtube_video_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       37 2024-05-18 08:48:38.000000 youtube_video_analyzer-0.1.2/youtube_video_analyzer.egg-info/requires.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       23 2024-05-18 08:48:38.000000 youtube_video_analyzer-0.1.2/youtube_video_analyzer.egg-info/top_level.txt
```

### Comparing `youtube_video_analyzer-0.1.1/PKG-INFO` & `youtube_video_analyzer-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube_video_analyzer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for downloading YouTube videos, extracting audio and frames, and analyzing sound intervals
 Home-page: https://github.com/Cornelius-BobCat/package-video-downloader
 Author: Cornelius Vincent
 Author-email: pro.cornelius@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,15 +35,15 @@
 You can install VideoSoundAnalyzer from PyPI using `pip`:
 
 ## Usage
 
 Here's an example of how to use the package:
 
 ```python
-from youtube_downloader import VideoDownloader, AudioExtractor, SoundIntervalAnalyzer
+from youtube_video_analyzer import VideoDownloader, AudioExtractor, SoundIntervalAnalyzer, FrameExtractor
 
 # Download a video from YouTube
 downloader = VideoDownloader(video_url, output_directory)
 video_path = downloader.download_video()
 
 # Extract frame of frame : select a intervals
 frame_extractor = FrameExtractor(video_path, output_directory, quality, oneperframe )
```

### Comparing `youtube_video_analyzer-0.1.1/setup.py` & `youtube_video_analyzer-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="youtube_video_analyzer",
-    version="0.1.1",
+    version="0.1.2",
     author="Cornelius Vincent",
     author_email="pro.cornelius@gmail.com",
     description="A package for downloading YouTube videos, extracting audio and frames, and analyzing sound intervals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Cornelius-BobCat/package-video-downloader",
     packages=setuptools.find_packages(),
```

### Comparing `youtube_video_analyzer-0.1.1/youtube_video_analyzer/frame_extract.py` & `youtube_video_analyzer-0.1.2/youtube_video_analyzer/frame_extract.py`

 * *Files identical despite different names*

### Comparing `youtube_video_analyzer-0.1.1/youtube_video_analyzer/sound_extract.py` & `youtube_video_analyzer-0.1.2/youtube_video_analyzer/sound_extract.py`

 * *Files identical despite different names*

### Comparing `youtube_video_analyzer-0.1.1/youtube_video_analyzer/sound_intervals.py` & `youtube_video_analyzer-0.1.2/youtube_video_analyzer/sound_intervals.py`

 * *Files identical despite different names*

### Comparing `youtube_video_analyzer-0.1.1/youtube_video_analyzer/video_downloader.py` & `youtube_video_analyzer-0.1.2/youtube_video_analyzer/video_downloader.py`

 * *Files identical despite different names*

### Comparing `youtube_video_analyzer-0.1.1/youtube_video_analyzer.egg-info/PKG-INFO` & `youtube_video_analyzer-0.1.2/youtube_video_analyzer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube_video_analyzer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for downloading YouTube videos, extracting audio and frames, and analyzing sound intervals
 Home-page: https://github.com/Cornelius-BobCat/package-video-downloader
 Author: Cornelius Vincent
 Author-email: pro.cornelius@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,15 +35,15 @@
 You can install VideoSoundAnalyzer from PyPI using `pip`:
 
 ## Usage
 
 Here's an example of how to use the package:
 
 ```python
-from youtube_downloader import VideoDownloader, AudioExtractor, SoundIntervalAnalyzer
+from youtube_video_analyzer import VideoDownloader, AudioExtractor, SoundIntervalAnalyzer, FrameExtractor
 
 # Download a video from YouTube
 downloader = VideoDownloader(video_url, output_directory)
 video_path = downloader.download_video()
 
 # Extract frame of frame : select a intervals
 frame_extractor = FrameExtractor(video_path, output_directory, quality, oneperframe )
```

