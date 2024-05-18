# Comparing `tmp/pinscrape-3.0.5.tar.gz` & `tmp/pinscrape-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinscrape-3.0.5.tar", last modified: Tue May 14 10:02:45 2024, max compression
+gzip compressed data, was "pinscrape-3.1.0.tar", last modified: Sat May 18 11:39:10 2024, max compression
```

## Comparing `pinscrape-3.0.5.tar` & `pinscrape-3.1.0.tar`

### file list

```diff
@@ -1,19 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:02:45.396049 pinscrape-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-14 10:02:30.000000 pinscrape-3.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-14 10:02:45.396049 pinscrape-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-14 10:02:30.000000 pinscrape-3.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:02:45.396049 pinscrape-3.0.5/pinscrape/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-14 10:02:30.000000 pinscrape-3.0.5/pinscrape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 10:02:30.000000 pinscrape-3.0.5/pinscrape/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-14 10:02:30.000000 pinscrape-3.0.5/pinscrape/pinscrape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:02:45.396049 pinscrape-3.0.5/pinscrape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-14 10:02:45.000000 pinscrape-3.0.5/pinscrape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-14 10:02:45.000000 pinscrape-3.0.5/pinscrape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:02:45.000000 pinscrape-3.0.5/pinscrape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-14 10:02:45.000000 pinscrape-3.0.5/pinscrape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 10:02:45.000000 pinscrape-3.0.5/pinscrape.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:02:45.396049 pinscrape-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-14 10:02:30.000000 pinscrape-3.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:02:45.396049 pinscrape-3.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:02:30.000000 pinscrape-3.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-14 10:02:30.000000 pinscrape-3.0.5/tests/e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:39:10.468636 pinscrape-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-18 11:38:50.000000 pinscrape-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-18 11:39:10.468636 pinscrape-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-18 11:38:50.000000 pinscrape-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:39:10.464636 pinscrape-3.1.0/pinscrape/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-18 11:38:50.000000 pinscrape-3.1.0/pinscrape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-18 11:38:50.000000 pinscrape-3.1.0/pinscrape/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-05-18 11:38:50.000000 pinscrape-3.1.0/pinscrape/pinscrape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 11:39:10.468636 pinscrape-3.1.0/pinscrape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-18 11:39:10.000000 pinscrape-3.1.0/pinscrape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-18 11:39:10.000000 pinscrape-3.1.0/pinscrape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 11:39:10.000000 pinscrape-3.1.0/pinscrape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-18 11:39:10.000000 pinscrape-3.1.0/pinscrape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-18 11:39:10.000000 pinscrape-3.1.0/pinscrape.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 11:39:10.468636 pinscrape-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-18 11:38:50.000000 pinscrape-3.1.0/setup.py
```

### Comparing `pinscrape-3.0.5/LICENSE` & `pinscrape-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pinscrape-3.0.5/PKG-INFO` & `pinscrape-3.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pinscrape
-Version: 3.0.5
-Summary: Pinterest data scraper
+Version: 3.1.0
+Summary: Pinterest | a simple data scraper for pinterest
 Home-page: https://github.com/iamatulsingh/pinscrape
 Author: Atul Singh
 Author-email: atulsingh0401@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pinscrape-3.0.5/README.md` & `pinscrape-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pinscrape-3.0.5/pinscrape/pinscrape.py` & `pinscrape-3.1.0/pinscrape/pinscrape.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import re
 import json
 import os
 import cv2
 import numpy as np
 
 from requests import get
 from bs4 import BeautifulSoup as soup
@@ -15,72 +14,62 @@
 
     def __init__(self):
         self.json_data_list = []
         self.unique_img = []
 
     # ---------------------------------------- GET GOOGLE RESULTS ---------------------------------
     @staticmethod
-    def get_pinterest_links(body, max_images):
+    def get_pinterest_links(body, max_images: int):
         searched_urls = []
         html = soup(body, 'html.parser')
-        links = html.select('#main > div > div > div > a')
+        links = html.select('#b_results cite')
         for link in links:
-            link = link.get('href')
-            link = re.sub(r'/url\?q=', '', link)
-            if link[0] != "/" and "pinterest" in link:
+            link = link.text
+            if "pinterest" in link:
                 searched_urls.append(link)
-                #stops adding links if the limit has been reached
+                # stops adding links if the limit has been reached
                 if max_images is not None and max_images == len(searched_urls):
                     break
-
         return searched_urls
 
     # -------------------------- save json data from source code of given pinterest url -------------
-    def get_source(self, url, proxies):
+    def get_source(self, url: str, proxies: dict) -> None:
         try:
             res = get(url, proxies=proxies)
-        except Exception as e:
+        except Exception:
             return
         html = soup(res.text, 'html.parser')
-        json_data = html.find_all("script", attrs={"id": "__PWS_DATA__"})
-        for a in json_data:
-            self.json_data_list.append(a.string)
+        json_data = html.find_all("script", attrs={"id": "__PWS_INITIAL_PROPS__"})
+        self.json_data_list.append(json.loads(json_data[0].string))
 
     # --------------------------- READ JSON OF PINTEREST WEBSITE ----------------------
