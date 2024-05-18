# Comparing `tmp/pyclassparser-0.4.tar.gz` & `tmp/pyclassparser-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclassparser-0.4.tar", last modified: Sat May 18 17:36:30 2024, max compression
+gzip compressed data, was "pyclassparser-0.5.tar", last modified: Sat May 18 18:12:27 2024, max compression
```

## Comparing `pyclassparser-0.4.tar` & `pyclassparser-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-18 17:36:30.254212 pyclassparser-0.4/
--rw-r--r--   0 andrei    (1000) andrei    (1000)     1076 2024-05-01 07:44:59.000000 pyclassparser-0.4/LICENSE
--rw-r--r--   0 andrei    (1000) andrei    (1000)     2523 2024-05-18 17:36:30.254212 pyclassparser-0.4/PKG-INFO
--rw-r--r--   0 andrei    (1000) andrei    (1000)     1850 2024-05-18 17:17:20.000000 pyclassparser-0.4/README.md
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-18 17:36:30.250878 pyclassparser-0.4/pyclassparser/
--rw-r--r--   0 andrei    (1000) andrei    (1000)     4728 2024-05-18 17:35:46.000000 pyclassparser-0.4/pyclassparser/__init__.py
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-18 17:36:30.254212 pyclassparser-0.4/pyclassparser.egg-info/
--rw-r--r--   0 andrei    (1000) andrei    (1000)     2523 2024-05-18 17:36:30.000000 pyclassparser-0.4/pyclassparser.egg-info/PKG-INFO
--rw-r--r--   0 andrei    (1000) andrei    (1000)      242 2024-05-18 17:36:30.000000 pyclassparser-0.4/pyclassparser.egg-info/SOURCES.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)        1 2024-05-18 17:36:30.000000 pyclassparser-0.4/pyclassparser.egg-info/dependency_links.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)       34 2024-05-18 17:36:30.000000 pyclassparser-0.4/pyclassparser.egg-info/requires.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)       14 2024-05-18 17:36:30.000000 pyclassparser-0.4/pyclassparser.egg-info/top_level.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)      837 2024-05-18 17:35:57.000000 pyclassparser-0.4/pyproject.toml
--rw-r--r--   0 andrei    (1000) andrei    (1000)       38 2024-05-18 17:36:30.254212 pyclassparser-0.4/setup.cfg
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-18 18:12:27.943748 pyclassparser-0.5/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     1076 2024-05-01 07:44:59.000000 pyclassparser-0.5/LICENSE
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     2523 2024-05-18 18:12:27.943748 pyclassparser-0.5/PKG-INFO
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     1850 2024-05-18 17:17:20.000000 pyclassparser-0.5/README.md
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-18 18:12:27.940415 pyclassparser-0.5/pyclassparser/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     5052 2024-05-18 18:11:09.000000 pyclassparser-0.5/pyclassparser/__init__.py
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2024-05-18 18:12:27.943748 pyclassparser-0.5/pyclassparser.egg-info/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     2523 2024-05-18 18:12:27.000000 pyclassparser-0.5/pyclassparser.egg-info/PKG-INFO
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      242 2024-05-18 18:12:27.000000 pyclassparser-0.5/pyclassparser.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)        1 2024-05-18 18:12:27.000000 pyclassparser-0.5/pyclassparser.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       34 2024-05-18 18:12:27.000000 pyclassparser-0.5/pyclassparser.egg-info/requires.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       14 2024-05-18 18:12:27.000000 pyclassparser-0.5/pyclassparser.egg-info/top_level.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      837 2024-05-18 18:11:48.000000 pyclassparser-0.5/pyproject.toml
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       38 2024-05-18 18:12:27.943748 pyclassparser-0.5/setup.cfg
```

### Comparing `pyclassparser-0.4/LICENSE` & `pyclassparser-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclassparser-0.4/PKG-INFO` & `pyclassparser-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclassparser
-Version: 0.4
+Version: 0.5
 Summary: Parse Python classes and attributes from a string of Python code.
 Author-email: "Carlos A. Planchón" <carlosandresplanchonprestes@gmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/carlosplanchon/pyclassparser.git
 Keywords: pydantic,parser,tool,schemas
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pyclassparser-0.4/README.md` & `pyclassparser-0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyclassparser-0.4/pyclassparser/__init__.py` & `pyclassparser-0.5/pyclassparser/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         validator=type_validator(),
         default=None
     )
     actual_line: Optional[str] = attrs.field(
         validator=type_validator(),
         default=None
     )
