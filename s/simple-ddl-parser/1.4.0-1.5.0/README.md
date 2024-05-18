# Comparing `tmp/simple_ddl_parser-1.4.0.tar.gz` & `tmp/simple_ddl_parser-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_ddl_parser-1.4.0.tar", max compression
+gzip compressed data, was "simple_ddl_parser-1.5.0.tar", max compression
```

## Comparing `simple_ddl_parser-1.4.0.tar` & `simple_ddl_parser-1.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1093 2024-04-21 13:06:45.341924 simple_ddl_parser-1.4.0/LICENSE
--rw-r--r--   0        0        0    35907 2024-05-14 20:23:38.463482 simple_ddl_parser-1.4.0/docs/README.rst
--rw-r--r--   0        0        0     1597 2024-05-14 20:20:00.664672 simple_ddl_parser-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      268 2024-04-21 13:06:45.342548 simple_ddl_parser-1.4.0/simple_ddl_parser/__init__.py
--rw-r--r--   0        0        0     2326 2024-04-21 13:06:45.342619 simple_ddl_parser-1.4.0/simple_ddl_parser/cli.py
--rwxr-xr-x   0        0        0     8860 2024-05-11 15:54:06.836621 simple_ddl_parser-1.4.0/simple_ddl_parser/ddl_parser.py
--rw-r--r--   0        0        0      755 2024-04-21 13:06:45.342889 simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/__init__.py
--rw-r--r--   0        0        0      702 2024-04-21 13:06:45.342962 simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/bigquery.py
--rw-r--r--   0        0        0     5326 2024-04-21 18:02:06.063289 simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/hql.py
--rw-r--r--   0        0        0      260 2024-04-21 13:06:45.343230 simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/ibm.py
--rw-r--r--   0        0        0     2608 2024-04-21 13:06:45.343300 simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/mssql.py
--rw-r--r--   0        0        0      510 2024-05-09 11:52:40.501830 simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/mysql.py
--rw-r--r--   0        0        0     2145 2024-05-09 12:49:40.928963 simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/oracle.py
--rw-r--r--   0        0        0      711 2024-05-11 16:32:31.477467 simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/psql.py
--rw-r--r--   0        0        0      928 2024-04-21 13:06:45.343627 simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/redshift.py
--rw-r--r--   0        0        0     7278 2024-04-21 18:13:32.614147 simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/snowflake.py
--rw-r--r--   0        0        0      305 2024-04-21 13:06:45.344047 simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/spark_sql.py
--rw-r--r--   0        0        0    59316 2024-05-14 20:20:46.487128 simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/sql.py
--rw-r--r--   0        0        0    13207 2024-04-21 13:06:45.344438 simple_ddl_parser-1.4.0/simple_ddl_parser/output/base_data.py
--rw-r--r--   0        0        0     5429 2024-05-14 20:20:45.599948 simple_ddl_parser-1.4.0/simple_ddl_parser/output/core.py
--rw-r--r--   0        0        0     9613 2024-05-14 20:20:45.653236 simple_ddl_parser-1.4.0/simple_ddl_parser/output/dialects.py
--rw-r--r--   0        0        0     2839 2024-05-14 20:19:40.189068 simple_ddl_parser-1.4.0/simple_ddl_parser/output/table_data.py
--rwxr-xr-x   0        0        0    13223 2024-05-09 11:53:06.889442 simple_ddl_parser-1.4.0/simple_ddl_parser/parser.py
--rw-r--r--   0        0        0   969353 2024-05-14 20:21:03.305087 simple_ddl_parser-1.4.0/simple_ddl_parser/parsetab.py
--rw-r--r--   0        0        0      713 2024-05-14 20:18:40.592170 simple_ddl_parser-1.4.0/simple_ddl_parser/test.py
--rw-r--r--   0        0        0     3148 2024-05-11 15:47:21.631201 simple_ddl_parser-1.4.0/simple_ddl_parser/tokens.py
--rw-r--r--   0        0        0     1391 2024-04-21 13:06:45.346777 simple_ddl_parser-1.4.0/simple_ddl_parser/utils.py
--rw-r--r--   0        0        0    37386 1970-01-01 00:00:00.000000 simple_ddl_parser-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-04-21 13:06:45.341924 simple_ddl_parser-1.5.0/LICENSE
+-rw-r--r--   0        0        0    36397 2024-05-18 21:22:31.497198 simple_ddl_parser-1.5.0/docs/README.rst
+-rw-r--r--   0        0        0     1597 2024-05-18 21:09:54.531131 simple_ddl_parser-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      268 2024-04-21 13:06:45.342548 simple_ddl_parser-1.5.0/simple_ddl_parser/__init__.py
+-rw-r--r--   0        0        0     2326 2024-04-21 13:06:45.342619 simple_ddl_parser-1.5.0/simple_ddl_parser/cli.py
+-rwxr-xr-x   0        0        0     8860 2024-05-11 15:54:06.836621 simple_ddl_parser-1.5.0/simple_ddl_parser/ddl_parser.py
+-rw-r--r--   0        0        0      755 2024-04-21 13:06:45.342889 simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/__init__.py
+-rw-r--r--   0        0        0      702 2024-04-21 13:06:45.342962 simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/bigquery.py
+-rw-r--r--   0        0        0     5326 2024-04-21 18:02:06.063289 simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/hql.py
+-rw-r--r--   0        0        0      260 2024-04-21 13:06:45.343230 simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/ibm.py
+-rw-r--r--   0        0        0     2608 2024-04-21 13:06:45.343300 simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/mssql.py
+-rw-r--r--   0        0        0      510 2024-05-09 11:52:40.501830 simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/mysql.py
+-rw-r--r--   0        0        0     2145 2024-05-09 12:49:40.928963 simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/oracle.py
+-rw-r--r--   0        0        0      711 2024-05-11 16:32:31.477467 simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/psql.py
+-rw-r--r--   0        0        0      928 2024-04-21 13:06:45.343627 simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/redshift.py
+-rw-r--r--   0        0        0     7278 2024-04-21 18:13:32.614147 simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/snowflake.py
+-rw-r--r--   0        0        0      305 2024-04-21 13:06:45.344047 simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/spark_sql.py
+-rw-r--r--   0        0        0    59429 2024-05-18 21:22:23.166369 simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/sql.py
+-rw-r--r--   0        0        0    13354 2024-05-18 21:22:22.560732 simple_ddl_parser-1.5.0/simple_ddl_parser/output/base_data.py
+-rw-r--r--   0        0        0     5429 2024-05-18 21:01:53.660711 simple_ddl_parser-1.5.0/simple_ddl_parser/output/core.py
+-rw-r--r--   0        0        0     9613 2024-05-18 21:01:53.661130 simple_ddl_parser-1.5.0/simple_ddl_parser/output/dialects.py
+-rw-r--r--   0        0        0     2839 2024-05-18 21:01:53.661488 simple_ddl_parser-1.5.0/simple_ddl_parser/output/table_data.py
+-rwxr-xr-x   0        0        0    13223 2024-05-09 11:53:06.889442 simple_ddl_parser-1.5.0/simple_ddl_parser/parser.py
+-rw-r--r--   0        0        0   969353 2024-05-18 21:01:53.663246 simple_ddl_parser-1.5.0/simple_ddl_parser/parsetab.py
+-rw-r--r--   0        0        0      367 2024-05-18 21:17:50.133061 simple_ddl_parser-1.5.0/simple_ddl_parser/test.py
+-rw-r--r--   0        0        0     3148 2024-05-11 15:47:21.631201 simple_ddl_parser-1.5.0/simple_ddl_parser/tokens.py
+-rw-r--r--   0        0        0     1391 2024-04-21 13:06:45.346777 simple_ddl_parser-1.5.0/simple_ddl_parser/utils.py
+-rw-r--r--   0        0        0    37876 1970-01-01 00:00:00.000000 simple_ddl_parser-1.5.0/PKG-INFO
```

### Comparing `simple_ddl_parser-1.4.0/LICENSE` & `simple_ddl_parser-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.4.0/docs/README.rst` & `simple_ddl_parser-1.5.0/docs/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,20 @@
 Is it Stable?
 ^^^^^^^^^^^^^
 
 Yes, library already has about 9000+ downloads per day  - https://pypistats.org/packages/simple-ddl-parser..
 
 As maintainer, I guarantee that any backward incompatible changes will not be done in patch or minor version. But! Pay attention that sometimes output in keywords can be changed in minor version because of fixing wrong behaviour in past.
 
