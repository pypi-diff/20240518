# Comparing `tmp/docketanalyzer-0.1.0-py3-none-any.whl.zip` & `tmp/docketanalyzer-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,32 +1,40 @@
-Zip file size: 19984 bytes, number of entries: 30
--rw-r--r--  2.0 unx      281 b- defN 24-Jan-18 19:09 docketanalyzer/__init__.py
--rw-r--r--  2.0 unx      480 b- defN 24-Jan-18 19:10 docketanalyzer/utils.py
--rw-r--r--  2.0 unx      407 b- defN 24-Jan-18 12:07 docketanalyzer/categories/__init__.py
--rw-r--r--  2.0 unx      411 b- defN 24-Jan-18 12:06 docketanalyzer/categories/category.py
--rw-r--r--  2.0 unx     3651 b- defN 24-Jan-18 12:06 docketanalyzer/categories/court.py
--rw-r--r--  2.0 unx      523 b- defN 24-Jan-18 12:07 docketanalyzer/categories/docket.py
--rw-r--r--  2.0 unx     3285 b- defN 24-Jan-18 18:51 docketanalyzer/categories/idb.py
--rw-r--r--  2.0 unx      234 b- defN 24-Jan-18 12:07 docketanalyzer/categories/judge.py
--rw-r--r--  2.0 unx     4464 b- defN 24-Jan-18 12:07 docketanalyzer/categories/nature_suit.py
+Zip file size: 43070 bytes, number of entries: 38
+-rw-r--r--  2.0 unx      786 b- defN 24-May-15 19:55 docketanalyzer/__init__.py
+-rw-r--r--  2.0 unx     2221 b- defN 24-May-15 22:29 docketanalyzer/utils.py
+-rw-r--r--  2.0 unx      335 b- defN 24-May-11 09:38 docketanalyzer/choices/__init__.py
+-rw-r--r--  2.0 unx      369 b- defN 24-Apr-26 04:10 docketanalyzer/choices/choice.py
+-rw-r--r--  2.0 unx     3665 b- defN 24-May-06 01:29 docketanalyzer/choices/court.py
+-rw-r--r--  2.0 unx      508 b- defN 24-Apr-25 23:06 docketanalyzer/choices/docket.py
+-rw-r--r--  2.0 unx     3254 b- defN 24-Apr-25 23:05 docketanalyzer/choices/idb.py
+-rw-r--r--  2.0 unx      223 b- defN 24-Apr-25 23:05 docketanalyzer/choices/judge.py
+-rw-r--r--  2.0 unx      885 b- defN 24-Apr-26 04:12 docketanalyzer/choices/labels.py
+-rw-r--r--  2.0 unx    29155 b- defN 24-Apr-25 23:05 docketanalyzer/choices/nature_suit.py
+-rw-r--r--  2.0 unx      331 b- defN 24-Apr-25 23:05 docketanalyzer/choices/party.py
+-rw-r--r--  2.0 unx      405 b- defN 24-May-15 17:43 docketanalyzer/cli/__init__.py
+-rw-r--r--  2.0 unx      299 b- defN 24-May-18 11:36 docketanalyzer/cli/check_dockets.py
+-rw-r--r--  2.0 unx    12551 b- defN 24-May-18 11:32 docketanalyzer/cli/check_idb.py
+-rw-r--r--  2.0 unx      454 b- defN 24-May-15 18:51 docketanalyzer/cli/configure.py
+-rw-r--r--  2.0 unx      215 b- defN 24-May-09 21:27 docketanalyzer/cli/open.py
+-rw-r--r--  2.0 unx     1346 b- defN 24-May-15 17:42 docketanalyzer/cli/sync.py
+-rw-r--r--  2.0 unx       47 b- defN 24-May-13 10:37 docketanalyzer/config/__init__.py
+-rw-r--r--  2.0 unx     4144 b- defN 24-May-15 19:24 docketanalyzer/config/config.py
+-rw-r--r--  2.0 unx     4461 b- defN 24-May-18 12:38 docketanalyzer/config/env_config.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 12:05 docketanalyzer/core/__init__.py
--rw-r--r--  2.0 unx      379 b- defN 24-Jan-18 17:46 docketanalyzer/core/elastic.py
--rw-r--r--  2.0 unx     1774 b- defN 24-Jan-18 19:09 docketanalyzer/core/recap_api.py
--rw-r--r--  2.0 unx     2425 b- defN 24-Jan-18 12:04 docketanalyzer/core/registry.py
--rw-r--r--  2.0 unx       47 b- defN 24-Jan-18 14:25 docketanalyzer/docket/__init__.py
--rw-r--r--  2.0 unx     3074 b- defN 24-Jan-18 18:07 docketanalyzer/docket/docket.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:52 docketanalyzer/docket/docket_index.py
--rw-r--r--  2.0 unx     1823 b- defN 24-Jan-19 15:02 docketanalyzer/docket/document.py
--rw-r--r--  2.0 unx     1063 b- defN 24-Jan-18 18:05 docketanalyzer/docket/entry.py
--rw-r--r--  2.0 unx     3617 b- defN 24-Jan-18 19:03 docketanalyzer/docket/idb_entry.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:53 docketanalyzer/docket/judge.py
--rw-r--r--  2.0 unx     2786 b- defN 24-Jan-19 15:22 docketanalyzer/docket/manager.py
--rw-r--r--  2.0 unx      543 b- defN 24-Jan-19 15:24 docketanalyzer/docket/manager_document_mixin.py
--rw-r--r--  2.0 unx     7458 b- defN 24-Jan-18 18:55 docketanalyzer/docket/manager_idb_mixin.py
--rw-r--r--  2.0 unx     1992 b- defN 24-Jan-18 17:06 docketanalyzer/docket/manager_pacer_mixin.py
--rw-r--r--  2.0 unx     5010 b- defN 24-Jan-19 15:24 docketanalyzer/docket/manager_recap_mixin.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-18 13:53 docketanalyzer/docket/party.py
--rw-r--r--  2.0 unx      676 b- defN 24-Jan-19 16:28 docketanalyzer-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-19 16:28 docketanalyzer-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 24-Jan-19 16:28 docketanalyzer-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2674 b- defN 24-Jan-19 16:28 docketanalyzer-0.1.0.dist-info/RECORD
-30 files, 49184 bytes uncompressed, 15592 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx     6889 b- defN 24-May-15 19:55 docketanalyzer/core/chat.py
+-rw-r--r--  2.0 unx    12683 b- defN 24-May-18 13:29 docketanalyzer/core/core_dataset.py
+-rw-r--r--  2.0 unx     2917 b- defN 24-May-18 11:35 docketanalyzer/core/docket_index.py
+-rw-r--r--  2.0 unx     5776 b- defN 24-May-18 15:02 docketanalyzer/core/docket_manager.py
+-rw-r--r--  2.0 unx      322 b- defN 24-May-18 15:38 docketanalyzer/core/elastic.py
+-rw-r--r--  2.0 unx     4240 b- defN 24-May-18 12:02 docketanalyzer/core/juri.py
+-rw-r--r--  2.0 unx     1523 b- defN 24-May-15 17:19 docketanalyzer/core/ocr.py
+-rw-r--r--  2.0 unx     2134 b- defN 24-May-05 11:22 docketanalyzer/core/registry.py
+-rw-r--r--  2.0 unx     1960 b- defN 24-May-15 17:37 docketanalyzer/core/s3.py
+-rw-r--r--  2.0 unx      691 b- defN 24-May-13 14:45 docketanalyzer/tasks/__init__.py
+-rw-r--r--  2.0 unx     5075 b- defN 24-May-18 13:42 docketanalyzer/tasks/task.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-18 16:25 docketanalyzer-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      724 b- defN 24-May-18 16:25 docketanalyzer-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-18 16:25 docketanalyzer-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       42 b- defN 24-May-18 16:25 docketanalyzer-0.1.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 24-May-18 16:25 docketanalyzer-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3312 b- defN 24-May-18 16:25 docketanalyzer-0.1.1.dist-info/RECORD
+38 files, 125406 bytes uncompressed, 37718 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -1,91 +1,115 @@
 Filename: docketanalyzer/__init__.py
 Comment: 
 
 Filename: docketanalyzer/utils.py
 Comment: 
 
