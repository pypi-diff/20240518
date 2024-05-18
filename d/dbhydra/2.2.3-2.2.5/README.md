# Comparing `tmp/dbhydra-2.2.3.tar.gz` & `tmp/dbhydra-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbhydra-2.2.3.tar", last modified: Sat May 18 12:46:31 2024, max compression
+gzip compressed data, was "dbhydra-2.2.5.tar", last modified: Sat May 18 12:55:20 2024, max compression
```

## Comparing `dbhydra-2.2.3.tar` & `dbhydra-2.2.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 12:46:31.956917 dbhydra-2.2.3/
--rw-rw-rw-   0        0        0     1091 2024-02-21 13:14:05.000000 dbhydra-2.2.3/LICENSE
--rw-rw-rw-   0        0        0     2141 2024-05-18 12:46:31.955925 dbhydra-2.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1701 2024-02-21 13:14:05.000000 dbhydra-2.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 12:46:31.870364 dbhydra-2.2.3/dbhydra/
--rw-rw-rw-   0        0        0       65 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/__init__.py
--rw-rw-rw-   0        0        0     2470 2024-04-08 00:11:52.000000 dbhydra-2.2.3/dbhydra/dbhydra_core.py
-drwxrwxrwx   0        0        0        0 2024-05-18 12:46:31.936158 dbhydra-2.2.3/dbhydra/src/
--rw-rw-rw-   0        0        0        0 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/src/__init__.py
--rw-rw-rw-   0        0        0     5901 2024-03-21 11:46:21.000000 dbhydra-2.2.3/dbhydra/src/abstract_db.py
--rw-rw-rw-   0        0        0    17278 2024-05-18 12:45:16.000000 dbhydra-2.2.3/dbhydra/src/abstract_table.py
--rw-rw-rw-   0        0        0     1834 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/src/bigquery_db.py
-drwxrwxrwx   0        0        0        0 2024-05-18 12:46:31.943298 dbhydra-2.2.3/dbhydra/src/errors/
--rw-rw-rw-   0        0        0        0 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/src/errors/__init__.py
--rw-rw-rw-   0        0        0      149 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/src/errors/exceptions.py
--rw-rw-rw-   0        0        0    18931 2024-03-22 12:51:05.000000 dbhydra-2.2.3/dbhydra/src/migrator.py
--rw-rw-rw-   0        0        0     1922 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/src/mongo_db.py
--rw-rw-rw-   0        0        0     3152 2024-04-08 00:11:52.000000 dbhydra-2.2.3/dbhydra/src/mysql_db.py
--rw-rw-rw-   0        0        0     1805 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/src/postgres_db.py
--rw-rw-rw-   0        0        0     3611 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/src/sqlserver_db.py
--rw-rw-rw-   0        0        0    46656 2024-04-08 00:11:52.000000 dbhydra-2.2.3/dbhydra/src/tables.py
--rw-rw-rw-   0        0        0     3514 2024-03-11 14:47:17.000000 dbhydra-2.2.3/dbhydra/src/xlsx_db.py
--rw-rw-rw-   0        0        0      803 2024-03-21 15:23:01.000000 dbhydra-2.2.3/dbhydra/test_migrator.py
-drwxrwxrwx   0        0        0        0 2024-05-18 12:46:31.955925 dbhydra-2.2.3/dbhydra/tests/
--rw-rw-rw-   0        0        0        0 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/tests/__init__.py
--rw-rw-rw-   0        0        0      508 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/tests/test_cases.py
--rw-rw-rw-   0        0        0     1979 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/tests/test_mongo.py
--rw-rw-rw-   0        0        0     3126 2024-02-21 13:14:05.000000 dbhydra-2.2.3/dbhydra/tests/test_sql.py
-drwxrwxrwx   0        0        0        0 2024-05-18 12:46:31.884061 dbhydra-2.2.3/dbhydra.egg-info/
--rw-rw-rw-   0        0        0     2141 2024-05-18 12:46:31.000000 dbhydra-2.2.3/dbhydra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      701 2024-05-18 12:46:31.000000 dbhydra-2.2.3/dbhydra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 12:46:31.000000 dbhydra-2.2.3/dbhydra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-05-18 12:46:31.000000 dbhydra-2.2.3/dbhydra.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-18 12:46:31.000000 dbhydra-2.2.3/dbhydra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 12:46:31.956917 dbhydra-2.2.3/setup.cfg
--rw-rw-rw-   0        0        0      793 2024-05-18 12:46:13.000000 dbhydra-2.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:55:20.846347 dbhydra-2.2.5/
+-rw-rw-rw-   0        0        0     1091 2024-02-21 13:14:05.000000 dbhydra-2.2.5/LICENSE
+-rw-rw-rw-   0        0        0     2141 2024-05-18 12:55:20.846347 dbhydra-2.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1701 2024-02-21 13:14:05.000000 dbhydra-2.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 12:55:20.811780 dbhydra-2.2.5/dbhydra/
+-rw-rw-rw-   0        0        0       65 2024-02-21 13:14:05.000000 dbhydra-2.2.5/dbhydra/__init__.py
+-rw-rw-rw-   0        0        0     2470 2024-04-08 00:11:52.000000 dbhydra-2.2.5/dbhydra/dbhydra_core.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:55:20.842347 dbhydra-2.2.5/dbhydra/src/
+-rw-rw-rw-   0        0        0        0 2024-02-21 13:14:05.000000 dbhydra-2.2.5/dbhydra/src/__init__.py
+-rw-rw-rw-   0        0        0     5901 2024-03-21 11:46:21.000000 dbhydra-2.2.5/dbhydra/src/abstract_db.py
+-rw-rw-rw-   0        0        0    17420 2024-05-18 12:49:56.000000 dbhydra-2.2.5/dbhydra/src/abstract_table.py
+-rw-rw-rw-   0        0        0     1834 2024-02-21 13:14:05.000000 dbhydra-2.2.5/dbhydra/src/bigquery_db.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:55:20.843349 dbhydra-2.2.5/dbhydra/src/errors/
+-rw-rw-rw-   0        0        0        0 2024-02-21 13:14:05.000000 dbhydra-2.2.5/dbhydra/src/errors/__init__.py
+-rw-rw-rw-   0        0        0      149 2024-02-21 13:14:05.000000 dbhydra-2.2.5/dbhydra/src/errors/exceptions.py
+-rw-rw-rw-   0        0        0    18931 2024-03-22 12:51:05.000000 dbhydra-2.2.5/dbhydra/src/migrator.py
+-rw-rw-rw-   0        0        0     1922 2024-02-21 13:14:05.000000 dbhydra-2.2.5/dbhydra/src/mongo_db.py
+-rw-rw-rw-   0        0        0     3152 2024-04-08 00:11:52.000000 dbhydra-2.2.5/dbhydra/src/mysql_db.py
+-rw-rw-rw-   0        0        0     1805 2024-02-21 13:14:05.000000 dbhydra-2.2.5/dbhydra/src/postgres_db.py
+-rw-rw-rw-   0        0        0     3611 2024-02-21 13:14:05.000000 dbhydra-2.2.5/dbhydra/src/sqlserver_db.py
+-rw-rw-rw-   0        0        0    46844 2024-05-18 12:54:16.000000 dbhydra-2.2.5/dbhydra/src/tables.py
+-rw-rw-rw-   0        0        0     3514 2024-03-11 14:47:17.000000 dbhydra-2.2.5/dbhydra/src/xlsx_db.py
+-rw-rw-rw-   0        0        0      803 2024-03-21 15:23:01.000000 dbhydra-2.2.5/dbhydra/test_migrator.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:55:20.845353 dbhydra-2.2.5/dbhydra/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-21 13:14:05.000000 dbhydra-2.2.5/dbhydra/tests/__init__.py
+-rw-rw-rw-   0        0        0      508 2024-02-21 13:14:05.000000 dbhydra-2.2.5/dbhydra/tests/test_cases.py
+-rw-rw-rw-   0        0        0     1979 2024-02-21 13:14:05.000000 dbhydra-2.2.5/dbhydra/tests/test_mongo.py
+-rw-rw-rw-   0        0        0     3126 2024-02-21 13:14:05.000000 dbhydra-2.2.5/dbhydra/tests/test_sql.py
+drwxrwxrwx   0        0        0        0 2024-05-18 12:55:20.836830 dbhydra-2.2.5/dbhydra.egg-info/
+-rw-rw-rw-   0        0        0     2141 2024-05-18 12:55:20.000000 dbhydra-2.2.5/dbhydra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      701 2024-05-18 12:55:20.000000 dbhydra-2.2.5/dbhydra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 12:55:20.000000 dbhydra-2.2.5/dbhydra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-18 12:55:20.000000 dbhydra-2.2.5/dbhydra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-18 12:55:20.000000 dbhydra-2.2.5/dbhydra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 12:55:20.846347 dbhydra-2.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      793 2024-05-18 12:54:51.000000 dbhydra-2.2.5/setup.py
```

### Comparing `dbhydra-2.2.3/LICENSE` & `dbhydra-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.3/PKG-INFO` & `dbhydra-2.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 2.2.3
+Version: 2.2.5
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dbhydra-2.2.3/README.md` & `dbhydra-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.3/dbhydra/dbhydra_core.py` & `dbhydra-2.2.5/dbhydra/dbhydra_core.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.3/dbhydra/src/abstract_db.py` & `dbhydra-2.2.5/dbhydra/src/abstract_db.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.3/dbhydra/src/abstract_table.py` & `dbhydra-2.2.5/dbhydra/src/abstract_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -254,29 +254,31 @@
         column_converted_type_dict = db1._convert_column_type_dict_from_python(column_type_dict)
         columns = list(column_converted_type_dict.keys())
         types = list(column_converted_type_dict.values())
 
         return cls(db1, name, columns, types, id_column_name=id_column_name)
     
     
