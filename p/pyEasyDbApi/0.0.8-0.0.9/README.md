# Comparing `tmp/pyeasydbapi-0.0.8.tar.gz` & `tmp/pyeasydbapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeasydbapi-0.0.8.tar", last modified: Sat May 18 19:19:19 2024, max compression
+gzip compressed data, was "pyeasydbapi-0.0.9.tar", last modified: Sat May 18 19:23:35 2024, max compression
```

## Comparing `pyeasydbapi-0.0.8.tar` & `pyeasydbapi-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:19:19.984383 pyeasydbapi-0.0.8/
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       12 2024-05-16 20:46:59.000000 pyeasydbapi-0.0.8/LICENSE
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      521 2024-05-18 19:19:19.984383 pyeasydbapi-0.0.8/PKG-INFO
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       93 2024-05-18 19:08:50.000000 pyeasydbapi-0.0.8/README.md
-drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:19:19.983384 pyeasydbapi-0.0.8/SimpleDB/
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       33 2024-05-18 19:12:23.000000 pyeasydbapi-0.0.8/SimpleDB/__init__.py
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)     4601 2024-05-18 19:16:15.000000 pyeasydbapi-0.0.8/SimpleDB/main.py
-drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:19:19.984383 pyeasydbapi-0.0.8/pyEasyDbApi.egg-info/
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      521 2024-05-18 19:19:19.000000 pyeasydbapi-0.0.8/pyEasyDbApi.egg-info/PKG-INFO
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      214 2024-05-18 19:19:19.000000 pyeasydbapi-0.0.8/pyEasyDbApi.egg-info/SOURCES.txt
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        1 2024-05-18 19:19:19.000000 pyeasydbapi-0.0.8/pyEasyDbApi.egg-info/dependency_links.txt
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        9 2024-05-18 19:19:19.000000 pyeasydbapi-0.0.8/pyEasyDbApi.egg-info/top_level.txt
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       38 2024-05-18 19:19:19.984383 pyeasydbapi-0.0.8/setup.cfg
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      704 2024-05-18 19:19:14.000000 pyeasydbapi-0.0.8/setup.py
+drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:23:35.478101 pyeasydbapi-0.0.9/
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       12 2024-05-16 20:46:59.000000 pyeasydbapi-0.0.9/LICENSE
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      521 2024-05-18 19:23:35.478101 pyeasydbapi-0.0.9/PKG-INFO
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       93 2024-05-18 19:08:50.000000 pyeasydbapi-0.0.9/README.md
+drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:23:35.478101 pyeasydbapi-0.0.9/SimpleDB/
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       33 2024-05-18 19:12:23.000000 pyeasydbapi-0.0.9/SimpleDB/__init__.py
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)     4543 2024-05-18 19:23:28.000000 pyeasydbapi-0.0.9/SimpleDB/main.py
+drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:23:35.478101 pyeasydbapi-0.0.9/pyEasyDbApi.egg-info/
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      521 2024-05-18 19:23:35.000000 pyeasydbapi-0.0.9/pyEasyDbApi.egg-info/PKG-INFO
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      214 2024-05-18 19:23:35.000000 pyeasydbapi-0.0.9/pyEasyDbApi.egg-info/SOURCES.txt
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        1 2024-05-18 19:23:35.000000 pyeasydbapi-0.0.9/pyEasyDbApi.egg-info/dependency_links.txt
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        9 2024-05-18 19:23:35.000000 pyeasydbapi-0.0.9/pyEasyDbApi.egg-info/top_level.txt
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       38 2024-05-18 19:23:35.478101 pyeasydbapi-0.0.9/setup.cfg
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      704 2024-05-18 19:23:28.000000 pyeasydbapi-0.0.9/setup.py
```

### Comparing `pyeasydbapi-0.0.8/PKG-INFO` & `pyeasydbapi-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEasyDbApi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple DataBase to use
 Home-page: https://t.me/n1grtr33x
 Author: n1grtr33x
 Author-email: dmitroluc7@gmail.com
 Keywords: easy-db
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyeasydbapi-0.0.8/SimpleDB/main.py` & `pyeasydbapi-0.0.9/SimpleDB/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,21 +134,19 @@
                     :param name: user name
         """
 
         if args is None:
             sql = f"INSERT INTO _users (id, name) VALUES ({id}, {name})"
         else:
             sql = f"INSERT INTO _users (id, name, {args}) VALUES ({id}, {name}, {args})"
-        self._lock.acquire()
 
         sql_1 = (f"CREATE TABLE IF NOT EXISTS 'users' (user_id TEXT UNIQUE NOT NULL,"
                  f" name TEXT NOT NULL, TEXT NOT NULL, {args})")
 
         self._cursor.execute(sql_1)
 
         if self._add_user(user_id) is False:
             self._cursor.execute(sql)
         else:
             return {'user': 'is table'}
 
         self._conn.commit()
-        self._lock.release()
```

### Comparing `pyeasydbapi-0.0.8/pyEasyDbApi.egg-info/PKG-INFO` & `pyeasydbapi-0.0.9/pyEasyDbApi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEasyDbApi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple DataBase to use
 Home-page: https://t.me/n1grtr33x
 Author: n1grtr33x
 Author-email: dmitroluc7@gmail.com
 Keywords: easy-db
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyeasydbapi-0.0.8/setup.py` & `pyeasydbapi-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='pyEasyDbApi',
-    version='0.0.8',
+    version='0.0.9',
     author='n1grtr33x',
     author_email='dmitroluc7@gmail.com',
     description='Simple DataBase to use',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://t.me/n1grtr33x',
     packages=find_packages(),
```

