# Comparing `tmp/SQLLite3HelperClass-0.5.tar.gz` & `tmp/SQLLite3HelperClass-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLLite3HelperClass-0.5.tar", last modified: Tue Apr 23 13:53:40 2024, max compression
+gzip compressed data, was "SQLLite3HelperClass-1.0.tar", last modified: Sat May 18 18:30:28 2024, max compression
```

## Comparing `SQLLite3HelperClass-0.5.tar` & `SQLLite3HelperClass-1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 13:53:40.548902 SQLLite3HelperClass-0.5/
--rw-rw-rw-   0        0        0     1084 2023-09-11 14:39:05.000000 SQLLite3HelperClass-0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      531 2024-04-23 13:53:40.549942 SQLLite3HelperClass-0.5/PKG-INFO
--rw-rw-rw-   0        0        0      368 2023-09-11 14:39:05.000000 SQLLite3HelperClass-0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 13:53:40.534939 SQLLite3HelperClass-0.5/SQLLite3HelperClass/
--rw-rw-rw-   0        0        0     3297 2024-04-23 12:36:38.000000 SQLLite3HelperClass-0.5/SQLLite3HelperClass/SQLLite3HelperClass.py
--rw-rw-rw-   0        0        0       66 2023-09-11 14:39:05.000000 SQLLite3HelperClass-0.5/SQLLite3HelperClass/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 13:53:40.546907 SQLLite3HelperClass-0.5/SQLLite3HelperClass.egg-info/
--rw-rw-rw-   0        0        0      531 2024-04-23 13:53:40.000000 SQLLite3HelperClass-0.5/SQLLite3HelperClass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2024-04-23 13:53:40.000000 SQLLite3HelperClass-0.5/SQLLite3HelperClass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 13:53:40.000000 SQLLite3HelperClass-0.5/SQLLite3HelperClass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-23 13:53:40.000000 SQLLite3HelperClass-0.5/SQLLite3HelperClass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-23 13:53:40.550924 SQLLite3HelperClass-0.5/setup.cfg
--rw-rw-rw-   0        0        0      587 2024-04-23 12:19:49.000000 SQLLite3HelperClass-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:30:28.374564 SQLLite3HelperClass-1.0/
+-rw-rw-rw-   0        0        0     1084 2023-09-11 14:39:05.000000 SQLLite3HelperClass-1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      534 2024-05-18 18:30:28.375566 SQLLite3HelperClass-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2024-05-18 18:17:06.000000 SQLLite3HelperClass-1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 18:30:28.353619 SQLLite3HelperClass-1.0/SQLLite3HelperClass/
+-rw-rw-rw-   0        0        0     3587 2024-05-18 18:24:15.000000 SQLLite3HelperClass-1.0/SQLLite3HelperClass/SQLLite3HelperClass.py
+-rw-rw-rw-   0        0        0       66 2023-09-11 14:39:05.000000 SQLLite3HelperClass-1.0/SQLLite3HelperClass/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:30:28.371572 SQLLite3HelperClass-1.0/SQLLite3HelperClass.egg-info/
+-rw-rw-rw-   0        0        0      534 2024-05-18 18:30:28.000000 SQLLite3HelperClass-1.0/SQLLite3HelperClass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2024-05-18 18:30:28.000000 SQLLite3HelperClass-1.0/SQLLite3HelperClass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 18:30:28.000000 SQLLite3HelperClass-1.0/SQLLite3HelperClass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-18 18:30:28.000000 SQLLite3HelperClass-1.0/SQLLite3HelperClass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-18 18:30:28.379551 SQLLite3HelperClass-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      590 2024-05-18 18:15:34.000000 SQLLite3HelperClass-1.0/setup.py
```

### Comparing `SQLLite3HelperClass-0.5/LICENSE.txt` & `SQLLite3HelperClass-1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SQLLite3HelperClass-0.5/PKG-INFO` & `SQLLite3HelperClass-1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: SQLLite3HelperClass
-Version: 0.5
-Summary: Initializes an sqlite3 database and has a basic query method. This class is meant to be subclassed and expanded.
+Version: 1.0
+Summary: Initializes an sqlite3 database and provides some basic methods. This class is meant to be subclassed and expanded.
 Home-page: https://github.com/amcsparron2793-Water/SQLLite3HelperClass
 Author: Amcsparron
 Author-email: amcsparron@albanyny.gov
 License: MIT License
-Download-URL: https://github.com/amcsparron2793-Water/SQLLite3HelperClass/archive/refs/tags/0.5.tar.gz
+Download-URL: https://github.com/amcsparron2793-Water/SQLLite3HelperClass/archive/refs/tags/1.0.tar.gz
 Keywords: Sqlite3,database
 Platform: UNKNOWN
 License-File: LICENSE.txt
 
 UNKNOWN
```

### Comparing `SQLLite3HelperClass-0.5/SQLLite3HelperClass/SQLLite3HelperClass.py` & `SQLLite3HelperClass-1.0/SQLLite3HelperClass/SQLLite3HelperClass.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,37 @@
         else:
             self._logger = Logger("fake")
             # print("DUMMY LOGGER IN USE")
 
         self.db_file_path = db_file_path
         self._connection = None
         self._cursor = None
