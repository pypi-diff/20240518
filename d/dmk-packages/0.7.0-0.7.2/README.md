# Comparing `tmp/dmk_packages-0.7.0.tar.gz` & `tmp/dmk_packages-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmk_packages-0.7.0.tar", last modified: Fri May 17 00:39:33 2024, max compression
+gzip compressed data, was "dmk_packages-0.7.2.tar", last modified: Sat May 18 05:42:54 2024, max compression
```

## Comparing `dmk_packages-0.7.0.tar` & `dmk_packages-0.7.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-17 00:39:33.187007 dmk_packages-0.7.0/
--rw-r--r--   0 layla      (501) staff       (20)    11347 2024-03-25 06:00:17.000000 dmk_packages-0.7.0/LICENSE
--rw-r--r--   0 layla      (501) staff       (20)     1854 2024-05-17 00:39:33.186645 dmk_packages-0.7.0/PKG-INFO
--rw-r--r--   0 layla      (501) staff       (20)     1365 2024-03-25 06:00:17.000000 dmk_packages-0.7.0/README.md
--rw-r--r--   0 layla      (501) staff       (20)      584 2024-05-17 00:39:18.000000 dmk_packages-0.7.0/pyproject.toml
--rw-r--r--   0 layla      (501) staff       (20)       38 2024-05-17 00:39:33.187101 dmk_packages-0.7.0/setup.cfg
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-17 00:39:33.171489 dmk_packages-0.7.0/src/
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-17 00:39:33.174862 dmk_packages-0.7.0/src/dmk_packages/
--rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.7.0/src/dmk_packages/__init__.py
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-17 00:39:33.183630 dmk_packages-0.7.0/src/dmk_packages/crawler/
--rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.7.0/src/dmk_packages/crawler/__init__.py
--rw-r--r--   0 layla      (501) staff       (20)     3534 2024-05-04 15:01:16.000000 dmk_packages-0.7.0/src/dmk_packages/crawler/bigkinds.py
--rw-r--r--   0 layla      (501) staff       (20)     6580 2024-05-04 15:01:16.000000 dmk_packages-0.7.0/src/dmk_packages/crawler/clien.py
--rw-r--r--   0 layla      (501) staff       (20)     6685 2024-05-04 15:01:16.000000 dmk_packages-0.7.0/src/dmk_packages/crawler/fnguide.py
--rw-r--r--   0 layla      (501) staff       (20)     2321 2024-04-03 06:07:52.000000 dmk_packages-0.7.0/src/dmk_packages/crawler/naver_blog.py
--rw-r--r--   0 layla      (501) staff       (20)    17245 2024-05-17 00:38:35.000000 dmk_packages-0.7.0/src/dmk_packages/crawler/naver_search_volume.py
--rw-r--r--   0 layla      (501) staff       (20)     1382 2024-05-04 15:01:16.000000 dmk_packages-0.7.0/src/dmk_packages/crawler/pdf_to_text.py
--rw-r--r--   0 layla      (501) staff       (20)    14699 2024-05-05 04:51:03.000000 dmk_packages-0.7.0/src/dmk_packages/crawler/youtube.py
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-17 00:39:33.184891 dmk_packages-0.7.0/src/dmk_packages/database/
--rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.7.0/src/dmk_packages/database/__init__.py
--rw-r--r--   0 layla      (501) staff       (20)     3057 2024-04-15 03:09:28.000000 dmk_packages-0.7.0/src/dmk_packages/database/database.py
--rw-r--r--   0 layla      (501) staff       (20)     1895 2024-03-25 06:00:17.000000 dmk_packages-0.7.0/src/dmk_packages/naver_datalab.py
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-17 00:39:33.185993 dmk_packages-0.7.0/src/dmk_packages.egg-info/
--rw-r--r--   0 layla      (501) staff       (20)     1854 2024-05-17 00:39:33.000000 dmk_packages-0.7.0/src/dmk_packages.egg-info/PKG-INFO
--rw-r--r--   0 layla      (501) staff       (20)      677 2024-05-17 00:39:33.000000 dmk_packages-0.7.0/src/dmk_packages.egg-info/SOURCES.txt
--rw-r--r--   0 layla      (501) staff       (20)        1 2024-05-17 00:39:33.000000 dmk_packages-0.7.0/src/dmk_packages.egg-info/dependency_links.txt
--rw-r--r--   0 layla      (501) staff       (20)       41 2024-05-17 00:39:33.000000 dmk_packages-0.7.0/src/dmk_packages.egg-info/requires.txt
--rw-r--r--   0 layla      (501) staff       (20)       13 2024-05-17 00:39:33.000000 dmk_packages-0.7.0/src/dmk_packages.egg-info/top_level.txt
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-18 05:42:54.309238 dmk_packages-0.7.2/
+-rw-r--r--   0 layla      (501) staff       (20)    11347 2024-03-25 06:00:17.000000 dmk_packages-0.7.2/LICENSE
+-rw-r--r--   0 layla      (501) staff       (20)     1854 2024-05-18 05:42:54.308694 dmk_packages-0.7.2/PKG-INFO
+-rw-r--r--   0 layla      (501) staff       (20)     1365 2024-03-25 06:00:17.000000 dmk_packages-0.7.2/README.md
+-rw-r--r--   0 layla      (501) staff       (20)      584 2024-05-18 05:39:47.000000 dmk_packages-0.7.2/pyproject.toml
+-rw-r--r--   0 layla      (501) staff       (20)       38 2024-05-18 05:42:54.309378 dmk_packages-0.7.2/setup.cfg
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-18 05:42:54.289260 dmk_packages-0.7.2/src/
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-18 05:42:54.292565 dmk_packages-0.7.2/src/dmk_packages/
+-rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.7.2/src/dmk_packages/__init__.py
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-18 05:42:54.304332 dmk_packages-0.7.2/src/dmk_packages/crawler/
+-rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.7.2/src/dmk_packages/crawler/__init__.py
+-rw-r--r--   0 layla      (501) staff       (20)     3534 2024-05-04 15:01:16.000000 dmk_packages-0.7.2/src/dmk_packages/crawler/bigkinds.py
+-rw-r--r--   0 layla      (501) staff       (20)     6580 2024-05-04 15:01:16.000000 dmk_packages-0.7.2/src/dmk_packages/crawler/clien.py
+-rw-r--r--   0 layla      (501) staff       (20)     6685 2024-05-04 15:01:16.000000 dmk_packages-0.7.2/src/dmk_packages/crawler/fnguide.py
+-rw-r--r--   0 layla      (501) staff       (20)     2321 2024-04-03 06:07:52.000000 dmk_packages-0.7.2/src/dmk_packages/crawler/naver_blog.py
+-rw-r--r--   0 layla      (501) staff       (20)    17895 2024-05-18 05:39:47.000000 dmk_packages-0.7.2/src/dmk_packages/crawler/naver_search_volume.py
+-rw-r--r--   0 layla      (501) staff       (20)     1382 2024-05-04 15:01:16.000000 dmk_packages-0.7.2/src/dmk_packages/crawler/pdf_to_text.py
+-rw-r--r--   0 layla      (501) staff       (20)    14699 2024-05-05 04:51:03.000000 dmk_packages-0.7.2/src/dmk_packages/crawler/youtube.py
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-18 05:42:54.305889 dmk_packages-0.7.2/src/dmk_packages/database/
+-rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.7.2/src/dmk_packages/database/__init__.py
+-rw-r--r--   0 layla      (501) staff       (20)     3057 2024-04-15 03:09:28.000000 dmk_packages-0.7.2/src/dmk_packages/database/database.py
+-rw-r--r--   0 layla      (501) staff       (20)     1895 2024-03-25 06:00:17.000000 dmk_packages-0.7.2/src/dmk_packages/naver_datalab.py
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-18 05:42:54.307746 dmk_packages-0.7.2/src/dmk_packages.egg-info/
+-rw-r--r--   0 layla      (501) staff       (20)     1854 2024-05-18 05:42:54.000000 dmk_packages-0.7.2/src/dmk_packages.egg-info/PKG-INFO
+-rw-r--r--   0 layla      (501) staff       (20)      677 2024-05-18 05:42:54.000000 dmk_packages-0.7.2/src/dmk_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 layla      (501) staff       (20)        1 2024-05-18 05:42:54.000000 dmk_packages-0.7.2/src/dmk_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 layla      (501) staff       (20)       41 2024-05-18 05:42:54.000000 dmk_packages-0.7.2/src/dmk_packages.egg-info/requires.txt
+-rw-r--r--   0 layla      (501) staff       (20)       13 2024-05-18 05:42:54.000000 dmk_packages-0.7.2/src/dmk_packages.egg-info/top_level.txt
```

### Comparing `dmk_packages-0.7.0/LICENSE` & `dmk_packages-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.7.0/PKG-INFO` & `dmk_packages-0.7.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.7.0
+Version: 0.7.2
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dmk_packages-0.7.0/README.md` & `dmk_packages-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.7.0/pyproject.toml` & `dmk_packages-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmk_packages"
-version = "0.7.0"
+version = "0.7.2"
 authors = [{ name = "DataMarketingKorea", email = "infra@datamarketing.co.kr" }]
 description = "Common packages for DataMKTKorea"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = ["SQLAlchemy", "python-dotenv", "psycopg2-binary"]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `dmk_packages-0.7.0/src/dmk_packages/crawler/bigkinds.py` & `dmk_packages-0.7.2/src/dmk_packages/crawler/bigkinds.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.7.0/src/dmk_packages/crawler/clien.py` & `dmk_packages-0.7.2/src/dmk_packages/crawler/clien.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.7.0/src/dmk_packages/crawler/fnguide.py` & `dmk_packages-0.7.2/src/dmk_packages/crawler/fnguide.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.7.0/src/dmk_packages/crawler/naver_blog.py` & `dmk_packages-0.7.2/src/dmk_packages/crawler/naver_blog.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.7.0/src/dmk_packages/crawler/naver_search_volume.py` & `dmk_packages-0.7.2/src/dmk_packages/crawler/naver_search_volume.py`

 * *Files 3% similar despite different names*

