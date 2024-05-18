# Comparing `tmp/pyeasydbapi-0.1.3.tar.gz` & `tmp/pyeasydbapi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeasydbapi-0.1.3.tar", last modified: Sat May 18 19:35:28 2024, max compression
+gzip compressed data, was "pyeasydbapi-0.1.4.tar", last modified: Sat May 18 19:38:32 2024, max compression
```

## Comparing `pyeasydbapi-0.1.3.tar` & `pyeasydbapi-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:35:28.274672 pyeasydbapi-0.1.3/
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       12 2024-05-16 20:46:59.000000 pyeasydbapi-0.1.3/LICENSE
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      521 2024-05-18 19:35:28.274672 pyeasydbapi-0.1.3/PKG-INFO
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       93 2024-05-18 19:08:50.000000 pyeasydbapi-0.1.3/README.md
-drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:35:28.274672 pyeasydbapi-0.1.3/SimpleDB/
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       33 2024-05-18 19:12:23.000000 pyeasydbapi-0.1.3/SimpleDB/__init__.py
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)     4669 2024-05-18 19:35:23.000000 pyeasydbapi-0.1.3/SimpleDB/main.py
-drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:35:28.274672 pyeasydbapi-0.1.3/pyEasyDbApi.egg-info/
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      521 2024-05-18 19:35:28.000000 pyeasydbapi-0.1.3/pyEasyDbApi.egg-info/PKG-INFO
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      214 2024-05-18 19:35:28.000000 pyeasydbapi-0.1.3/pyEasyDbApi.egg-info/SOURCES.txt
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        1 2024-05-18 19:35:28.000000 pyeasydbapi-0.1.3/pyEasyDbApi.egg-info/dependency_links.txt
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        9 2024-05-18 19:35:28.000000 pyeasydbapi-0.1.3/pyEasyDbApi.egg-info/top_level.txt
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       38 2024-05-18 19:35:28.274672 pyeasydbapi-0.1.3/setup.cfg
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      704 2024-05-18 19:35:23.000000 pyeasydbapi-0.1.3/setup.py
+drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:38:32.658748 pyeasydbapi-0.1.4/
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       12 2024-05-16 20:46:59.000000 pyeasydbapi-0.1.4/LICENSE
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      521 2024-05-18 19:38:32.658748 pyeasydbapi-0.1.4/PKG-INFO
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       93 2024-05-18 19:08:50.000000 pyeasydbapi-0.1.4/README.md
+drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:38:32.657748 pyeasydbapi-0.1.4/SimpleDB/
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       33 2024-05-18 19:12:23.000000 pyeasydbapi-0.1.4/SimpleDB/__init__.py
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)     4672 2024-05-18 19:38:21.000000 pyeasydbapi-0.1.4/SimpleDB/main.py
+drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:38:32.658748 pyeasydbapi-0.1.4/pyEasyDbApi.egg-info/
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      521 2024-05-18 19:38:32.000000 pyeasydbapi-0.1.4/pyEasyDbApi.egg-info/PKG-INFO
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      214 2024-05-18 19:38:32.000000 pyeasydbapi-0.1.4/pyEasyDbApi.egg-info/SOURCES.txt
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        1 2024-05-18 19:38:32.000000 pyeasydbapi-0.1.4/pyEasyDbApi.egg-info/dependency_links.txt
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        9 2024-05-18 19:38:32.000000 pyeasydbapi-0.1.4/pyEasyDbApi.egg-info/top_level.txt
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       38 2024-05-18 19:38:32.658748 pyeasydbapi-0.1.4/setup.cfg
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      704 2024-05-18 19:38:21.000000 pyeasydbapi-0.1.4/setup.py
```

### Comparing `pyeasydbapi-0.1.3/PKG-INFO` & `pyeasydbapi-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEasyDbApi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple DataBase to use
 Home-page: https://t.me/n1grtr33x
 Author: n1grtr33x
 Author-email: dmitroluc7@gmail.com
 Keywords: easy-db
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyeasydbapi-0.1.3/SimpleDB/main.py` & `pyeasydbapi-0.1.4/SimpleDB/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
         sql_1 = (f"CREATE TABLE IF NOT EXISTS '_users' (user_id TEXT UNIQUE NOT NULL,"
                  f" name TEXT NOT NULL, TEXT NOT NULL, {args})")
 
         self._cursor.execute(sql_1)
         self._conn.commit()
 
-        sql = f"SELECT * FROM _users WHERE user-_id={user_id}"
-        cur = self._cursor.execute(sql)
+        sql_1 = f"SELECT * FROM _users WHERE user_id={user_id}"
+        cur = self._cursor.execute(sql_1)
 
         row = cur.fetchone()
         if row is None:
             self._cursor.execute(sql)
             self._conn.commit()
         return {'user': 'is table'}
```

### Comparing `pyeasydbapi-0.1.3/pyEasyDbApi.egg-info/PKG-INFO` & `pyeasydbapi-0.1.4/pyEasyDbApi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEasyDbApi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple DataBase to use
 Home-page: https://t.me/n1grtr33x
 Author: n1grtr33x
 Author-email: dmitroluc7@gmail.com
 Keywords: easy-db
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyeasydbapi-0.1.3/setup.py` & `pyeasydbapi-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='pyEasyDbApi',
-    version='0.1.3',
+    version='0.1.4',
     author='n1grtr33x',
     author_email='dmitroluc7@gmail.com',
     description='Simple DataBase to use',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://t.me/n1grtr33x',
     packages=find_packages(),
```

