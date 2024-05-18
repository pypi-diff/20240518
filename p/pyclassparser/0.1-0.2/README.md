# Comparing `tmp/pyclassparser-0.1.tar.gz` & `tmp/pyclassparser-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclassparser-0.1.tar", last modified: Fri May 17 03:02:01 2024, max compression
+gzip compressed data, was "pyclassparser-0.2.tar", last modified: Sat May 18 17:17:36 2024, max compression
```

## Comparing `pyclassparser-0.1.tar` & `pyclassparser-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-17 03:02:01.724692 pyclassparser-0.1/
--rw-r--r--   0 andrei    (1000) andrei    (1000)     1076 2024-05-01 07:44:59.000000 pyclassparser-0.1/LICENSE
--rw-r--r--   0 andrei    (1000) andrei    (1000)     2522 2024-05-17 03:02:01.724692 pyclassparser-0.1/PKG-INFO
--rw-r--r--   0 andrei    (1000) andrei    (1000)     1849 2024-05-17 02:58:28.000000 pyclassparser-0.1/README.md
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-17 03:02:01.721359 pyclassparser-0.1/pyclassparser/
--rw-r--r--   0 andrei    (1000) andrei    (1000)     3937 2024-05-17 02:54:48.000000 pyclassparser-0.1/pyclassparser/__init__.py
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-17 03:02:01.724692 pyclassparser-0.1/pyclassparser.egg-info/
--rw-r--r--   0 andrei    (1000) andrei    (1000)     2522 2024-05-17 03:02:01.000000 pyclassparser-0.1/pyclassparser.egg-info/PKG-INFO
--rw-r--r--   0 andrei    (1000) andrei    (1000)      242 2024-05-17 03:02:01.000000 pyclassparser-0.1/pyclassparser.egg-info/SOURCES.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)        1 2024-05-17 03:02:01.000000 pyclassparser-0.1/pyclassparser.egg-info/dependency_links.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)       34 2024-05-17 03:02:01.000000 pyclassparser-0.1/pyclassparser.egg-info/requires.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)       14 2024-05-17 03:02:01.000000 pyclassparser-0.1/pyclassparser.egg-info/top_level.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)      837 2024-05-17 02:59:17.000000 pyclassparser-0.1/pyproject.toml
--rw-r--r--   0 andrei    (1000) andrei    (1000)       38 2024-05-17 03:02:01.724692 pyclassparser-0.1/setup.cfg
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-18 17:17:36.427512 pyclassparser-0.2/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     1076 2024-05-01 07:44:59.000000 pyclassparser-0.2/LICENSE
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     2523 2024-05-18 17:17:36.427512 pyclassparser-0.2/PKG-INFO
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     1850 2024-05-18 17:17:20.000000 pyclassparser-0.2/README.md
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-18 17:17:36.424179 pyclassparser-0.2/pyclassparser/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     4679 2024-05-18 17:15:13.000000 pyclassparser-0.2/pyclassparser/__init__.py
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-18 17:17:36.427512 pyclassparser-0.2/pyclassparser.egg-info/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     2523 2024-05-18 17:17:36.000000 pyclassparser-0.2/pyclassparser.egg-info/PKG-INFO
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      242 2024-05-18 17:17:36.000000 pyclassparser-0.2/pyclassparser.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)        1 2024-05-18 17:17:36.000000 pyclassparser-0.2/pyclassparser.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       34 2024-05-18 17:17:36.000000 pyclassparser-0.2/pyclassparser.egg-info/requires.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       14 2024-05-18 17:17:36.000000 pyclassparser-0.2/pyclassparser.egg-info/top_level.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      837 2024-05-18 17:15:40.000000 pyclassparser-0.2/pyproject.toml
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       38 2024-05-18 17:17:36.427512 pyclassparser-0.2/setup.cfg
```

### Comparing `pyclassparser-0.1/LICENSE` & `pyclassparser-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclassparser-0.1/PKG-INFO` & `pyclassparser-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclassparser
-Version: 0.1
+Version: 0.2
 Summary: Parse Python classes and attributes from a string of Python code.
 Author-email: "Carlos A. Planchón" <carlosandresplanchonprestes@gmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/carlosplanchon/pyclassparser.git
 Keywords: pydantic,parser,tool,schemas
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -15,15 +15,15 @@
 Requires-Dist: attrs>=23.2.0
 Requires-Dist: attrs_strict>=1.0.1
 
 # PyClassParser
 
 `PyClassParser` is a Python library designed to parse Python class definitions and extract class attributes. It uses the `attrs` library for defining class attributes and ensures type safety with `attrs-strict`.
 
-Actually it only supports Pydantic class format.
+Currently it only supports Pydantic class format.
 
 ## Features
 
 - Parses Python class definitions to extract class names and their attributes.
 - Uses `attrs` for attribute definition and `attrs-strict` for type validation.
 - Handles optional attributes and attributes with default values.