-Filename: docketanalyzer/categories/__init__.py
+Filename: docketanalyzer/choices/__init__.py
 Comment: 
 
-Filename: docketanalyzer/categories/category.py
+Filename: docketanalyzer/choices/choice.py
 Comment: 
 
-Filename: docketanalyzer/categories/court.py
+Filename: docketanalyzer/choices/court.py
 Comment: 
 
-Filename: docketanalyzer/categories/docket.py
+Filename: docketanalyzer/choices/docket.py
 Comment: 
 
-Filename: docketanalyzer/categories/idb.py
+Filename: docketanalyzer/choices/idb.py
 Comment: 
 
-Filename: docketanalyzer/categories/judge.py
+Filename: docketanalyzer/choices/judge.py
 Comment: 
 
-Filename: docketanalyzer/categories/nature_suit.py
+Filename: docketanalyzer/choices/labels.py
 Comment: 
 
-Filename: docketanalyzer/core/__init__.py
+Filename: docketanalyzer/choices/nature_suit.py
 Comment: 
 
-Filename: docketanalyzer/core/elastic.py
+Filename: docketanalyzer/choices/party.py
 Comment: 
 
-Filename: docketanalyzer/core/recap_api.py
+Filename: docketanalyzer/cli/__init__.py
 Comment: 
 
-Filename: docketanalyzer/core/registry.py
+Filename: docketanalyzer/cli/check_dockets.py
+Comment: 
+
+Filename: docketanalyzer/cli/check_idb.py
+Comment: 
+
+Filename: docketanalyzer/cli/configure.py
+Comment: 
+
+Filename: docketanalyzer/cli/open.py
+Comment: 
+
+Filename: docketanalyzer/cli/sync.py
 Comment: 
 
-Filename: docketanalyzer/docket/__init__.py
+Filename: docketanalyzer/config/__init__.py
 Comment: 
 
