# Comparing `tmp/pyeasydbapi-0.1.6.tar.gz` & `tmp/pyeasydbapi-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeasydbapi-0.1.6.tar", last modified: Sat May 18 19:44:09 2024, max compression
+gzip compressed data, was "pyeasydbapi-0.1.7.tar", last modified: Sat May 18 19:47:09 2024, max compression
```

## Comparing `pyeasydbapi-0.1.6.tar` & `pyeasydbapi-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:44:09.602041 pyeasydbapi-0.1.6/
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       12 2024-05-16 20:46:59.000000 pyeasydbapi-0.1.6/LICENSE
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      521 2024-05-18 19:44:09.602041 pyeasydbapi-0.1.6/PKG-INFO
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       93 2024-05-18 19:08:50.000000 pyeasydbapi-0.1.6/README.md
-drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:44:09.602041 pyeasydbapi-0.1.6/SimpleDB/
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       33 2024-05-18 19:12:23.000000 pyeasydbapi-0.1.6/SimpleDB/__init__.py
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)     4678 2024-05-18 19:44:03.000000 pyeasydbapi-0.1.6/SimpleDB/main.py
-drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:44:09.602041 pyeasydbapi-0.1.6/pyEasyDbApi.egg-info/
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      521 2024-05-18 19:44:09.000000 pyeasydbapi-0.1.6/pyEasyDbApi.egg-info/PKG-INFO
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      214 2024-05-18 19:44:09.000000 pyeasydbapi-0.1.6/pyEasyDbApi.egg-info/SOURCES.txt
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        1 2024-05-18 19:44:09.000000 pyeasydbapi-0.1.6/pyEasyDbApi.egg-info/dependency_links.txt
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        9 2024-05-18 19:44:09.000000 pyeasydbapi-0.1.6/pyEasyDbApi.egg-info/top_level.txt
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       38 2024-05-18 19:44:09.602041 pyeasydbapi-0.1.6/setup.cfg
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      704 2024-05-18 19:44:03.000000 pyeasydbapi-0.1.6/setup.py
+drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:47:09.475274 pyeasydbapi-0.1.7/
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       12 2024-05-16 20:46:59.000000 pyeasydbapi-0.1.7/LICENSE
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      521 2024-05-18 19:47:09.475274 pyeasydbapi-0.1.7/PKG-INFO
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       93 2024-05-18 19:08:50.000000 pyeasydbapi-0.1.7/README.md
+drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:47:09.474274 pyeasydbapi-0.1.7/SimpleDB/
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       33 2024-05-18 19:12:23.000000 pyeasydbapi-0.1.7/SimpleDB/__init__.py
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)     4688 2024-05-18 19:47:04.000000 pyeasydbapi-0.1.7/SimpleDB/main.py
+drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:47:09.474274 pyeasydbapi-0.1.7/pyEasyDbApi.egg-info/
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      521 2024-05-18 19:47:09.000000 pyeasydbapi-0.1.7/pyEasyDbApi.egg-info/PKG-INFO
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      214 2024-05-18 19:47:09.000000 pyeasydbapi-0.1.7/pyEasyDbApi.egg-info/SOURCES.txt
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        1 2024-05-18 19:47:09.000000 pyeasydbapi-0.1.7/pyEasyDbApi.egg-info/dependency_links.txt
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        9 2024-05-18 19:47:09.000000 pyeasydbapi-0.1.7/pyEasyDbApi.egg-info/top_level.txt
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       38 2024-05-18 19:47:09.475274 pyeasydbapi-0.1.7/setup.cfg
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      704 2024-05-18 19:47:04.000000 pyeasydbapi-0.1.7/setup.py
```

### Comparing `pyeasydbapi-0.1.6/PKG-INFO` & `pyeasydbapi-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEasyDbApi
-Version: 0.1.6
+Version: 0.1.7
 Summary: Simple DataBase to use
 Home-page: https://t.me/n1grtr33x
 Author: n1grtr33x
 Author-email: dmitroluc7@gmail.com
 Keywords: easy-db
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyeasydbapi-0.1.6/SimpleDB/main.py` & `pyeasydbapi-0.1.7/SimpleDB/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,17 +131,17 @@
     def add_user(self, user_id, name, args = None):
         """         :param user_id: user id
                     :param args your vars
                     :param name: user name
         """
 
         if args is None:
-            sql = f"INSERT INTO _users (user_id, name) VALUES ({id}, {name})"
+            sql = f"INSERT INTO _users (user_id, name) VALUES ({user_id}, {name})"
         else:
-            sql = f"INSERT INTO _users (user_id, name), {args}) VALUES ({id}, {name}, {args})"
+            sql = f"INSERT INTO _users (user_id, name), {args}) VALUES ({user_id}, {name}, {args})"
 
         sql_1 = (f"CREATE TABLE IF NOT EXISTS '_users' (user_id TEXT UNIQUE NOT NULL,"
                  f" name TEXT NOT NULL, TEXT NOT NULL, {args})")
 
         self._cursor.execute(sql_1)
         self._conn.commit()
```

### Comparing `pyeasydbapi-0.1.6/pyEasyDbApi.egg-info/PKG-INFO` & `pyeasydbapi-0.1.7/pyEasyDbApi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEasyDbApi
-Version: 0.1.6
+Version: 0.1.7
 Summary: Simple DataBase to use
 Home-page: https://t.me/n1grtr33x
 Author: n1grtr33x
 Author-email: dmitroluc7@gmail.com
 Keywords: easy-db
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyeasydbapi-0.1.6/setup.py` & `pyeasydbapi-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='pyEasyDbApi',
-    version='0.1.6',
+    version='0.1.7',
     author='n1grtr33x',
     author_email='dmitroluc7@gmail.com',
     description='Simple DataBase to use',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://t.me/n1grtr33x',
     packages=find_packages(),
```

