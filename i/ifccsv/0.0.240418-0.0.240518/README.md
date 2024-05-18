# Comparing `tmp/ifccsv-0.0.240418.tar.gz` & `tmp/ifccsv-0.0.240518.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifccsv-0.0.240418.tar", last modified: Thu Apr 18 01:11:53 2024, max compression
+gzip compressed data, was "ifccsv-0.0.240518.tar", last modified: Sat May 18 01:15:31 2024, max compression
```

## Comparing `ifccsv-0.0.240418.tar` & `ifccsv-0.0.240518.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:11:53.745140 ifccsv-0.0.240418/
--rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-04-18 01:11:49.000000 ifccsv-0.0.240418/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-18 01:11:49.000000 ifccsv-0.0.240418/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-18 01:11:53.745140 ifccsv-0.0.240418/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:11:53.745140 ifccsv-0.0.240418/ifccsv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-18 01:11:53.000000 ifccsv-0.0.240418/ifccsv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-18 01:11:53.000000 ifccsv-0.0.240418/ifccsv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 01:11:53.000000 ifccsv-0.0.240418/ifccsv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 01:11:53.000000 ifccsv-0.0.240418/ifccsv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 01:11:53.000000 ifccsv-0.0.240418/ifccsv.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    21294 2024-04-18 01:11:49.000000 ifccsv-0.0.240418/ifccsv.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-18 01:11:51.000000 ifccsv-0.0.240418/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 01:11:53.745140 ifccsv-0.0.240418/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:15:31.592301 ifccsv-0.0.240518/
+-rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-05-18 01:15:25.000000 ifccsv-0.0.240518/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-18 01:15:25.000000 ifccsv-0.0.240518/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-18 01:15:31.592301 ifccsv-0.0.240518/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:15:31.592301 ifccsv-0.0.240518/ifccsv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-18 01:15:31.000000 ifccsv-0.0.240518/ifccsv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-18 01:15:31.000000 ifccsv-0.0.240518/ifccsv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 01:15:31.000000 ifccsv-0.0.240518/ifccsv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-18 01:15:31.000000 ifccsv-0.0.240518/ifccsv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-18 01:15:31.000000 ifccsv-0.0.240518/ifccsv.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21569 2024-05-18 01:15:25.000000 ifccsv-0.0.240518/ifccsv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-18 01:15:29.000000 ifccsv-0.0.240518/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 01:15:31.596301 ifccsv-0.0.240518/setup.cfg
```

### Comparing `ifccsv-0.0.240418/COPYING` & `ifccsv-0.0.240518/COPYING`

 * *Files identical despite different names*

### Comparing `ifccsv-0.0.240418/COPYING.LESSER` & `ifccsv-0.0.240518/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `ifccsv-0.0.240418/PKG-INFO` & `ifccsv-0.0.240518/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifccsv
-Version: 0.0.240418
+Version: 0.0.240518
 Summary: IFC import and export from CSV, XLSX, ODS, and Pandas Dataframes
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Documentation, https://docs.ifcopenshell.org
 Project-URL: Issues, https://github.com/IfcOpenShell/IfcOpenShell/issues
 Keywords: IFC,CSV,XLS,XLSX,ODS,BIM
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ifccsv-0.0.240418/ifccsv.egg-info/PKG-INFO` & `ifccsv-0.0.240518/ifccsv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifccsv
-Version: 0.0.240418
+Version: 0.0.240518
 Summary: IFC import and export from CSV, XLSX, ODS, and Pandas Dataframes
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Documentation, https://docs.ifcopenshell.org
 Project-URL: Issues, https://github.com/IfcOpenShell/IfcOpenShell/issues
 Keywords: IFC,CSV,XLS,XLSX,ODS,BIM
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ifccsv-0.0.240418/ifccsv.py` & `ifccsv-0.0.240518/ifccsv.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,28 +57,28 @@
     def __init__(self):
         self.headers = []
         self.results = []
         self.dataframe = None
 
     def export(
         self,
-        ifc_file,
-        elements,
+        ifc_file: ifcopenshell.file,
+        elements: ifcopenshell.entity_instance,
         attributes,
         headers=None,
         output=None,
         format=None,
-        should_preserve_existing=False,
-        include_global_id=True,
-        delimiter=",",
-        null="-",
-        empty="",
-        bool_true="YES",
-        bool_false="NO",
-        concat=", ",
+        should_preserve_existing: bool = False,
+        include_global_id: bool = True,
+        delimiter: str = ",",
+        null: str = "-",
+        empty: str = "",
+        bool_true: str = "YES",
+        bool_false: str = "NO",
+        concat: str = ", ",
         sort=None,
         groups=None,
         summaries=None,
         formatting=None,
     ):
         self.ifc_file = ifc_file
         self.results = []
@@ -378,16 +378,24 @@
             if element.is_a("IfcPropertySet"):
                 results.update([p.Name for p in element.HasProperties])
             else:
                 results.update([p.Name for p in element.Quantities])
         return ["{}.{}".format(pset_qto_name, n) for n in results]
 
     def Import(
-        self, ifc_file, table, attributes=None, delimiter=",", null="-", empty="", bool_true="YES", bool_false="NO"
-    ):
+        self,
+        ifc_file: ifcopenshell.file,
+        table: str,
+        attributes: Optional[list[Union[str, None]]] = None,
+        delimiter: str = ",",
+        null: str = "-",
+        empty: str = "",
+        bool_true: str = "YES",
+        bool_false: str = "NO",
+    ) -> None:
         ext = table.split(".")[-1].lower()
 
         if ext == "csv":
             self.import_csv(ifc_file, table, attributes, delimiter, null, empty, bool_true, bool_false)
         elif ext == "ods":
             self.import_ods(ifc_file, table, attributes, null, empty, bool_true, bool_false)
         elif ext == "xlsx":
```