-Filename: docketanalyzer/docket/docket.py
+Filename: docketanalyzer/config/config.py
 Comment: 
 
-Filename: docketanalyzer/docket/docket_index.py
+Filename: docketanalyzer/config/env_config.py
 Comment: 
 
-Filename: docketanalyzer/docket/document.py
+Filename: docketanalyzer/core/__init__.py
+Comment: 
+
+Filename: docketanalyzer/core/chat.py
 Comment: 
 
-Filename: docketanalyzer/docket/entry.py
+Filename: docketanalyzer/core/core_dataset.py
 Comment: 
 
-Filename: docketanalyzer/docket/idb_entry.py
+Filename: docketanalyzer/core/docket_index.py
 Comment: 
 
-Filename: docketanalyzer/docket/judge.py
+Filename: docketanalyzer/core/docket_manager.py
+Comment: 
+
+Filename: docketanalyzer/core/elastic.py
 Comment: 
 
-Filename: docketanalyzer/docket/manager.py
+Filename: docketanalyzer/core/juri.py
+Comment: 
+
+Filename: docketanalyzer/core/ocr.py
+Comment: 
+
+Filename: docketanalyzer/core/registry.py
 Comment: 
 
-Filename: docketanalyzer/docket/manager_document_mixin.py
+Filename: docketanalyzer/core/s3.py
 Comment: 
 
-Filename: docketanalyzer/docket/manager_idb_mixin.py
+Filename: docketanalyzer/tasks/__init__.py
 Comment: 
 
-Filename: docketanalyzer/docket/manager_pacer_mixin.py
+Filename: docketanalyzer/tasks/task.py
 Comment: 
 
-Filename: docketanalyzer/docket/manager_recap_mixin.py
+Filename: docketanalyzer-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: docketanalyzer/docket/party.py
+Filename: docketanalyzer-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: docketanalyzer-0.1.0.dist-info/METADATA
+Filename: docketanalyzer-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: docketanalyzer-0.1.0.dist-info/WHEEL
+Filename: docketanalyzer-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: docketanalyzer-0.1.0.dist-info/top_level.txt
+Filename: docketanalyzer-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: docketanalyzer-0.1.0.dist-info/RECORD
+Filename: docketanalyzer-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## docketanalyzer/__init__.py

```diff
@@ -1,8 +1,22 @@
+from docketanalyzer.config import config
 import docketanalyzer.utils as utils
 
-from docketanalyzer.core.elastic import load_elastic
-from docketanalyzer.core.recap_api import RECAPApi
 from docketanalyzer.core.registry import Registry
+import docketanalyzer.choices as choices
+
+from docketanalyzer.core.chat import Chat, ChatThread
+from docketanalyzer.core.elastic import load_elastic
+from docketanalyzer.core.s3 import S3Utility
+from docketanalyzer.core.juri import JuriscraperUtility
+from docketanalyzer.core.ocr import OCRUtility
+
+from docketanalyzer.core.core_dataset import CoreDataset, load_dataset
+from docketanalyzer.core.docket_manager import DocketManager
+from docketanalyzer.core.docket_index import DocketIndex, load_docket_index
+
+from docketanalyzer.tasks import Task, DocketTask, load_tasks, load_task, register_task
+
+from docketanalyzer.cli import cli
 
-import docketanalyzer.categories as categories
-from docketanalyzer.docket import Docket
+class RecapApi:
+    pass
```

## docketanalyzer/utils.py

