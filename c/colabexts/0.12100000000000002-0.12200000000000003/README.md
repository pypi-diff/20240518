# Comparing `tmp/colabexts-0.12100000000000002.tar.gz` & `tmp/colabexts-0.12200000000000003.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colabexts-0.12100000000000002.tar", last modified: Thu Apr 25 19:23:31 2024, max compression
+gzip compressed data, was "colabexts-0.12200000000000003.tar", last modified: Sat May 18 09:39:23 2024, max compression
```

## Comparing `colabexts-0.12100000000000002.tar` & `colabexts-0.12200000000000003.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-04-25 19:23:31.301974 colabexts-0.12100000000000002/
--rw-r--r--   0 snarayan   (501) wheel        (0)      780 2024-04-25 19:23:31.301129 colabexts-0.12100000000000002/PKG-INFO
--rw-r--r--   0 snarayan   (501) wheel        (0)     1081 2022-11-26 05:52:19.000000 colabexts-0.12100000000000002/README.md
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-04-25 19:23:31.298113 colabexts-0.12100000000000002/colabexts/
--rw-r--r--   0 snarayan   (501) wheel        (0)        0 2022-11-26 05:52:19.000000 colabexts-0.12100000000000002/colabexts/__init__.py
--rw-r--r--   0 snarayan   (501) wheel        (0)    11567 2024-04-23 12:55:18.000000 colabexts-0.12100000000000002/colabexts/jcommon.ipynb
--rw-r--r--   0 snarayan   (501) wheel        (0)     4669 2024-04-23 12:57:14.000000 colabexts-0.12100000000000002/colabexts/jcommon.py
--rw-r--r--   0 snarayan   (501) wheel        (0)      454 2022-11-26 05:52:19.000000 colabexts-0.12100000000000002/colabexts/log.py
--rw-r--r--   0 snarayan   (501) wheel        (0)     3846 2024-04-23 21:58:20.000000 colabexts-0.12100000000000002/colabexts/utils.py
--rw-r--r--   0 snarayan   (501) wheel        (0)       27 2024-04-25 19:23:31.000000 colabexts-0.12100000000000002/colabexts/version.txt
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-04-25 19:23:31.300711 colabexts-0.12100000000000002/colabexts.egg-info/
--rw-r--r--   0 snarayan   (501) wheel        (0)      780 2024-04-25 19:23:31.000000 colabexts-0.12100000000000002/colabexts.egg-info/PKG-INFO
--rw-r--r--   0 snarayan   (501) wheel        (0)      339 2024-04-25 19:23:31.000000 colabexts-0.12100000000000002/colabexts.egg-info/SOURCES.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)        1 2024-04-25 19:23:31.000000 colabexts-0.12100000000000002/colabexts.egg-info/dependency_links.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)        1 2024-04-23 15:26:14.000000 colabexts-0.12100000000000002/colabexts.egg-info/not-zip-safe
--rw-r--r--   0 snarayan   (501) wheel        (0)       20 2024-04-25 19:23:31.000000 colabexts-0.12100000000000002/colabexts.egg-info/requires.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)       10 2024-04-25 19:23:31.000000 colabexts-0.12100000000000002/colabexts.egg-info/top_level.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)       38 2024-04-25 19:23:31.302126 colabexts-0.12100000000000002/setup.cfg
--rw-r--r--   0 snarayan   (501) wheel        (0)     1678 2024-04-25 19:23:31.000000 colabexts-0.12100000000000002/setup.py
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-18 09:39:23.583473 colabexts-0.12200000000000003/
+-rw-r--r--   0 snarayan   (501) wheel        (0)      780 2024-05-18 09:39:23.583044 colabexts-0.12200000000000003/PKG-INFO
+-rw-r--r--   0 snarayan   (501) wheel        (0)     1081 2022-11-26 05:52:19.000000 colabexts-0.12200000000000003/README.md
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-18 09:39:23.580352 colabexts-0.12200000000000003/colabexts/
+-rw-r--r--   0 snarayan   (501) wheel        (0)        0 2022-11-26 05:52:19.000000 colabexts-0.12200000000000003/colabexts/__init__.py
+-rw-r--r--   0 snarayan   (501) wheel        (0)    11567 2024-04-23 12:55:18.000000 colabexts-0.12200000000000003/colabexts/jcommon.ipynb
+-rw-r--r--   0 snarayan   (501) wheel        (0)     4669 2024-04-23 12:57:14.000000 colabexts-0.12200000000000003/colabexts/jcommon.py
+-rw-r--r--   0 snarayan   (501) wheel        (0)      454 2022-11-26 05:52:19.000000 colabexts-0.12200000000000003/colabexts/log.py
+-rw-r--r--   0 snarayan   (501) wheel        (0)     3667 2024-05-18 09:38:08.000000 colabexts-0.12200000000000003/colabexts/utils.py
+-rw-r--r--   0 snarayan   (501) wheel        (0)       27 2024-05-18 09:39:23.000000 colabexts-0.12200000000000003/colabexts/version.txt
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-05-18 09:39:23.582590 colabexts-0.12200000000000003/colabexts.egg-info/
+-rw-r--r--   0 snarayan   (501) wheel        (0)      780 2024-05-18 09:39:23.000000 colabexts-0.12200000000000003/colabexts.egg-info/PKG-INFO
+-rw-r--r--   0 snarayan   (501) wheel        (0)      339 2024-05-18 09:39:23.000000 colabexts-0.12200000000000003/colabexts.egg-info/SOURCES.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)        1 2024-05-18 09:39:23.000000 colabexts-0.12200000000000003/colabexts.egg-info/dependency_links.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)        1 2024-04-23 15:26:14.000000 colabexts-0.12200000000000003/colabexts.egg-info/not-zip-safe
+-rw-r--r--   0 snarayan   (501) wheel        (0)       20 2024-05-18 09:39:23.000000 colabexts-0.12200000000000003/colabexts.egg-info/requires.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)       10 2024-05-18 09:39:23.000000 colabexts-0.12200000000000003/colabexts.egg-info/top_level.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)       38 2024-05-18 09:39:23.583552 colabexts-0.12200000000000003/setup.cfg
+-rw-r--r--   0 snarayan   (501) wheel        (0)     1678 2024-05-18 09:39:23.000000 colabexts-0.12200000000000003/setup.py
```

### Comparing `colabexts-0.12100000000000002/PKG-INFO` & `colabexts-0.12200000000000003/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colabexts
-Version: 0.12100000000000002
+Version: 0.12200000000000003
 Summary: Some simple Utilities
 Home-page: https://github.com/meyers007/colabext.git
 Author: Code Red
 Author-email: meyers@geospaces.org
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `colabexts-0.12100000000000002/README.md` & `colabexts-0.12200000000000003/README.md`

 * *Files identical despite different names*

