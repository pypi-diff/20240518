# Comparing `tmp/dbhydra-2.2.1.tar.gz` & `tmp/dbhydra-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbhydra-2.2.1.tar", last modified: Mon Apr  8 00:22:43 2024, max compression
+gzip compressed data, was "dbhydra-2.2.3.tar", last modified: Sat May 18 12:46:31 2024, max compression
```

## Comparing `dbhydra-2.2.1.tar` & `dbhydra-2.2.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 00:22:43.020197 dbhydra-2.2.1/
--rw-rw-rw-   0        0        0     1091 2024-02-21 13:14:05.000000 dbhydra-2.2.1/LICENSE
--rw-rw-rw-   0        0        0     2141 2024-04-08 00:22:43.019206 dbhydra-2.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1701 2024-02-21 13:14:05.000000 dbhydra-2.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 00:22:42.885111 dbhydra-2.2.1/dbhydra/
--rw-rw-rw-   0        0        0       65 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/__init__.py
--rw-rw-rw-   0        0        0     2470 2024-04-08 00:11:52.000000 dbhydra-2.2.1/dbhydra/dbhydra_core.py
-drwxrwxrwx   0        0        0        0 2024-04-08 00:22:42.997865 dbhydra-2.2.1/dbhydra/src/
--rw-rw-rw-   0        0        0        0 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/src/__init__.py
--rw-rw-rw-   0        0        0     5901 2024-03-21 11:46:21.000000 dbhydra-2.2.1/dbhydra/src/abstract_db.py
--rw-rw-rw-   0        0        0    17081 2024-03-21 11:46:21.000000 dbhydra-2.2.1/dbhydra/src/abstract_table.py
--rw-rw-rw-   0        0        0     1834 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/src/bigquery_db.py
-drwxrwxrwx   0        0        0        0 2024-04-08 00:22:43.005084 dbhydra-2.2.1/dbhydra/src/errors/
--rw-rw-rw-   0        0        0        0 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/src/errors/__init__.py
--rw-rw-rw-   0        0        0      149 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/src/errors/exceptions.py
--rw-rw-rw-   0        0        0    18931 2024-03-22 12:51:05.000000 dbhydra-2.2.1/dbhydra/src/migrator.py
--rw-rw-rw-   0        0        0     1922 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/src/mongo_db.py
--rw-rw-rw-   0        0        0     3152 2024-04-08 00:11:52.000000 dbhydra-2.2.1/dbhydra/src/mysql_db.py
--rw-rw-rw-   0        0        0     1805 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/src/postgres_db.py
--rw-rw-rw-   0        0        0     3611 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/src/sqlserver_db.py
--rw-rw-rw-   0        0        0    46656 2024-04-08 00:11:52.000000 dbhydra-2.2.1/dbhydra/src/tables.py
--rw-rw-rw-   0        0        0     3514 2024-03-11 14:47:17.000000 dbhydra-2.2.1/dbhydra/src/xlsx_db.py
--rw-rw-rw-   0        0        0      803 2024-03-21 15:23:01.000000 dbhydra-2.2.1/dbhydra/test_migrator.py
-drwxrwxrwx   0        0        0        0 2024-04-08 00:22:43.018198 dbhydra-2.2.1/dbhydra/tests/
--rw-rw-rw-   0        0        0        0 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/tests/__init__.py
--rw-rw-rw-   0        0        0      508 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/tests/test_cases.py
--rw-rw-rw-   0        0        0     1979 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/tests/test_mongo.py
--rw-rw-rw-   0        0        0     3126 2024-02-21 13:14:05.000000 dbhydra-2.2.1/dbhydra/tests/test_sql.py
-drwxrwxrwx   0        0        0        0 2024-04-08 00:22:42.923657 dbhydra-2.2.1/dbhydra.egg-info/
--rw-rw-rw-   0        0        0     2141 2024-04-08 00:22:42.000000 dbhydra-2.2.1/dbhydra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      701 2024-04-08 00:22:42.000000 dbhydra-2.2.1/dbhydra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 00:22:42.000000 dbhydra-2.2.1/dbhydra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-04-08 00:22:42.000000 dbhydra-2.2.1/dbhydra.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-08 00:22:42.000000 dbhydra-2.2.1/dbhydra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 00:22:43.020197 dbhydra-2.2.1/setup.cfg
--rw-rw-rw-   0        0        0      793 2024-04-08 00:22:35.000000 dbhydra-2.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:46:31.956917 dbhydra-2.2.3/
+-rw-rw-rw-   0        0        0     1091 2024-02-21 13:14:05.000000 dbhydra-2.2.3/LICENSE
+-rw-rw-rw-   0        0        0     2141 2024-05-18 12:46:31.955925 dbhydra-2.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1701 2024-02-21 13:14:05.000000 dbhydra-2.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 12:46:31.870364 dbhydra-2.2.3/dbhydra/
+-rw-rw-rw-   0        0        0       65 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/__init__.py
+-rw-rw-rw-   0        0        0     2470 2024-04-08 00:11:52.000000 dbhydra-2.2.3/dbhydra/dbhydra_core.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:46:31.936158 dbhydra-2.2.3/dbhydra/src/
+-rw-rw-rw-   0        0        0        0 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/src/__init__.py
+-rw-rw-rw-   0        0        0     5901 2024-03-21 11:46:21.000000 dbhydra-2.2.3/dbhydra/src/abstract_db.py
+-rw-rw-rw-   0        0        0    17278 2024-05-18 12:45:16.000000 dbhydra-2.2.3/dbhydra/src/abstract_table.py
+-rw-rw-rw-   0        0        0     1834 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/src/bigquery_db.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:46:31.943298 dbhydra-2.2.3/dbhydra/src/errors/
+-rw-rw-rw-   0        0        0        0 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/src/errors/__init__.py
+-rw-rw-rw-   0        0        0      149 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/src/errors/exceptions.py
+-rw-rw-rw-   0        0        0    18931 2024-03-22 12:51:05.000000 dbhydra-2.2.3/dbhydra/src/migrator.py
+-rw-rw-rw-   0        0        0     1922 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/src/mongo_db.py
+-rw-rw-rw-   0        0        0     3152 2024-04-08 00:11:52.000000 dbhydra-2.2.3/dbhydra/src/mysql_db.py
+-rw-rw-rw-   0        0        0     1805 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/src/postgres_db.py
+-rw-rw-rw-   0        0        0     3611 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/src/sqlserver_db.py
+-rw-rw-rw-   0        0        0    46656 2024-04-08 00:11:52.000000 dbhydra-2.2.3/dbhydra/src/tables.py
+-rw-rw-rw-   0        0        0     3514 2024-03-11 14:47:17.000000 dbhydra-2.2.3/dbhydra/src/xlsx_db.py
+-rw-rw-rw-   0        0        0      803 2024-03-21 15:23:01.000000 dbhydra-2.2.3/dbhydra/test_migrator.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:46:31.955925 dbhydra-2.2.3/dbhydra/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/tests/__init__.py
+-rw-rw-rw-   0        0        0      508 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/tests/test_cases.py
+-rw-rw-rw-   0        0        0     1979 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/tests/test_mongo.py
+-rw-rw-rw-   0        0        0     3126 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/tests/test_sql.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:46:31.884061 dbhydra-2.2.3/dbhydra.egg-info/
+-rw-rw-rw-   0        0        0     2141 2024-05-18 12:46:31.000000 dbhydra-2.2.3/dbhydra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      701 2024-05-18 12:46:31.000000 dbhydra-2.2.3/dbhydra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 12:46:31.000000 dbhydra-2.2.3/dbhydra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-18 12:46:31.000000 dbhydra-2.2.3/dbhydra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-18 12:46:31.000000 dbhydra-2.2.3/dbhydra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 12:46:31.956917 dbhydra-2.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      793 2024-05-18 12:46:13.000000 dbhydra-2.2.3/setup.py
```

### Comparing `dbhydra-2.2.1/LICENSE` & `dbhydra-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.1/PKG-INFO` & `dbhydra-2.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 2.2.1
+Version: 2.2.3
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dbhydra-2.2.1/README.md` & `dbhydra-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.1/dbhydra/dbhydra_core.py` & `dbhydra-2.2.3/dbhydra/dbhydra_core.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.1/dbhydra/src/abstract_db.py` & `dbhydra-2.2.3/dbhydra/src/abstract_db.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.1/dbhydra/src/abstract_table.py` & `dbhydra-2.2.3/dbhydra/src/abstract_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,26 +98,27 @@
         
         
         results=cast_rows_to_list_of_lists(rows, columns_count)
         
         return (results)
 
 
