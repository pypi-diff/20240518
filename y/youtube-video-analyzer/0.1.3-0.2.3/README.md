# Comparing `tmp/youtube_video_analyzer-0.1.3.tar.gz` & `tmp/youtube_video_analyzer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtube_video_analyzer-0.1.3.tar", last modified: Sat May 18 09:01:08 2024, max compression
+gzip compressed data, was "youtube_video_analyzer-0.2.3.tar", last modified: Sat May 18 12:47:43 2024, max compression
```

## Comparing `youtube_video_analyzer-0.1.3.tar` & `youtube_video_analyzer-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-18 09:01:08.038646 youtube_video_analyzer-0.1.3/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     2652 2024-05-18 09:01:08.038337 youtube_video_analyzer-0.1.3/PKG-INFO
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       38 2024-05-18 09:01:08.038721 youtube_video_analyzer-0.1.3/setup.cfg
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      900 2024-05-18 08:59:47.000000 youtube_video_analyzer-0.1.3/setup.py
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-18 09:01:08.036334 youtube_video_analyzer-0.1.3/youtube_video_analyzer/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      181 2024-05-18 07:54:47.000000 youtube_video_analyzer-0.1.3/youtube_video_analyzer/__init__.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     2286 2024-05-18 08:03:45.000000 youtube_video_analyzer-0.1.3/youtube_video_analyzer/frame_extract.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     1288 2024-05-18 08:02:32.000000 youtube_video_analyzer-0.1.3/youtube_video_analyzer/sound_extract.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     3479 2024-05-18 08:01:14.000000 youtube_video_analyzer-0.1.3/youtube_video_analyzer/sound_intervals.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     2125 2024-05-18 08:01:36.000000 youtube_video_analyzer-0.1.3/youtube_video_analyzer/video_downloader.py
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-18 09:01:08.037865 youtube_video_analyzer-0.1.3/youtube_video_analyzer.egg-info/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     2652 2024-05-18 09:01:07.000000 youtube_video_analyzer-0.1.3/youtube_video_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      437 2024-05-18 09:01:08.000000 youtube_video_analyzer-0.1.3/youtube_video_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)        1 2024-05-18 09:01:07.000000 youtube_video_analyzer-0.1.3/youtube_video_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       37 2024-05-18 09:01:07.000000 youtube_video_analyzer-0.1.3/youtube_video_analyzer.egg-info/requires.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       23 2024-05-18 09:01:07.000000 youtube_video_analyzer-0.1.3/youtube_video_analyzer.egg-info/top_level.txt
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-18 12:47:43.678034 youtube_video_analyzer-0.2.3/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     2652 2024-05-18 12:47:43.677808 youtube_video_analyzer-0.2.3/PKG-INFO
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       38 2024-05-18 12:47:43.678105 youtube_video_analyzer-0.2.3/setup.cfg
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      959 2024-05-18 12:47:32.000000 youtube_video_analyzer-0.2.3/setup.py
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-18 12:47:43.676538 youtube_video_analyzer-0.2.3/youtube_video_analyzer/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      181 2024-05-18 07:54:47.000000 youtube_video_analyzer-0.2.3/youtube_video_analyzer/__init__.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     2286 2024-05-18 08:03:45.000000 youtube_video_analyzer-0.2.3/youtube_video_analyzer/frame_extract.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     1288 2024-05-18 08:02:32.000000 youtube_video_analyzer-0.2.3/youtube_video_analyzer/sound_extract.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     3579 2024-05-18 12:46:05.000000 youtube_video_analyzer-0.2.3/youtube_video_analyzer/sound_intervals.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     2125 2024-05-18 08:01:36.000000 youtube_video_analyzer-0.2.3/youtube_video_analyzer/video_downloader.py
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-18 12:47:43.677569 youtube_video_analyzer-0.2.3/youtube_video_analyzer.egg-info/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     2652 2024-05-18 12:47:43.000000 youtube_video_analyzer-0.2.3/youtube_video_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      437 2024-05-18 12:47:43.000000 youtube_video_analyzer-0.2.3/youtube_video_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)        1 2024-05-18 12:47:43.000000 youtube_video_analyzer-0.2.3/youtube_video_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       37 2024-05-18 12:47:43.000000 youtube_video_analyzer-0.2.3/youtube_video_analyzer.egg-info/requires.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       23 2024-05-18 12:47:43.000000 youtube_video_analyzer-0.2.3/youtube_video_analyzer.egg-info/top_level.txt
```

### Comparing `youtube_video_analyzer-0.1.3/PKG-INFO` & `youtube_video_analyzer-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube_video_analyzer
-Version: 0.1.3
+Version: 0.2.3
 Summary: A package for downloading YouTube videos, extracting audio and frames, and analyzing sound intervals
 Home-page: https://github.com/Cornelius-BobCat/package-video-downloader
 Author: Cornelius Vincent
 Author-email: pro.cornelius@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `youtube_video_analyzer-0.1.3/setup.py` & `youtube_video_analyzer-0.2.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="youtube_video_analyzer",
-    version="0.1.3",
+    version="0.2.3",
     author="Cornelius Vincent",
     author_email="pro.cornelius@gmail.com",
     description="A package for downloading YouTube videos, extracting audio and frames, and analyzing sound intervals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Cornelius-BobCat/package-video-downloader",
     packages=setuptools.find_packages(),
@@ -23,7 +23,10 @@
         "pytube",
         "moviepy",
         "librosa",
         "imageio",
         "numpy",
     ],
 )
+
+# python setup.py sdist bdist_wheel
+# twine upload dist/*
```