-    def drop(self):
+    def drop(self, debug_mode = False):
         query = "DROP TABLE " + self.name
-        print(query)
+        if debug_mode:
+            print(query)
         self.execute(query)
 
-    def update(self, variable_assign, where=None):
+    def update(self, variable_assign, where=None, debug_mode = False):
         if where is None:
             query = "UPDATE " + self.name + " SET " + variable_assign
         else:
             query = "UPDATE " + self.name + " SET " + variable_assign + " WHERE " + where
-        print(query)
+        if debug_mode:
+            print(query)
         return self.execute(query)
 
     def update_from_df(
-            self, update_df: pd.DataFrame, where_column: Optional[str] = None, where_value: Any = None) -> None:
+            self, update_df: pd.DataFrame, where_column: Optional[str] = None, where_value: Any = None, debug_mode = False) -> None:
         """Build UPDATE SQL query from a dataframe and execute it.
 
         :param update_df: Dataframe with updated values - MUST only hold a single row
         :type update_df: pd.DataFrame
         :param where_column: Column name to use for WHERE clause.
         :type where_column: str
         :param where_value: Value to use for WHERE clause.
@@ -318,16 +320,16 @@
         quote = self.db1.identifier_quote
         sql_query = f"UPDATE {quote}{self.name}{quote} SET {column_value_string}"
 
         if where_column is not None and where_value is not None:
             sql_query += f" WHERE {where_column} = {where_value};"
         else:
             sql_query += ";"
-
-        print(sql_query)
+        if debug_mode:
+            print(sql_query)
         self.execute(sql_query)
 
     def _adjust_df(self, df: pd.DataFrame, debug_mode=False) -> pd.DataFrame:
         """
         Adjust DataFrame in case number of its columns differs from number of columns in DB table.
         :param df: original DF
         :param debug_mode: in debug mode a warning will be printed to console