+Articles with examples
+^^^^^^^^^^^^^^^^^^^^^^
+
+
+#. SQL Diagram (Part 3): SQL-to-ERD with DDL: https://levelup.gitconnected.com/sql-diagram-part-3-sql-to-erd-with-ddl-4c9840ee86c3 
+
 Updates in version 1.x
 ^^^^^^^^^^^^^^^^^^^^^^
 
 The full list of updates can be found in the Changelog below (at the end of README).
 
 Version 1.0.0 was released due to significant changes in the output structure and a stricter approach regarding the scope of the produced output. Now, you must provide the argument 'output_mode=name_of_your_dialect' if you wish to see arguments/properties specific to a particular dialect
 
@@ -545,14 +551,23 @@
 
 * https://github.com/ankitdata ,
 * https://github.com/kalyan939
 
 Changelog
 ---------
 
+**v1.5.0**
+
+Fixes
+^^^^^
+
+
+#. Now, ``unique`` set up to column only if it was only one column in unique constraint/index. Issue - https://github.com/xnuinside/simple-ddl-parser/issues/255
+#. Fixed issue when UNIQUE KEY was identified as primary key - https://github.com/xnuinside/simple-ddl-parser/issues/253
+
 **v1.4.0**
 
 Fixes
 ^^^^^
 
 BigQuery:
 ~~~~~~~~~