-    def select(self, query, flattening_of_results=False):
+    def select(self, query, flattening_of_results=False, debug_mode = False):
         """given SELECT query returns Python list"""
         """Columns give the number of selected columns"""
         
 
         if self.query_building_enabled:
             columns=self._get_selected_columns(query)
             self._query_blocks.append(Select(columns, self))
             return(self) #to enable chaining
         
         else:
-            print(query)
+            if debug_mode:
+                print(query)
             self.db1.cursor.execute(query)
             
             columns_count=len(self._get_selected_columns(query))
             rows=self._fetch_results(columns_count)
                 
             def flatten_results(rows, columns_count):
                 """Returns flat list for one column and list of lists for multiple columns"""   
@@ -127,26 +128,26 @@
             
             if flattening_of_results:
                 rows=flatten_results(rows, columns_count)
                 
             return(rows)
             
 
-    def select_all(self):
+    def select_all(self, debug_mode = False):
         quote = self.db1.identifier_quote
         all_cols_query = ""
         for col in self.columns:
             all_cols_query = all_cols_query + quote + col + quote + ","
         if all_cols_query[-1] == ",":
             all_cols_query = all_cols_query[:-1]
-        list1 = self.select(f"SELECT {all_cols_query} FROM {quote}{self.name}{quote};")
+        list1 = self.select(f"SELECT {all_cols_query} FROM {quote}{self.name}{quote};", debug_mode = debug_mode)
         return (list1)
 