```diff
@@ -1,19 +1,72 @@
-import os
+from datetime import datetime, date
+from dateutil.parser._parser import ParserError
+import pandas as pd
+from pandas._libs.tslibs.np_datetime import OutOfBoundsDatetime
 from pathlib import Path
-from dotenv import load_dotenv
+import regex as re
+from docketanalyzer import config
 
 
-load_dotenv(override=True)
+# Configuration
+DATA_DIR = config['DA_DATA_DIR']
+COURTLISTENER_TOKEN = config['COURTLISTENER_TOKEN']
+PACER_USERNAME = config['PACER_USERNAME']
+PACER_PASSWORD = config['PACER_PASSWORD']
+HF_TOKEN = config['HF_TOKEN']
+GROQ_API_KEY = config['GROQ_API_KEY']
+GROQ_DEFAULT_CHAT_MODEL = config['GROQ_DEFAULT_CHAT_MODEL']
+OPENAI_API_KEY = config['OPENAI_API_KEY']
+OPENAI_ORG_ID = config['OPENAI_ORG_ID']
+OPENAI_DEFAULT_CHAT_MODEL = config['OPENAI_DEFAULT_CHAT_MODEL']
+OPENAI_DEFAULT_EMBEDDING_MODEL = config['OPENAI_DEFAULT_EMBEDDING_MODEL']
+POSTGRES_HOST = config['POSTGRES_HOST']
+POSTGRES_PORT = config['POSTGRES_PORT']
+POSTGRES_USERNAME = config['POSTGRES_USERNAME']
+POSTGRES_PASSWORD = config['POSTGRES_PASSWORD']
+POSTGRES_DB = config['POSTGRES_DB']
+ELASTIC_HOST = config['ELASTIC_HOST']
+ELASTIC_PORT = config['ELASTIC_PORT']
+ELASTIC_USERNAME = config['ELASTIC_USERNAME']
+ELASTIC_PASSWORD = config['ELASTIC_PASSWORD']
+AWS_ACCESS_KEY_ID = config['AWS_ACCESS_KEY_ID']
+AWS_SECRET_ACCESS_KEY = config['AWS_SECRET_ACCESS_KEY']
+AWS_S3_BUCKET_NAME = config['AWS_S3_BUCKET_NAME']
+AWS_S3_ENDPOINT_URL = config['AWS_S3_ENDPOINT_URL']
+AWS_S3_REGION_NAME = config['AWS_S3_REGION_NAME']
+
+# Other Utilities
+def notabs(text):
+    return '\n'.join([x.strip() for x in text.split('\n')]).strip()
+
+
+def convert_date(x):
+    if x:
+        try:
+            return pd.to_datetime(x).date()
+        except (ParserError, OutOfBoundsDatetime):
+            pass
+
+
+def convert_int(x):
+    if x is not None:
+        try:
+            return int(x)
+        except ValueError:
+            pass
+
+
+def json_default(obj):
+    if isinstance(obj, (datetime, date)):
+        return obj.isoformat()
+
+
+def pd_save_or_append(data, path, **kwargs):
+    path = Path(path)
+    if path.exists():
+        data.to_csv(path, mode='a', header=False, index=False, **kwargs)
+    else:
+        data.to_csv(path, index=False, **kwargs)
 
 
-DATA_DIR = Path(os.environ.get(
-    'DOCKETANALYZER_DATA_DIR',
-    Path.home().resolve() / 'data' / 'docketanalyzer',
-))
-
-COURTLISTENER_TOKEN = os.environ.get('COURTLISTENER_TOKEN')
-
-ELASTIC_HOST = os.environ.get('ELASTIC_HOST')
-ELASTIC_PORT = os.environ.get('ELASTIC_PORT')
-ELASTIC_PASSWORD = os.environ.get('ELASTIC_PASSWORD')
-ELASTIC_USERNAME = os.environ.get('ELASTIC_USERNAME')
+def get_clean_name(name):
+    return re.sub(r"[,.;@#?!&$]+\ *", " ", name.lower()).strip()
```

## docketanalyzer/core/elastic.py

```diff
@@ -1,12 +1,10 @@
 from elasticsearch import Elasticsearch
 from docketanalyzer.utils import ELASTIC_HOST, ELASTIC_PORT, ELASTIC_USERNAME, ELASTIC_PASSWORD
 
 
-def load_elastic():
-    """
-    Load the Elasticsearch client with the appropriate credentials.
-    """
+def load_elastic(**kwargs):
     return Elasticsearch(
         f"http://{ELASTIC_HOST}:{ELASTIC_PORT}",
-        basic_auth=(ELASTIC_USERNAME, ELASTIC_PASSWORD)
+        basic_auth=(ELASTIC_USERNAME, ELASTIC_PASSWORD),
+        **kwargs,
     )
```

## docketanalyzer/core/registry.py

```diff
@@ -3,53 +3,41 @@
 import pkgutil
 from typing import Any, Optional
 from types import ModuleType
 
 
 class Registry:
     """
-    Base class to create a registry of objects.
+    Implement a custom 'find' condition and automatically build a registry of relevant objects in the current module.
     """
 
     def __init__(self) -> None:
         self._registry: dict[str, Any] = {}
         self.module: ModuleType = inspect.getmodule(inspect.stack()[1][0])
 
     def register(self, name: str, obj: Any) -> None:
-        """
-        Add an object to the registry.
-        """
         if name in self._registry:
             raise ValueError(f"'{name}' already exists.")
         self._registry[name] = obj
 
     def get(self, name: str) -> Any:
-        """
-        Retrieve an object from the registry.
-        """
         if name not in self._registry:
             raise ValueError(f"'{name}' does not exist.")
         return self._registry[name]
 
     def all(self) -> list[Any]:
-        """
-        Get a list of all registered objects.
-        """
         return list(self._registry.values())
 
     def find_filter(self, obj: Any) -> bool:
         """
-        A filter used by the `find` method to determine if an object should be registered.
+        Add your custom object test here.
         """
         raise NotImplementedError("find_filter() must be implemented by a subclass.")
 
     def find(self, module: Optional[ModuleType] = None, recurse: bool = False) -> None:
-        """
-        Find all objects in current module and registers those that pass the filter.
-        """
         if module is None:
             module = self.module
         if isinstance(module, str):
             module = importlib.import_module(module)
         for _, submodule_name, _ in pkgutil.walk_packages(module.__path__):
             submodule = importlib.import_module(f"{module.__name__}.{submodule_name}")
             for name in dir(submodule):
```