```

### Comparing `simple_ddl_parser-1.4.0/pyproject.toml` & `simple_ddl_parser-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simple-ddl-parser"
-version = "1.4.0"
+version = "1.5.0"
 description = "Simple DDL Parser to parse SQL & dialects like HQL, TSQL (MSSQL), Oracle, AWS Redshift, Snowflake, MySQL, PostgreSQL, etc ddl files to json/python dict with full information about columns: types, defaults, primary keys, etc.; sequences, alters, custom types & other entities from ddl."
 authors = ["Iuliia Volkova <xnuinside@gmail.com>"]
 license = "MIT"
 readme = "docs/README.rst"
 homepage = "https://github.com/xnuinside/simple-ddl-parser"
 repository = "https://github.com/xnuinside/simple-ddl-parser"
 classifiers = [
```

### Comparing `simple_ddl_parser-1.4.0/simple_ddl_parser/cli.py` & `simple_ddl_parser-1.5.0/simple_ddl_parser/cli.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.4.0/simple_ddl_parser/ddl_parser.py` & `simple_ddl_parser-1.5.0/simple_ddl_parser/ddl_parser.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/__init__.py` & `simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/bigquery.py` & `simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/bigquery.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/hql.py` & `simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/hql.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/mssql.py` & `simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/mssql.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/oracle.py` & `simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/oracle.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/psql.py` & `simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/psql.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/redshift.py` & `simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/redshift.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/snowflake.py` & `simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/snowflake.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.4.0/simple_ddl_parser/dialects/sql.py` & `simple_ddl_parser-1.5.0/simple_ddl_parser/dialects/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,17 +417,20 @@
         pk = False
         nullable = True
         default = None
         unique = False
         references = None
         if isinstance(p_list[-1], str):
             if p_list[-1].upper() == "KEY":
-                pk = True
-                nullable = False
-            elif p_list[-1].upper() == "UNIQUE":
+                if p_list[-2].upper() == "UNIQUE":
+                    unique = True
+                else:
+                    pk = True
+                    nullable = False
+            if p_list[-1].upper() == "UNIQUE":
                 unique = True
         elif isinstance(p_list[-1], dict) and "references" in p_list[-1]:
             p_list[-1]["references"]["column"] = p_list[-1]["references"]["columns"][0]
             del p_list[-1]["references"]["columns"]
             references = p_list[-1]["references"]
         return pk, default, unique, references, nullable
```

### Comparing `simple_ddl_parser-1.4.0/simple_ddl_parser/output/base_data.py` & `simple_ddl_parser-1.5.0/simple_ddl_parser/output/base_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
                 unique = getattr(self, key, {}).get("unique", [])
                 if unique:
                     check_in = unique["columns"]
                 else:
                     check_in = []
             else:
                 check_in = getattr(self, key, {})
-            if column["name"] in check_in:
+            if len(check_in) == 1 and column["name"] in check_in:
                 column["unique"] = True
 
     def normalize_ref_columns_in_final_output(self):
         for col_ref in self.ref_columns:
             name = col_ref["name"]
             for column in self.columns:
                 if name == column["name"]:
@@ -152,14 +152,15 @@
             for key_constraints in self.constraints["primary_keys"]:
                 pk.extend(key_constraints["columns"])
 
         self.primary_key = pk
 
     def add_unique_columns(self) -> None:
         for column in self.columns:
+
             if column["name"] in self.unique:
                 column["unique"] = True
 
     def iter_class_fields(self):
         for key, value in self.__dataclass_fields__.items():
             yield key, value
 
@@ -281,17 +282,20 @@
             if statement["default"]["columns"]:
                 for column_name in statement["default"]["columns"]:
                     if column["name"] == column_name:
                         column["default"] = statement["default"]["value"]
 
     def set_unique_columns_from_alter(self, statement: Dict) -> None:
         for column in self.columns:
-            for column_name in statement["unique"]["columns"]:
-                if column["name"] == column_name:
-                    column["unique"] = True
+
+            if len(statement["unique"]["columns"]) == 1:
+                # if unique index only on one column
+                for column_name in statement["unique"]["columns"]:
+                    if column["name"] == column_name:
+                        column["unique"] = True
 
     def alter_modify_columns(self, statement) -> None:
         alter_key = "columns_to_modify"
         table_alter_key = "modified_columns"
 
         if not self.alter.get(table_alter_key):
             self.alter[table_alter_key] = []
```

### Comparing `simple_ddl_parser-1.4.0/simple_ddl_parser/output/core.py` & `simple_ddl_parser-1.5.0/simple_ddl_parser/output/core.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.4.0/simple_ddl_parser/output/dialects.py` & `simple_ddl_parser-1.5.0/simple_ddl_parser/output/dialects.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.4.0/simple_ddl_parser/output/table_data.py` & `simple_ddl_parser-1.5.0/simple_ddl_parser/output/table_data.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.4.0/simple_ddl_parser/parser.py` & `simple_ddl_parser-1.5.0/simple_ddl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.4.0/simple_ddl_parser/parsetab.py` & `simple_ddl_parser-1.5.0/simple_ddl_parser/parsetab.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.4.0/simple_ddl_parser/tokens.py` & `simple_ddl_parser-1.5.0/simple_ddl_parser/tokens.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.4.0/simple_ddl_parser/utils.py` & `simple_ddl_parser-1.5.0/simple_ddl_parser/utils.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.4.0/PKG-INFO` & `simple_ddl_parser-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-ddl-parser
-Version: 1.4.0
+Version: 1.5.0
 Summary: Simple DDL Parser to parse SQL & dialects like HQL, TSQL (MSSQL), Oracle, AWS Redshift, Snowflake, MySQL, PostgreSQL, etc ddl files to json/python dict with full information about columns: types, defaults, primary keys, etc.; sequences, alters, custom types & other entities from ddl.
 Home-page: https://github.com/xnuinside/simple-ddl-parser
 License: MIT
 Author: Iuliia Volkova
 Author-email: xnuinside@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -54,14 +54,20 @@
 Is it Stable?
 ^^^^^^^^^^^^^
 
 Yes, library already has about 9000+ downloads per day  - https://pypistats.org/packages/simple-ddl-parser..
 
 As maintainer, I guarantee that any backward incompatible changes will not be done in patch or minor version. But! Pay attention that sometimes output in keywords can be changed in minor version because of fixing wrong behaviour in past.
 
+Articles with examples
+^^^^^^^^^^^^^^^^^^^^^^
+
+
+#. SQL Diagram (Part 3): SQL-to-ERD with DDL: https://levelup.gitconnected.com/sql-diagram-part-3-sql-to-erd-with-ddl-4c9840ee86c3 
+
 Updates in version 1.x
 ^^^^^^^^^^^^^^^^^^^^^^
 
 The full list of updates can be found in the Changelog below (at the end of README).
 
 Version 1.0.0 was released due to significant changes in the output structure and a stricter approach regarding the scope of the produced output. Now, you must provide the argument 'output_mode=name_of_your_dialect' if you wish to see arguments/properties specific to a particular dialect
 
@@ -574,14 +580,23 @@
 
 * https://github.com/ankitdata ,
 * https://github.com/kalyan939
 
 Changelog
 ---------
 
+**v1.5.0**
+
+Fixes
+^^^^^
+
+
+#. Now, ``unique`` set up to column only if it was only one column in unique constraint/index. Issue - https://github.com/xnuinside/simple-ddl-parser/issues/255
+#. Fixed issue when UNIQUE KEY was identified as primary key - https://github.com/xnuinside/simple-ddl-parser/issues/253
+
 **v1.4.0**
 
 Fixes
 ^^^^^
 
 BigQuery:
 ~~~~~~~~~
```