-    def select_to_df(self):
-        rows = self.select_all()
+    def select_to_df(self, debug_mode = False):
+        rows = self.select_all(debug_mode = debug_mode)
         if self.query_building_enabled:
             self.to_df()
             df=None
         else:
             table_columns = self.columns
             df = pd.DataFrame(rows, columns=table_columns)
         return (df)
@@ -310,15 +311,16 @@
                 column_value_string += f"{column_name} = '{cell_value}', "
             elif column_type in ["json", "text", "mediumtext", "longtext", "datetime"]:
                 column_value_string += f"{column_name} = '{cell_value}', "
             else:
                 raise AttributeError(f"Unknown column type '{column_type}'")
 
         column_value_string = column_value_string.rstrip(", ")
-        sql_query = f"UPDATE {self.name} SET {column_value_string}"
+        quote = self.db1.identifier_quote
+        sql_query = f"UPDATE {quote}{self.name}{quote} SET {column_value_string}"
 
         if where_column is not None and where_value is not None:
             sql_query += f" WHERE {where_column} = {where_value};"
         else:
             sql_query += ";"
 
         print(sql_query)
```

### Comparing `dbhydra-2.2.1/dbhydra/src/bigquery_db.py` & `dbhydra-2.2.3/dbhydra/src/bigquery_db.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.1/dbhydra/src/migrator.py` & `dbhydra-2.2.3/dbhydra/src/migrator.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.1/dbhydra/src/mongo_db.py` & `dbhydra-2.2.3/dbhydra/src/mongo_db.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.1/dbhydra/src/mysql_db.py` & `dbhydra-2.2.3/dbhydra/src/mysql_db.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.1/dbhydra/src/postgres_db.py` & `dbhydra-2.2.3/dbhydra/src/postgres_db.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.1/dbhydra/src/sqlserver_db.py` & `dbhydra-2.2.3/dbhydra/src/sqlserver_db.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.1/dbhydra/src/tables.py` & `dbhydra-2.2.3/dbhydra/src/tables.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.1/dbhydra/src/xlsx_db.py` & `dbhydra-2.2.3/dbhydra/src/xlsx_db.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.1/dbhydra/test_migrator.py` & `dbhydra-2.2.3/dbhydra/test_migrator.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.1/dbhydra/tests/test_mongo.py` & `dbhydra-2.2.3/dbhydra/tests/test_mongo.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.1/dbhydra/tests/test_sql.py` & `dbhydra-2.2.3/dbhydra/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.1/dbhydra.egg-info/PKG-INFO` & `dbhydra-2.2.3/dbhydra.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 2.2.1
+Version: 2.2.3
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dbhydra-2.2.1/dbhydra.egg-info/SOURCES.txt` & `dbhydra-2.2.3/dbhydra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.1/setup.py` & `dbhydra-2.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='dbhydra',
-    version='2.2.1',
+    version='2.2.3',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Data science friendly ORM combining Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/dbhydra',
     packages=setuptools.find_packages(),
```