```diff
@@ -354,37 +354,35 @@
     def calc_search_volume(
         self,
         keywords_bundle,
         searchad_data: List[SearchadResult],
         datalab_data: List[DatalabResult],
         age_gender=False
     ):
-        def __add_results_to_search_volume(p_data, p_total_volume, p_search_volume, p_age_gender):
-            total_ratio = sum(
-                [d["ratio"] for d in p_data.get("data")]
-            )
-
-            volume_per_ratio = (
-                p_total_volume / total_ratio if total_ratio > 0 else 0
-            )
+        def __add_results_to_search_volume(p_data, p_total_ratio, p_total_volume, p_search_volume, p_age_gender):
+            volume_per_ratio = p_total_volume / p_total_ratio if p_total_ratio > 0 else 0
 
             for d in p_data.get("data"):
                 if p_age_gender:
                     new_data = {
                         "keyword_text": kwd,
                         "keyword_date": pendulum.parse(d["period"], tz=tz),
+                        "total_volume": p_total_volume,
+                        "volume_ratio": d["ratio"],
                         "keyword_volume": int(d["ratio"] * volume_per_ratio),
                         "gender": d["gender"],
                         "age": d["age"],
                         "collected_at": pendulum.today(),
                     }
                 else:
                     new_data = {
                         "keyword_text": kwd,
                         "keyword_date": pendulum.parse(d["period"], tz=tz),
+                        "total_volume": p_total_volume,
+                        "volume_ratio": d["ratio"],
                         "keyword_volume": int(d["ratio"] * volume_per_ratio),
                         "collected_at": pendulum.today(),
                     }
                 p_search_volume.append(new_data)
 
         try:
             search_volume = []
@@ -395,18 +393,28 @@
 
                 if tgt_searchad_datum and tgt_datalab_datum:
                     monthly_pc_volume = tgt_searchad_datum[0].get(self.MPQC)
                     monthly_mo_volume = tgt_searchad_datum[0].get(self.MMQC)
                     total_volume = monthly_pc_volume + monthly_mo_volume
 
                     if age_gender:
+                        total_ratio = sum(age_gender_data["ratio"]
+                                          for keyword_age_gender_data in tgt_datalab_datum
+                                          for age_gender_data in keyword_age_gender_data.get("data"))
                         for datum in tgt_datalab_datum:
-                            __add_results_to_search_volume(datum, total_volume, search_volume, age_gender)
+                            __add_results_to_search_volume(datum, total_ratio, total_volume, search_volume, age_gender)
                     else:
-                        __add_results_to_search_volume(tgt_datalab_datum[0], total_volume, search_volume, age_gender)
+                        total_ratio = sum([d["ratio"] for d in tgt_datalab_datum[0].get("data")])
+                        __add_results_to_search_volume(
+                            tgt_datalab_datum[0],
+                            total_ratio,
+                            total_volume,
+                            search_volume,
+                            age_gender
+                        )
 
             return search_volume
 
         except Exception as error:
             logger.error(error)
 
     def get_search_volume(self, age_gender=False):
@@ -440,13 +448,13 @@
         except Exception as error:
             logger.error(error)
 
 
 # if __name__ == "__main__":
 #     try:
 #         naver_search_volume_crawler = NaverSearchVolumeCrawler()
-#         search_volume = naver_search_volume_crawler.get_searchad_data()
+#         search_volume = naver_search_volume_crawler.get_search_volume()
 #
 #         for vol in search_volume:
 #             logger.debug(vol)
 #     except Exception as error:
 #         logger.error(error)
```

### Comparing `dmk_packages-0.7.0/src/dmk_packages/crawler/pdf_to_text.py` & `dmk_packages-0.7.2/src/dmk_packages/crawler/pdf_to_text.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.7.0/src/dmk_packages/crawler/youtube.py` & `dmk_packages-0.7.2/src/dmk_packages/crawler/youtube.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.7.0/src/dmk_packages/database/database.py` & `dmk_packages-0.7.2/src/dmk_packages/database/database.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.7.0/src/dmk_packages/naver_datalab.py` & `dmk_packages-0.7.2/src/dmk_packages/naver_datalab.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.7.0/src/dmk_packages.egg-info/PKG-INFO` & `dmk_packages-0.7.2/src/dmk_packages.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.7.0
+Version: 0.7.2
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dmk_packages-0.7.0/src/dmk_packages.egg-info/SOURCES.txt` & `dmk_packages-0.7.2/src/dmk_packages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