## Comparing `docketanalyzer/categories/court.py` & `docketanalyzer/choices/court.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from docketanalyzer.categories.category import Category
+from docketanalyzer.choices.choice import Choice
 
 
-class DistrictCourt(Category):
+class DistrictCourt(Choice):
     dcd = "District of Columbia"
     almd = "Alabama, Middle District"
     alnd = "Alabama, Northern District"
     alsd = "Alabama, Southern District"
     akd = "Alaska, District"
     azd = "Arizona, District"
     ared = "Arkansas, Eastern District"
@@ -92,7 +92,8 @@
     wied = "Wisconsin, Eastern District"
     wiwd = "Wisconsin, Western District"
     wyd = "Wyoming, District"
     gud = "Guam, District"
     nmid = "Northern Mariana Islands, District"
     prd = "Puerto Rico, District"
     vid = "Virgin Islands, District"
+    psc = "Demo Court"
```

## Comparing `docketanalyzer/categories/idb.py` & `docketanalyzer/choices/idb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from docketanalyzer.categories.category import Category
+from docketanalyzer.choices.choice import Choice
 
 
-class IDBArbitrationAtFiling(Category):
+class IDBArbitrationAtFiling(Choice):
     _0 = "Exempt"
     _1 = "Mandatory"
     _2 = "Missing"
     _3 = "No"
     _4 = "Voluntary"
     _5 = "Yes, Type Unknown"
 
 
-class IDBArbitrationAtTermination(Category):
+class IDBArbitrationAtTermination(Choice):
     _0 = "Exempt"
     _1 = "Mandatory"
     _2 = "Missing"
     _3 = "Voluntary"
 
 
-class IDBClassAction(Category):
+class IDBClassAction(Choice):
     _0 = "Yes"
     _1 = "No"
     _2 = "Missing"
 
 
-class IDBDisposition(Category):
+class IDBDisposition(Choice):
     _0 = "Appeal Affirmed (Magistrate Judge)"
     _1 = "Appeal Denied (Magistrate Judge)"
     _2 = "Dismissal - Lack of Jurisdiction"
     _3 = "Dismissal - Other"
     _4 = "Dismissal - Settled"
     _5 = "Dismissal - Voluntarily"
     _6 = "Dismissal - Want of Prosecution"
@@ -44,46 +44,46 @@
     _17 = "Remanded to State Court"
     _18 = "Remanded to U.S. Agency"
     _19 = "Statistical Closing"
     _20 = "Stayed Pending Bankruptcy"
     _21 = "Transfer to Another District"
 
 
-class IDBIFP(Category):
+class IDBIFP(Choice):
     _0 = "Yes"
     _1 = "No"
     _2 = "Missing"
 
 
-class IDBJudgment(Category):
+class IDBJudgment(Choice):
     _0 = "Both"
     _1 = "Defendant"
     _2 = "Missing"
     _3 = "Plaintiff"
     _4 = "Unknown"
 
 
-class IDBMDL(Category):
+class IDBMDL(Choice):
     _0 = "Yes"
     _1 = "No"
     _2 = "Missing"
 
 
-class IDBNatureOfJudgment(Category):
+class IDBNatureOfJudgment(Choice):
     _0 = "Costs Only"
     _1 = "Costs and Attorney Fees"
     _2 = "Forfeiture/Foreclosure/Condemnation, etc."
     _3 = "Injunction"
     _4 = "Missing"
     _5 = "Monetary Award Only"
     _6 = "Monetary Award and Other"
     _7 = "No Monetary Award"
 
 
-class IDBOrigin(Category):
+class IDBOrigin(Choice):
     _0 = "Appeal to District Judge of Magistrate Judge Decision"
     _1 = "Fifth Reopen"
     _2 = "Fourth Reopen"
     _3 = "Multi District Litigation"
     _4 = "Multi District Litigation Originating in the District"
     _5 = "Original Proceeding"
     _6 = "Reinstated/Reopened"
@@ -91,15 +91,15 @@
     _8 = "Removed"
     _9 = "Second Reopen"
     _10 = "Sixth Reopen"
     _11 = "Third Reopen"
     _12 = "Transferred from Another District"
 
 
-class IDBProceduralProgress(Category):
+class IDBProceduralProgress(Choice):
     _0 = "After Issue Joined - After Court Trial"
     _1 = "After Issue Joined - After Jury Trial"
     _2 = "After Issue Joined - During Court Trial"
     _3 = "After Issue Joined - During Jury Trial"
     _4 = "After Issue Joined - Judgment on Motion"
     _5 = "After Issue Joined - No Court Action"
     _6 = "After Issue Joined - Other"
@@ -108,19 +108,19 @@
     _9 = "Before Issue Joined - Hearing Held"
     _10 = "Before Issue Joined - No Court Action"
     _11 = "Before Issue Joined - Order Decided"
     _12 = "Before Issue Joined - Order Entered"
     _13 = "Missing"
 
 
-class IDBProSe(Category):
+class IDBProSe(Choice):
     _0 = "Both Plaintiff & Defendant"
     _1 = "Defendant"
     _2 = "Missing"
     _3 = "None"
     _4 = "Plaintiff"
 
 
-class IDBStatusCode(Category):
+class IDBStatusCode(Choice):
     _0 = "Missing"
     _1 = "Pending Record"
     _2 = "Terminated Record"