### Comparing `colabexts-0.12100000000000002/colabexts/jcommon.ipynb` & `colabexts-0.12200000000000003/colabexts/jcommon.ipynb`

 * *Files identical despite different names*

### Comparing `colabexts-0.12100000000000002/colabexts/jcommon.py` & `colabexts-0.12200000000000003/colabexts/jcommon.py`

 * *Files identical despite different names*

### Comparing `colabexts-0.12100000000000002/colabexts/utils.py` & `colabexts-0.12200000000000003/colabexts/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,33 +32,15 @@
 
     def __delattr__(self, item):
         self.__delitem__(item)
 
     def __delitem__(self, key):
         super(Map, self).__delitem__(key)
         del self.__dict__[key]
-#-----------------------------------------------------------------------------------
-class mydict(dict):
-    def __init__(self, default_type="|key|locals|globals", *args, **kwargs):
-        super(mydict, self).__init__(*args, **kwargs)
-        for arg in args:
-            if isinstance(arg, dict):
-                for k, v in arg.items():
-                    self[k] = v
-        if kwargs:
-            for k, v in kwargs.items():
-                self[k] = v
 
-    def __missing__(self, key):
-        if key in  locals():
-            return locals()[key]
-        return key
-        
-def parsej(s, *args, **kwargs):
-    return eval(s, mydict(*args, **kwargs))
 
 #-----------------------------------------------------------------------------------
 def inJupyter():
     try:    get_ipython; return True
     except: return False
 #--------------------------------------------------------------------------------
 def is_number(s):
@@ -99,18 +81,36 @@
             if isinstance(arg, dict):
                 for k, v in arg.items():
                     self[k] = v
         if kwargs:
             for k, v in kwargs.items():
                 self[k] = v
 
+    def __getattr__(self, attr):
+        return self.get(attr)
+
+    def __setattr__(self, key, value):
+        self.__setitem__(key, value)
+
+    def __setitem__(self, key, value):
+        super(mydict, self).__setitem__(key, value)
+        self.__dict__.update({key: value})
+
+    def __delattr__(self, item):
+        self.__delitem__(item)
+
+    def __delitem__(self, key):
+        super(mydict, self).__delitem__(key)
+        del self.__dict__[key]
+
     def __missing__(self, key):
-        if key in  locals():
-            return locals()[key]
-        return key
+         if key in  locals():
+             return locals()[key]
+         return key
 
     def parsej(self, s):
         eval(s, **self)
+
         
 def parsej(s, *args, **kwargs):
-    return eval(s, mydict(*args, **kwargs))
+    return mydict(eval(s.strip() or "{}", mydict(*args, **kwargs)))
```

### Comparing `colabexts-0.12100000000000002/colabexts.egg-info/PKG-INFO` & `colabexts-0.12200000000000003/colabexts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colabexts
-Version: 0.12100000000000002
+Version: 0.12200000000000003
 Summary: Some simple Utilities
 Home-page: https://github.com/meyers007/colabext.git
 Author: Code Red
 Author-email: meyers@geospaces.org
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `colabexts-0.12100000000000002/setup.py` & `colabexts-0.12200000000000003/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version=0.12100000000000002
+version=0.12200000000000003
 
 setup(name='colabexts', 
       version=str(version), 
       description='Some simple Utilities',
       url='https://github.com/meyers007/colabext.git',
       author='Code Red',
       author_email='meyers@geospaces.org',
```

