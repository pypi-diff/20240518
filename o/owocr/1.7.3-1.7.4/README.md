# Comparing `tmp/owocr-1.7.3.tar.gz` & `tmp/owocr-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owocr-1.7.3.tar", last modified: Fri Mar  8 02:40:32 2024, max compression
+gzip compressed data, was "owocr-1.7.4.tar", last modified: Sat May 18 16:44:06 2024, max compression
```

## Comparing `owocr-1.7.3.tar` & `owocr-1.7.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 aurora     (501) staff       (20)        0 2024-03-08 02:40:32.607790 owocr-1.7.3/
--rw-r--r--   0 aurora     (501) staff       (20)    11357 2023-09-15 09:18:57.000000 owocr-1.7.3/LICENSE
--rw-r--r--   0 aurora     (501) staff       (20)     6803 2024-03-08 02:40:32.607584 owocr-1.7.3/PKG-INFO
--rw-r--r--   0 aurora     (501) staff       (20)     6023 2024-03-04 18:53:18.000000 owocr-1.7.3/README.md
-drwxr-xr-x   0 aurora     (501) staff       (20)        0 2024-03-08 02:40:32.606399 owocr-1.7.3/owocr/
--rw-r--r--   0 aurora     (501) staff       (20)       51 2024-03-08 02:38:01.000000 owocr-1.7.3/owocr/__init__.py
--rw-r--r--   0 aurora     (501) staff       (20)      426 2024-03-08 02:38:01.000000 owocr-1.7.3/owocr/__main__.py
--rw-r--r--   0 aurora     (501) staff       (20)     2929 2024-03-08 02:38:01.000000 owocr-1.7.3/owocr/config.py
--rw-r--r--   0 aurora     (501) staff       (20)    20490 2024-03-08 02:38:01.000000 owocr-1.7.3/owocr/ocr.py
--rw-r--r--   0 aurora     (501) staff       (20)    40344 2024-03-08 02:38:01.000000 owocr-1.7.3/owocr/run.py
-drwxr-xr-x   0 aurora     (501) staff       (20)        0 2024-03-08 02:40:32.607346 owocr-1.7.3/owocr.egg-info/
--rw-r--r--   0 aurora     (501) staff       (20)     6803 2024-03-08 02:40:32.000000 owocr-1.7.3/owocr.egg-info/PKG-INFO
--rw-r--r--   0 aurora     (501) staff       (20)      280 2024-03-08 02:40:32.000000 owocr-1.7.3/owocr.egg-info/SOURCES.txt
--rw-r--r--   0 aurora     (501) staff       (20)        1 2024-03-08 02:40:32.000000 owocr-1.7.3/owocr.egg-info/dependency_links.txt
--rw-r--r--   0 aurora     (501) staff       (20)       46 2024-03-08 02:40:32.000000 owocr-1.7.3/owocr.egg-info/entry_points.txt
--rw-r--r--   0 aurora     (501) staff       (20)      232 2024-03-08 02:40:32.000000 owocr-1.7.3/owocr.egg-info/requires.txt
--rw-r--r--   0 aurora     (501) staff       (20)        6 2024-03-08 02:40:32.000000 owocr-1.7.3/owocr.egg-info/top_level.txt
--rw-r--r--   0 aurora     (501) staff       (20)       38 2024-03-08 02:40:32.607833 owocr-1.7.3/setup.cfg
--rw-r--r--   0 aurora     (501) staff       (20)     1106 2024-03-08 02:40:01.000000 owocr-1.7.3/setup.py
+drwxr-xr-x   0 aurora     (501) staff       (20)        0 2024-05-18 16:44:06.379126 owocr-1.7.4/
+-rw-r--r--   0 aurora     (501) staff       (20)    11357 2023-09-15 09:18:57.000000 owocr-1.7.4/LICENSE
+-rw-r--r--   0 aurora     (501) staff       (20)     6803 2024-05-18 16:44:06.378841 owocr-1.7.4/PKG-INFO
+-rw-r--r--   0 aurora     (501) staff       (20)     6023 2024-03-04 18:53:18.000000 owocr-1.7.4/README.md
+drwxr-xr-x   0 aurora     (501) staff       (20)        0 2024-05-18 16:44:06.376534 owocr-1.7.4/owocr/
+-rw-r--r--   0 aurora     (501) staff       (20)       51 2024-03-08 02:38:01.000000 owocr-1.7.4/owocr/__init__.py
+-rw-r--r--   0 aurora     (501) staff       (20)      426 2024-03-08 02:38:01.000000 owocr-1.7.4/owocr/__main__.py
+-rw-r--r--   0 aurora     (501) staff       (20)     2929 2024-03-08 02:38:01.000000 owocr-1.7.4/owocr/config.py
+-rw-r--r--   0 aurora     (501) staff       (20)    20480 2024-05-18 16:34:30.000000 owocr-1.7.4/owocr/ocr.py
+-rw-r--r--   0 aurora     (501) staff       (20)    40344 2024-03-08 02:38:01.000000 owocr-1.7.4/owocr/run.py
+drwxr-xr-x   0 aurora     (501) staff       (20)        0 2024-05-18 16:44:06.378438 owocr-1.7.4/owocr.egg-info/
+-rw-r--r--   0 aurora     (501) staff       (20)     6803 2024-05-18 16:44:06.000000 owocr-1.7.4/owocr.egg-info/PKG-INFO
+-rw-r--r--   0 aurora     (501) staff       (20)      280 2024-05-18 16:44:06.000000 owocr-1.7.4/owocr.egg-info/SOURCES.txt
+-rw-r--r--   0 aurora     (501) staff       (20)        1 2024-05-18 16:44:06.000000 owocr-1.7.4/owocr.egg-info/dependency_links.txt
+-rw-r--r--   0 aurora     (501) staff       (20)       46 2024-05-18 16:44:06.000000 owocr-1.7.4/owocr.egg-info/entry_points.txt
+-rw-r--r--   0 aurora     (501) staff       (20)      232 2024-05-18 16:44:06.000000 owocr-1.7.4/owocr.egg-info/requires.txt
+-rw-r--r--   0 aurora     (501) staff       (20)        6 2024-05-18 16:44:06.000000 owocr-1.7.4/owocr.egg-info/top_level.txt
+-rw-r--r--   0 aurora     (501) staff       (20)       38 2024-05-18 16:44:06.379188 owocr-1.7.4/setup.cfg
+-rw-r--r--   0 aurora     (501) staff       (20)     1106 2024-05-18 16:37:39.000000 owocr-1.7.4/setup.py
```

### Comparing `owocr-1.7.3/LICENSE` & `owocr-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `owocr-1.7.3/PKG-INFO` & `owocr-1.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owocr
-Version: 1.7.3
+Version: 1.7.4
 Summary: Japanese OCR
 Home-page: https://github.com/AuroraWright/owocr
 Author: AuroraWright
 Author-email: fallingluma@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `owocr-1.7.3/README.md` & `owocr-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `owocr-1.7.3/owocr/config.py` & `owocr-1.7.4/owocr/config.py`

 * *Files identical despite different names*