```

## Comparing `docketanalyzer/docket/manager_pacer_mixin.py` & `docketanalyzer/core/ocr.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,49 @@
-import simplejson as json
+import os
+import time
+from pathlib import Path
+import requests
 
 
-class PACERMixin:
-    @property
-    def pacer_html_paths(self):
-        return self.dir.glob('pacer.*.html')
+class OCRUtility:
+    def __init__(self, host='http://localhost', port=5050, workers=6):
+        self.host = host
+        self.port = port
+        self.workers = workers
+        self.started = False
 
     @property
-    def pacer_json_path(self):
-        return self.dir / 'pacer.json'
+    def url(self):
+        return f'{self.host}:{self.port}'
 
     @property
-    def pacer_json(self):
-        if self.pacer_json_path.exists():
-            return json.loads(self.pacer_json_path.read_text())
-        print(f'No pacer.json for {self.dir}')
-
-    def pacer_add_html(self, html):
-        path = self.dir / f'pacer.{len(list(self.html_paths))}.html'
-        path.write_text(html)
-
-    def pacer_consolidate_header(self):
-        pacer_json = self.pacer_json
-        if pacer_json is not None:
-            pacer_json['docket_number'] = pacer_json['ucid'].split(';;')[-1]
-            pacer_json['nature_suit'] = f"_{pacer_json['nature_suit'].split()[0]}"
-            fields = [
-                'court', 'docket_number', 'filing_date', 'terminating_date',
-                'nature_suit', 'cause'
-            ]
-            return {k: pacer_json[k] for k in fields}
-        return {}
-
-    def pacer_consolidate_entries(self):
-        pacer_json = self.pacer_json
-        entries = []
-        if pacer_json is not None:
-            for row_number, entry in enumerate(pacer_json['docket']):
-                docs = []
-                for attachment_number, doc in entry['documents'].items():
-                    attachment_number = int(attachment_number)
-                    attachment_number = None if attachment_number == 0 else attachment_number
-                    docs.append({
-                        'attachment_number': attachment_number,
-                        'pacer_url': doc['url'],
-                    })
-                entries.append({
-                    'row_number': row_number,
-                    'entry_number': entry['ind'],
-                    'text': entry['docket_text'],
-                    'date_filed': entry['date_filed'],
-                    'docs': docs,
-                })
-        return entries
+    def is_running(self):
+        try:
+            requests.get(self.url)
+            return True
+        except requests.exceptions.ConnectionError:
+            return False
+
+    def start(self, workers):
+        if self.is_running:
+            print('OCR server already running.')
+        else:
+            workers_arg = '' if workers <= 1 else f' -e DOCTOR_WORKERS={workers} '
+            cmd = f'docker run -d -p {self.port}:5050 {workers_arg} freelawproject/doctor:latest'
+            print(f'Starting OCR server with command: {cmd}')
+            os.system(cmd)
+            while not self.is_running:
+                print('Waiting for service to start...')
+                time.sleep(5)
+            print(f'OCR server running at {self.url}')
+        self.started = True
+
+    def extract_text(self, pdf_path, ocr_available=True):
+        if not self.started:
+            self.start(self.workers)
+        pdf_path = Path(pdf_path)
+        url = self.url + '/extract/doc/text/'
+        if ocr_available:
+            url += '?ocr_available=True'
+        return requests.post(
+            url, files={'file': (pdf_path.name, pdf_path.read_bytes())},
+        ).json()
```

## Comparing `docketanalyzer-0.1.0.dist-info/METADATA` & `docketanalyzer-0.1.1.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: docketanalyzer
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://github.com/docketanalyzer/docketanalyzer
 Author: Nathan Dahlberg
+License-File: LICENSE
 Requires-Dist: awscli
 Requires-Dist: boto3
+Requires-Dist: bs4
 Requires-Dist: click
-Requires-Dist: datasets
-Requires-Dist: evaluate
-Requires-Dist: faiss-cpu
+Requires-Dist: django
+Requires-Dist: elasticsearch
 Requires-Dist: flake8
-Requires-Dist: gunicorn
+Requires-Dist: groq
+Requires-Dist: instructor
+Requires-Dist: juriscraper
+Requires-Dist: openai
 Requires-Dist: pandas
-Requires-Dist: pdf2image
-Requires-Dist: pdoc
-Requires-Dist: protobuf
-Requires-Dist: python-dotenv
 Requires-Dist: psycopg2-binary
-Requires-Dist: runpod
-Requires-Dist: scikit-learn
-Requires-Dist: sentencepiece
-Requires-Dist: shortuuid
+Requires-Dist: pydantic
+Requires-Dist: python-dotenv
+Requires-Dist: regex
+Requires-Dist: requests
 Requires-Dist: simplejson
+Requires-Dist: sqlalchemy
+Requires-Dist: tiktoken
 Requires-Dist: toolz
 Requires-Dist: tqdm
