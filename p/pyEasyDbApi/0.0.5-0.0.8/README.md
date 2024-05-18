# Comparing `tmp/pyeasydbapi-0.0.5.tar.gz` & `tmp/pyeasydbapi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeasydbapi-0.0.5.tar", last modified: Thu May 16 21:26:20 2024, max compression
+gzip compressed data, was "pyeasydbapi-0.0.8.tar", last modified: Sat May 18 19:19:19 2024, max compression
```

## Comparing `pyeasydbapi-0.0.5.tar` & `pyeasydbapi-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-16 21:26:20.211448 pyeasydbapi-0.0.5/
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       12 2024-05-16 20:46:59.000000 pyeasydbapi-0.0.5/LICENSE
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      473 2024-05-16 21:26:20.211448 pyeasydbapi-0.0.5/PKG-INFO
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       45 2024-05-16 21:18:47.000000 pyeasydbapi-0.0.5/README.md
-drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-16 21:26:20.210448 pyeasydbapi-0.0.5/SimpleDB/
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       37 2024-05-16 21:22:53.000000 pyeasydbapi-0.0.5/SimpleDB/__init__.py
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)     3625 2024-05-16 21:26:15.000000 pyeasydbapi-0.0.5/SimpleDB/main.py
-drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-16 21:26:20.210448 pyeasydbapi-0.0.5/pyEasyDbApi.egg-info/
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      473 2024-05-16 21:26:20.000000 pyeasydbapi-0.0.5/pyEasyDbApi.egg-info/PKG-INFO
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      214 2024-05-16 21:26:20.000000 pyeasydbapi-0.0.5/pyEasyDbApi.egg-info/SOURCES.txt
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        1 2024-05-16 21:26:20.000000 pyeasydbapi-0.0.5/pyEasyDbApi.egg-info/dependency_links.txt
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        9 2024-05-16 21:26:20.000000 pyeasydbapi-0.0.5/pyEasyDbApi.egg-info/top_level.txt
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       38 2024-05-16 21:26:20.211448 pyeasydbapi-0.0.5/setup.cfg
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      704 2024-05-16 21:26:15.000000 pyeasydbapi-0.0.5/setup.py
+drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:19:19.984383 pyeasydbapi-0.0.8/
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       12 2024-05-16 20:46:59.000000 pyeasydbapi-0.0.8/LICENSE
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      521 2024-05-18 19:19:19.984383 pyeasydbapi-0.0.8/PKG-INFO
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       93 2024-05-18 19:08:50.000000 pyeasydbapi-0.0.8/README.md
+drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:19:19.983384 pyeasydbapi-0.0.8/SimpleDB/
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       33 2024-05-18 19:12:23.000000 pyeasydbapi-0.0.8/SimpleDB/__init__.py
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)     4601 2024-05-18 19:16:15.000000 pyeasydbapi-0.0.8/SimpleDB/main.py
+drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-18 19:19:19.984383 pyeasydbapi-0.0.8/pyEasyDbApi.egg-info/
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      521 2024-05-18 19:19:19.000000 pyeasydbapi-0.0.8/pyEasyDbApi.egg-info/PKG-INFO
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      214 2024-05-18 19:19:19.000000 pyeasydbapi-0.0.8/pyEasyDbApi.egg-info/SOURCES.txt
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        1 2024-05-18 19:19:19.000000 pyeasydbapi-0.0.8/pyEasyDbApi.egg-info/dependency_links.txt
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        9 2024-05-18 19:19:19.000000 pyeasydbapi-0.0.8/pyEasyDbApi.egg-info/top_level.txt
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       38 2024-05-18 19:19:19.984383 pyeasydbapi-0.0.8/setup.cfg
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      704 2024-05-18 19:19:14.000000 pyeasydbapi-0.0.8/setup.py
```

### Comparing `pyeasydbapi-0.0.5/SimpleDB/main.py` & `pyeasydbapi-0.0.8/SimpleDB/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,19 +20,23 @@
         """Get database for selected module"""
         raise NotImplementedError
 
     def close(self):
         """Close the database"""
         raise NotImplementedError
 
+    def add_user(self, user_id, name, args):
+        """Add user to database"""
+
 
 class SqliteDatabase(Database):
     """
     :param file: DataBase file
     """
+
     def __init__(self, file):
         self._conn = sqlite3.connect(file, check_same_thread=False)
         self._conn.row_factory = sqlite3.Row
         self._cursor = self._conn.cursor()
         self._lock = threading.Lock()
 
     @staticmethod
@@ -116,9 +120,35 @@
 
         return collection
 
     def close(self):
         self._conn.commit()
         self._conn.close()
 
+    def _add_user(self, user_id):
+        if self.get('_users', user_id) is not None:
+            return False
+
+    def add_user(self, user_id, name, args: str = None):
+        """         :param user_id: user id
+                    :param args your vars
+                    :param name: user name
+        """
+
+        if args is None:
+            sql = f"INSERT INTO _users (id, name) VALUES ({id}, {name})"
+        else:
+            sql = f"INSERT INTO _users (id, name, {args}) VALUES ({id}, {name}, {args})"
+        self._lock.acquire()
 
-db = SqliteDatabase("data.db")
+        sql_1 = (f"CREATE TABLE IF NOT EXISTS 'users' (user_id TEXT UNIQUE NOT NULL,"
+                 f" name TEXT NOT NULL, TEXT NOT NULL, {args})")
+
+        self._cursor.execute(sql_1)
+
+        if self._add_user(user_id) is False:
+            self._cursor.execute(sql)
+        else:
+            return {'user': 'is table'}
+
+        self._conn.commit()
+        self._lock.release()
```

### Comparing `pyeasydbapi-0.0.5/setup.py` & `pyeasydbapi-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='pyEasyDbApi',
-    version='0.0.5',
+    version='0.0.8',
     author='n1grtr33x',
     author_email='dmitroluc7@gmail.com',
     description='Simple DataBase to use',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://t.me/n1grtr33x',
     packages=find_packages(),
```