### Comparing `owocr-1.7.3/owocr/ocr.py` & `owocr-1.7.4/owocr/ocr.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,31 +328,31 @@
                                     2: {'type': b'@'},
                                 }
                             }
                         }
                     }
                 }
             )
-            self.analyzer = VKCImageAnalyzer.alloc().init()
             self.available = True
             logger.info('Apple Live Text ready')
 
     def __call__(self, img_or_path):
         if isinstance(img_or_path, str) or isinstance(img_or_path, Path):
             img = Image.open(img_or_path)
         elif isinstance(img_or_path, Image.Image):
             img = img_or_path
         else:
             raise ValueError(f'img_or_path must be a path or PIL.Image, instead got: {img_or_path}')
 
         with objc.autorelease_pool():
+            analyzer = VKCImageAnalyzer.alloc().init()
             req = VKCImageAnalyzerRequest.alloc().initWithImage_requestType_(self._preprocess(img), 1) #VKAnalysisTypeText
             req.setLocales_(['ja','en'])
             self.result = None
-            self.analyzer.processRequest_progressHandler_completionHandler_(req, lambda progress: None, self._process)
+            analyzer.processRequest_progressHandler_completionHandler_(req, lambda progress: None, self._process)
 
             CFRunLoopRunInMode(kCFRunLoopDefaultMode, 10.0, False)
 
             if self.result == None:
                 return (False, 'Unknown error!')
             return (True, self.result)
```

### Comparing `owocr-1.7.3/owocr/run.py` & `owocr-1.7.4/owocr/run.py`

 * *Files identical despite different names*

### Comparing `owocr-1.7.3/owocr.egg-info/PKG-INFO` & `owocr-1.7.4/owocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owocr
-Version: 1.7.3
+Version: 1.7.4
 Summary: Japanese OCR
 Home-page: https://github.com/AuroraWright/owocr
 Author: AuroraWright
 Author-email: fallingluma@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `owocr-1.7.3/setup.py` & `owocr-1.7.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from setuptools import setup
 
 long_description = (Path(__file__).parent / "README.md").read_text('utf-8')
 
 setup(
     name="owocr",
-    version='1.7.3',
+    version='1.7.4',
     description="Japanese OCR",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AuroraWright/owocr",
     author="AuroraWright",
     author_email="fallingluma@gmail.com",
     license="Apache License 2.0",
```

