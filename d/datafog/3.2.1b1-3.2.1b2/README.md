# Comparing `tmp/datafog-3.2.1b1.tar.gz` & `tmp/datafog-3.2.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-3.2.1b1.tar", last modified: Sat May 18 00:01:25 2024, max compression
+gzip compressed data, was "datafog-3.2.1b2.tar", last modified: Sat May 18 20:02:38 2024, max compression
```

## Comparing `datafog-3.2.1b1.tar` & `datafog-3.2.1b2.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 00:01:25.251688 datafog-3.2.1b1/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-17 23:38:08.000000 datafog-3.2.1b1/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     7966 2024-05-18 00:01:25.251544 datafog-3.2.1b1/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     6742 2024-05-17 23:38:08.000000 datafog-3.2.1b1/README.md
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 00:01:25.248324 datafog-3.2.1b1/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-17 23:39:53.000000 datafog-3.2.1b1/datafog/__about__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      862 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      222 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/config.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     3275 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/main.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 00:01:25.249143 datafog-3.2.1b1/datafog/processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)      350 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/processing/__init__.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 00:01:25.249736 datafog-3.2.1b1/datafog/processing/image_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)      146 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/processing/image_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2872 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/processing/image_processing/donut_processor.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      787 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/processing/image_processing/image_downloader.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      297 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/processing/image_processing/pytesseract_processor.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 00:01:25.250107 datafog-3.2.1b1/datafog/processing/spark_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)       69 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/processing/spark_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2225 2024-05-17 23:57:03.000000 datafog-3.2.1b1/datafog/processing/spark_processing/pyspark_udfs.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 00:01:25.250402 datafog-3.2.1b1/datafog/processing/text_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)       51 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/processing/text_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1300 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/processing/text_processing/spacy_pii_annotator.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 00:01:25.250939 datafog-3.2.1b1/datafog/services/
--rw-r--r--   0 sidmohan   (501) staff       (20)      118 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/services/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1802 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/services/image_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1035 2024-05-17 23:47:08.000000 datafog-3.2.1b1/datafog/services/spark_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      633 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/services/text_service.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 00:01:25.249000 datafog-3.2.1b1/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     7966 2024-05-18 00:01:25.000000 datafog-3.2.1b1/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      906 2024-05-18 00:01:25.000000 datafog-3.2.1b1/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-18 00:01:25.000000 datafog-3.2.1b1/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)      144 2024-05-18 00:01:25.000000 datafog-3.2.1b1/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       14 2024-05-18 00:01:25.000000 datafog-3.2.1b1/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-18 00:01:25.251742 datafog-3.2.1b1/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1944 2024-05-17 23:57:53.000000 datafog-3.2.1b1/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 00:01:25.251321 datafog-3.2.1b1/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2024-05-17 23:38:08.000000 datafog-3.2.1b1/tests/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2447 2024-05-17 23:38:08.000000 datafog-3.2.1b1/tests/test_image_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2945 2024-05-17 23:38:08.000000 datafog-3.2.1b1/tests/test_main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 20:02:38.207993 datafog-3.2.1b2/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-18 18:25:55.000000 datafog-3.2.1b2/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     7966 2024-05-18 20:02:38.207742 datafog-3.2.1b2/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6742 2024-05-18 18:25:55.000000 datafog-3.2.1b2/README.md
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 20:02:38.199816 datafog-3.2.1b2/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-18 18:31:18.000000 datafog-3.2.1b2/datafog/__about__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      909 2024-05-18 19:55:14.000000 datafog-3.2.1b2/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      190 2024-05-18 19:53:32.000000 datafog-3.2.1b2/datafog/config.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     3275 2024-05-18 18:25:55.000000 datafog-3.2.1b2/datafog/main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 20:02:38.200763 datafog-3.2.1b2/datafog/processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      400 2024-05-18 19:55:14.000000 datafog-3.2.1b2/datafog/processing/__init__.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 20:02:38.202001 datafog-3.2.1b2/datafog/processing/image_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      146 2024-05-18 18:25:55.000000 datafog-3.2.1b2/datafog/processing/image_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2872 2024-05-18 18:25:55.000000 datafog-3.2.1b2/datafog/processing/image_processing/donut_processor.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      787 2024-05-18 18:25:55.000000 datafog-3.2.1b2/datafog/processing/image_processing/image_downloader.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      297 2024-05-18 18:25:55.000000 datafog-3.2.1b2/datafog/processing/image_processing/pytesseract_processor.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 20:02:38.203489 datafog-3.2.1b2/datafog/processing/spark_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      225 2024-05-18 19:53:34.000000 datafog-3.2.1b2/datafog/processing/spark_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2204 2024-05-18 19:55:14.000000 datafog-3.2.1b2/datafog/processing/spark_processing/pyspark_udfs.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 20:02:38.203922 datafog-3.2.1b2/datafog/processing/text_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       51 2024-05-18 18:25:55.000000 datafog-3.2.1b2/datafog/processing/text_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1300 2024-05-18 18:25:55.000000 datafog-3.2.1b2/datafog/processing/text_processing/spacy_pii_annotator.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 20:02:38.204934 datafog-3.2.1b2/datafog/services/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      118 2024-05-18 18:25:55.000000 datafog-3.2.1b2/datafog/services/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1802 2024-05-18 19:55:14.000000 datafog-3.2.1b2/datafog/services/image_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1030 2024-05-18 19:53:34.000000 datafog-3.2.1b2/datafog/services/spark_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      633 2024-05-18 19:55:14.000000 datafog-3.2.1b2/datafog/services/text_service.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 20:02:38.205756 datafog-3.2.1b2/datafog/telemetry/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       39 2024-05-18 19:53:34.000000 datafog-3.2.1b2/datafog/telemetry/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     4435 2024-05-18 19:53:34.000000 datafog-3.2.1b2/datafog/telemetry/open_telemetry.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 20:02:38.200628 datafog-3.2.1b2/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     7966 2024-05-18 20:02:38.000000 datafog-3.2.1b2/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      972 2024-05-18 20:02:38.000000 datafog-3.2.1b2/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-18 20:02:38.000000 datafog-3.2.1b2/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)      144 2024-05-18 20:02:38.000000 datafog-3.2.1b2/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       14 2024-05-18 20:02:38.000000 datafog-3.2.1b2/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-18 20:02:38.208040 datafog-3.2.1b2/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1944 2024-05-18 20:02:23.000000 datafog-3.2.1b2/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 20:02:38.207388 datafog-3.2.1b2/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2024-05-18 18:25:55.000000 datafog-3.2.1b2/tests/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2447 2024-05-18 18:25:55.000000 datafog-3.2.1b2/tests/test_image_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2785 2024-05-18 19:55:12.000000 datafog-3.2.1b2/tests/test_main.py
```

### Comparing `datafog-3.2.1b1/LICENSE` & `datafog-3.2.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b1/PKG-INFO` & `datafog-3.2.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.1b1
+Version: 3.2.1b2
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: Sid Mohan
 Author-email: sid@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.2.1b1 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.1b2 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: Sid Mohan
 Author-email: sid@datafog.ai Maintainer: DataFog Maintainer-email:
 hi@datafog.ai License: MIT Project-URL: Homepage, https://datafog.ai Project-
 URL: Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-3.2.1b1/README.md` & `datafog-3.2.1b2/README.md`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b1/datafog/__init__.py` & `datafog-3.2.1b2/datafog/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+from .__about__ import __version__
 from .config import OperationType
 from .main import DataFog, OCRPIIAnnotator, TextPIIAnnotator
 from .processing.image_processing.donut_processor import DonutProcessor
 from .processing.image_processing.image_downloader import ImageDownloader
 from .processing.image_processing.pytesseract_processor import PytesseractProcessor
 from .processing.text_processing.spacy_pii_annotator import SpacyPIIAnnotator
 from .services.image_service import ImageService
 from .services.spark_service import SparkService
 from .services.text_service import TextService
-
-# from .__about__ import __version__
+from .telemetry import OTelLogger
 
 __all__ = [
     "DonutProcessor",
     "DataFog",
     "ImageService",
     "OCRPIIAnnotator",
     "OperationType",
     "SparkService",
     "TextPIIAnnotator",
     "TextService",
     "SpacyPIIAnnotator",
     "ImageDownloader",
     "PytesseractProcessor",
-    # "__version__",
+    "__version__",
+    "OTelLogger",
 ]
```