```

### Comparing `dbhydra-2.2.3/dbhydra/src/bigquery_db.py` & `dbhydra-2.2.5/dbhydra/src/bigquery_db.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.3/dbhydra/src/migrator.py` & `dbhydra-2.2.5/dbhydra/src/migrator.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.3/dbhydra/src/mongo_db.py` & `dbhydra-2.2.5/dbhydra/src/mongo_db.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.3/dbhydra/src/mysql_db.py` & `dbhydra-2.2.5/dbhydra/src/mysql_db.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.3/dbhydra/src/postgres_db.py` & `dbhydra-2.2.5/dbhydra/src/postgres_db.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.3/dbhydra/src/sqlserver_db.py` & `dbhydra-2.2.5/dbhydra/src/sqlserver_db.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.3/dbhydra/src/tables.py` & `dbhydra-2.2.5/dbhydra/src/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,25 +137,26 @@
             columns.insert(0, temporary_table.id_column_name)
             types.pop(id_col_index)
             types.insert(0, "int")
 
         return (cls(db1, name, columns, types))
 
     # @save_migration
-    def create(self, foreign_keys=None):
+    def create(self, foreign_keys=None, debug_mode = False):
         assert len(self.columns) == len(self.types)
         assert self.columns[0] == self.id_column_name
         assert self.types[0].lower() == "int" or self.types[0].lower() == "integer"
         query = "CREATE TABLE " + self.name + "("+self.id_column_name+" SERIAL PRIMARY KEY,"
         for i in range(1, len(self.columns)):
             query += self.columns[i] + " " + self.types[i] + ","
 
         query = query[:-1]
         query += ");"