-    def save_image_url(self, max_images):
-        url_list = [i for i in self.json_data_list if i.strip()]
-        if not len(url_list):
-            return url_list
+    def save_image_url(self, max_images: int) -> list:
         url_list = []
         for js in self.json_data_list:
             try:
-                data = DotMap(json.loads(js))
+                data = DotMap(js)
                 urls = []
-                for pin in data.props.initialReduxState.pins:
-                    if isinstance(data.props.initialReduxState.pins[pin].images.get("orig"), list):
-                        for i in data.props.initialReduxState.pins[pin].images.get("orig"):
+                for pin in data.initialReduxState.pins:
+                    if isinstance(data.initialReduxState.pins[pin].images.get("orig"), list):
+                        for i in data.initialReduxState.pins[pin].images.get("orig"):
                             urls.append(i.get("url"))
                     else:
-                        urls.append(data.props.initialReduxState.pins[pin].images.get("orig").get("url"))
+                        urls.append(data.initialReduxState.pins[pin].images.get("orig").get("url"))
 
                 for url in urls:
                     url_list.append(url)
-
-                    #if the maximum has been achieved, return early
                     if max_images is not None and max_images == len(url_list):
                         return list(set(url_list))
-                    
-
-            except Exception as e:
+            except Exception:
                 continue
-        
+
         return list(set(url_list))
 
     # ------------------------------ image hash calculation -------------------------
-    def dhash(self, image, hashSize=8):
+    def dhash(self, image, hashSize: int = 8):
         resized = cv2.resize(image, (hashSize + 1, hashSize))
         diff = resized[:, 1:] > resized[:, :-1]
         return sum([2 ** i for (i, v) in enumerate(diff.flatten()) if v])
 
     # ------------------------------  save all downloaded images to folder ---------------------------
     def saving_op(self, var):
         url_list, folder_name = var
@@ -104,27 +93,25 @@
             param.append((url_list[((i*idx)):(idx*(i+1))], output_folder))
         with ThreadPoolExecutor(max_workers=num_of_workers) as executor:
             executor.map(self.saving_op, param)
 
     # -------------------------- get user keyword and google search for that keywords ---------------------
     @staticmethod
     def start_scraping(max_images, key=None, proxies={}):
-        assert key != None, "Please provide keyword for searching images"
+        assert key is not None, "Please provide keyword for searching images"
         keyword = key + " pinterest"
         keyword = keyword.replace("+", "%20")
-        url = f'http://www.google.co.in/search?hl=en&q={keyword}'
+        url = f'https://www.bing.com/search?q={keyword}&pq=messi+pinterest&first=1&FORM=PERE'
         res = get(url, proxies=proxies)
-        searched_urls = PinterestImageScraper.get_pinterest_links(res.content,max_images)
+        searched_urls = PinterestImageScraper.get_pinterest_links(res.content, max_images)
 
         return searched_urls, key.replace(" ", "_")
 
-
-    def scrape(self, key=None, output_folder="", proxies={}, threads=10, max_images: int = None):
-        extracted_urls, keyword = PinterestImageScraper.start_scraping(max_images,key, proxies)
-        return_data = {}
+    def scrape(self, key: str = None, output_folder: str = "", proxies: dict = {}, threads: int = 10, max_images: int = None) -> dict:
+        extracted_urls, keyword = PinterestImageScraper.start_scraping(max_images, key, proxies)
         self.unique_img = []
         self.json_data_list = []
 
         for i in extracted_urls:
             self.get_source(i, proxies)
 
         # get all urls of images and save in a list
@@ -140,23 +127,24 @@
         # download images from saved images url
         if len(url_list):
             try:
                 out_folder = output_folder if output_folder else key
                 self.download(url_list, threads, out_folder)
             except KeyboardInterrupt:
                 return return_data
-            
+
             return_data["isDownloaded"] = True
             return return_data
-        
+
         return return_data
 
 
 scraper = PinterestImageScraper()
 
+
 if __name__ == "__main__":
-    details = scraper.scrape("messi", "output")
+    details = scraper.scrape("messi", "output", {}, 10, None)
 
     if details["isDownloaded"]:
         print("\nDownloading completed !!")
     else:
         print("\nNothing to download !!")
```

### Comparing `pinscrape-3.0.5/pinscrape.egg-info/PKG-INFO` & `pinscrape-3.1.0/pinscrape.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pinscrape
-Version: 3.0.5
-Summary: Pinterest data scraper
+Version: 3.1.0
+Summary: Pinterest | a simple data scraper for pinterest
 Home-page: https://github.com/iamatulsingh/pinscrape
 Author: Atul Singh
 Author-email: atulsingh0401@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pinscrape-3.0.5/setup.py` & `pinscrape-3.1.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     reqs = req.read().split("\n")
 
 setuptools.setup(
     name="pinscrape",
     version=__version__,
     author="Atul Singh",
     author_email="atulsingh0401@gmail.com",
-    description="Pinterest data scraper",
+    description="Pinterest | a simple data scraper for pinterest",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iamatulsingh/pinscrape",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