-Requires-Dist: transformers
+Requires-Dist: uuid
+Requires-Dist: wget
```

## Comparing `docketanalyzer-0.1.0.dist-info/RECORD` & `docketanalyzer-0.1.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,38 @@
-docketanalyzer/__init__.py,sha256=qsskP_BzmjMxXR_qWJY2Oznsui38Ln609C_BYwEWwRM,281
-docketanalyzer/utils.py,sha256=M1-0WrOMNYVS12VhEpOzKPU6XsdvIpmAXFgZQFzf8HE,480
-docketanalyzer/categories/__init__.py,sha256=cN8x2lM3O21uOVv9a_GCLT7Gmky7ml9A_o-NcgQ1bAg,407
-docketanalyzer/categories/category.py,sha256=LQGuxOXde7F7KCXxcOepR3JbzPtSo00DBvZP2la5dTo,411
-docketanalyzer/categories/court.py,sha256=zqWyywvdOogdUIpgCQ8FJ_AeqM_ldWL_7iomAfh1FSs,3651
-docketanalyzer/categories/docket.py,sha256=NhbJ0U__lqcToisZ0hitTplZxTXWdl5Mxmt42XRftOw,523
-docketanalyzer/categories/idb.py,sha256=Iem_l-0vzWh5OTez3YFQma8vuXqGRFAHegn8_WUnE0M,3285
-docketanalyzer/categories/judge.py,sha256=xczX6rvm3qaKQ24Xzd8guk_JHerRoqDsUn_F6darLcU,234
-docketanalyzer/categories/nature_suit.py,sha256=Ok3FAsf4OZ4NzZMPQjAbwIryqKsE4v_A75lte1rufn8,4464
+docketanalyzer/__init__.py,sha256=u6fQHIKvVG4jvZxqNbZeBLO0TNkCo8ZT3BvIKzl5M3w,786
+docketanalyzer/utils.py,sha256=dcQKphPxzqmnZdSh8nzB6rsYTWek_Noa8vbOT8GcFtg,2221
+docketanalyzer/choices/__init__.py,sha256=ksPDNySxYNCWPMURUfV0fNKRlCqt_QaecNoJy48VI8s,335
+docketanalyzer/choices/choice.py,sha256=SCWm2wV4iNvL-CFrvk_wh3mBCUEpRbm7yfCA_AUN7Yg,369
+docketanalyzer/choices/court.py,sha256=lf8ga3ClHiiCVNBh_RD-y4L4Ej1bCtF2xHMbdTNwfJI,3665
+docketanalyzer/choices/docket.py,sha256=L-He8VBAKGTGgVMurp_6Vw-uNdGq8lgse_o03nUwLLM,508
+docketanalyzer/choices/idb.py,sha256=4pDRjQK7ZbGM27jvCQVH1nnAvZfbCcq5XMgde4ksLjk,3254
+docketanalyzer/choices/judge.py,sha256=Xx0u1Md-OcGeY0BK0iLSnC1GoSX0dWJ1V3jGbFtWcGM,223
+docketanalyzer/choices/labels.py,sha256=HcvDcysbP-6VIlxE6iUeYrGWRnTxJBhIzMvThSXmpkY,885
+docketanalyzer/choices/nature_suit.py,sha256=TP7o8deg27E385OLZ2vMvHcZwe76auRrsAHHJcztKls,29155
+docketanalyzer/choices/party.py,sha256=Kt9TndeHbZgygLaOyRy0iKC1ikc0uGLAo4Ki6AWx8x0,331
+docketanalyzer/cli/__init__.py,sha256=FDYooNitZbebwguiY4WsdZ4wTfTqa_ceqsizwrRBhjE,405
+docketanalyzer/cli/check_dockets.py,sha256=UGtzx-6KS7Vd7AoQg4H5i0OWTwbH5hn6XgzlJI93lko,299
+docketanalyzer/cli/check_idb.py,sha256=nmq4JGeIaUGapp1_WCF45yVJlAnFGBOtdJj62v315AE,12551
+docketanalyzer/cli/configure.py,sha256=d5tvCRVF5XQRT4I2uVV0HTMHEXWcwsZFr_iZaO9Oqv0,454
+docketanalyzer/cli/open.py,sha256=4PcRQsFZD0wV6_XLz9FZqqsPOBwwoAd9PuQj_0Z31aI,215
+docketanalyzer/cli/sync.py,sha256=HxLSBpix7zjXJ08aKvey3M2IuA5TpwGtjxAJqLOP5_E,1346
+docketanalyzer/config/__init__.py,sha256=mftnxUdK-s4xkEILGIU-wSPn11ZaarRUKjsDGwmDu2c,47
+docketanalyzer/config/config.py,sha256=4Q0LQFdg8PwmaS1h6Ikcs3SrzM7SDWv9NP5xSkjYhSQ,4144
+docketanalyzer/config/env_config.py,sha256=DBkv9dSPKT9aW_SAGpVzZKrEHHydqcNegrhCqiO6N0U,4461
 docketanalyzer/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-docketanalyzer/core/elastic.py,sha256=h5LJksQcY2Y9vKjk8sv90HnpNT2PWiNjbOLDAFk1Ets,379
