# Comparing `tmp/pyclassparser-0.3.tar.gz` & `tmp/pyclassparser-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclassparser-0.3.tar", last modified: Sat May 18 17:28:54 2024, max compression
+gzip compressed data, was "pyclassparser-0.4.tar", last modified: Sat May 18 17:36:30 2024, max compression
```

## Comparing `pyclassparser-0.3.tar` & `pyclassparser-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-18 17:28:54.815395 pyclassparser-0.3/
--rw-r--r--   0 andrei    (1000) andrei    (1000)     1076 2024-05-01 07:44:59.000000 pyclassparser-0.3/LICENSE
--rw-r--r--   0 andrei    (1000) andrei    (1000)     2523 2024-05-18 17:28:54.815395 pyclassparser-0.3/PKG-INFO
--rw-r--r--   0 andrei    (1000) andrei    (1000)     1850 2024-05-18 17:17:20.000000 pyclassparser-0.3/README.md
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-18 17:28:54.812062 pyclassparser-0.3/pyclassparser/
--rw-r--r--   0 andrei    (1000) andrei    (1000)     4729 2024-05-18 17:28:18.000000 pyclassparser-0.3/pyclassparser/__init__.py
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-18 17:28:54.815395 pyclassparser-0.3/pyclassparser.egg-info/
--rw-r--r--   0 andrei    (1000) andrei    (1000)     2523 2024-05-18 17:28:54.000000 pyclassparser-0.3/pyclassparser.egg-info/PKG-INFO
--rw-r--r--   0 andrei    (1000) andrei    (1000)      242 2024-05-18 17:28:54.000000 pyclassparser-0.3/pyclassparser.egg-info/SOURCES.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)        1 2024-05-18 17:28:54.000000 pyclassparser-0.3/pyclassparser.egg-info/dependency_links.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)       34 2024-05-18 17:28:54.000000 pyclassparser-0.3/pyclassparser.egg-info/requires.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)       14 2024-05-18 17:28:54.000000 pyclassparser-0.3/pyclassparser.egg-info/top_level.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)      837 2024-05-18 17:28:30.000000 pyclassparser-0.3/pyproject.toml
--rw-r--r--   0 andrei    (1000) andrei    (1000)       38 2024-05-18 17:28:54.815395 pyclassparser-0.3/setup.cfg
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-18 17:36:30.254212 pyclassparser-0.4/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     1076 2024-05-01 07:44:59.000000 pyclassparser-0.4/LICENSE
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     2523 2024-05-18 17:36:30.254212 pyclassparser-0.4/PKG-INFO
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     1850 2024-05-18 17:17:20.000000 pyclassparser-0.4/README.md
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-18 17:36:30.250878 pyclassparser-0.4/pyclassparser/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     4728 2024-05-18 17:35:46.000000 pyclassparser-0.4/pyclassparser/__init__.py
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-18 17:36:30.254212 pyclassparser-0.4/pyclassparser.egg-info/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     2523 2024-05-18 17:36:30.000000 pyclassparser-0.4/pyclassparser.egg-info/PKG-INFO
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      242 2024-05-18 17:36:30.000000 pyclassparser-0.4/pyclassparser.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)        1 2024-05-18 17:36:30.000000 pyclassparser-0.4/pyclassparser.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       34 2024-05-18 17:36:30.000000 pyclassparser-0.4/pyclassparser.egg-info/requires.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       14 2024-05-18 17:36:30.000000 pyclassparser-0.4/pyclassparser.egg-info/top_level.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      837 2024-05-18 17:35:57.000000 pyclassparser-0.4/pyproject.toml
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       38 2024-05-18 17:36:30.254212 pyclassparser-0.4/setup.cfg
```

### Comparing `pyclassparser-0.3/LICENSE` & `pyclassparser-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclassparser-0.3/PKG-INFO` & `pyclassparser-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclassparser
-Version: 0.3
+Version: 0.4
 Summary: Parse Python classes and attributes from a string of Python code.
 Author-email: "Carlos A. Planchón" <carlosandresplanchonprestes@gmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/carlosplanchon/pyclassparser.git
 Keywords: pydantic,parser,tool,schemas
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pyclassparser-0.3/README.md` & `pyclassparser-0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyclassparser-0.3/pyclassparser/__init__.py` & `pyclassparser-0.4/pyclassparser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             attr_type = None
 
         attr_value: str = attr_value.strip(" ")
 
         if attr_type is not None:
             attr_type: str = attr_type.strip(" ")
 
-        if attrs_value != "":
+        if attr_value != "":
             class_attr = ClassATTR(
                 attr_value=attr_value,
                 attr_type=attr_type
             )
             self.class_data_dict[class_name].append(class_attr)
 
     def get_class_attributes(self, class_name: str):
```

### Comparing `pyclassparser-0.3/pyclassparser.egg-info/PKG-INFO` & `pyclassparser-0.4/pyclassparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclassparser
-Version: 0.3
+Version: 0.4
 Summary: Parse Python classes and attributes from a string of Python code.
 Author-email: "Carlos A. Planchón" <carlosandresplanchonprestes@gmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/carlosplanchon/pyclassparser.git
 Keywords: pydantic,parser,tool,schemas
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pyclassparser-0.3/pyproject.toml` & `pyclassparser-0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [options]
 package_dir = "pyclassparser"
 packages = ["pyclassparser"]
 
 [project]
 name = "pyclassparser"
-version = "0.3"
+version = "0.4"
 authors = [
     {name = "Carlos A. Planchón", email = "carlosandresplanchonprestes@gmail.com"}
 ]
 description = "Parse Python classes and attributes from a string of Python code."
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
```