### Comparing `datafog-3.2.1b1/datafog/main.py` & `datafog-3.2.1b2/datafog/main.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b1/datafog/processing/image_processing/donut_processor.py` & `datafog-3.2.1b2/datafog/processing/image_processing/donut_processor.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b1/datafog/processing/image_processing/image_downloader.py` & `datafog-3.2.1b2/datafog/processing/image_processing/image_downloader.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b1/datafog/processing/spark_processing/pyspark_udfs.py` & `datafog-3.2.1b2/datafog/processing/spark_processing/pyspark_udfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import requests
-import spacy
 import importlib
 import subprocess
 import sys
 
+import requests
+import spacy
+
 PII_ANNOTATION_LABELS = ["DATE_TIME", "LOC", "NRP", "ORG", "PER"]
 MAXIMAL_STRING_SIZE = 1000000
 
 
 def pii_annotator(text: str, broadcasted_nlp) -> list[list[str]]:
     """Extract features using en_spacy_pii_fast model.
 
@@ -36,21 +37,22 @@
 
         return [_ent for _ent in classified_entities.values()]
     else:
         return [[] for _ in PII_ANNOTATION_LABELS]
 
 
 def broadcast_pii_annotator_udf(
-    spark_session = None, spacy_model: str = "en_spacy_pii_fast"
+    spark_session=None, spacy_model: str = "en_spacy_pii_fast"
 ):
     """Broadcast PII annotator across Spark cluster and create UDF"""
     ensure_installed("pyspark")
     from pyspark.sql import SparkSession
     from pyspark.sql.functions import udf
     from pyspark.sql.types import ArrayType, StringType, StructField, StructType
+
     if not spark_session:
         spark_session = SparkSession.builder.getOrCreate()
     broadcasted_nlp = spark_session.sparkContext.broadcast(spacy.load(spacy_model))
 
     pii_annotation_udf = udf(
         lambda text: pii_annotator(text, broadcasted_nlp),
         ArrayType(ArrayType(StringType())),
@@ -58,10 +60,8 @@
     return pii_annotation_udf
 
 
 def ensure_installed(self, package_name):
     try:
         importlib.import_module(package_name)
     except ImportError:
-        subprocess.check_call(
-            [sys.executable, "-m", "pip", "install", package_name]
-        )
+        subprocess.check_call([sys.executable, "-m", "pip", "install", package_name])
```

### Comparing `datafog-3.2.1b1/datafog/processing/text_processing/spacy_pii_annotator.py` & `datafog-3.2.1b2/datafog/processing/text_processing/spacy_pii_annotator.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b1/datafog/services/image_service.py` & `datafog-3.2.1b2/datafog/services/image_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b1/datafog/services/spark_service.py` & `datafog-3.2.1b2/datafog/services/spark_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-import json
-from typing import Any, List
 import importlib
+import json
 import subprocess
 import sys
-
+from typing import Any, List
 
 
 class SparkService:
     def __init__(self):
         self.spark = self.create_spark_session()
         self.ensure_installed("pyspark")
 
         from pyspark.sql import DataFrame, SparkSession
         from pyspark.sql.functions import udf
         from pyspark.sql.types import ArrayType, StringType
+
         self.SparkSession = SparkSession
         self.DataFrame = DataFrame
         self.udf = udf
         self.ArrayType = ArrayType
         self.StringType = StringType
 
     def create_spark_session(self):
         return self.SparkSession.builder.appName("datafog").getOrCreate()
-    
+
     def read_json(self, path: str) -> List[dict]:
         return self.spark.read.json(path).collect()
 
     def ensure_installed(self, package_name):
         try:
             importlib.import_module(package_name)
         except ImportError:
             subprocess.check_call(
                 [sys.executable, "-m", "pip", "install", package_name]
             )
-
```

### Comparing `datafog-3.2.1b1/datafog/services/text_service.py` & `datafog-3.2.1b2/datafog/services/text_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b1/datafog.egg-info/PKG-INFO` & `datafog-3.2.1b2/datafog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.1b1
+Version: 3.2.1b2
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: Sid Mohan
 Author-email: sid@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.2.1b1 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.1b2 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: Sid Mohan
 Author-email: sid@datafog.ai Maintainer: DataFog Maintainer-email:
 hi@datafog.ai License: MIT Project-URL: Homepage, https://datafog.ai Project-
 URL: Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-3.2.1b1/datafog.egg-info/SOURCES.txt` & `datafog-3.2.1b2/datafog.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,10 +19,12 @@
 datafog/processing/spark_processing/pyspark_udfs.py
 datafog/processing/text_processing/__init__.py
 datafog/processing/text_processing/spacy_pii_annotator.py
 datafog/services/__init__.py
 datafog/services/image_service.py
 datafog/services/spark_service.py
 datafog/services/text_service.py
+datafog/telemetry/__init__.py
+datafog/telemetry/open_telemetry.py
 tests/__init__.py
 tests/test_image_service.py
 tests/test_main.py
```

### Comparing `datafog-3.2.1b1/setup.py` & `datafog-3.2.1b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "3.2.1b1"
+    return "3.2.1b2"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
```

### Comparing `datafog-3.2.1b1/tests/test_image_service.py` & `datafog-3.2.1b2/tests/test_image_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b1/tests/test_main.py` & `datafog-3.2.1b2/tests/test_main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,12 @@
-import asyncio
 import json
-from typing import List
 
-import aiohttp
 import pytest
 
-from datafog import (
-    DataFog,
-    ImageService,
-    OCRPIIAnnotator,
-    OperationType,
-    SparkService,
-    TextPIIAnnotator,
-    TextService,
-)
+from datafog import DataFog, TextPIIAnnotator
 
 
 def search_nested_dict(d, target):
     """Recursively search for a target value in nested dictionaries."""
     if isinstance(d, dict):
         for key, value in d.items():
             if target in value:
```

