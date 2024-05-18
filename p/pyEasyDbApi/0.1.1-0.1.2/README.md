# Comparing `tmp/pyeasydbapi-0.1.1.tar.gz` & `tmp/pyeasydbapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeasydbapi-0.1.1.tar", last modified: Sat May 18 19:30:57 2024, max compression
+gzip compressed data, was "pyeasydbapi-0.1.2.tar", last modified: Sat May 18 19:33:05 2024, max compression
```

## Comparing `pyeasydbapi-0.1.1.tar` & `pyeasydbapi-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:30:57.201804 pyeasydbapi-0.1.1/
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       12 2024-05-16 20:46:59.000000 pyeasydbapi-0.1.1/LICENSE
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      521 2024-05-18 19:30:57.201804 pyeasydbapi-0.1.1/PKG-INFO
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       93 2024-05-18 19:08:50.000000 pyeasydbapi-0.1.1/README.md
-drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:30:57.200804 pyeasydbapi-0.1.1/SimpleDB/
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       33 2024-05-18 19:12:23.000000 pyeasydbapi-0.1.1/SimpleDB/__init__.py
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)     4687 2024-05-18 19:30:50.000000 pyeasydbapi-0.1.1/SimpleDB/main.py
-drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:30:57.200804 pyeasydbapi-0.1.1/pyEasyDbApi.egg-info/
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      521 2024-05-18 19:30:57.000000 pyeasydbapi-0.1.1/pyEasyDbApi.egg-info/PKG-INFO
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      214 2024-05-18 19:30:57.000000 pyeasydbapi-0.1.1/pyEasyDbApi.egg-info/SOURCES.txt
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        1 2024-05-18 19:30:57.000000 pyeasydbapi-0.1.1/pyEasyDbApi.egg-info/dependency_links.txt
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        9 2024-05-18 19:30:57.000000 pyeasydbapi-0.1.1/pyEasyDbApi.egg-info/top_level.txt
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       38 2024-05-18 19:30:57.201804 pyeasydbapi-0.1.1/setup.cfg
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      704 2024-05-18 19:30:50.000000 pyeasydbapi-0.1.1/setup.py
+drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:33:05.349144 pyeasydbapi-0.1.2/
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       12 2024-05-16 20:46:59.000000 pyeasydbapi-0.1.2/LICENSE
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      521 2024-05-18 19:33:05.349144 pyeasydbapi-0.1.2/PKG-INFO
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       93 2024-05-18 19:08:50.000000 pyeasydbapi-0.1.2/README.md
+drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:33:05.349144 pyeasydbapi-0.1.2/SimpleDB/
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       33 2024-05-18 19:12:23.000000 pyeasydbapi-0.1.2/SimpleDB/__init__.py
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)     4755 2024-05-18 19:32:58.000000 pyeasydbapi-0.1.2/SimpleDB/main.py
+drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:33:05.349144 pyeasydbapi-0.1.2/pyEasyDbApi.egg-info/
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      521 2024-05-18 19:33:05.000000 pyeasydbapi-0.1.2/pyEasyDbApi.egg-info/PKG-INFO
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      214 2024-05-18 19:33:05.000000 pyeasydbapi-0.1.2/pyEasyDbApi.egg-info/SOURCES.txt
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        1 2024-05-18 19:33:05.000000 pyeasydbapi-0.1.2/pyEasyDbApi.egg-info/dependency_links.txt
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        9 2024-05-18 19:33:05.000000 pyeasydbapi-0.1.2/pyEasyDbApi.egg-info/top_level.txt
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       38 2024-05-18 19:33:05.350144 pyeasydbapi-0.1.2/setup.cfg
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      704 2024-05-18 19:32:58.000000 pyeasydbapi-0.1.2/setup.py
```

### Comparing `pyeasydbapi-0.1.1/PKG-INFO` & `pyeasydbapi-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEasyDbApi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple DataBase to use
 Home-page: https://t.me/n1grtr33x
 Author: n1grtr33x
 Author-email: dmitroluc7@gmail.com
 Keywords: easy-db
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyeasydbapi-0.1.1/SimpleDB/main.py` & `pyeasydbapi-0.1.2/SimpleDB/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -140,17 +140,17 @@
             sql = f"INSERT INTO _users (id, name, {args}) VALUES ({id}, {name}, {args})"
 
         sql_1 = (f"CREATE TABLE IF NOT EXISTS '_users' (user_id TEXT UNIQUE NOT NULL,"
                  f" name TEXT NOT NULL, TEXT NOT NULL, {args})")
 
         self._cursor.execute(sql_1)
         self._conn.commit()
+        try:
+            sql = f"SELECT * FROM _users WHERE user-_id={user_id}"
+            cur = self._cursor.execute(sql)
 
-        sql = f"SELECT * FROM _users WHERE user-_id={user_id}"
-        cur = self._cursor.execute(sql)
-
-        row = cur.fetchone()
-        if row is None:
-            self._cursor.execute(sql)
-            self._conn.commit()
-        else:
+            row = cur.fetchone()
+            if row is None:
+                self._cursor.execute(sql)
+                self._conn.commit()
+        except sqlite3.OperationalError as e:
             return {'user': 'is table'}
```

### Comparing `pyeasydbapi-0.1.1/pyEasyDbApi.egg-info/PKG-INFO` & `pyeasydbapi-0.1.2/pyEasyDbApi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEasyDbApi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple DataBase to use
 Home-page: https://t.me/n1grtr33x
 Author: n1grtr33x
 Author-email: dmitroluc7@gmail.com
 Keywords: easy-db
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyeasydbapi-0.1.1/setup.py` & `pyeasydbapi-0.1.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='pyEasyDbApi',
-    version='0.1.1',
+    version='0.1.2',
     author='n1grtr33x',
     author_email='dmitroluc7@gmail.com',
     description='Simple DataBase to use',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://t.me/n1grtr33x',
     packages=find_packages(),
```

