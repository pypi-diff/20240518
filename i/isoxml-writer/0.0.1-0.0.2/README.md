# Comparing `tmp/isoxml_writer-0.0.1.tar.gz` & `tmp/isoxml_writer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isoxml_writer-0.0.1.tar", last modified: Sat May 18 10:58:20 2024, max compression
+gzip compressed data, was "isoxml_writer-0.0.2.tar", last modified: Sat May 18 11:48:10 2024, max compression
```

## Comparing `isoxml_writer-0.0.1.tar` & `isoxml_writer-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 markus    (1000) users      (984)        0 2024-05-18 10:58:20.861694 isoxml_writer-0.0.1/
--rw-r--r--   0 markus    (1000) users      (984)     1082 2024-05-18 10:12:35.000000 isoxml_writer-0.0.1/LICENSE
--rw-r--r--   0 markus    (1000) users      (984)     1800 2024-05-18 10:58:20.861694 isoxml_writer-0.0.1/PKG-INFO
--rw-r--r--   0 markus    (1000) users      (984)     1305 2024-05-18 10:52:16.000000 isoxml_writer-0.0.1/README.md
--rw-r--r--   0 markus    (1000) users      (984)      704 2024-05-18 10:50:39.000000 isoxml_writer-0.0.1/pyproject.toml
--rw-r--r--   0 markus    (1000) users      (984)       38 2024-05-18 10:58:20.861694 isoxml_writer-0.0.1/setup.cfg
-drwxr-xr-x   0 markus    (1000) users      (984)        0 2024-05-18 10:58:20.858361 isoxml_writer-0.0.1/src/
-drwxr-xr-x   0 markus    (1000) users      (984)        0 2024-05-18 10:58:20.861694 isoxml_writer-0.0.1/src/isoxml_writer/
-drwxr-xr-x   0 markus    (1000) users      (984)        0 2024-05-18 10:58:20.861694 isoxml_writer-0.0.1/src/isoxml_writer/ISOXML_schema/
--rw-r--r--   0 markus    (1000) users      (984)   144216 2024-05-18 10:08:08.000000 isoxml_writer-0.0.1/src/isoxml_writer/ISOXML_schema/ISO11783_Common_V4-3.xsd
--rw-r--r--   0 markus    (1000) users      (984)     4021 2024-05-18 10:08:08.000000 isoxml_writer-0.0.1/src/isoxml_writer/ISOXML_schema/ISO11783_ExternalFile_V4-3.xsd
--rw-r--r--   0 markus    (1000) users      (984)     7913 2024-05-18 10:08:08.000000 isoxml_writer-0.0.1/src/isoxml_writer/ISOXML_schema/ISO11783_LinkListFile_V4-3.xsd
--rw-r--r--   0 markus    (1000) users      (984)    15740 2024-05-18 10:08:08.000000 isoxml_writer-0.0.1/src/isoxml_writer/ISOXML_schema/ISO11783_TaskFile_V4-3.xsd
--rw-r--r--   0 markus    (1000) users      (984)    12258 2024-05-18 10:08:08.000000 isoxml_writer-0.0.1/src/isoxml_writer/ISOXML_schema/ISO11783_TimeLog_V4-3.xsd
--rw-r--r--   0 markus    (1000) users      (984)        0 2024-05-18 10:06:57.000000 isoxml_writer-0.0.1/src/isoxml_writer/__init__.py
--rw-r--r--   0 markus    (1000) users      (984)     2131 2024-05-18 10:07:37.000000 isoxml_writer-0.0.1/src/isoxml_writer/ddi.py
--rw-r--r--   0 markus    (1000) users      (984)     8628 2024-05-18 10:43:41.000000 isoxml_writer-0.0.1/src/isoxml_writer/isoxml.py
-drwxr-xr-x   0 markus    (1000) users      (984)        0 2024-05-18 10:58:20.861694 isoxml_writer-0.0.1/src/isoxml_writer.egg-info/
--rw-r--r--   0 markus    (1000) users      (984)     1800 2024-05-18 10:58:20.000000 isoxml_writer-0.0.1/src/isoxml_writer.egg-info/PKG-INFO
--rw-r--r--   0 markus    (1000) users      (984)      619 2024-05-18 10:58:20.000000 isoxml_writer-0.0.1/src/isoxml_writer.egg-info/SOURCES.txt
--rw-r--r--   0 markus    (1000) users      (984)        1 2024-05-18 10:58:20.000000 isoxml_writer-0.0.1/src/isoxml_writer.egg-info/dependency_links.txt
--rw-r--r--   0 markus    (1000) users      (984)        5 2024-05-18 10:58:20.000000 isoxml_writer-0.0.1/src/isoxml_writer.egg-info/requires.txt
--rw-r--r--   0 markus    (1000) users      (984)       14 2024-05-18 10:58:20.000000 isoxml_writer-0.0.1/src/isoxml_writer.egg-info/top_level.txt
+drwxr-xr-x   0 markus    (1000) users      (984)        0 2024-05-18 11:48:10.485387 isoxml_writer-0.0.2/
+-rw-r--r--   0 markus    (1000) users      (984)     1082 2024-05-18 10:12:35.000000 isoxml_writer-0.0.2/LICENSE
+-rw-r--r--   0 markus    (1000) users      (984)     1800 2024-05-18 11:48:10.485387 isoxml_writer-0.0.2/PKG-INFO
+-rw-r--r--   0 markus    (1000) users      (984)     1305 2024-05-18 10:52:16.000000 isoxml_writer-0.0.2/README.md
+-rw-r--r--   0 markus    (1000) users      (984)      704 2024-05-18 11:47:31.000000 isoxml_writer-0.0.2/pyproject.toml
+-rw-r--r--   0 markus    (1000) users      (984)       38 2024-05-18 11:48:10.485387 isoxml_writer-0.0.2/setup.cfg
+drwxr-xr-x   0 markus    (1000) users      (984)        0 2024-05-18 11:48:10.485387 isoxml_writer-0.0.2/src/
+drwxr-xr-x   0 markus    (1000) users      (984)        0 2024-05-18 11:48:10.485387 isoxml_writer-0.0.2/src/isoxml_writer/
+drwxr-xr-x   0 markus    (1000) users      (984)        0 2024-05-18 11:48:10.485387 isoxml_writer-0.0.2/src/isoxml_writer/ISOXML_schema/
+-rw-r--r--   0 markus    (1000) users      (984)   144216 2024-05-18 10:08:08.000000 isoxml_writer-0.0.2/src/isoxml_writer/ISOXML_schema/ISO11783_Common_V4-3.xsd
+-rw-r--r--   0 markus    (1000) users      (984)     4021 2024-05-18 10:08:08.000000 isoxml_writer-0.0.2/src/isoxml_writer/ISOXML_schema/ISO11783_ExternalFile_V4-3.xsd
+-rw-r--r--   0 markus    (1000) users      (984)     7913 2024-05-18 10:08:08.000000 isoxml_writer-0.0.2/src/isoxml_writer/ISOXML_schema/ISO11783_LinkListFile_V4-3.xsd
+-rw-r--r--   0 markus    (1000) users      (984)    15740 2024-05-18 10:08:08.000000 isoxml_writer-0.0.2/src/isoxml_writer/ISOXML_schema/ISO11783_TaskFile_V4-3.xsd
+-rw-r--r--   0 markus    (1000) users      (984)    12258 2024-05-18 10:08:08.000000 isoxml_writer-0.0.2/src/isoxml_writer/ISOXML_schema/ISO11783_TimeLog_V4-3.xsd
+-rw-r--r--   0 markus    (1000) users      (984)        0 2024-05-18 10:06:57.000000 isoxml_writer-0.0.2/src/isoxml_writer/__init__.py
+-rw-r--r--   0 markus    (1000) users      (984)     2131 2024-05-18 10:07:37.000000 isoxml_writer-0.0.2/src/isoxml_writer/ddi.py
+-rw-r--r--   0 markus    (1000) users      (984)     8770 2024-05-18 11:44:21.000000 isoxml_writer-0.0.2/src/isoxml_writer/isoxml.py
+drwxr-xr-x   0 markus    (1000) users      (984)        0 2024-05-18 11:48:10.485387 isoxml_writer-0.0.2/src/isoxml_writer.egg-info/
+-rw-r--r--   0 markus    (1000) users      (984)     1800 2024-05-18 11:48:10.000000 isoxml_writer-0.0.2/src/isoxml_writer.egg-info/PKG-INFO
+-rw-r--r--   0 markus    (1000) users      (984)      619 2024-05-18 11:48:10.000000 isoxml_writer-0.0.2/src/isoxml_writer.egg-info/SOURCES.txt
+-rw-r--r--   0 markus    (1000) users      (984)        1 2024-05-18 11:48:10.000000 isoxml_writer-0.0.2/src/isoxml_writer.egg-info/dependency_links.txt
+-rw-r--r--   0 markus    (1000) users      (984)        5 2024-05-18 11:48:10.000000 isoxml_writer-0.0.2/src/isoxml_writer.egg-info/requires.txt
+-rw-r--r--   0 markus    (1000) users      (984)       14 2024-05-18 11:48:10.000000 isoxml_writer-0.0.2/src/isoxml_writer.egg-info/top_level.txt
```

### Comparing `isoxml_writer-0.0.1/LICENSE` & `isoxml_writer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `isoxml_writer-0.0.1/PKG-INFO` & `isoxml_writer-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isoxml_writer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Create ISO11783 Taskdata
 Author-email: just-read-the-instructions <bla@imperius.cloud>
 Project-URL: Homepage, https://github.com/just-read-the-instructions/python-isoxml-writer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `isoxml_writer-0.0.1/README.md` & `isoxml_writer-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `isoxml_writer-0.0.1/pyproject.toml` & `isoxml_writer-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 where = ["src"]
 
 [tool.setuptools.package-data]
 "isoxml_writer.ISOXML_schema" = ["*.xsd"]
 
 [project]
 name = "isoxml_writer"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="just-read-the-instructions", email="bla@imperius.cloud" },
 ]
 description = "Create ISO11783 Taskdata"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `isoxml_writer-0.0.1/src/isoxml_writer/ISOXML_schema/ISO11783_Common_V4-3.xsd` & `isoxml_writer-0.0.2/src/isoxml_writer/ISOXML_schema/ISO11783_Common_V4-3.xsd`

 * *Files identical despite different names*

### Comparing `isoxml_writer-0.0.1/src/isoxml_writer/ISOXML_schema/ISO11783_ExternalFile_V4-3.xsd` & `isoxml_writer-0.0.2/src/isoxml_writer/ISOXML_schema/ISO11783_ExternalFile_V4-3.xsd`

 * *Files identical despite different names*

### Comparing `isoxml_writer-0.0.1/src/isoxml_writer/ISOXML_schema/ISO11783_LinkListFile_V4-3.xsd` & `isoxml_writer-0.0.2/src/isoxml_writer/ISOXML_schema/ISO11783_LinkListFile_V4-3.xsd`

 * *Files identical despite different names*

### Comparing `isoxml_writer-0.0.1/src/isoxml_writer/ISOXML_schema/ISO11783_TaskFile_V4-3.xsd` & `isoxml_writer-0.0.2/src/isoxml_writer/ISOXML_schema/ISO11783_TaskFile_V4-3.xsd`

 * *Files identical despite different names*

### Comparing `isoxml_writer-0.0.1/src/isoxml_writer/ISOXML_schema/ISO11783_TimeLog_V4-3.xsd` & `isoxml_writer-0.0.2/src/isoxml_writer/ISOXML_schema/ISO11783_TimeLog_V4-3.xsd`

 * *Files identical despite different names*

### Comparing `isoxml_writer-0.0.1/src/isoxml_writer/ddi.py` & `isoxml_writer-0.0.2/src/isoxml_writer/ddi.py`

 * *Files identical despite different names*

### Comparing `isoxml_writer-0.0.1/src/isoxml_writer/isoxml.py` & `isoxml_writer-0.0.2/src/isoxml_writer/isoxml.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,20 @@
 
     def add_polygon(self, polygon):
         self.et.append(polygon.et)
 
     def add_guidance_group(self, guidance_group):
         self.et.append(guidance_group.et)
 
+    def set_customer(self, customer):
+        self.et.set("E", customer.id)
+
+    def set_farm(self, farm):
+        self.et.set("F", farm.id)
+
 
 
 class Polygon:
     """
     Types:
         1: Partfield Boundary
         2: TreatmentZone
```

### Comparing `isoxml_writer-0.0.1/src/isoxml_writer.egg-info/PKG-INFO` & `isoxml_writer-0.0.2/src/isoxml_writer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isoxml_writer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Create ISO11783 Taskdata
 Author-email: just-read-the-instructions <bla@imperius.cloud>
 Project-URL: Homepage, https://github.com/just-read-the-instructions/python-isoxml-writer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `isoxml_writer-0.0.1/src/isoxml_writer.egg-info/SOURCES.txt` & `isoxml_writer-0.0.2/src/isoxml_writer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