### Comparing `youtube_video_analyzer-0.1.3/youtube_video_analyzer/frame_extract.py` & `youtube_video_analyzer-0.2.3/youtube_video_analyzer/frame_extract.py`

 * *Files identical despite different names*

### Comparing `youtube_video_analyzer-0.1.3/youtube_video_analyzer/sound_extract.py` & `youtube_video_analyzer-0.2.3/youtube_video_analyzer/sound_extract.py`

 * *Files identical despite different names*

### Comparing `youtube_video_analyzer-0.1.3/youtube_video_analyzer/sound_intervals.py` & `youtube_video_analyzer-0.2.3/youtube_video_analyzer/sound_intervals.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,13 +69,16 @@
                     if start_silence is not None:
                         end_silence = librosa.frames_to_time(
                             t, sr=sr, hop_length=self.hop_length
                         )
                         if end_silence - start_silence >= self.min_silence_duration:
                             sound_intervals.append((start_silence, end_silence))
                         start_silence = None
-            if self.output_json:
+
+            if not self.output_json:
                 with open(self.output_json, "w") as json_file:
                     json.dump(sound_intervals, json_file, indent=2)
                 self.logger.info(f"Intervals are save {self.output_json}.")
+            else:
+                self.logger.info(f"file {self.output_json} already exists.")
         except Exception as e:
             self.logger.error(f"Error when analysis : {e}")
```

### Comparing `youtube_video_analyzer-0.1.3/youtube_video_analyzer/video_downloader.py` & `youtube_video_analyzer-0.2.3/youtube_video_analyzer/video_downloader.py`

 * *Files identical despite different names*

### Comparing `youtube_video_analyzer-0.1.3/youtube_video_analyzer.egg-info/PKG-INFO` & `youtube_video_analyzer-0.2.3/youtube_video_analyzer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube_video_analyzer
-Version: 0.1.3
+Version: 0.2.3
 Summary: A package for downloading YouTube videos, extracting audio and frames, and analyzing sound intervals
 Home-page: https://github.com/Cornelius-BobCat/package-video-downloader
 Author: Cornelius Vincent
 Author-email: pro.cornelius@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