+        self._query_results = None
+
+    @property
+    def query_results(self):
+        return self._query_results
+
+    @query_results.setter
+    def query_results(self, value: List[dict] or None):
+        self._query_results = value
+
+    @property
+    def list_dict_results(self):
+        if self.query_results:
+            return self._ConvertToFinalListDict(self.query_results)
+        else:
+            return None
+
+    @property
+    def results_column_names(self) -> List[str] or None:
+        try:
+            return [d[0] for d in self._cursor.description]
+        except AttributeError as e:
+            return None
 
     def GetConnectionAndCursor(self):
         try:
             # print(f"Attempting  to connect to {self.db_file_path}")
             self._logger.info(f"Attempting  to connect to {self.db_file_path}")
             self._connection = sqlite3.connect(self.db_file_path)
 
@@ -37,58 +60,44 @@
         except sqlite3.IntegrityError as e:
             self._logger.error(e, exc_info=True)
             raise e
         except sqlite3.OperationalError as e:
             self._logger.error(e, exc_info=True)
             raise e
 
-    @property
-    def results_column_names(self) -> List[str] or None:
-        try:
-            return [d[0] for d in self._cursor.description]
-        except AttributeError as e:
-            return None
-
     def _ConvertToFinalListDict(self, results: List[tuple]) -> List[dict] or None:
         row_list_dict = []
         final_list_dict = []
 
         for row in results:
             if self.results_column_names:
                 for cell, col in zip(row, self.results_column_names):
                     row_list_dict.append({col: cell})
                 final_list_dict.append(dict(ChainMap(*row_list_dict)))
                 row_list_dict.clear()
             else:
                 raise AttributeError("A query has not been executed, "
                                      "please execute a query before calling this function.")
         if len(final_list_dict) > 0:
-            return final_list_dict
+            # this returns a sorted list dict instead of an unsorted list dict
+            return [dict(sorted(x.items())) for x in final_list_dict]
         else:
             return None
 
-    def Query(self, sql_string: str, **kwargs):
-        return_dict = False
-        if kwargs:
-            if 'return_dict' in kwargs:
-                return_dict = kwargs['return_dict']
+    def Query(self, sql_string: str):
         try:
             self._cursor.execute(sql_string)
 
             res = self._cursor.fetchall()
 
             if res:
                 self._logger.info(f"{len(res)} item(s) returned.")
             else:
                 self._logger.warning(f"query returned no results")
-
-            if return_dict:
-                return self._ConvertToFinalListDict(res)
-            else:
-                return res or None
+            self.query_results = res
 
         except sqlite3.IntegrityError as e:
             self._logger.error(e, exc_info=True)
             raise e
         except sqlite3.OperationalError as e:
             self._logger.error(e, exc_info=True)
             raise e
```

### Comparing `SQLLite3HelperClass-0.5/SQLLite3HelperClass.egg-info/PKG-INFO` & `SQLLite3HelperClass-1.0/SQLLite3HelperClass.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: SQLLite3HelperClass
-Version: 0.5
-Summary: Initializes an sqlite3 database and has a basic query method. This class is meant to be subclassed and expanded.
+Version: 1.0
+Summary: Initializes an sqlite3 database and provides some basic methods. This class is meant to be subclassed and expanded.
 Home-page: https://github.com/amcsparron2793-Water/SQLLite3HelperClass
 Author: Amcsparron
 Author-email: amcsparron@albanyny.gov
 License: MIT License
-Download-URL: https://github.com/amcsparron2793-Water/SQLLite3HelperClass/archive/refs/tags/0.5.tar.gz
+Download-URL: https://github.com/amcsparron2793-Water/SQLLite3HelperClass/archive/refs/tags/1.0.tar.gz
 Keywords: Sqlite3,database
 Platform: UNKNOWN
 License-File: LICENSE.txt
 
 UNKNOWN
```

### Comparing `SQLLite3HelperClass-0.5/setup.py` & `SQLLite3HelperClass-1.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name='SQLLite3HelperClass',
-    version='0.5',
+    version='1.0',
     packages=['SQLLite3HelperClass'],
     url='https://github.com/amcsparron2793-Water/SQLLite3HelperClass',
-    download_url='https://github.com/amcsparron2793-Water/SQLLite3HelperClass/archive/refs/tags/0.5.tar.gz',
+    download_url='https://github.com/amcsparron2793-Water/SQLLite3HelperClass/archive/refs/tags/1.0.tar.gz',
     keywords=["Sqlite3", "database"],
     license='MIT License',
     author='Amcsparron',
     author_email='amcsparron@albanyny.gov',
-    description='Initializes an sqlite3 database and has a basic query method. This class is meant to be subclassed and expanded.'
+    description='Initializes an sqlite3 database and provides some basic methods. This class is meant to be subclassed and expanded.'
 )
```