```

### Comparing `pyclassparser-0.1/README.md` & `pyclassparser-0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # PyClassParser
 
 `PyClassParser` is a Python library designed to parse Python class definitions and extract class attributes. It uses the `attrs` library for defining class attributes and ensures type safety with `attrs-strict`.
 
-Actually it only supports Pydantic class format.
+Currently it only supports Pydantic class format.
 
 ## Features
 
 - Parses Python class definitions to extract class names and their attributes.
 - Uses `attrs` for attribute definition and `attrs-strict` for type validation.
 - Handles optional attributes and attributes with default values.
```

### Comparing `pyclassparser-0.1/pyclassparser/__init__.py` & `pyclassparser-0.2/pyclassparser/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -37,14 +37,19 @@
     )
 
     lines: list[str] = attrs.field(
         validator=type_validator(),
         init=False
     )
 
+    class_indentation_level: Optional[int] = attrs.field(
+        validator=type_validator(),
+        init=False
+    )
+
     class_data_dict: dict[str, list[ClassATTR]] = attrs.field(
         validator=type_validator(),
         init=False
     )
 
     def __attrs_post_init__(self):
         self.start()
@@ -100,15 +105,16 @@
         first_attr_indentation: int = self.get_indentation_spaces_amt()
         attrs_indentation: int = first_attr_indentation
         # print(f"> ATTRS Indentation: {attrs_indentation}")
         while attrs_indentation == first_attr_indentation:
             # print(self.actual_line)
             self.output += self.actual_line + "\n"
 
-            self.add_attr(class_name=class_name)
+            if self.actual_line.lstrip(" ").startswith("class") is False:
+                self.add_attr(class_name=class_name)
 
             self.advance()
 
             attrs_indentation: int = self.get_indentation_spaces_amt()
 
     def actual_line_is_class(self) -> bool:
         return self.actual_line.lstrip(" ").startswith("class ")
@@ -117,30 +123,39 @@
         if self.actual_line is None:
             self.advance()
 
         while self.actual_line_is_class() is False:
             self.advance()
 
         if self.actual_line_is_class() is True:
-            class_name: str = self.get_class_name()
-            # print(self.actual_line)
-            self.output += "\n\n" + self.actual_line + "\n"
-
-            # Add class data.
-            if class_name in self.class_data_dict:
-                raise Exception(f"Class name {class_name} already exists.")
-
-            self.class_data_dict[class_name] = []
-
-            self.get_class_attributes(class_name=class_name)
+            if self.class_indentation_level is None:
+                self.class_indentation_level = self.get_indentation_spaces_amt()
+            else:
+                if self.get_indentation_spaces_amt() == self.class_indentation_level:
+                    class_name: str = self.get_class_name()
+                    # print(self.actual_line)
+                    self.output += "\n\n" + self.actual_line + "\n"
+
+                    # Add class data.
+                    if class_name in self.class_data_dict:
+                        raise Exception(f"Class name {class_name} already exists.")
+
+                    self.class_data_dict[class_name] = []
+
+                    self.get_class_attributes(class_name=class_name)
+                else:
+                    # print(f"Indentation error: {self.get_indentation_spaces_amt()}")
+                    self.advance()
 
     def start(self):
         self.lines = self.code.split("\n")
         self.class_data_dict: list[list[ClassATTR]] = {}
 
+        self.class_indentation_level: int | None = None
         while True:
             try:
+                # print(self.actual_line)
                 self.get_next_class()
             except StopIteration:
                 break
 
         self.output = self.output.strip("\n") + "\n"
```

### Comparing `pyclassparser-0.1/pyclassparser.egg-info/PKG-INFO` & `pyclassparser-0.2/pyclassparser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclassparser
-Version: 0.1
+Version: 0.2
 Summary: Parse Python classes and attributes from a string of Python code.
 Author-email: "Carlos A. Planchón" <carlosandresplanchonprestes@gmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/carlosplanchon/pyclassparser.git
 Keywords: pydantic,parser,tool,schemas
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -15,15 +15,15 @@
 Requires-Dist: attrs>=23.2.0
 Requires-Dist: attrs_strict>=1.0.1
 
 # PyClassParser
 
 `PyClassParser` is a Python library designed to parse Python class definitions and extract class attributes. It uses the `attrs` library for defining class attributes and ensures type safety with `attrs-strict`.
 
-Actually it only supports Pydantic class format.
+Currently it only supports Pydantic class format.
 
 ## Features
 
 - Parses Python class definitions to extract class names and their attributes.
 - Uses `attrs` for attribute definition and `attrs-strict` for type validation.
 - Handles optional attributes and attributes with default values.
```

### Comparing `pyclassparser-0.1/pyproject.toml` & `pyclassparser-0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [options]
 package_dir = "pyclassparser"
 packages = ["pyclassparser"]
 
 [project]
 name = "pyclassparser"
-version = "0.1"
+version = "0.2"
 authors = [
     {name = "Carlos A. Planchón", email = "carlosandresplanchonprestes@gmail.com"}
 ]
 description = "Parse Python classes and attributes from a string of Python code."
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
```