-        print(query)
+        if debug_mode:
+            print(query)
         try:
             self.db1.execute(query)
         except Exception as e:
             print("Table " + self.name + " already exists:", e)
             print("Check the specification of table columns and their types")
 
     def insert(self, rows, batch=1, replace_apostrophes=True, try_mode=False, debug_mode=False, insert_id=False):
@@ -491,24 +492,24 @@
 
     def get_all_types(self):
         information_schema_table = SqlServerTable(self.db1, 'INFORMATION_SCHEMA.COLUMNS', ['DATA_TYPE'], ['nvarchar(50)'])
         query = "SELECT DATA_TYPE FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_NAME  = '" + self.name + "'"
         types = information_schema_table.select(query)
         return (types)
 
-    def create(self):
+    def create(self, debug_mode = False):
         assert len(self.columns) == len(self.types)
         assert self.columns[0] == self.id_column_name
         assert self.types[0].lower() == "int"
         query = "CREATE TABLE " + self.name + "("+self.id_column_name+" INT IDENTITY(1,1) NOT NULL,"
         for i in range(1, len(self.columns)):
             query += self.columns[i] + " " + self.types[i] + ","
         query += "PRIMARY KEY("+self.id_column_name+"))"
-
-        print(query)
+        if debug_mode:
+            print(query)
         try:
             self.db1.execute(query)
         except Exception as e:
             print("Table " + self.name + " already exists:", e)
             print("Check the specification of table columns and their types")
 
     def insert(self, rows, batch=1, replace_apostrophes=True, try_mode=False, debug_mode=False):
@@ -725,32 +726,33 @@
         Returns the number of records in table
         """
 
         num_of_records = self.select(f"SELECT COUNT(*) FROM `{self.name}`;")
 
         return num_of_records[0][0]
 
-    def drop(self):
+    def drop(self, debug_mode = False):
         query = "DROP TABLE `" + self.name + "`;"
-        print(query)
+        if debug_mode:
+            print(query)
         self.db1.execute(query)
 
     # @save_migration #TODO: Uncomment
-    def create(self, foreign_keys=None):
+    def create(self, foreign_keys=None, debug_mode = False):
         assert len(self.columns) == len(self.types)
         assert self.columns[0] == self.id_column_name
         assert self.types[0].lower() == "int"
 
         column_type_pairs = list(zip(self.columns, self.types))[1:]
         fields = ", ".join(
             [f"`{column}` {type_.upper()}" for column, type_ in column_type_pairs]
         )
         query = f"CREATE TABLE `{self.name}` ({self.id_column_name} INT UNSIGNED AUTO_INCREMENT PRIMARY KEY, {fields})"
-
-        print(query)
+        if debug_mode:
+            print(query)
         try:
             self.db1.execute(query)
         except Exception as e:
             print("Table " + self.name + " already exists:", e)
             print("Check the specification of table columns and their types")
 
     def insert(self, rows, batch=1, replace_apostrophes=True, try_mode=False, debug_mode=False, insert_id=False):
```

### Comparing `dbhydra-2.2.3/dbhydra/src/xlsx_db.py` & `dbhydra-2.2.5/dbhydra/src/xlsx_db.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.3/dbhydra/test_migrator.py` & `dbhydra-2.2.5/dbhydra/test_migrator.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.3/dbhydra/tests/test_mongo.py` & `dbhydra-2.2.5/dbhydra/tests/test_mongo.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.3/dbhydra/tests/test_sql.py` & `dbhydra-2.2.5/dbhydra/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `dbhydra-2.2.3/dbhydra.egg-info/PKG-INFO` & `dbhydra-2.2.5/dbhydra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbhydra
-Version: 2.2.3
+Version: 2.2.5
 Summary: Data science friendly ORM combining Python
 Home-page: https://github.com/DovaX/dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dbhydra-2.2.3/dbhydra.egg-info/SOURCES.txt` & `dbhydra-2.2.5/dbhydra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