-    output: str = attrs.field(
+    parsed_code: str = attrs.field(
         validator=type_validator(),
         default=""
     )
 
     lines: list[str] = attrs.field(
         validator=type_validator(),
         init=False
@@ -104,41 +104,49 @@
     def get_class_attributes(self, class_name: str):
         self.advance()
         first_attr_indentation: int = self.get_indentation_spaces_amt()
         attrs_indentation: int = first_attr_indentation
         # print(f"> ATTRS Indentation: {attrs_indentation}")
         while attrs_indentation == first_attr_indentation:
             # print(self.actual_line)
-            self.output += self.actual_line + "\n"
+            self.parsed_code += self.actual_line + "\n"
 
             if self.actual_line.lstrip(" ").startswith("class") is False:
                 self.add_attr(class_name=class_name)
 
             self.advance()
 
             attrs_indentation: int = self.get_indentation_spaces_amt()
 
     def actual_line_is_class(self) -> bool:
         return self.actual_line.lstrip(" ").startswith("class ")
 
+    def actual_line_is_import(self) -> bool:
+        return self.actual_line.startswith("import ") or\
+            self.actual_line.startswith("from ")
+
     def get_next_class(self):
         if self.actual_line is None:
             self.advance()
 
+        if self.actual_line_is_import() is True:
+            self.parsed_code += self.actual_line.strip("\n ") + "\n"
+            self.advance()
+
         while self.actual_line_is_class() is False:
             self.advance()
 
         if self.actual_line_is_class() is True:
             if self.class_indentation_level is None:
                 self.class_indentation_level = self.get_indentation_spaces_amt()
             else:
                 if self.get_indentation_spaces_amt() == self.class_indentation_level:
                     class_name: str = self.get_class_name()
                     # print(self.actual_line)
-                    self.output += "\n\n" + self.actual_line + "\n"
+                    self.parsed_code += "\n\n" + self.actual_line + "\n"
 
                     # Add class data.
                     if class_name in self.class_data_dict:
                         raise Exception(f"Class name {class_name} already exists.")
 
                     self.class_data_dict[class_name] = []
 
@@ -155,8 +163,8 @@
         while True:
             try:
                 # print(self.actual_line)
                 self.get_next_class()
             except StopIteration:
                 break
 
-        self.output = self.output.strip("\n") + "\n"
+        self.parsed_code = self.parsed_code.strip("\n") + "\n"
```

### Comparing `pyclassparser-0.4/pyclassparser.egg-info/PKG-INFO` & `pyclassparser-0.5/pyclassparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclassparser
-Version: 0.4
+Version: 0.5
 Summary: Parse Python classes and attributes from a string of Python code.
 Author-email: "Carlos A. Planchón" <carlosandresplanchonprestes@gmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/carlosplanchon/pyclassparser.git
 Keywords: pydantic,parser,tool,schemas
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pyclassparser-0.4/pyproject.toml` & `pyclassparser-0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [options]
 package_dir = "pyclassparser"
 packages = ["pyclassparser"]
 
 [project]
 name = "pyclassparser"
-version = "0.4"
+version = "0.5"
 authors = [
     {name = "Carlos A. Planchón", email = "carlosandresplanchonprestes@gmail.com"}
 ]
 description = "Parse Python classes and attributes from a string of Python code."
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
```