-docketanalyzer/core/recap_api.py,sha256=RfQ7EM43vE3MIDr7KgVRxeuxKIWlCHQPxPySs1rHxfM,1774
-docketanalyzer/core/registry.py,sha256=DysFM7Ybt-Hoc_BGcDku9PlRoU2jOVnHK6135EB6-JQ,2425
-docketanalyzer/docket/__init__.py,sha256=R9HuWyJ2ilOkkFPxk4JdLiyV1-b190ol3wS87PGfRuM,47
-docketanalyzer/docket/docket.py,sha256=VmAN38YBL4FtZtrwRmaaqgn-I11NJxh_S759fUdYmj4,3074
-docketanalyzer/docket/docket_index.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-docketanalyzer/docket/document.py,sha256=AUUxuesvJAW2pE3ffFgfWJ24TcvebC6uKTYX91nMCMk,1823
-docketanalyzer/docket/entry.py,sha256=izVzo6Alr2uOVyoASsAAHm2CcCOK-WeaaTb-oPe3kGI,1063
-docketanalyzer/docket/idb_entry.py,sha256=J6IHeGEI_VmpFSpZ807quWSPVmDYpFfE9DK505BftpQ,3617
-docketanalyzer/docket/judge.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-docketanalyzer/docket/manager.py,sha256=BM5CuQLBC05kAkOnIpFCCnb40C_wtOMo_WxofEYBtxU,2786
-docketanalyzer/docket/manager_document_mixin.py,sha256=kGjlsnjvkAHgxy4gY91tfYtE-wu_oU-CHAgkugfzFnE,543
-docketanalyzer/docket/manager_idb_mixin.py,sha256=scj3idZ6vAK_QQI0u2VCRenSfeWp4b_GxNb0HDe8Smc,7458
-docketanalyzer/docket/manager_pacer_mixin.py,sha256=KHdMzDETeCLEToSB0A42Ty9vKlVc1y92zEw7bBllAG4,1992
-docketanalyzer/docket/manager_recap_mixin.py,sha256=rKBKD6tiMKYweWAt93eMwKgF-Jc1sCIo4RWX7nVu_Yg,5010
-docketanalyzer/docket/party.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-docketanalyzer-0.1.0.dist-info/METADATA,sha256=qU5-gX9AYaYEarnRmJTr377pD3Q_SjqyP_NPSrL5D_M,676
-docketanalyzer-0.1.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-docketanalyzer-0.1.0.dist-info/top_level.txt,sha256=SAf8EHScfmRuAp94vyx0-f9NyY_eE_SM91xE7zayoq4,15
-docketanalyzer-0.1.0.dist-info/RECORD,,
+docketanalyzer/core/chat.py,sha256=AM8S4mseOml8CuzPrBC8RVF3v8_hVeDgK8cOu43Z49s,6889
+docketanalyzer/core/core_dataset.py,sha256=z0s_zrvU0yo16wn4mHMCNcwvckKQO6J1B85tOjlsF5Y,12683
+docketanalyzer/core/docket_index.py,sha256=jx6fHVgZQZNpe3nWeVfwV-gHRSxK_ft49B-Xodv3tR0,2917
+docketanalyzer/core/docket_manager.py,sha256=RqlciN2ih4tbgopuhcGnxigPWxtrIgtSZ6ynmgQfPoE,5776
+docketanalyzer/core/elastic.py,sha256=munMq8f0RJvY9uKCriax7Y8Vq0kQ1C2EIg8WThHKUdk,322
+docketanalyzer/core/juri.py,sha256=0qC40iV37AS2zqKVUmaNG0pCnVp56HQ97u0ygdFt5KM,4240
+docketanalyzer/core/ocr.py,sha256=y7I5z4wIu3bIRX7kj7WBiOMO_uYUPqMmM56x4KNmk-M,1523
+docketanalyzer/core/registry.py,sha256=J-xzP-UTyXqwtZgrPQRUVyagh4Bwkbr0bscNVrF59hc,2134
+docketanalyzer/core/s3.py,sha256=cotMQClmXT0Wn2O6_9AWDyHtZhyMJ5uOlphXBYZ6JMQ,1960
+docketanalyzer/tasks/__init__.py,sha256=H2NohkZlaoyhuXP-dmq4gBFYA9YYL-LKLyPoyb2t3Wc,691
+docketanalyzer/tasks/task.py,sha256=ZPuRiV5e8uOo1M1ZmGP2wdC2kmrNPd48BJkoMpsdkfo,5075
+docketanalyzer-0.1.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+docketanalyzer-0.1.1.dist-info/METADATA,sha256=gDuVgghRLU5WAWkKgoHx5dZd8vWL9bFxjCHwvF8seJs,724
+docketanalyzer-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+docketanalyzer-0.1.1.dist-info/entry_points.txt,sha256=H-gWnemUSro0E8BMhV1pRz5QgBZd_4A-j-km3wBxOVs,42
+docketanalyzer-0.1.1.dist-info/top_level.txt,sha256=SAf8EHScfmRuAp94vyx0-f9NyY_eE_SM91xE7zayoq4,15
+docketanalyzer-0.1.1.dist-info/RECORD,,
```

