# Comparing `tmp/gqlitedb-1.0.0.tar.gz` & `tmp/gqlitedb-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gqlitedb-1.0.0.tar", last modified: Fri Nov 17 20:05:58 2023, max compression
+gzip compressed data, was "gqlitedb-1.1.0.tar", last modified: Sat May 18 19:39:26 2024, max compression
```

## Comparing `gqlitedb-1.0.0.tar` & `gqlitedb-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 cyrille   (1000) cyrille   (1000)        0 2023-11-17 20:05:58.238918 gqlitedb-1.0.0/
--rw-rw-r--   0 cyrille   (1000) cyrille   (1000)       26 2023-11-16 20:32:57.000000 gqlitedb-1.0.0/MANIFEST.in
--rw-rw-r--   0 cyrille   (1000) cyrille   (1000)     2028 2023-11-17 20:05:58.238918 gqlitedb-1.0.0/PKG-INFO
--rwxrwxr-x   0 cyrille   (1000) cyrille   (1000)     1518 2023-11-16 20:32:57.000000 gqlitedb-1.0.0/README.md
--rwxrwxr-x   0 cyrille   (1000) cyrille   (1000)     1710 2023-11-16 20:32:57.000000 gqlitedb-1.0.0/build-ffi.py
-drwxrwxr-x   0 cyrille   (1000) cyrille   (1000)        0 2023-11-17 20:05:58.234917 gqlitedb-1.0.0/gqlite/
--rwxrwxr-x   0 cyrille   (1000) cyrille   (1000)     1350 2023-11-16 20:32:57.000000 gqlitedb-1.0.0/gqlite/__init__.py
-drwxrwxr-x   0 cyrille   (1000) cyrille   (1000)        0 2023-11-17 20:05:58.234917 gqlitedb-1.0.0/gqlitedb.egg-info/
--rw-rw-r--   0 cyrille   (1000) cyrille   (1000)     2028 2023-11-17 20:05:58.000000 gqlitedb-1.0.0/gqlitedb.egg-info/PKG-INFO
--rw-rw-r--   0 cyrille   (1000) cyrille   (1000)      290 2023-11-17 20:05:58.000000 gqlitedb-1.0.0/gqlitedb.egg-info/SOURCES.txt
--rw-rw-r--   0 cyrille   (1000) cyrille   (1000)        1 2023-11-17 20:05:58.000000 gqlitedb-1.0.0/gqlitedb.egg-info/dependency_links.txt
--rw-rw-r--   0 cyrille   (1000) cyrille   (1000)       12 2023-11-17 20:05:58.000000 gqlitedb-1.0.0/gqlitedb.egg-info/requires.txt
--rw-rw-r--   0 cyrille   (1000) cyrille   (1000)       18 2023-11-17 20:05:58.000000 gqlitedb-1.0.0/gqlitedb.egg-info/top_level.txt
--rwxrwxr-x   0 cyrille   (1000) cyrille   (1000)      736 2023-11-16 20:32:57.000000 gqlitedb-1.0.0/pyproject.toml
--rw-rw-r--   0 cyrille   (1000) cyrille   (1000)       38 2023-11-17 20:05:58.238918 gqlitedb-1.0.0/setup.cfg
--rwxrwxr-x   0 cyrille   (1000) cyrille   (1000)      889 2023-11-16 20:32:57.000000 gqlitedb-1.0.0/setup.py
-drwxrwxr-x   0 cyrille   (1000) cyrille   (1000)        0 2023-11-17 20:05:58.238918 gqlitedb-1.0.0/src/
--rw-rw-r--   0 cyrille   (1000) cyrille   (1000)   321885 2023-11-17 18:56:27.000000 gqlitedb-1.0.0/src/gqlite-amalgamate.cpp
--rwxrwxr-x   0 cyrille   (1000) cyrille   (1000)     2656 2023-11-16 20:32:57.000000 gqlitedb-1.0.0/src/gqlite-c.h
--rwxrwxr-x   0 cyrille   (1000) cyrille   (1000)     3725 2023-11-16 20:32:57.000000 gqlitedb-1.0.0/src/gqlite.h
+drwxrwxr-x   0 cyrille   (1000) cyrille   (1000)        0 2024-05-18 19:39:26.820511 gqlitedb-1.1.0/
+-rw-rw-r--   0 cyrille   (1000) cyrille   (1000)       26 2023-11-16 20:32:57.000000 gqlitedb-1.1.0/MANIFEST.in
+-rw-rw-r--   0 cyrille   (1000) cyrille   (1000)     2028 2024-05-18 19:39:26.820511 gqlitedb-1.1.0/PKG-INFO
+-rwxrwxr-x   0 cyrille   (1000) cyrille   (1000)     1518 2023-11-16 20:32:57.000000 gqlitedb-1.1.0/README.md
+-rwxrwxr-x   0 cyrille   (1000) cyrille   (1000)     1710 2023-11-16 20:32:57.000000 gqlitedb-1.1.0/build-ffi.py
+drwxrwxr-x   0 cyrille   (1000) cyrille   (1000)        0 2024-05-18 19:39:26.816511 gqlitedb-1.1.0/gqlite/
+-rwxrwxr-x   0 cyrille   (1000) cyrille   (1000)     1350 2023-11-16 20:32:57.000000 gqlitedb-1.1.0/gqlite/__init__.py
+drwxrwxr-x   0 cyrille   (1000) cyrille   (1000)        0 2024-05-18 19:39:26.816511 gqlitedb-1.1.0/gqlitedb.egg-info/
+-rw-rw-r--   0 cyrille   (1000) cyrille   (1000)     2028 2024-05-18 19:39:26.000000 gqlitedb-1.1.0/gqlitedb.egg-info/PKG-INFO
+-rw-rw-r--   0 cyrille   (1000) cyrille   (1000)      290 2024-05-18 19:39:26.000000 gqlitedb-1.1.0/gqlitedb.egg-info/SOURCES.txt
+-rw-rw-r--   0 cyrille   (1000) cyrille   (1000)        1 2024-05-18 19:39:26.000000 gqlitedb-1.1.0/gqlitedb.egg-info/dependency_links.txt
+-rw-rw-r--   0 cyrille   (1000) cyrille   (1000)       12 2024-05-18 19:39:26.000000 gqlitedb-1.1.0/gqlitedb.egg-info/requires.txt
+-rw-rw-r--   0 cyrille   (1000) cyrille   (1000)       18 2024-05-18 19:39:26.000000 gqlitedb-1.1.0/gqlitedb.egg-info/top_level.txt
+-rwxrwxr-x   0 cyrille   (1000) cyrille   (1000)      736 2024-05-18 17:24:06.000000 gqlitedb-1.1.0/pyproject.toml
+-rw-rw-r--   0 cyrille   (1000) cyrille   (1000)       38 2024-05-18 19:39:26.820511 gqlitedb-1.1.0/setup.cfg
+-rwxrwxr-x   0 cyrille   (1000) cyrille   (1000)      889 2024-05-18 17:23:13.000000 gqlitedb-1.1.0/setup.py
+drwxrwxr-x   0 cyrille   (1000) cyrille   (1000)        0 2024-05-18 19:39:26.820511 gqlitedb-1.1.0/src/
+-rw-rw-r--   0 cyrille   (1000) cyrille   (1000)   332712 2024-05-18 17:11:07.000000 gqlitedb-1.1.0/src/gqlite-amalgamate.cpp
+-rwxrwxr-x   0 cyrille   (1000) cyrille   (1000)     2656 2023-11-16 20:32:57.000000 gqlitedb-1.1.0/src/gqlite-c.h
+-rwxrwxr-x   0 cyrille   (1000) cyrille   (1000)     3725 2023-11-16 20:32:57.000000 gqlitedb-1.1.0/src/gqlite.h
```

### Comparing `gqlitedb-1.0.0/PKG-INFO` & `gqlitedb-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gqlitedb
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python bindings for GQLite, a Graph Query library
 Home-page: https://gitlab.com/gqlite/gqlite
 Author: Cyrille Berger
 Project-URL: Homepage, https://gitlab.com/gqlite/gqlite
 Project-URL: Bug Tracker, https://github.com/gqlite/gqlite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gqlitedb-1.0.0/README.md` & `gqlitedb-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gqlitedb-1.0.0/build-ffi.py` & `gqlitedb-1.1.0/build-ffi.py`

 * *Files identical despite different names*

### Comparing `gqlitedb-1.0.0/gqlite/__init__.py` & `gqlitedb-1.1.0/gqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `gqlitedb-1.0.0/gqlitedb.egg-info/PKG-INFO` & `gqlitedb-1.1.0/gqlitedb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gqlitedb
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python bindings for GQLite, a Graph Query library
 Home-page: https://gitlab.com/gqlite/gqlite
 Author: Cyrille Berger
 Project-URL: Homepage, https://gitlab.com/gqlite/gqlite
 Project-URL: Bug Tracker, https://github.com/gqlite/gqlite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gqlitedb-1.0.0/pyproject.toml` & `gqlitedb-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 host-requires = [
   "pkg:generic/sqlite3",
 ]
 
 [project]
 name = "gqlitedb"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Cyrille Berger" },
 ]
 description = "Python bindings for GQLite, a Graph Query library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `gqlitedb-1.0.0/setup.py` & `gqlitedb-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import setup, find_packages, Extension
 from setuptools.command.build_clib import build_clib
 from distutils.ccompiler import new_compiler
 
 setup(
     name="gqlitedb",
-    version="1.0.0",
+    version="1.1.0",
     description="Python bindings for GQLite, a Graph Query library",
     long_description=open("README.md", "rt").read(),
     url="https://gitlab.com/gqlite/gqlite",
     author="Cyrille Berger",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
```

### Comparing `gqlitedb-1.0.0/src/gqlite-amalgamate.cpp` & `gqlitedb-1.1.0/src/gqlite-amalgamate.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,19 @@
   std::string to_string(const value& _value);
   template<>
   inline std::string to_string<std::string>(const std::string& _v)
   {
     return _v;
   }
   template<>
+  inline std::string to_string<std::string_view>(const std::string_view& _v)
+  {
+    return std::string(_v);
+  }
+  template<>
   inline std::string to_string<const char*>(const char* const& _v)
   {
     return _v;
   }
   template<>
   inline std::string to_string<char>(const char& _v)
   {
@@ -245,15 +250,17 @@
     internal_error, ///< this should never happen
     invalid_json, ///< error that occurs when parsing json
     table_error,
     value_error, ///< generic error that occurs in the value class
     unimplemented_error,
     // OpenCypher error code
     column_name_conflict = 100,
+    delete_connected_node,
     integer_overflow,
+    invalid_aggregation,
     invalid_argument_type,
     invalid_delete,
     invalid_number_literal,
     invalid_number_of_arguments,
     invalid_parameter_use,
     negative_integer_argument,
     non_constant_expression,
@@ -519,20 +526,21 @@
 //BEGIN oc/algebra/expression_info.h
 
 
 namespace gqlite::oc::algebra
 {
   enum class expression_type
   {
-    empty, value, boolean, integer, floating_point, string, map, vector, node, edge, path
+    empty, value, boolean, integer, floating_point, string, map, vector, node, edge, path, all
   };
   struct expression_info
   {
     expression_type type = expression_type::empty;
     bool constant = true;
+    bool aggregation_result;
   };
 }
 //END oc/algebra/expression_info.h
 //BEGIN errors.h
 #include <algorithm>
 
 
@@ -665,14 +673,15 @@
 TOKEN_KEYWORD(IN)
 TOKEN_KEYWORD(IS)
 TOKEN_KEYWORD(LIMIT)
 TOKEN_KEYWORD(NOT)
 TOKEN_KEYWORD(MATCH)
 TOKEN_KEYWORD2(NULL_CAPS, "NULL")
 TOKEN_KEYWORD2(NULL_TOKEN, "null")
+TOKEN_KEYWORD(OPTIONAL)
 TOKEN_KEYWORD(OR)
 TOKEN_KEYWORD(ORDER)
 TOKEN_KEYWORD(REMOVE)
 TOKEN_KEYWORD(RETURN)
 TOKEN_KEYWORD(SET)
 TOKEN_KEYWORD(SKIP)
 TOKEN_KEYWORD(TRUE)
@@ -771,15 +780,16 @@
 #define OC_ALGEBRA_CREATE_NODES_MEMBERS(_KLASS_NAME_, F)                                    \
   F(_KLASS_NAME_, std::vector<alternative<GQLITE_LIST(graph_node, graph_edge)>>, patterns)
 
 OC_ALGEBRA_GENERATE(create, OC_ALGEBRA_CREATE_NODES_MEMBERS)
 
 #define OC_ALGEBRA_MATCH_NODES_MEMBERS(_KLASS_NAME_, F)                                     \
   F(_KLASS_NAME_, std::vector<alternative<GQLITE_LIST(graph_node, graph_edge)>>, patterns)  \
-  F(_KLASS_NAME_, node_csp, where)
+  F(_KLASS_NAME_, node_csp, where)                                                          \
+  F(_KLASS_NAME_, bool, optional)
 
 OC_ALGEBRA_GENERATE(match, OC_ALGEBRA_MATCH_NODES_MEMBERS)
 
 // Statements
 
 #define OC_ALGEBRA_NODES_LIST_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::vector<node_csp>, nodes)
@@ -873,14 +883,15 @@
 OC_ALGEBRA_GENERATE(edit_labels, OC_ALGEBRA_EDIT_LABELS_MEMBERS)
 
 
 // Values
 
 #define OC_ALGEBRA_NO_MEMBERS(_KLASS_NAME_, F)
 
+OC_ALGEBRA_GENERATE(all, OC_ALGEBRA_NO_MEMBERS)
 OC_ALGEBRA_GENERATE(end_of_list, OC_ALGEBRA_NO_MEMBERS)
 
 #define OC_ALGEBRA_GRAPH_NODE_MEMBERS(_KLASS_NAME_, F)          \
   F(_KLASS_NAME_, std::string, variable)                        \
   F(_KLASS_NAME_, std::vector<std::string>, labels)             \
   F(_KLASS_NAME_, node_csp, properties)
 
@@ -897,15 +908,14 @@
 OC_ALGEBRA_GENERATE(graph_edge, OC_ALGEBRA_GRAPH_EDGE_MEMBERS)
 
 #define OC_ALGEBRA_VALUE_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, gqlite::value, value)
 
 OC_ALGEBRA_GENERATE(value, OC_ALGEBRA_VALUE_MEMBERS)
 
-
 #define OC_ALGEBRA_MAP_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::unordered_map<GQLITE_LIST(std::string, node_csp)>, map)
 
 OC_ALGEBRA_GENERATE(map, OC_ALGEBRA_MAP_MEMBERS)
 
 #define OC_ALGEBRA_ARRAY_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::vector<node_csp>, array)
@@ -1129,15 +1139,16 @@
 #define OC_ALGEBRA_CREATE_NODES_MEMBERS(_KLASS_NAME_, F)                                    \
   F(_KLASS_NAME_, std::vector<alternative<GQLITE_LIST(graph_node, graph_edge)>>, patterns)
 
 OC_ALGEBRA_GENERATE(create, OC_ALGEBRA_CREATE_NODES_MEMBERS)
 
 #define OC_ALGEBRA_MATCH_NODES_MEMBERS(_KLASS_NAME_, F)                                     \
   F(_KLASS_NAME_, std::vector<alternative<GQLITE_LIST(graph_node, graph_edge)>>, patterns)  \
-  F(_KLASS_NAME_, node_csp, where)
+  F(_KLASS_NAME_, node_csp, where)                                                          \
+  F(_KLASS_NAME_, bool, optional)
 
 OC_ALGEBRA_GENERATE(match, OC_ALGEBRA_MATCH_NODES_MEMBERS)
 
 // Statements
 
 #define OC_ALGEBRA_NODES_LIST_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::vector<node_csp>, nodes)
@@ -1231,14 +1242,15 @@
 OC_ALGEBRA_GENERATE(edit_labels, OC_ALGEBRA_EDIT_LABELS_MEMBERS)
 
 
 // Values
 
 #define OC_ALGEBRA_NO_MEMBERS(_KLASS_NAME_, F)
 
+OC_ALGEBRA_GENERATE(all, OC_ALGEBRA_NO_MEMBERS)
 OC_ALGEBRA_GENERATE(end_of_list, OC_ALGEBRA_NO_MEMBERS)
 
 #define OC_ALGEBRA_GRAPH_NODE_MEMBERS(_KLASS_NAME_, F)          \
   F(_KLASS_NAME_, std::string, variable)                        \
   F(_KLASS_NAME_, std::vector<std::string>, labels)             \
   F(_KLASS_NAME_, node_csp, properties)
 
@@ -1255,15 +1267,14 @@
 OC_ALGEBRA_GENERATE(graph_edge, OC_ALGEBRA_GRAPH_EDGE_MEMBERS)
 
 #define OC_ALGEBRA_VALUE_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, gqlite::value, value)
 
 OC_ALGEBRA_GENERATE(value, OC_ALGEBRA_VALUE_MEMBERS)
 
-
 #define OC_ALGEBRA_MAP_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::unordered_map<GQLITE_LIST(std::string, node_csp)>, map)
 
 OC_ALGEBRA_GENERATE(map, OC_ALGEBRA_MAP_MEMBERS)
 
 #define OC_ALGEBRA_ARRAY_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::vector<node_csp>, array)
@@ -1372,15 +1383,16 @@
 #define OC_ALGEBRA_CREATE_NODES_MEMBERS(_KLASS_NAME_, F)                                    \
   F(_KLASS_NAME_, std::vector<alternative<GQLITE_LIST(graph_node, graph_edge)>>, patterns)
 
 OC_ALGEBRA_GENERATE(create, OC_ALGEBRA_CREATE_NODES_MEMBERS)
 
 #define OC_ALGEBRA_MATCH_NODES_MEMBERS(_KLASS_NAME_, F)                                     \
   F(_KLASS_NAME_, std::vector<alternative<GQLITE_LIST(graph_node, graph_edge)>>, patterns)  \
-  F(_KLASS_NAME_, node_csp, where)
+  F(_KLASS_NAME_, node_csp, where)                                                          \
+  F(_KLASS_NAME_, bool, optional)
 
 OC_ALGEBRA_GENERATE(match, OC_ALGEBRA_MATCH_NODES_MEMBERS)
 
 // Statements
 
 #define OC_ALGEBRA_NODES_LIST_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::vector<node_csp>, nodes)
@@ -1474,14 +1486,15 @@
 OC_ALGEBRA_GENERATE(edit_labels, OC_ALGEBRA_EDIT_LABELS_MEMBERS)
 
 
 // Values
 
 #define OC_ALGEBRA_NO_MEMBERS(_KLASS_NAME_, F)
 
+OC_ALGEBRA_GENERATE(all, OC_ALGEBRA_NO_MEMBERS)
 OC_ALGEBRA_GENERATE(end_of_list, OC_ALGEBRA_NO_MEMBERS)
 
 #define OC_ALGEBRA_GRAPH_NODE_MEMBERS(_KLASS_NAME_, F)          \
   F(_KLASS_NAME_, std::string, variable)                        \
   F(_KLASS_NAME_, std::vector<std::string>, labels)             \
   F(_KLASS_NAME_, node_csp, properties)
 
@@ -1498,15 +1511,14 @@
 OC_ALGEBRA_GENERATE(graph_edge, OC_ALGEBRA_GRAPH_EDGE_MEMBERS)
 
 #define OC_ALGEBRA_VALUE_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, gqlite::value, value)
 
 OC_ALGEBRA_GENERATE(value, OC_ALGEBRA_VALUE_MEMBERS)
 
-
 #define OC_ALGEBRA_MAP_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::unordered_map<GQLITE_LIST(std::string, node_csp)>, map)
 
 OC_ALGEBRA_GENERATE(map, OC_ALGEBRA_MAP_MEMBERS)
 
 #define OC_ALGEBRA_ARRAY_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::vector<node_csp>, array)
@@ -1614,15 +1626,16 @@
 #define OC_ALGEBRA_CREATE_NODES_MEMBERS(_KLASS_NAME_, F)                                    \
   F(_KLASS_NAME_, std::vector<alternative<GQLITE_LIST(graph_node, graph_edge)>>, patterns)
 
 OC_ALGEBRA_GENERATE(create, OC_ALGEBRA_CREATE_NODES_MEMBERS)
 
 #define OC_ALGEBRA_MATCH_NODES_MEMBERS(_KLASS_NAME_, F)                                     \
   F(_KLASS_NAME_, std::vector<alternative<GQLITE_LIST(graph_node, graph_edge)>>, patterns)  \
-  F(_KLASS_NAME_, node_csp, where)
+  F(_KLASS_NAME_, node_csp, where)                                                          \
+  F(_KLASS_NAME_, bool, optional)
 
 OC_ALGEBRA_GENERATE(match, OC_ALGEBRA_MATCH_NODES_MEMBERS)
 
 // Statements
 
 #define OC_ALGEBRA_NODES_LIST_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::vector<node_csp>, nodes)
@@ -1716,14 +1729,15 @@
 OC_ALGEBRA_GENERATE(edit_labels, OC_ALGEBRA_EDIT_LABELS_MEMBERS)
 
 
 // Values
 
 #define OC_ALGEBRA_NO_MEMBERS(_KLASS_NAME_, F)
 
+OC_ALGEBRA_GENERATE(all, OC_ALGEBRA_NO_MEMBERS)
 OC_ALGEBRA_GENERATE(end_of_list, OC_ALGEBRA_NO_MEMBERS)
 
 #define OC_ALGEBRA_GRAPH_NODE_MEMBERS(_KLASS_NAME_, F)          \
   F(_KLASS_NAME_, std::string, variable)                        \
   F(_KLASS_NAME_, std::vector<std::string>, labels)             \
   F(_KLASS_NAME_, node_csp, properties)
 
@@ -1740,15 +1754,14 @@
 OC_ALGEBRA_GENERATE(graph_edge, OC_ALGEBRA_GRAPH_EDGE_MEMBERS)
 
 #define OC_ALGEBRA_VALUE_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, gqlite::value, value)
 
 OC_ALGEBRA_GENERATE(value, OC_ALGEBRA_VALUE_MEMBERS)
 
-
 #define OC_ALGEBRA_MAP_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::unordered_map<GQLITE_LIST(std::string, node_csp)>, map)
 
 OC_ALGEBRA_GENERATE(map, OC_ALGEBRA_MAP_MEMBERS)
 
 #define OC_ALGEBRA_ARRAY_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::vector<node_csp>, array)
@@ -1873,15 +1886,16 @@
 #define OC_ALGEBRA_CREATE_NODES_MEMBERS(_KLASS_NAME_, F)                                    \
   F(_KLASS_NAME_, std::vector<alternative<GQLITE_LIST(graph_node, graph_edge)>>, patterns)
 
 OC_ALGEBRA_GENERATE(create, OC_ALGEBRA_CREATE_NODES_MEMBERS)
 
 #define OC_ALGEBRA_MATCH_NODES_MEMBERS(_KLASS_NAME_, F)                                     \
   F(_KLASS_NAME_, std::vector<alternative<GQLITE_LIST(graph_node, graph_edge)>>, patterns)  \
-  F(_KLASS_NAME_, node_csp, where)
+  F(_KLASS_NAME_, node_csp, where)                                                          \
+  F(_KLASS_NAME_, bool, optional)
 
 OC_ALGEBRA_GENERATE(match, OC_ALGEBRA_MATCH_NODES_MEMBERS)
 
 // Statements
 
 #define OC_ALGEBRA_NODES_LIST_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::vector<node_csp>, nodes)
@@ -1975,14 +1989,15 @@
 OC_ALGEBRA_GENERATE(edit_labels, OC_ALGEBRA_EDIT_LABELS_MEMBERS)
 
 
 // Values
 
 #define OC_ALGEBRA_NO_MEMBERS(_KLASS_NAME_, F)
 
+OC_ALGEBRA_GENERATE(all, OC_ALGEBRA_NO_MEMBERS)
 OC_ALGEBRA_GENERATE(end_of_list, OC_ALGEBRA_NO_MEMBERS)
 
 #define OC_ALGEBRA_GRAPH_NODE_MEMBERS(_KLASS_NAME_, F)          \
   F(_KLASS_NAME_, std::string, variable)                        \
   F(_KLASS_NAME_, std::vector<std::string>, labels)             \
   F(_KLASS_NAME_, node_csp, properties)
 
@@ -1999,15 +2014,14 @@
 OC_ALGEBRA_GENERATE(graph_edge, OC_ALGEBRA_GRAPH_EDGE_MEMBERS)
 
 #define OC_ALGEBRA_VALUE_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, gqlite::value, value)
 
 OC_ALGEBRA_GENERATE(value, OC_ALGEBRA_VALUE_MEMBERS)
 
-
 #define OC_ALGEBRA_MAP_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::unordered_map<GQLITE_LIST(std::string, node_csp)>, map)
 
 OC_ALGEBRA_GENERATE(map, OC_ALGEBRA_MAP_MEMBERS)
 
 #define OC_ALGEBRA_ARRAY_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::vector<node_csp>, array)
@@ -2133,15 +2147,16 @@
 #define OC_ALGEBRA_CREATE_NODES_MEMBERS(_KLASS_NAME_, F)                                    \
   F(_KLASS_NAME_, std::vector<alternative<GQLITE_LIST(graph_node, graph_edge)>>, patterns)
 
 OC_ALGEBRA_GENERATE(create, OC_ALGEBRA_CREATE_NODES_MEMBERS)
 
 #define OC_ALGEBRA_MATCH_NODES_MEMBERS(_KLASS_NAME_, F)                                     \
   F(_KLASS_NAME_, std::vector<alternative<GQLITE_LIST(graph_node, graph_edge)>>, patterns)  \
-  F(_KLASS_NAME_, node_csp, where)
+  F(_KLASS_NAME_, node_csp, where)                                                          \
+  F(_KLASS_NAME_, bool, optional)
 
 OC_ALGEBRA_GENERATE(match, OC_ALGEBRA_MATCH_NODES_MEMBERS)
 
 // Statements
 
 #define OC_ALGEBRA_NODES_LIST_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::vector<node_csp>, nodes)
@@ -2235,14 +2250,15 @@
 OC_ALGEBRA_GENERATE(edit_labels, OC_ALGEBRA_EDIT_LABELS_MEMBERS)
 
 
 // Values
 
 #define OC_ALGEBRA_NO_MEMBERS(_KLASS_NAME_, F)
 
+OC_ALGEBRA_GENERATE(all, OC_ALGEBRA_NO_MEMBERS)
 OC_ALGEBRA_GENERATE(end_of_list, OC_ALGEBRA_NO_MEMBERS)
 
 #define OC_ALGEBRA_GRAPH_NODE_MEMBERS(_KLASS_NAME_, F)          \
   F(_KLASS_NAME_, std::string, variable)                        \
   F(_KLASS_NAME_, std::vector<std::string>, labels)             \
   F(_KLASS_NAME_, node_csp, properties)
 
@@ -2259,15 +2275,14 @@
 OC_ALGEBRA_GENERATE(graph_edge, OC_ALGEBRA_GRAPH_EDGE_MEMBERS)
 
 #define OC_ALGEBRA_VALUE_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, gqlite::value, value)
 
 OC_ALGEBRA_GENERATE(value, OC_ALGEBRA_VALUE_MEMBERS)
 
-
 #define OC_ALGEBRA_MAP_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::unordered_map<GQLITE_LIST(std::string, node_csp)>, map)
 
 OC_ALGEBRA_GENERATE(map, OC_ALGEBRA_MAP_MEMBERS)
 
 #define OC_ALGEBRA_ARRAY_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::vector<node_csp>, array)
@@ -2396,15 +2411,16 @@
 #define OC_ALGEBRA_CREATE_NODES_MEMBERS(_KLASS_NAME_, F)                                    \
   F(_KLASS_NAME_, std::vector<alternative<GQLITE_LIST(graph_node, graph_edge)>>, patterns)
 
 OC_ALGEBRA_GENERATE(create, OC_ALGEBRA_CREATE_NODES_MEMBERS)
 
 #define OC_ALGEBRA_MATCH_NODES_MEMBERS(_KLASS_NAME_, F)                                     \
   F(_KLASS_NAME_, std::vector<alternative<GQLITE_LIST(graph_node, graph_edge)>>, patterns)  \
-  F(_KLASS_NAME_, node_csp, where)
+  F(_KLASS_NAME_, node_csp, where)                                                          \
+  F(_KLASS_NAME_, bool, optional)
 
 OC_ALGEBRA_GENERATE(match, OC_ALGEBRA_MATCH_NODES_MEMBERS)
 
 // Statements
 
 #define OC_ALGEBRA_NODES_LIST_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::vector<node_csp>, nodes)
@@ -2498,14 +2514,15 @@
 OC_ALGEBRA_GENERATE(edit_labels, OC_ALGEBRA_EDIT_LABELS_MEMBERS)
 
 
 // Values
 
 #define OC_ALGEBRA_NO_MEMBERS(_KLASS_NAME_, F)
 
+OC_ALGEBRA_GENERATE(all, OC_ALGEBRA_NO_MEMBERS)
 OC_ALGEBRA_GENERATE(end_of_list, OC_ALGEBRA_NO_MEMBERS)
 
 #define OC_ALGEBRA_GRAPH_NODE_MEMBERS(_KLASS_NAME_, F)          \
   F(_KLASS_NAME_, std::string, variable)                        \
   F(_KLASS_NAME_, std::vector<std::string>, labels)             \
   F(_KLASS_NAME_, node_csp, properties)
 
@@ -2522,15 +2539,14 @@
 OC_ALGEBRA_GENERATE(graph_edge, OC_ALGEBRA_GRAPH_EDGE_MEMBERS)
 
 #define OC_ALGEBRA_VALUE_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, gqlite::value, value)
 
 OC_ALGEBRA_GENERATE(value, OC_ALGEBRA_VALUE_MEMBERS)
 
-
 #define OC_ALGEBRA_MAP_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::unordered_map<GQLITE_LIST(std::string, node_csp)>, map)
 
 OC_ALGEBRA_GENERATE(map, OC_ALGEBRA_MAP_MEMBERS)
 
 #define OC_ALGEBRA_ARRAY_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::vector<node_csp>, array)
@@ -2635,27 +2651,27 @@
       throw_exception(stage, exception_code::unimplemented_error, "Unimplemented node {} in expression_analyser visitor", oc::algebra::node_type_name(_node->get_type()));
     }
     expression_info visit(algebra::value_csp _var) override
     {
       switch(_var->get_value().get_type())
       {
         case value_type::invalid:
-          return {expression_type::empty, true };
+          return {expression_type::empty, true, false};
         case value_type::boolean:
-          return {expression_type::boolean, true };
+          return {expression_type::boolean, true, false};
         case value_type::integer:
-          return {expression_type::integer, true };
+          return {expression_type::integer, true , false};
         case value_type::floating_point:
-          return {expression_type::floating_point, true };
+          return {expression_type::floating_point, true, false};
         case value_type::string:
-          return {expression_type::string, true };
+          return {expression_type::string, true, false};
         case value_type::map:
-          return {expression_type::map, true };
+          return {expression_type::map, true, false};
         case value_type::vector:
-          return {expression_type::vector, true };
+          return {expression_type::vector, true, false};
       };
       throw_exception(exception_stage::unspecified, exception_code::internal_error, "Unknown value type.");
     }
     template<typename _T_>
     bool constant_nodes(const _T_& _nodes)
     {
       for(algebra::node_csp n : _nodes)
@@ -2663,134 +2679,177 @@
         if(not start(n).constant)
         {
           return false;
         }
       }
       return true;
     }
+    template<typename _T_>
+    bool aggregation_result_nodes(const _T_& _nodes)
+    {
+      for(algebra::node_csp n : _nodes)
+      {
+        if(start(n).aggregation_result)
+        {
+          return true;
+        }
+      }
+      return false;
+    }
     expression_info visit(algebra::array_csp _value) override
     {
-      return {expression_type::vector, constant_nodes(_value->get_array())};
+      return {expression_type::vector, constant_nodes(_value->get_array()), aggregation_result_nodes(_value->get_array())};
     }
     expression_info visit(algebra::map_csp _value) override
     {
-      return {expression_type::map, constant_nodes(workarounds::views::values(_value->get_map()))};
+      return {expression_type::map, constant_nodes(workarounds::views::values(_value->get_map())), aggregation_result_nodes(workarounds::views::values(_value->get_map()))};
     }
     expression_info visit(algebra::member_access_csp _ma) override
     {
-      return {expression_type::value, start(_ma->get_left()).constant};
+      return {expression_type::value, start(_ma->get_left()).constant, false};
+    }
+    expression_info visit(algebra::all_csp) override
+    {
+      return {expression_type::all, false, false};
     }
     expression_info visit(algebra::indexed_access_csp _ia) override
     {
-      return {expression_type::value, start(_ia->get_left()).constant};
+      return {expression_type::value, start(_ia->get_left()).constant, false};
     }
     expression_info visit(algebra::has_labels_csp) override
     {
-      return {expression_type::boolean, false};
+      return {expression_type::boolean, false, false};
     }
-#define GQLITE_ET_LOGICAL_OP(_NAME_)                              \
-    expression_info visit(algebra::_NAME_ ## _csp _node) override \
-    {                                                             \
-      bool constant = start(_node->get_left()).constant           \
-                  and start(_node->get_right()).constant;         \
-      return {expression_type::boolean, constant};                \
+#define GQLITE_ET_LOGICAL_OP(_NAME_)                                                  \
+    expression_info visit(algebra::_NAME_ ## _csp _node) override                     \
+    {                                                                                 \
+      expression_info left = start(_node->get_left());                                \
+      expression_info right = start(_node->get_right());                              \
+      bool constant = left.constant and right.constant;                               \
+      bool aggregation_result = left.aggregation_result or right.aggregation_result;  \
+      return {expression_type::boolean, constant, aggregation_result};                \
     }
     GQLITE_ET_LOGICAL_OP(logical_and)
     GQLITE_ET_LOGICAL_OP(logical_or)
     GQLITE_ET_LOGICAL_OP(logical_xor)
     GQLITE_ET_LOGICAL_OP(relational_equal)
     GQLITE_ET_LOGICAL_OP(relational_different)
     GQLITE_ET_LOGICAL_OP(relational_inferior)
     GQLITE_ET_LOGICAL_OP(relational_superior)
     GQLITE_ET_LOGICAL_OP(relational_inferior_equal)
     GQLITE_ET_LOGICAL_OP(relational_superior_equal)
     GQLITE_ET_LOGICAL_OP(relational_in)
     GQLITE_ET_LOGICAL_OP(relational_not_in)
-#define GQLITE_ET_LOGICAL_UNARY_OP(_NAME_)                          \
-    expression_info visit(algebra::_NAME_ ## _csp _node) override   \
-    {                                                               \
-      bool constant = start(_node->get_value()).constant;           \
-      return {expression_type::boolean, constant};                  \
+#define GQLITE_ET_LOGICAL_UNARY_OP(_NAME_)                                        \
+    expression_info visit(algebra::_NAME_ ## _csp _node) override                 \
+    {                                                                             \
+      expression_info info = start(_node->get_value());                           \
+      return {expression_type::boolean, info.constant, info.aggregation_result};  \
     }
     GQLITE_ET_LOGICAL_UNARY_OP(is_null)
     GQLITE_ET_LOGICAL_UNARY_OP(is_not_null)
 #define GQLITE_ET_BINARY_OP(_NAME_)                                                                       \
     expression_info visit(algebra::_NAME_ ## _csp _node) override                                         \
     {                                                                                                     \
       expression_info left = start(_node->get_left());                                                    \
       expression_info right = start(_node->get_right());                                                  \
       bool constant = left.constant and right.constant;                                                   \
-      if(left.type == right.type) return {left.type, constant};                                           \
+      bool aggregation_result = left.aggregation_result or right.aggregation_result;                      \
+      if(left.type == right.type) return {left.type, constant, aggregation_result};                       \
       if(left.type == expression_type::value or right.type == expression_type::value)                     \
-        return {expression_type::value, constant};                                                        \
+        return {expression_type::value, constant, aggregation_result};                                    \
       if(left.type == expression_type::floating_point or right.type == expression_type::floating_point)   \
       {                                                                                                   \
-        return {expression_type::floating_point, constant};                                               \
+        return {expression_type::floating_point, constant, aggregation_result};                           \
       }                                                                                                   \
       if(left.type == expression_type::string or right.type == expression_type::string)                   \
       {                                                                                                   \
-        return {expression_type::string, constant};                                                       \
+        return {expression_type::string, constant, aggregation_result};                                   \
       }                                                                                                   \
       if(std::is_same_v<algebra::_NAME_ ## _csp, algebra::addition_csp>                                   \
             and left.type == expression_type::vector)                                                     \
       {                                                                                                   \
-        return {expression_type::vector, constant};                                                       \
+        return {expression_type::vector, constant, aggregation_result};                                   \
       }                                                                                                   \
       errors::invalid_argument_type(stage, "In binary operation.");                                       \
     }
     GQLITE_ET_BINARY_OP(addition)
     GQLITE_ET_BINARY_OP(substraction)
     GQLITE_ET_BINARY_OP(multiplication)
     GQLITE_ET_BINARY_OP(division)
     GQLITE_ET_BINARY_OP(modulo)
 
     expression_info visit(algebra::logical_negation_csp _node)
     {
-      bool constant = start(_node->get_value()).constant;
-      return {expression_type::boolean, constant};
+      expression_info ei = start(_node->get_value());
+      return {expression_type::boolean, ei.constant, ei.aggregation_result};
     }
     expression_info visit(algebra::variable_csp _var) override
     {
-      return {variables_f(_var->get_identifier()), false};
+      return {variables_f(_var->get_identifier()), false, false};
     }
     struct function_info
     {
       expression_type return_type;
       std::vector<expression_type> arguments_types;
       bool deterministic;
+      bool aggregation;
     };
     static std::unordered_multimap<std::string, function_info> create_functions()
     {
       std::unordered_multimap<std::string, function_info> f;
       using enum expression_type;
       using FI = function_info;
       using V = std::vector<expression_type>;
-      f.emplace("head", FI{value, V{vector}, true});
-      f.emplace("id", FI{integer, V{node}, true});
-      f.emplace("id", FI{integer, V{edge}, true});
-      f.emplace("keys", FI{vector, V{edge}, true});
-      f.emplace("keys", FI{vector, V{node}, true});
-      f.emplace("keys", FI{vector, V{map}, true});
-      f.emplace("labels", FI{vector, V{node}, true});
-      f.emplace("properties", FI{map, V{node}, true});
-      f.emplace("properties", FI{map, V{edge}, true});
-      f.emplace("properties", FI{map, V{map}, true});
-      f.emplace("range", FI{string, V{integer, integer}, true});
-      f.emplace("size", FI{integer, V{vector}, true});
-      f.emplace("tail", FI{vector, V{vector}, true});
-      f.emplace("toInteger", FI{integer, V{integer}, true});
-      f.emplace("toInteger", FI{integer, V{floating_point}, true});
-      f.emplace("type", FI{string, V{edge}, true});
+      f.emplace("head", FI{value, V{vector}, true, false});
+      f.emplace("id", FI{integer, V{node}, true, false});
+      f.emplace("id", FI{integer, V{edge}, true, false});
+      f.emplace("keys", FI{vector, V{edge}, true, false});
+      f.emplace("keys", FI{vector, V{node}, true, false});
+      f.emplace("keys", FI{vector, V{map}, true, false});
+      f.emplace("labels", FI{vector, V{node}, true, false});
+      f.emplace("properties", FI{map, V{node}, true, false});
+      f.emplace("properties", FI{map, V{edge}, true, false});
+      f.emplace("properties", FI{map, V{map}, true, false});
+      f.emplace("range", FI{string, V{integer, integer}, true, false});
+      f.emplace("size", FI{integer, V{vector}, true, false});
+      f.emplace("tail", FI{vector, V{vector}, true, false});
+      f.emplace("toInteger", FI{integer, V{integer}, true, false});
+      f.emplace("toInteger", FI{integer, V{floating_point}, true, false});
+      f.emplace("type", FI{string, V{edge}, true, false});
+      // aggregations
+      f.emplace("avg", FI{integer, V{value}, true, true});
+      f.emplace("count", FI{integer, V{value}, true, true});
+      f.emplace("count", FI{integer, V{all}, true, true});
+      f.emplace("collect", FI{vector, V{value}, true, true});
+      f.emplace("max", FI{value, V{value}, true, true});
+      f.emplace("min", FI{value, V{value}, true, true});
+      f.emplace("sum", FI{value, V{value}, true, true});
       return f;
     }
     expression_info visit(algebra::function_call_csp _node) override
     {
       if(_node->get_name() == "coalesce")
       { // coalesce is a special case that can accept any value
-        return {expression_type::value, constant_nodes(_node->get_arguments())};
+        expression_type et = expression_type::empty;
+        bool first = true;
+        for(const algebra::node_csp& n : _node->get_arguments())
+        {
+          expression_info ei = start(n);
+          if(first)
+          {
+            first = false;
+            et = ei.type;
+          } else if(et != ei.type)
+          {
+            et = expression_type::value;
+            break;
+          }
+        }
+        return {et, constant_nodes(_node->get_arguments()), aggregation_result_nodes(_node->get_arguments())};
       }
       // 1) Check if all arguments are constant and get their type
       bool constant_arguments = true;
       std::vector<expression_type> argument_types;
       for(algebra::node_csp arg : _node->get_arguments())
       {
         expression_info arg_ei = start(arg);
@@ -2811,15 +2870,15 @@
             expression_type f_type = it->second.arguments_types[i];
             if(arg_type != f_type and arg_type != expression_type::value and f_type != expression_type::value and arg_type != expression_type::empty)
             {
               match = false;
             }
             break;
           }
-          if(match) return {it->second.return_type, it->second.deterministic and constant_arguments};
+          if(match) return {it->second.return_type, it->second.deterministic and constant_arguments, it->second.aggregation};
         }
       }
       // 3) If no function was found, return an exception for unknown function or invalid arguments
       if(it_functions.first == it_functions.second)
       {
         throw_exception(stage, exception_code::unknown_function, "Function {} is unknown.", _node->get_name());
       } else {
@@ -2873,14 +2932,18 @@
     {
       throw_exception(exception_stage::unspecified, exception_code::unimplemented_error, "Unimplemented node {} in stringify", oc::algebra::node_type_name(_node->get_type()));
     }
     std::string visit(algebra::value_csp _var) override
     {
       return _var->get_value().to_json();
     }
+    std::string visit(algebra::all_csp) override
+    {
+      return "*";
+    }
      std::string visit(algebra::array_csp _var) override
     {
       std::string r = "[";
       bool first = true;
       for(algebra::node_csp n : _var->get_array())
       {
         if(not first) r += ", ";
@@ -2918,17 +2981,24 @@
     GQLITE_STRINGIFY_BIN_OP(logical_or, OR)
     GQLITE_STRINGIFY_BIN_OP(logical_xor, XOR)
     GQLITE_STRINGIFY_BIN_OP(relational_in, IN)
     GQLITE_STRINGIFY_BIN_OP(relational_not_in, NOT IN)
 #define GQLITE_STRINGIFY_UNARY_OP(_NAME_, _OP_)                                   \
     std::string visit(algebra::_NAME_ ## _csp _var) override                      \
     {                                                                             \
-      return # _OP_ " " + start(_var->get_value());                                 \
+      return # _OP_ " " + start(_var->get_value());                               \
     }
     GQLITE_STRINGIFY_UNARY_OP(logical_negation, NOT)
+#define GQLITE_STRINGIFY_UNARY_END_OP(_NAME_, _OP_)                               \
+    std::string visit(algebra::_NAME_ ## _csp _var) override                      \
+    {                                                                             \
+      return start(_var->get_value()) + " " # _OP_;                               \
+    }
+    GQLITE_STRINGIFY_UNARY_END_OP(is_null, IS NULL)
+    GQLITE_STRINGIFY_UNARY_END_OP(is_not_null, IS NOT NULL)
     std::string visit(algebra::variable_csp _var) override
     {
       return _var->get_identifier();
     }
     std::string visit(algebra::function_call_csp _var) override
     {
       std::string args;
@@ -3006,23 +3076,28 @@
 
 stream << " WHERE tblu.id = ";
 
 stream << ( _edge_id );
 
     return stream.str();
   }
-  inline std::string edge_count_by_node(const std::string& _graph_name)
+  inline std::string edge_count_by_nodes(const std::string& _graph_name, const std::string& _what)
   {
     std::stringstream stream;
     
-stream << "SELECT count(*) FROM gqlite_";
+stream << "WITH source_delete AS NOT MATERIALIZED (";
+
+stream << ( _what );
+
+stream << ")\n"
+"SELECT count(*) FROM gqlite_";
 
 stream << ( _graph_name );
 
-stream << "_edges WHERE left=?001 or right=?001";
+stream << "_edges WHERE left IN source_delete or right IN source_delete";
 
     return stream.str();
   }
   inline std::string edge_create(const std::string& _graph_name, const std::string& _values)
   {
     std::stringstream stream;
     
@@ -3052,15 +3127,15 @@
 
 stream << ( _what );
 
 stream << ")";
 
     return stream.str();
   }
-  inline std::string edge_delete_by_node(const std::string& _graph_name, const std::string& _what)
+  inline std::string edge_delete_by_nodes(const std::string& _graph_name, const std::string& _what)
   {
     std::stringstream stream;
     
 stream << "WITH source_delete AS NOT MATERIALIZED (";
 
 stream << ( _what );
 
@@ -3133,25 +3208,33 @@
 
     return stream.str();
   }
   inline std::string function_labels(const std::string& _graph_name, const std::string& _node_id)
   {
     std::stringstream stream;
     
-stream << "(SELECT json_group_array(labels.label)\n"
-"            FROM gqlite_";
+stream << "(CASE WHEN ";
+
+stream << ( _node_id );
+
+stream << " IS NULL\n"
+"  THEN NULL\n"
+"  ELSE\n"
+"    (SELECT json_group_array(labels.label)\n"
+"                FROM gqlite_";
 
 stream << ( _graph_name );
 
 stream << "_labels as l\n"
-"            JOIN gqlite_labels AS labels ON labels.id = l.label WHERE l.node_id = ";
+"                JOIN gqlite_labels AS labels ON labels.id = l.label WHERE l.node_id = ";
 
 stream << ( _node_id );
 
 stream << ")\n"
+"  END)\n"
 "";
 
     return stream.str();
   }
   inline std::string get_debug_stats(const std::string& _graph_name)
   {
     std::stringstream stream;
@@ -3182,15 +3265,30 @@
 
 stream << "_edges t, json_each(properties) j\n"
 "UNION ALL SELECT COUNT(*) FROM gqlite_labels\n"
 "UNION ALL SELECT COUNT(DISTINCT label) FROM gqlite_";
 
 stream << ( _graph_name );
 
-stream << "_labels";
+stream << "_labels\n"
+"UNION ALL SELECT COUNT(DISTINCT label) FROM (SELECT label FROM gqlite_";
+
+stream << ( _graph_name );
+
+stream << "_edges UNION SELECT label FROM gqlite_";
+
+stream << ( _graph_name );
+
+stream << "_labels)\n"
+"UNION ALL SELECT COUNT(DISTINCT label) FROM gqlite_";
+
+stream << ( _graph_name );
+
+stream << "_labels\n"
+"";
 
     return stream.str();
   }
   inline std::string graph_create(const std::string& _graph_name)
   {
     std::stringstream stream;
     
@@ -3265,15 +3363,16 @@
 stream << "_nodes n\n"
 "            LEFT JOIN gqlite_";
 
 stream << ( _graph_name );
 
 stream << "_labels as l ON l.node_id = n.id\n"
 "            LEFT JOIN gqlite_labels AS labels ON labels.id = l.label\n"
-"            GROUP BY n.id);\n"
+"            GROUP BY n.id)\n"
+"        UNION SELECT NULL, NULL;\n"
 "\n"
 "CREATE VIEW gqlite_";
 
 stream << ( _graph_name );
 
 stream << "_edges_as_json (id, edge) AS\n"
 "        SELECT e.id, json_object('id', e.id, 'properties', json(e.properties), \n"
@@ -3281,15 +3380,15 @@
 "          'type', 'edge') FROM\n"
 "          gqlite_";
 
 stream << ( _graph_name );
 
 stream << "_edges e\n"
 "          JOIN gqlite_labels label ON label.id = e.label\n"
-"\n"
+"        UNION SELECT NULL, NULL\n"
 "";
 
     return stream.str();
   }
   inline std::string graph_has(const std::string& _graph_name)
   {
     std::stringstream stream;
@@ -3351,15 +3450,15 @@
   {
     std::stringstream stream;
     
 stream << "INSERT INTO gqlite_";
 
 stream << ( _graph_name );
 
-stream << "_labels(label, node_id)  SELECT label.value, node.value FROM json_each(?001) label  JOIN json_each(?002) node";
+stream << "_labels(label, node_id)  SELECT label.value, node.value FROM json_each(?001) label  JOIN json_each(?002) node WHERE node.value IS NOT NULL";
 
     return stream.str();
   }
   inline std::string node_add_labels(const std::string& _graph_name, const std::string& _what)
   {
     std::stringstream stream;
     
@@ -3662,14 +3761,19 @@
 connection connection::create_from_sqlite_file(const std::string& _filename, const gqlite::value&)
 {
   return connection(backends::sqlite::from_file(_filename));
 }
 
 value connection::execute_oc_query(const std::string& _string, const value_map& _bindings)
 {
+#if 0
+  std::cout << "============= execute_oc_query =============\n"
+            << _string <<
+             "\n============================================" << std::endl;
+#endif
   std::stringstream ss(_string);
   oc::lexer l(&ss);
   oc::parser parser(&l, _bindings);
   oc::algebra::node_csp node = parser.parse();
   return d->backend_->execute_oc_query(node);
 }
 //END connection.cpp
@@ -3792,16 +3896,20 @@
         d->full_error += "TableError: "; break;
       case value_error:
         d->full_error += "ValueError: "; break;
       case unimplemented_error:
         d->full_error += "UnimplementedError: "; break;
       case column_name_conflict:
         d->full_error += "ColumnNameConflict: "; break;
+      case delete_connected_node:
+        d->full_error += "DeleteConnectedNode: "; break;
       case integer_overflow:
         d->full_error += "IntegerOverflow: "; break;
+      case invalid_aggregation:
+        d->full_error += "InvalidAggregation: "; break;
       case invalid_argument_type:
         d->full_error += "InvalidArgumentType: "; break;
       case invalid_delete:
         d->full_error += "InvalidDelete: "; break;
       case invalid_number_literal:
         d->full_error += "InvalidNumberLiteral: "; break;
       case invalid_number_of_arguments:
@@ -4565,14 +4673,15 @@
 TOKEN_KEYWORD(IN)
 TOKEN_KEYWORD(IS)
 TOKEN_KEYWORD(LIMIT)
 TOKEN_KEYWORD(NOT)
 TOKEN_KEYWORD(MATCH)
 TOKEN_KEYWORD2(NULL_CAPS, "NULL")
 TOKEN_KEYWORD2(NULL_TOKEN, "null")
+TOKEN_KEYWORD(OPTIONAL)
 TOKEN_KEYWORD(OR)
 TOKEN_KEYWORD(ORDER)
 TOKEN_KEYWORD(REMOVE)
 TOKEN_KEYWORD(RETURN)
 TOKEN_KEYWORD(SET)
 TOKEN_KEYWORD(SKIP)
 TOKEN_KEYWORD(TRUE)
@@ -4802,22 +4911,22 @@
     algebra::expression_type type;
   };
   std::unordered_map<std::string, variable_info> bounded_variables;
   algebra::visitors::expression_analyser expression_analyser;
   int id = 0;
   algebra::node_csp parse_call();
   algebra::node_csp parse_create();
-  algebra::node_csp parse_match();
+  algebra::node_csp parse_match(bool _optional);
   algebra::node_csp parse_return();
   algebra::node_csp parse_with();
   algebra::node_csp parse_unwind();
   algebra::node_csp parse_delete();
   algebra::node_csp parse_set();
   algebra::node_csp parse_remove();
-  algebra::modifiers_csp parse_modifiers();
+  algebra::modifiers_csp parse_modifiers(const std::vector<algebra::named_expression_csp>& _expressions);
   std::vector<algebra::alternative<algebra::graph_node, algebra::graph_edge>> parse_patterns(bool _creation_mode);
   algebra::node_csp parse_map();
   algebra::node_csp parse_properties();
   algebra::node_csp parse_expression();
   algebra::node_csp parse_unary_expression();
   algebra::node_csp parse_multiplicative_expression();
   algebra::node_csp parse_additive_expression();
@@ -4989,25 +5098,29 @@
 
 algebra::node_csp parser::data::parse_create()
 {
   get_next_token();
   return std::make_shared<algebra::create>(parse_patterns(true));
 }
 
-algebra::node_csp parser::data::parse_match()
+algebra::node_csp parser::data::parse_match(bool _optional)
 {
   get_next_token();
   std::vector<algebra::alternative<algebra::graph_node, algebra::graph_edge>> patterns = parse_patterns(false);
   algebra::node_csp where;
   if(tok.type == token_type::WHERE)
   {
     get_next_token();
     where = parse_expression();
+    if(expression_analyser.start(where).aggregation_result)
+    {
+      report_error(tok, exception_code::invalid_aggregation, "in where expression.");
+    }
   }
-  return std::make_shared<algebra::match>(patterns, where);
+  return std::make_shared<algebra::match>(patterns, where, _optional);
 }
 
 std::vector<algebra::named_expression_csp> parser::data::parse_named_expressions()
 {
   std::vector<algebra::named_expression_csp> expressions;
   std::vector<std::string> labels;
   do
@@ -5046,15 +5159,15 @@
 
 algebra::node_csp parser::data::parse_with()
 {
   get_next_token();
   if(tok.type == token_type::STAR)
   {
     get_next_token();
-    return std::make_shared<algebra::with>(true, std::vector<algebra::named_expression_csp>(), parse_modifiers());
+    return std::make_shared<algebra::with>(true, std::vector<algebra::named_expression_csp>(), parse_modifiers({}));
   }
   std::vector<algebra::named_expression_csp> named_expressions = parse_named_expressions();
   std::vector<std::string> new_variables;
   for(algebra::named_expression_csp ne : named_expressions)
   {
     new_variables.push_back(ne->get_name());
     bind_variable(ne->get_name(), ne->get_expression(), expression_analyser.start(ne->get_expression()).type, true);
@@ -5064,16 +5177,16 @@
     if(std::find(new_variables.begin(), new_variables.end(), it->first) == new_variables.end())
     {
       it = bounded_variables.erase(it);
     } else {
       ++it;
     }
   }
-  gqlite_debug("With new variables {} kept variables {}", new_variables, std::views::keys(bounded_variables));
-  return std::make_shared<algebra::with>(false, named_expressions, parse_modifiers());
+  // gqlite_debug("With new variables {} kept variables {}", new_variables, std::views::keys(bounded_variables));
+  return std::make_shared<algebra::with>(false, named_expressions, parse_modifiers(named_expressions));
 }
 
 algebra::node_csp parser::data::parse_unwind()
 {
   get_next_token();
   algebra::node_csp expr = parse_expression();
   is_of_type(token_type::AS);
@@ -5234,22 +5347,22 @@
 
 algebra::node_csp parser::data::parse_return()
 {
   get_next_token();
   if(tok.type == token_type::STAR)
   {
     get_next_token();
-    return std::make_shared<algebra::return_statement>(true, std::vector<algebra::named_expression_csp>(), parse_modifiers());
+    return std::make_shared<algebra::return_statement>(true, std::vector<algebra::named_expression_csp>(), parse_modifiers({}));
   }
   std::vector<algebra::named_expression_csp> named_expressions = parse_named_expressions();
   for(algebra::named_expression_csp ne : named_expressions)
   {
     bind_variable(ne->get_name(), ne->get_expression(), expression_analyser.start(ne->get_expression()).type, true);
   }
-  return std::make_shared<algebra::return_statement>(false, named_expressions, parse_modifiers());
+  return std::make_shared<algebra::return_statement>(false, named_expressions, parse_modifiers(named_expressions));
 }
 
 namespace
 {
   struct edge
   {
     bool active = false;
@@ -5257,15 +5370,15 @@
     algebra::graph_node_csp source, destination;
     std::string variable;
     std::vector<std::string> labels;
     algebra::node_csp properties;
   };
 }
 
-algebra::modifiers_csp parser::data::parse_modifiers()
+algebra::modifiers_csp parser::data::parse_modifiers(const std::vector<algebra::named_expression_csp>& _expressions)
 {
   algebra::node_csp skip, limit;
   algebra::order_by_csp order_by;
 
   while(tok.type == token_type::SKIP or tok.type == token_type::LIMIT or tok.type == token_type::ORDER)
   {
     switch(tok.type)
@@ -5301,14 +5414,32 @@
         is_of_type(token_type::BY);
         get_next_token();
         std::vector<algebra::order_by_expression_csp> expressions;
         while(true)
         {
           bool asc = true;
           algebra::node_csp expression = parse_expression();
+          if(expression_analyser.start(expression).aggregation_result)
+          {
+            bool has_same = false;
+
+            for(const algebra::named_expression_csp& ne : _expressions)
+            {
+              if(ne->get_expression()->equals(expression))
+              {
+                has_same = true;
+                break;
+              }
+            }
+            if(not has_same)
+            {
+              report_error(tok, exception_code::invalid_aggregation, "in order by expression.");
+            }
+
+          }
           if(tok.type == token_type::ASC)
           {
             get_next_token();
           } else if(tok.type == token_type::DESC)
           {
             asc = false;
             get_next_token();
@@ -5676,14 +5807,19 @@
     if(it == bindings.end())
     {
       report_error(tok, exception_code::invalid_parameter_use, "Unknown parameter '{}'", tok.string);
     }
     get_next_token();
     return std::make_shared<algebra::value>(it->second);
   }
+  case token_type::STAR:
+  {
+    get_next_token();
+    return std::make_shared<algebra::all>();
+  }
   default:
     report_unexpected(tok);
   }
 }
 
 algebra::node_csp parser::data::parse_expression_list()
 {
@@ -5785,37 +5921,79 @@
       } else {
         is_of_type(token_type::NULL_CAPS);
         get_next_token();
         return std::make_shared<algebra::is_null>(node);
       }
     }
     case token_type::EQUAL:
-      get_next_token();
-      return std::make_shared<algebra::relational_equal>(node, parse_relational_expression());
     case token_type::DIFFERENT:
-      get_next_token();
-      return std::make_shared<algebra::relational_different>(node, parse_relational_expression());
     case token_type::INFERIOR:
-      get_next_token();
-      return std::make_shared<algebra::relational_inferior>(node, parse_relational_expression());
     case token_type::SUPERIOR:
-      get_next_token();
-      return std::make_shared<algebra::relational_superior>(node, parse_relational_expression());
     case token_type::INFERIOR_EQUAL:
-      get_next_token();
-      return std::make_shared<algebra::relational_inferior_equal>(node, parse_relational_expression());
     case token_type::SUPERIOR_EQUAL:
-      get_next_token();
-      return std::make_shared<algebra::relational_superior_equal>(node, parse_relational_expression());
+    {
+      algebra::node_csp out_node;
+      while(tok.type != token_type::END_OF_FILE)
+      {
+        token_type current_op = tok.type;
+        get_next_token();
+        algebra::node_csp node_rhs = parse_additive_expression();
+        algebra::node_csp current_rel_node;
+        switch (current_op)
+        {
+        case token_type::EQUAL:
+          current_rel_node = std::make_shared<algebra::relational_equal>(node, node_rhs);
+          break;
+        case token_type::DIFFERENT:
+          current_rel_node =  std::make_shared<algebra::relational_different>(node, node_rhs);
+          break;
+        case token_type::INFERIOR:
+          current_rel_node =  std::make_shared<algebra::relational_inferior>(node, node_rhs);
+          break;
+        case token_type::SUPERIOR:
+          current_rel_node =  std::make_shared<algebra::relational_superior>(node, node_rhs);
+          break;
+        case token_type::INFERIOR_EQUAL:
+          current_rel_node =  std::make_shared<algebra::relational_inferior_equal>(node, node_rhs);
+          break;
+        case token_type::SUPERIOR_EQUAL:
+          current_rel_node =  std::make_shared<algebra::relational_superior_equal>(node, node_rhs);
+          break;
+        default:
+          report_error(tok, exception_code::internal_error, "While parsing relational expression.");
+        }
+        if(out_node)
+        {
+          out_node = std::make_shared<algebra::logical_and>(out_node, current_rel_node);
+        } else {
+          out_node = current_rel_node;
+        }
+        switch(tok.type)
+        {
+        case token_type::EQUAL:
+        case token_type::DIFFERENT:
+        case token_type::INFERIOR:
+        case token_type::SUPERIOR:
+        case token_type::INFERIOR_EQUAL:
+        case token_type::SUPERIOR_EQUAL:
+          node = node_rhs;
+          break;
+        default:
+          return out_node;
+        }
+      }
+      report_unexpected(tok);
+    }
+
     case token_type::IN:
       {
         get_next_token();
         algebra::node_csp container = parse_expression();
         algebra::expression_type container_type = expression_analyser.start(container).type;
-        errors::check_argument_types(container_type, {algebra::expression_type::map, algebra::expression_type::vector, algebra::expression_type::value}, exception_stage::compiletime, "Relational IN can only be applied on vector/map.");
+        errors::check_argument_types(container_type, {algebra::expression_type::map, algebra::expression_type::vector, algebra::expression_type::value, algebra::expression_type::empty}, exception_stage::compiletime, "Relational IN can only be applied on vector/map.");
         if(container_type == algebra::expression_type::map)
         {
           errors::check_argument_types(expression_analyser.start(node).type, {algebra::expression_type::string, algebra::expression_type::value}, exception_stage::compiletime, "Relational IN on map expect a string.");
         }
         return std::make_shared<algebra::relational_in>(node, container);
       }
     case token_type::NOT:
@@ -6037,16 +6215,21 @@
   while(d->tok.type != token_type::END_OF_FILE)
   {
     switch(d->tok.type)
     {
     case token_type::CREATE:
       nodes.push_back(d->parse_create());
       break;
+    case token_type::OPTIONAL:
+      d->get_next_token();
+      d->is_of_type(token_type::MATCH);
+      nodes.push_back(d->parse_match(true));
+      break;
     case token_type::MATCH:
-      nodes.push_back(d->parse_match());
+      nodes.push_back(d->parse_match(false));
       break;
     case token_type::WITH:
       nodes.push_back(d->parse_with());
       break;
     case token_type::UNWIND:
       nodes.push_back(d->parse_unwind());
       break;
@@ -6191,14 +6374,15 @@
 TOKEN_KEYWORD(IN)
 TOKEN_KEYWORD(IS)
 TOKEN_KEYWORD(LIMIT)
 TOKEN_KEYWORD(NOT)
 TOKEN_KEYWORD(MATCH)
 TOKEN_KEYWORD2(NULL_CAPS, "NULL")
 TOKEN_KEYWORD2(NULL_TOKEN, "null")
+TOKEN_KEYWORD(OPTIONAL)
 TOKEN_KEYWORD(OR)
 TOKEN_KEYWORD(ORDER)
 TOKEN_KEYWORD(REMOVE)
 TOKEN_KEYWORD(RETURN)
 TOKEN_KEYWORD(SET)
 TOKEN_KEYWORD(SKIP)
 TOKEN_KEYWORD(TRUE)
@@ -6261,15 +6445,16 @@
 #define OC_ALGEBRA_CREATE_NODES_MEMBERS(_KLASS_NAME_, F)                                    \
   F(_KLASS_NAME_, std::vector<alternative<GQLITE_LIST(graph_node, graph_edge)>>, patterns)
 
 OC_ALGEBRA_GENERATE(create, OC_ALGEBRA_CREATE_NODES_MEMBERS)
 
 #define OC_ALGEBRA_MATCH_NODES_MEMBERS(_KLASS_NAME_, F)                                     \
   F(_KLASS_NAME_, std::vector<alternative<GQLITE_LIST(graph_node, graph_edge)>>, patterns)  \
-  F(_KLASS_NAME_, node_csp, where)
+  F(_KLASS_NAME_, node_csp, where)                                                          \
+  F(_KLASS_NAME_, bool, optional)
 
 OC_ALGEBRA_GENERATE(match, OC_ALGEBRA_MATCH_NODES_MEMBERS)
 
 // Statements
 
 #define OC_ALGEBRA_NODES_LIST_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::vector<node_csp>, nodes)
@@ -6363,14 +6548,15 @@
 OC_ALGEBRA_GENERATE(edit_labels, OC_ALGEBRA_EDIT_LABELS_MEMBERS)
 
 
 // Values
 
 #define OC_ALGEBRA_NO_MEMBERS(_KLASS_NAME_, F)
 
+OC_ALGEBRA_GENERATE(all, OC_ALGEBRA_NO_MEMBERS)
 OC_ALGEBRA_GENERATE(end_of_list, OC_ALGEBRA_NO_MEMBERS)
 
 #define OC_ALGEBRA_GRAPH_NODE_MEMBERS(_KLASS_NAME_, F)          \
   F(_KLASS_NAME_, std::string, variable)                        \
   F(_KLASS_NAME_, std::vector<std::string>, labels)             \
   F(_KLASS_NAME_, node_csp, properties)
 
@@ -6387,15 +6573,14 @@
 OC_ALGEBRA_GENERATE(graph_edge, OC_ALGEBRA_GRAPH_EDGE_MEMBERS)
 
 #define OC_ALGEBRA_VALUE_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, gqlite::value, value)
 
 OC_ALGEBRA_GENERATE(value, OC_ALGEBRA_VALUE_MEMBERS)
 
-
 #define OC_ALGEBRA_MAP_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::unordered_map<GQLITE_LIST(std::string, node_csp)>, map)
 
 OC_ALGEBRA_GENERATE(map, OC_ALGEBRA_MAP_MEMBERS)
 
 #define OC_ALGEBRA_ARRAY_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::vector<node_csp>, array)
@@ -6608,15 +6793,16 @@
 #define OC_ALGEBRA_CREATE_NODES_MEMBERS(_KLASS_NAME_, F)                                    \
   F(_KLASS_NAME_, std::vector<alternative<GQLITE_LIST(graph_node, graph_edge)>>, patterns)
 
 OC_ALGEBRA_GENERATE(create, OC_ALGEBRA_CREATE_NODES_MEMBERS)
 
 #define OC_ALGEBRA_MATCH_NODES_MEMBERS(_KLASS_NAME_, F)                                     \
   F(_KLASS_NAME_, std::vector<alternative<GQLITE_LIST(graph_node, graph_edge)>>, patterns)  \
-  F(_KLASS_NAME_, node_csp, where)
+  F(_KLASS_NAME_, node_csp, where)                                                          \
+  F(_KLASS_NAME_, bool, optional)
 
 OC_ALGEBRA_GENERATE(match, OC_ALGEBRA_MATCH_NODES_MEMBERS)
 
 // Statements
 
 #define OC_ALGEBRA_NODES_LIST_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::vector<node_csp>, nodes)
@@ -6710,14 +6896,15 @@
 OC_ALGEBRA_GENERATE(edit_labels, OC_ALGEBRA_EDIT_LABELS_MEMBERS)
 
 
 // Values
 
 #define OC_ALGEBRA_NO_MEMBERS(_KLASS_NAME_, F)
 
+OC_ALGEBRA_GENERATE(all, OC_ALGEBRA_NO_MEMBERS)
 OC_ALGEBRA_GENERATE(end_of_list, OC_ALGEBRA_NO_MEMBERS)
 
 #define OC_ALGEBRA_GRAPH_NODE_MEMBERS(_KLASS_NAME_, F)          \
   F(_KLASS_NAME_, std::string, variable)                        \
   F(_KLASS_NAME_, std::vector<std::string>, labels)             \
   F(_KLASS_NAME_, node_csp, properties)
 
@@ -6734,15 +6921,14 @@
 OC_ALGEBRA_GENERATE(graph_edge, OC_ALGEBRA_GRAPH_EDGE_MEMBERS)
 
 #define OC_ALGEBRA_VALUE_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, gqlite::value, value)
 
 OC_ALGEBRA_GENERATE(value, OC_ALGEBRA_VALUE_MEMBERS)
 
-
 #define OC_ALGEBRA_MAP_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::unordered_map<GQLITE_LIST(std::string, node_csp)>, map)
 
 OC_ALGEBRA_GENERATE(map, OC_ALGEBRA_MAP_MEMBERS)
 
 #define OC_ALGEBRA_ARRAY_MEMBERS(_KLASS_NAME_, F) \
   F(_KLASS_NAME_, std::vector<node_csp>, array)
@@ -7249,19 +7435,25 @@
   enum class sql_join
   {
     inner, left
   };
   struct sql_query_builder
   {
     std::size_t uid = 0;
-    std::size_t table_count = 0;
     std::string variables;
-    std::string tables;
+    std::string group_variables;
+    bool has_aggregation_result = false;
+    struct table
+    {
+      sql_join join;
+      std::string table, name;
+    };
+    std::vector<table> tables;
     std::string join_conditions;
-    std::string where_conditions;
+    // std::string where_conditions;
     std::string modifiers;
     std::map<int, value> bindings;
     std::size_t next_uid()
     {
       return uid++;
     }
     std::string bind_value(const value& _value)
@@ -7269,84 +7461,112 @@
       std::size_t binding_id = bindings.size() + 1;
       bindings[binding_id] = _value;
       return format_string("?{}", to_string_fixed_width(binding_id, 3));
     }
     /**
      * Add a new variable with a generic name format.
      */
-    std::string add_variable(const std::string& _expression, const char* _format = "var_{}")
+    std::string add_variable(const std::string& _expression, bool _is_aggregation_result, const char* _format = "var_{}")
     {
       std::string name = format_string(_format, next_uid());
-      return add_variable_with_name(_expression, name);
+      return add_variable_with_name(_expression, name, _is_aggregation_result);
     }
     /**
      * Add a new variable with the given name.
      */
-    std::string add_variable_with_name(const std::string& _expression, const std::string& _name)
+    std::string add_variable_with_name(const std::string& _expression, const std::string& _name, bool _is_aggregation_result)
     {
+      has_aggregation_result = has_aggregation_result or _is_aggregation_result;
       if(not variables.empty()) variables += ", ";
       variables += format_string("{} AS {}", _expression, _name);
+      if(not _is_aggregation_result) group_variables += _name + ", ";
       return _name;
     }
+    void add_fake_table()
+    {
+      errors::check_condition(tables.empty(), exception_stage::runtime, exception_code::internal_error, "Fake table can only be added when the number of table is 0.");
+      tables.push_back({sql_join::inner, "(SELECT 1 AS fake)", "faketable"});
+    }
     std::string add_table(const std::string& _table, sql_join _join, const char* _table_name_format= "tbl_{}")
     {
-      if(table_count == 0)
+      if(tables.empty())
       {
         errors::check_condition(_join == sql_join::inner, exception_stage::runtime, exception_code::internal_error, "Joining with non-inner join on first table.");
-        tables += " FROM ";
-      } else {
-        switch(_join)
-        {
-          case sql_join::inner:
-            tables += " JOIN ";
-            break;
-          case sql_join::left:
-            tables += " LEFT JOIN ";
-            break;
-        }
       }
-      ++table_count;
       std::string table_name = format_string(_table_name_format, next_uid());
-      tables += format_string(" {} {} ", _table, table_name);
+      tables.push_back({_join, _table, table_name});
       return table_name;
     }
     template<typename... _T_>
     void add_join_condition(const std::string& _condition, const _T_&... _args)
     {
       if(_condition.empty()) return;
       if(not join_conditions.empty()) join_conditions += " AND ";
       join_conditions += format_string(_condition, _args...);
     }
     template<typename... _T_>
     void add_where_condition(const std::string& _condition, const _T_&... _args)
     {
-      if(_condition.empty()) return;
-      where_conditions += where_conditions.empty() ? " WHERE " : " AND ";
-      where_conditions += format_string(_condition, _args...);
+      add_join_condition(_condition, _args...);
+      // if(_condition.empty()) return;
+      // where_conditions += where_conditions.empty() ? " WHERE " : " AND ";
+      // where_conditions += format_string(_condition, _args...);
     }
     void add_modifier(const std::string& _modifier)
     {
       modifiers += _modifier;
     }
     std::string assemble()
     {
       std::string q = "SELECT ";
       q += variables.empty() ? " null " : variables;
-      q += tables;
+      if(not tables.empty())
+      {
+      // errors::check_condition(not tables.empty(), exception_stage::runtime, exception_code::internal_error, "Missing tables in query.");
+        q += format_string(" FROM {} {}", tables[0].table, tables[0].name);
+        for(std::size_t i = 1; i < tables.size(); ++i)
+        {
+          table& tbl = tables[i];
+          const char* join_type;
+          switch(tbl.join)
+          {
+            case sql_join::inner:
+              join_type = "JOIN";
+              break;
+            case sql_join::left:
+              join_type = "LEFT JOIN";
+              break;
+          }
+          if(i == tables.size() - 1)
+          {
+            q += format_string(" {} {} {}", join_type, tbl.table, tbl.name);
+          } else {
+            q += format_string(" {} ({} {}", join_type, tbl.table, tbl.name);          
+          }
+        }
+        for(std::size_t i = 1; i < tables.size() - 1; ++i)
+        {
+          q += ")";
+        }
+      }
       if(not join_conditions.empty())
       {
-        if(table_count == 1)
+        if(tables.size() == 1)
         {
           q += " WHERE ";
         } else {
           q += " ON ";
         }
         q += join_conditions;
       }
-      q += where_conditions;
+      // q += where_conditions;
+      if(has_aggregation_result and not group_variables.empty())
+      {
+        q += " GROUP BY {}" % std::string_view(group_variables).substr(0, group_variables.size() - 2);
+      }
       q += modifiers;
       return q;
     }
   };
 
   /**
    * Context for the generation of the sql match query
@@ -7357,34 +7577,39 @@
     sql_query_builder query_builder;
     std::map<std::string, sql_variable_info> variables;
     std::string previous_table_ref;
   
     // std::string view_name;
     oc::algebra::visitors::expression_analyser expression_analyser;
 
-    table prepare(const table& _table, bool _create_new_table)
+    table prepare(const table& _table, bool _create_new_table, bool _optional)
     {
       expression_analyser.stage = exception_stage::runtime;
       expression_analyser.variables_f = [this](const std::string& _var_name)
       {
         return get_variable_info(_var_name).type;
       };
       table new_table;
       if(_create_new_table) new_table.view_name = "__view" + std::to_string(++exec_c->next_view_id);
-      if(not _table.view_name.empty())
+      if(_table.view_name.empty())
       {
+        if(_optional)
+        {
+          query_builder.add_fake_table();
+        }
+      } else {
         previous_table_ref = query_builder.add_table(_table.view_name, sql_join::inner, "pt_{}");
 
         for(auto const& [k, v] : _table.variables)
         {
           std::string sql_var = format_string("{}.{}", previous_table_ref, v.sql_var_name);
           variables[k] = { sql_var, v.type };
           if(_create_new_table)
           {
-            std::string col_name = query_builder.add_variable(sql_var);
+            std::string col_name = query_builder.add_variable(sql_var, false);
             new_table.variables[k] = { col_name, v.type };
           }
         }
       }
       return new_table;
     }
     sql_variable_info& get_variable_info(const std::string& _oc_variable)
@@ -7444,14 +7669,18 @@
     {
       return eval_c->query_builder.bind_value(std::numeric_limits<int64_t>::max());
     }
     std::string visit(algebra::value_csp _node) override
     {
       return eval_c->query_builder.bind_value(_node->get_value());
     }
+    std::string visit(algebra::all_csp) override
+    {
+      return "*";
+    }
     std::string visit(algebra::has_labels_csp _node) override
     {
       oc::algebra::expression_type et = eval_c->get_variable_info(_node->get_left()).type;
       std::string label_ids;
       for(const std::string& l : _node->get_labels())
       {
         if(not label_ids.empty()) label_ids += ", ";
@@ -7479,15 +7708,15 @@
       std::size_t var_uuid = eval_c->query_builder.next_uid();
       std::string map = ("(SELECT json_group_object(name_{}, val_{}) FROM ("s % var_uuid, var_uuid);
       bool first = true;
       for(const auto& [k, v] : _map->get_map())
       {
         if(not first)
         {
-          map += " UNION ";
+          map += " UNION ALL ";
         }
         map += "SELECT " + eval_c->query_builder.bind_value(k);
         if(first)
         {
           map += " AS name_{}"s % var_uuid;
         }
         map += ", " + start(v);
@@ -7504,15 +7733,15 @@
       std::size_t var_uuid = eval_c->query_builder.next_uid();
       std::string array = "(SELECT json_group_array(val_{}) FROM ("s % var_uuid;
       bool first = true;
       for(algebra::node_csp v : _array->get_array())
       {
         if(not first)
         {
-          array += " UNION ";
+          array += " UNION ALL ";
         }
         array += "SELECT " + start(v);
         if(first)
         {
           array += " AS val_{}"s % var_uuid;
         }
         first = false;
@@ -7606,27 +7835,45 @@
         } else {
           errors::check_condition(arg_0->get_type() == algebra::node_type::variable, exception_stage::runtime, exception_code::internal_error, "Only variable are supported yet for getting properties for node/edge.");
           map_expr = eval_c->get_sql_properties_variable(std::static_pointer_cast<const algebra::variable>(arg_0)->get_identifier());
         }
         return "(SELECT json_group_array(key) FROM json_each({}))" % map_expr;
       } else if(_node->get_name() == "toInteger")
       {
-        return "CAST({} AS INTEGER)"s % start(_node->get_arguments()[0]);
+        return "gqlite_to_integer({})"s % start(_node->get_arguments()[0]);
       } else if(_node->get_name() == "size")
       {
         return "json_array_length({})"s % start(_node->get_arguments()[0]);
       } else if(_node->get_name() == "id")
       {
         return start(_node->get_arguments()[0]);
       } else if(_node->get_name() == "head")
       {
         return "json_extract({}, '$[0]')" % start(_node->get_arguments()[0]);
       } else if(_node->get_name() == "tail")
       {
         return "gqlite_tail({})" % start(_node->get_arguments()[0]);
+      } else if(_node->get_name() == "avg")
+      {
+        return "avg({})" % start(_node->get_arguments()[0]);
+      } else if(_node->get_name() == "count")
+      {
+        return "count({})" % start(_node->get_arguments()[0]);
+      } else if(_node->get_name() == "collect")
+      {
+        return "json_group_array({})" % start(_node->get_arguments()[0]);
+      } else if(_node->get_name() == "max")
+      {
+        return "max({})" % start(_node->get_arguments()[0]);
+      } else if(_node->get_name() == "min")
+      {
+        return "min({})" % start(_node->get_arguments()[0]);
+      } else if(_node->get_name() == "sum")
+      {
+        return "sum({})" % start(_node->get_arguments()[0]);
       }
       throw_exception(exception_stage::runtime, exception_code::unimplemented_error, "Function call to {} is not implemented.", _node->get_name());
     }
 #define FILTER_VISITOR_BINARY_OP(_AL_, _OP_)                                                          \
     std::string visit(algebra::_AL_ ## _csp _node) override                                           \
     {                                                                                                 \
       return "({} " _OP_ " {})"s % start(_node->get_left()), start(_node->get_right());               \
@@ -7634,16 +7881,16 @@
     FILTER_VISITOR_BINARY_OP(logical_and, "AND")
     FILTER_VISITOR_BINARY_OP(logical_or, "OR")
     FILTER_VISITOR_BINARY_OP(logical_xor, "<>")
     FILTER_VISITOR_BINARY_OP(relational_equal, "=")
     FILTER_VISITOR_BINARY_OP(relational_different, "!=")
     FILTER_VISITOR_BINARY_OP(relational_inferior, "<")
     FILTER_VISITOR_BINARY_OP(relational_superior, ">")
-    FILTER_VISITOR_BINARY_OP(relational_inferior_equal, "<")
-    FILTER_VISITOR_BINARY_OP(relational_superior_equal, ">")
+    FILTER_VISITOR_BINARY_OP(relational_inferior_equal, "<=")
+    FILTER_VISITOR_BINARY_OP(relational_superior_equal, ">=")
     FILTER_VISITOR_BINARY_OP(substraction, "-")
     FILTER_VISITOR_BINARY_OP(multiplication, "*")
     FILTER_VISITOR_BINARY_OP(division, "/")
     FILTER_VISITOR_BINARY_OP(modulo, "%")
 
     std::string visit(algebra::relational_in_csp _node) override
     {
@@ -7742,26 +7989,26 @@
     }
     //////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
     // Creation functions
     value_vector create_node(algebra::graph_node_csp _node)
     {
       sql_evaluation_context mc;
       mc.exec_c = &exec_c;
-      mc.prepare(current_table, false);
+      mc.prepare(current_table, false, false);
       sql_expression_visitor sev{&mc};
-      mc.query_builder.add_variable("gqlite_next_uid('nodes')");
+      mc.query_builder.add_variable("gqlite_next_uid('nodes')", false);
 
       std::string properties_str;
       if(_node->get_properties())
       {
         properties_str = sev.start(_node->get_properties());
       } else {
         properties_str = "'{}'";
       }
-      mc.query_builder.add_variable(properties_str);
+      mc.query_builder.add_variable(properties_str, false);
       std::string query = sqlite_queries::node_create(
         exec_c.graph_name, sev.eval_c->query_builder.assemble());
       value res = exec_c.data->execute_sql(query, sev.eval_c->query_builder.bindings);
       value_vector ret_v;
       value_vector res_v = res.to_vector();
       for(std::size_t i = 0; i < res_v.size(); ++i)
       {
@@ -7809,42 +8056,42 @@
         return std::make_tuple(value(), false, it_var->second.sql_var_name);
       }
     }
     std::tuple<value_vector, value_vector, value_vector> create_edge(algebra::graph_edge_csp _edge, const std::map<std::string, value_vector>& _new_nodes)
     {
       sql_evaluation_context mc;
       mc.exec_c = &exec_c;
-      mc.prepare(current_table, false);
+      mc.prepare(current_table, false, false);
       sql_expression_visitor sev{&mc};
-      mc.query_builder.add_variable("gqlite_next_uid('edges')");
+      mc.query_builder.add_variable("gqlite_next_uid('edges')", false);
       // Handle label
       std::string label = _edge->get_labels().empty() ? std::string() : _edge->get_labels().front();
       std::string label_binding_idx = sev.eval_c->query_builder.bind_value(exec_c.data->id_for_label(label));
-      mc.query_builder.add_variable(label_binding_idx, "label_{}");
+      mc.query_builder.add_variable(label_binding_idx, false, "label_{}");
 
       // Handle properties
       std::string properties_str;
       if(_edge->get_properties())
       {
         properties_str = sev.start(_edge->get_properties());
       } else {
         properties_str = "'{}'";
       }
-      mc.query_builder.add_variable(properties_str, "properties_{}");
+      mc.query_builder.add_variable(properties_str, false, "properties_{}");
 
       // Handle source
       auto const&[left_value, new_left_value, left_expr] = create_node_if_needed(&sev, _edge->get_source(), _new_nodes, "source_node_{}");
-      mc.query_builder.add_variable(left_expr, "source_{}");
+      mc.query_builder.add_variable(left_expr, false, "source_{}");
 
       // Check if destination == source
       auto const&[right_value, new_right_value, right_expr]
         = (_edge->get_source()->get_variable() == _edge->get_destination()->get_variable()) ?
             std::make_tuple(gqlite::value(), false, left_expr)
           : create_node_if_needed(&sev, _edge->get_destination(), _new_nodes, "destination_node_{}");
-      mc.query_builder.add_variable(right_expr, "destination_{}");
+      mc.query_builder.add_variable(right_expr, false, "destination_{}");
 
       // Execute queries
       std::string query = sqlite_queries::edge_create(exec_c.graph_name, sev.eval_c->query_builder.assemble());
       value res = sev.eval_c->exec_c->data->execute_sql(query, sev.eval_c->query_builder.bindings);
 
       // Prepare return
       value_vector ret_v;
@@ -7898,15 +8145,15 @@
       }
 
       if(new_non_anonymous_nodes)
       {
         // 2) Create the resulting table
         sql_evaluation_context mc;
         mc.exec_c = &exec_c;
-        table new_table = mc.prepare(current_table, true);
+        table new_table = mc.prepare(current_table, true, false);
         sql_expression_visitor sev{&mc};
         std::string first_table_ref;
         // loop over new things
         for(const auto& [new_things, type, var_format]
            : std::initializer_list<std::tuple<std::map<std::string, gqlite::value_vector>, oc::algebra::expression_type, const char*>>
              {{new_nodes, oc::algebra::expression_type::node, "new_node_{}"}, {new_edges, oc::algebra::expression_type::edge, "new_edge_{}"}})
         {
@@ -7918,15 +8165,15 @@
               std::string table_ref = mc.query_builder.add_table(format_string("json_each({})", idx), sql_join::inner, var_format);
               if(first_table_ref.empty())
               {
                 first_table_ref = table_ref;
               } else {
                 mc.query_builder.add_join_condition("{}.key = {}.key", first_table_ref, table_ref);
               }
-              mc.query_builder.add_variable_with_name(format_string(" {}.value ", table_ref), table_ref);
+              mc.query_builder.add_variable_with_name(format_string(" {}.value ", table_ref), table_ref, false);
               new_table.variables[k] = {table_ref, type};
             }
           }
         }
         if(not mc.previous_table_ref.empty())
         {
           mc.query_builder.add_join_condition("{}.rowid = {}.key + 1", mc.previous_table_ref, first_table_ref);
@@ -8005,67 +8252,77 @@
     void generate_var_match(sql_match_evaluation_context* _mc, table* _table, const std::string& _oc_var, const std::string& _sql_var, const std::string& _sql_properties_var, const std::string& _label_var, oc::algebra::expression_type _variable_type)
     {
       if(not _oc_var.empty())
       {
         auto it = _mc->variables.find(_oc_var);
         if(it == _mc->variables.end())
         {
-          std::string var_name = _mc->query_builder.add_variable(_sql_var, "new_match_{}");
+          std::string var_name = _mc->query_builder.add_variable(_sql_var, false, "new_match_{}");
           _table->variables[_oc_var] = {var_name, _variable_type};
           _mc->variables[_oc_var] = {_sql_var, _variable_type, _sql_properties_var, _label_var};
         } else {
           errors::check_variable_type(it->second.type, _variable_type, exception_stage::runtime, _oc_var);
           // Generate match
           _mc->query_builder.add_join_condition(" {} = {} ", _sql_var, it->second.sql_var_name);
         }
       }
     }
     value visit(algebra::match_csp _node) override
     {
       sql_match_evaluation_context mc;
       mc.exec_c = &exec_c;
-      table new_table = mc.prepare(current_table, true);
+      table new_table = mc.prepare(current_table, true, _node->get_optional());
       sql_match_expression_visitor sev{&mc};
 
+      const bool is_optional = _node->get_optional();
+
       // 1) Go through the patterns
       for(const algebra::alternative<algebra::graph_node, algebra::graph_edge>& pattern : _node->get_patterns())
       {
-        pattern.visit<void>([this, &mc, &sev, &new_table](const algebra::graph_node_csp _node)
+        pattern.visit<void>([this, &mc, &sev, &new_table, is_optional](const algebra::graph_node_csp _node)
         {
-          std::string table_ref = sev.eval_c->query_builder.add_table(format_string("gqlite_{}_nodes", exec_c.graph_name), sql_join::inner, "node_{}");
+          sql_join s_join = is_optional ? sql_join::left : sql_join::inner;
+          std::string table_ref = sev.eval_c->query_builder.add_table(format_string("gqlite_{}_nodes", exec_c.graph_name), s_join, "node_{}");
           std::string sql_var = format_string("{}.id", table_ref);
           std::string sql_properties_var = format_string("{}.properties", table_ref);
           mc.query_builder.add_join_condition(mc.generate_labels_match(_node->get_labels(), format_string("{}.id", table_ref)));
           if(_node->get_properties())
           {
             mc.query_builder.add_where_condition(generate_filter(_node->get_properties(), sql_properties_var + ", '$", &sev));
           }
           generate_var_match(&mc, &new_table, _node->get_variable(), sql_var, sql_properties_var, std::string(), algebra::expression_type::node);
         },
-        [this, &mc, &sev, &new_table](const algebra::graph_edge_csp _edge)
+        [this, &mc, &sev, &new_table, is_optional](const algebra::graph_edge_csp _edge)
         {
+          sql_join s_join = is_optional ? sql_join::left : sql_join::inner;
           std::string table_ref;
           if(_edge->get_directivity() == algebra::edge_directivity::undirected)
           {
-            table_ref = sev.eval_c->query_builder.add_table(format_string("gqlite_{}_edges_undirected", exec_c.graph_name), sql_join::inner, "undirected_edge_{}");
+            table_ref = sev.eval_c->query_builder.add_table(format_string("gqlite_{}_edges_undirected", exec_c.graph_name), s_join, "undirected_edge_{}");
           } else {
-            table_ref = sev.eval_c->query_builder.add_table(format_string("gqlite_{}_edges", exec_c.graph_name), sql_join::inner, "edge_{}");
+            table_ref = sev.eval_c->query_builder.add_table(format_string("gqlite_{}_edges", exec_c.graph_name), s_join, "edge_{}");
           }
           std::string sql_source_var = format_string("{}.left", table_ref);
           std::string sql_edge_var = format_string("{}.id", table_ref);
           std::string sql_properties_edge_var = format_string("{}.properties", table_ref);
           std::string sql_label_edge_var = format_string("{}.label", table_ref);
           std::string sql_source_properties_var;
           std::string sql_destination_properties_var;
           std::string sql_destination_var = format_string("{}.right", table_ref);
           mc.query_builder.add_where_condition(mc.generate_labels_match(_edge->get_source()->get_labels(), table_ref+ ".left"));
           mc.query_builder.add_where_condition(mc.generate_labels_match(_edge->get_destination()->get_labels(), table_ref + ".right"));
           if(not _edge->get_labels().empty())
           {
-            std::string label_conds = "(FALSE ";
+            std::string label_conds;
+            if(is_optional)
+            {
+              label_conds = format_string("({} IS NULL", sql_label_edge_var);
+            } else {
+              label_conds = "(FALSE ";
+            }
             for(const std::string& label : _edge->get_labels())
             {
               label_conds += format_string(" OR {} = {}", sql_label_edge_var, exec_c.data->id_for_label(label));
             }
             label_conds += ")";
             mc.query_builder.add_where_condition(label_conds);
           }
@@ -8116,28 +8373,35 @@
     // delete
     value visit(algebra::delete_statement_csp _ds) override
     {
       for(algebra::node_csp node : _ds->get_expressions())
       {
         sql_match_evaluation_context mc;
         mc.exec_c = &exec_c;
-        mc.prepare(current_table, false);
+        mc.prepare(current_table, false, false);
         sql_match_expression_visitor sev{&mc};
         std::string expr = sev.start(node);
-        mc.query_builder.add_variable(expr);
+        mc.query_builder.add_variable(expr, false);
         std::string what = mc.query_builder.assemble();
 
         switch(mc.expression_analyser.start(node).type)
         {
           case algebra::expression_type::node:
           {
             if(_ds->get_detach())
             {
-              std::string query = sqlite_queries::edge_delete_by_node(exec_c.graph_name, what);
+              std::string query = sqlite_queries::edge_delete_by_nodes(exec_c.graph_name, what);
               mc.exec_c->data->execute_sql(query, mc.query_builder.bindings);
+            } else {
+              std::string query = sqlite_queries::edge_count_by_nodes(exec_c.graph_name, what);
+              gqlite::value count = mc.exec_c->data->execute_sql(query, mc.query_builder.bindings);
+              if(count.to_vector().front().to_vector().front().to_integer() > 0)
+              {
+                throw_exception(exception_stage::runtime, exception_code::delete_connected_node, "delete connected node not allowed, unless using detach.");
+              }
             }
             std::string query = sqlite_queries::node_delete(exec_c.graph_name, what);
             mc.exec_c->data->execute_sql(query, mc.query_builder.bindings);
             break;
           }
           case algebra::expression_type::edge:
           {
@@ -8146,67 +8410,14 @@
             break;
           }
           default:
             errors::invalid_argument_type(exception_stage::runtime, "Delete expect a node/edge.");
         }
       }
       return value();
-      #if 0
-      evaluation_context eval_c;
-      eval_c.table = table;
-      evaluator_visitor eval_v;
-      eval_v.exec_c = &exec_c;
-      eval_v.eval_c = &eval_c;
-
-      struct deleter
-      {
-        statement_visitor* self;
-        bool detach;
-        void operator()(const node_ref_sp& _node)
-        {
-          if(detach)
-          {
-            self->exec_c.data->execute_sql(sqlite_queries::edge_delete_by_node(self->exec_c.graph_name), {{1, _node->id}});
-          } else {
-            value result = self->exec_c.data->execute_sql(sqlite_queries::edge_count_by_node(self->exec_c.graph_name), {{1, _node->id}});
-            value_vector rows = result.to_vector();
-            errors::check_condition(rows.size() == 1, exception_stage::runtime, exception_code::internal_error, "Invalid number of rows for counting edges got {} expected 1.", rows.size());
-            value_vector row = rows.front().to_vector();
-            errors::check_condition(row.size() == 1, exception_stage::runtime, exception_code::internal_error, "Invalid number of columns for counting edges got {} expected 1.", rows.size());
-            int count = row.front().to_integer();
-            errors::check_condition(count == 0, exception_stage::runtime, exception_code::unspecified, "Cannot delete node with {} relationships.", count);
-          }
-          self->exec_c.data->execute_sql(sqlite_queries::node_delete(self->exec_c.graph_name), {{1, _node->id}});
-        }
-        void operator()(const edge_ref_sp& _edge)
-        {
-          self->exec_c.data->execute_sql(sqlite_queries::edge_delete(self->exec_c.graph_name), {{1, _edge->id}});
-        }
-        void operator()(const value&)
-        {
-          throw_exception(exception_stage::runtime, exception_code::invalid_argument_type, "Cannot delete a value.");
-        }
-        void operator()(const empty&)
-        {
-          throw_exception(exception_stage::runtime, exception_code::invalid_argument_type, "Cannot delete an empty value.");
-        }
-      };
-
-      for(std::size_t i = 0; i < table.get_rows_count(); ++i)
-      {
-        value_vector row;
-        eval_c.prepare_current_row(table, i, false);
-        for(const algebra::node_csp& rv : _ds->get_expressions())
-        {
-          exec_value ev =eval_v.start(rv);
-          std::visit(deleter{this, _ds->get_detach()}, ev);
-        }
-      }
-      return value();
-      #endif
     }
     std::string to_sqlite_path(const std::vector<std::string>& _path)
     {
       std::string path_string = "$";
       for(const std::string& pe : _path)
       {
         path_string += "." + pe;
@@ -8226,15 +8437,15 @@
           {
             throw_exception(exception_stage::runtime, exception_code::unimplemented_error, "Unimplemented node {} in set_visitor", oc::algebra::node_type_name(_node->get_type()));
           }
           void visit(algebra::set_property_csp _property)
           {
             sql_match_evaluation_context mc;
             mc.exec_c = &self->exec_c;
-            mc.prepare(self->current_table, false);
+            mc.prepare(self->current_table, false, false);
             sql_match_expression_visitor sev{&mc};
             sql_variable_info svi = mc.get_variable_info(_property->get_left());
             // mc.query_builder.add_variable(svi.sql_var_name);
             std::string expr = sev.start(_property->get_expression());
             std::string what = mc.query_builder.assemble().substr(sizeof("SELECT null"));
 
             switch(svi.type)
@@ -8255,15 +8466,15 @@
               errors::invalid_argument_type(exception_stage::runtime, "Delete expect a node/edge.");
             }
           }
           void visit(algebra::add_property_csp _property)
           {
             sql_match_evaluation_context mc;
             mc.exec_c = &self->exec_c;
-            mc.prepare(self->current_table, false);
+            mc.prepare(self->current_table, false, false);
             sql_match_expression_visitor sev{&mc};
             sql_variable_info svi = mc.get_variable_info(_property->get_left());
             std::string expr = sev.start(_property->get_expression());
             std::string what = mc.query_builder.assemble().substr(sizeof("SELECT null"));
 
             switch(svi.type)
             {
@@ -8283,22 +8494,23 @@
               errors::invalid_argument_type(exception_stage::runtime, "Delete expect a node/edge.");
             }
           }
           void visit(algebra::edit_labels_csp _edit_label)
           {
             sql_match_evaluation_context mc;
             mc.exec_c = &self->exec_c;
-            mc.prepare(self->current_table, false);
+            mc.prepare(self->current_table, false, false);
             sql_match_expression_visitor sev{&mc};
             sql_variable_info svi = mc.get_variable_info(_edit_label->get_target());
             std::vector<std::string> labels = _edit_label->get_labels();
             auto label_ids_view = labels | std::views::transform([this](const std::string& _label) { return value(self->exec_c.data->id_for_label(_label)); });
             std::string labels_ref = mc.query_builder.add_table("json_each({})"s % mc.query_builder.bind_value(value_vector(label_ids_view.begin(), label_ids_view.end())), sql_join::inner);
-            mc.query_builder.add_variable("{}.value" % labels_ref);
-            mc.query_builder.add_variable(svi.sql_var_name);
+            mc.query_builder.add_variable("{}.value" % labels_ref, false);
+            mc.query_builder.add_variable(svi.sql_var_name, false);
+            mc.query_builder.add_where_condition("{} IS NOT NULL", svi.sql_var_name);
             std::string what = mc.query_builder.assemble();
 
             switch(svi.type)
             {
             case algebra::expression_type::node:
             {
               std::string query = sqlite_queries::node_add_labels(self->exec_c.graph_name, what);
@@ -8329,15 +8541,15 @@
           {
             throw_exception(exception_stage::runtime, exception_code::unimplemented_error, "Unimplemented node {} in remove_visitor", oc::algebra::node_type_name(_node->get_type()));
           }
           void visit(algebra::remove_property_csp _property)
           {
             sql_match_evaluation_context mc;
             mc.exec_c = &self->exec_c;
-            mc.prepare(self->current_table, false);
+            mc.prepare(self->current_table, false, false);
             sql_match_expression_visitor sev{&mc};
             sql_variable_info svi = mc.get_variable_info(_property->get_left());
             std::string what = mc.query_builder.assemble().substr(sizeof("SELECT null"));
 
             switch(svi.type)
             {
             case algebra::expression_type::node:
@@ -8356,21 +8568,21 @@
               errors::invalid_argument_type(exception_stage::runtime, "Delete expect a node/edge.");
             }
           }
           void visit(algebra::edit_labels_csp _edit_label)
           {
             sql_match_evaluation_context mc;
             mc.exec_c = &self->exec_c;
-            mc.prepare(self->current_table, false);
+            mc.prepare(self->current_table, false, false);
             sql_match_expression_visitor sev{&mc};
             sql_variable_info svi = mc.get_variable_info(_edit_label->get_target());
             std::vector<std::string> labels = _edit_label->get_labels();
             auto label_ids_view = labels | std::views::transform([this](const std::string& _label) { return std::to_string(self->exec_c.data->id_for_label(_label)); });
             std::string labels_ref = string::join(label_ids_view, ", ");
-            mc.query_builder.add_variable(svi.sql_var_name);
+            mc.query_builder.add_variable(svi.sql_var_name, false);
             std::string what = mc.query_builder.assemble();
 
             switch(svi.type)
             {
             case algebra::expression_type::node:
             {
               std::string query = sqlite_queries::node_remove_label(self->exec_c.graph_name, what, labels_ref);
@@ -8427,55 +8639,55 @@
       if(w->get_all() and not w->get_expressions().empty())
       {
         throw_exception(exception_stage::runtime, exception_code::unspecified, "Unimplemented WITH *, expressions");
       }
 
       sql_evaluation_context mc;
       mc.exec_c = &exec_c;
-      table new_table = mc.prepare(current_table, true);
+      table new_table = mc.prepare(current_table, true, false);
       new_table.variables.clear();
       sql_expression_visitor sev{&mc};
       // Generate SQL Query
       for(const algebra::named_expression_csp& rv : w->get_expressions())
       {
-        std::string var = mc.query_builder.add_variable(sev.start(rv->get_expression()));
-        algebra::expression_type et = mc.expression_analyser.start(rv->get_expression()).type; 
-        new_table.variables[rv->get_name()] = {var, et};
-        mc.variables[rv->get_name()] = {var, et};
+        algebra::expression_info expr_info = mc.expression_analyser.start(rv->get_expression()); 
+        std::string var = mc.query_builder.add_variable(sev.start(rv->get_expression()), expr_info.aggregation_result);
+        new_table.variables[rv->get_name()] = {var, expr_info.type};
+        mc.variables[rv->get_name()] = {var, expr_info.type};
       }
       add_filter_expressions(&sev, w->get_modifiers());
       std::string query = "CREATE TEMPORARY TABLE " + new_table.view_name + " AS " + mc.query_builder.assemble();
       exec_c.data->execute_sql(query, mc.query_builder.bindings);
 
       current_table = new_table;
       return value();
     }
     //////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
     // unwind
     value visit(algebra::unwind_csp uw) override
     {
       sql_evaluation_context mc;
       mc.exec_c = &exec_c;
-      table new_table = mc.prepare(current_table, true);
+      table new_table = mc.prepare(current_table, true, false);
       sql_expression_visitor sev{&mc};
       std::string table_ref = mc.query_builder.add_table("json_each(" + sev.start(uw->get_expression()) + ")", sql_join::inner, "a_uw_{}");
-      std::string var = mc.query_builder.add_variable(format_string("{}.value", table_ref));
+      std::string var = mc.query_builder.add_variable(format_string("{}.value", table_ref), false);
       std::string query = "CREATE TEMPORARY TABLE " + new_table.view_name + " AS " + mc.query_builder.assemble();
       new_table.variables[uw->get_name()] = {var, oc::algebra::expression_type::value};
       exec_c.data->execute_sql(query, mc.query_builder.bindings);
       current_table = new_table;
       return value();
     }
     //////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
     // Return
     value visit(algebra::return_statement_csp _rs) override
     {
       sql_evaluation_context mc;
       mc.exec_c = &exec_c;
-      mc.prepare(current_table, false);
+      mc.prepare(current_table, false, false);
       sql_expression_visitor sev{&mc};
       std::vector<gqlite::oc::algebra::named_expression_csp> expressions;
       if(_rs->get_all())
       {
         for(const auto& [k, var_info] : current_table.variables)
         {
           if(not k.starts_with("__gqlite_anon_"))
@@ -8489,95 +8701,99 @@
       // Generate SQL Query
       value_vector labels;
       std::vector<oc::algebra::expression_type> column_types;
       std::map<std::string, sql_variable_info> variables_extra; /// new variables to set for modifier
 
       for(const algebra::named_expression_csp& rv : expressions)
       {
-        oc::algebra::expression_type et = mc.expression_analyser.start(rv->get_expression()).type;
-        switch(et)
+        oc::algebra::expression_info expr_info = mc.expression_analyser.start(rv->get_expression());
+        switch(expr_info.type)
         {
         case oc::algebra::expression_type::node:
           {
             std::string table_ref = mc.query_builder.add_table(format_string("gqlite_{}_nodes_as_json", exec_c.graph_name), sql_join::inner, "node_{}");
-            mc.query_builder.add_join_condition("{}.id = {}", table_ref, sev.start(rv->get_expression()));
-            std::string var_expr = mc.query_builder.add_variable("{}.node" % table_ref);
+            mc.query_builder.add_join_condition("{}.id IS {}", table_ref, sev.start(rv->get_expression()));
+            std::string var_expr = mc.query_builder.add_variable("{}.node" % table_ref, expr_info.aggregation_result);
             variables_extra[rv->get_name()] = {var_expr, oc::algebra::expression_type::node,
                                   "json_extract({}, '$.properties')" % var_expr, "json_extract({}, '$.labels')" % var_expr};
             break;
           }
         case oc::algebra::expression_type::edge:
           {
             std::string table_ref = mc.query_builder.add_table(format_string("gqlite_{}_edges_as_json", exec_c.graph_name), sql_join::inner, "edge_{}");
-            mc.query_builder.add_join_condition("{}.id = {}", table_ref, sev.start(rv->get_expression()));
-            std::string var_expr = mc.query_builder.add_variable("{}.edge" % table_ref);
+            mc.query_builder.add_join_condition("{}.id IS {}", table_ref, sev.start(rv->get_expression()));
+            std::string var_expr = mc.query_builder.add_variable("{}.edge" % table_ref, expr_info.aggregation_result);
             variables_extra[rv->get_name()] = {var_expr, oc::algebra::expression_type::edge,
                                     "json_extract({}, '$.properties')" % var_expr, "json_extract({}, '$.label')" % var_expr};
             break;
           }
         case oc::algebra::expression_type::boolean:
         case oc::algebra::expression_type::vector:
         case oc::algebra::expression_type::map:
           [[fallthrough]];
         default:
           {
-            std::string var_expr = mc.query_builder.add_variable(sev.start(rv->get_expression()));
-            variables_extra[rv->get_name()] = {var_expr, et};
+            std::string var_expr = mc.query_builder.add_variable(sev.start(rv->get_expression()), expr_info.aggregation_result);
+            variables_extra[rv->get_name()] = {var_expr, expr_info.type};
             break;
           }
         }
         labels.push_back(rv->get_name());
-        column_types.push_back(et);
+        column_types.push_back(expr_info.type);
       }
       // Execute SQL query
       if(_rs->get_modifiers())
       {
-        mc.variables.insert(variables_extra.begin(), variables_extra.end());
+        std::swap(mc.variables, variables_extra);
+        mc.variables.merge(variables_extra);
         add_filter_expressions(&sev, _rs->get_modifiers());
       }
       value res = exec_c.data->execute_sql(mc.query_builder.assemble(), mc.query_builder.bindings);
       // Prepare to return results
       value_vector res_v = res.to_vector();
       value_vector ret_v;
       ret_v.push_back(labels);
       for(const value& r : res_v)
       {
         value_vector r_v = r.to_vector();
         for(std::size_t c = 0; c < r_v.size(); ++c)
         {
           value& v = r_v[c];
-          switch(column_types[c])
+          if(v.get_type() != value_type::invalid)
           {
-          case oc::algebra::expression_type::boolean:
-            if(v.get_type() != value_type::invalid)
+            switch(column_types[c])
             {
-              v = (v.to_integer() == 1);
-            }
-            break;
-          case oc::algebra::expression_type::map:
-          case oc::algebra::expression_type::vector:
-            v = value::from_json(v.to_string());
-            break;
-          case oc::algebra::expression_type::node:
-          case oc::algebra::expression_type::edge:
-            v = value::from_json(v.to_string());
-            break;
-          default:
-            if(v.get_type() == value_type::string)
-            {
-              // Attempt to parse strings as json
-              try
+            case oc::algebra::expression_type::boolean:
+              if(v.get_type() != value_type::invalid)
               {
-                v = value::from_json(v.to_string());
+                v = (v.to_integer() == 1);
               }
-              catch(const exception&)
+              break;
+            case oc::algebra::expression_type::map:
+            case oc::algebra::expression_type::vector:
+              v = value::from_json(v.to_string());
+              break;
+            case oc::algebra::expression_type::node:
+            case oc::algebra::expression_type::edge:
+              v = value::from_json(v.to_string());
+              break;
+            default:
+              if(v.get_type() == value_type::string)
               {
-                // ignore, that probably means it is a real string
+                // Attempt to parse strings as json
+                try
+                {
+                  v = value::from_json(v.to_string());
+                }
+                catch(const exception&)
+                {
+                  // ignore, that probably means it is a real string
+                }
+                break;
               }
-              break;
             }
           }
         }
         ret_v.push_back(r_v);
       }
       return ret_v;
     }
@@ -8627,22 +8843,24 @@
     d->graph_create("default");
   }
 
   d->procedures["gqlite.internal.stats"] = [this](const value_vector&)
   {
     gqlite::value result = d->execute_sql(sqlite_queries::get_debug_stats("default"));
     value_vector rows = result.to_vector();
-    errors::check_condition(rows.size() == 7, exception_stage::runtime, exception_code::internal_error, "Invalid number of debug stats got {} expected 7.", rows.size());
+    errors::check_condition(rows.size() == 9, exception_stage::runtime, exception_code::internal_error, "Invalid number of debug stats got {} expected 7.", rows.size());
     value_map stats;
     stats["nodes_count"] = rows[0].to_vector()[0].to_integer();
     stats["edges_count"] = rows[1].to_vector()[0].to_integer();
     stats["labels_assignment_count"] = rows[2].to_vector()[0].to_integer();
     stats["properties_count"] = rows[3].to_vector()[0].to_integer() + rows[4].to_vector()[0].to_integer();
     stats["labels_count"] = rows[5].to_vector()[0].to_integer();
     stats["labels_assignment_nodes_count"] = rows[6].to_vector()[0].to_integer();
+    stats["used_labels_count"] = rows[7].to_vector()[0].to_integer();
+    stats["used_labels_nodes_count"] = rows[8].to_vector()[0].to_integer();
     return stats;
   };
 }
 
 sqlite::~sqlite()
 {}
 
@@ -8690,14 +8908,19 @@
 
 
 
 
 
 
 
+// Older version of SQLITE don*t have SQLITE_RESULT_SUBTYPE
+#ifndef SQLITE_RESULT_SUBTYPE
+#define SQLITE_RESULT_SUBTYPE 0
+#endif
+
 namespace gqlite::backends
 {
   template<typename... _TArgs_>
   void report_error(sqlite3_context* _context, exception_code _code, const std::string& _format, const _TArgs_&... _args)
   {
     value_map err;
     err["code"] = int64_t(_code);
@@ -8715,14 +8938,23 @@
   }
 #define SAFE(_X_)                             \
   try { _X_; }                                \
   catch(const exception& ex)                  \
   {                                           \
     report_exception(_context, ex); return;   \
   }
+
+#define NULL_CHECK_AT(_ARG_INDEX_)                            \
+  {                                                           \
+    if(sqlite3_value_type(_argv[_ARG_INDEX_]) == SQLITE_NULL) \
+    {                                                         \
+      sqlite3_result_null(_context); return ;                 \
+    }                                                         \
+  }
+
 #define NULL_CHECK(_ARGS_COUNT_)                      \
   for(std::size_t i = 0; i < _ARGS_COUNT_; ++i)       \
   {                                                   \
     if(sqlite3_value_type(_argv[i]) == SQLITE_NULL)   \
     {                                                 \
       sqlite3_result_null(_context); return ;         \
     }                                                 \
@@ -8831,15 +9063,15 @@
     return (compared_to_null) ? comparison_result::compared_null : comparison_result::true_result;
   }
   comparison_result contains(const gqlite::value_vector& _container, const gqlite::value& _value)
   {
     using enum value_type;
     if(_value.get_type() == invalid)
     {
-      return comparison_result::compared_null;
+      return _container.empty() ? comparison_result::false_result : comparison_result::compared_null;
     }
     bool has_compared_to_null = false;
     for(const value& v_c : _container)
     {
       switch(compare(v_c, _value))
       {
       case comparison_result::true_result:
@@ -9261,28 +9493,30 @@
         return;
       }
     }
     report_value(_context, val);
   }
   void gqlite_contains(sqlite3_context* _context,int,sqlite3_value** _argv)
   {
-    NULL_CHECK(2);
+    NULL_CHECK_AT(0);
     std::string left = reinterpret_cast<const char*>(sqlite3_value_text(_argv[0]));
     value val_left;
     SAFE(val_left = value::from_json(left));
     bool contains_result = false;
     switch(val_left.get_type())
     {
       case value_type::vector:
       {
-        std::string right = reinterpret_cast<const char*>(sqlite3_value_text(_argv[1]));
-        value_vector vv = val_left.to_vector();
         value val_right;
-        SAFE(val_right = value::from_json(right));
-
+        value_vector vv = val_left.to_vector();
+        if(sqlite3_value_type(_argv[1]) != SQLITE_NULL)
+        {
+          std::string right = reinterpret_cast<const char*>(sqlite3_value_text(_argv[1]));
+          SAFE(val_right = value::from_json(right));
+        }
         switch(contains(vv, val_right))
         {
         case comparison_result::true_result:
           contains_result = true;
           break;
         case comparison_result::false_result:
           contains_result = false;
@@ -9324,21 +9558,42 @@
       } else {
         report_value(_context, value_vector(std::next(vv.begin()), vv.end()));
       }
     } else {
       report_error(_context, exception_code::invalid_argument_type, "Invalid argument to function tail, list was expected.");
     }
   }
-
+  void gqlite_to_integer(sqlite3_context* _context,int,sqlite3_value** _argv)
+  {
+    int type = sqlite3_value_type(_argv[0]);
+    switch(type)
+    {
+      case SQLITE_INTEGER:
+        sqlite3_result_int64(_context, sqlite3_value_int64(_argv[0]));
+        break;
+      case SQLITE_FLOAT:
+        sqlite3_result_int64(_context, sqlite3_value_double(_argv[0]));
+        break;
+      case SQLITE_TEXT:
+      {
+        std::string s(reinterpret_cast<const char*>(sqlite3_value_text(_argv[0])));
+        sqlite3_result_int64(_context, std::stol(s));
+      }
+        break;
+      default:
+        report_error(_context, exception_code::invalid_argument_type, "Invalid arguments for toInteger.");
+    }
+  }
   void initialise_sqlite_ext(sqlite3* db)
   {
-    sqlite3_create_function(db, "gqlite_jsonify", 1, SQLITE_UTF8, nullptr, &gqlite_jsonify, nullptr, nullptr);
+    sqlite3_create_function(db, "gqlite_jsonify", 1, SQLITE_SUBTYPE | SQLITE_RESULT_SUBTYPE | SQLITE_UTF8, nullptr, &gqlite_jsonify, nullptr, nullptr);
     sqlite3_create_function(db, "gqlite_next_uid", 1, SQLITE_UTF8, nullptr, &gqlite_next_uid, nullptr, nullptr);
     sqlite3_create_function(db, "gqlite_range", 2, SQLITE_DETERMINISTIC | SQLITE_UTF8, nullptr, &gqlite_range, nullptr, nullptr);
     sqlite3_create_function(db, "gqlite_concat", 2, SQLITE_DETERMINISTIC | SQLITE_UTF8, nullptr, &gqlite_concat, nullptr, nullptr);
     sqlite3_create_function(db, "gqlite_addition", 2, SQLITE_DETERMINISTIC | SQLITE_UTF8, nullptr, &gqlite_addition, nullptr, nullptr);
     sqlite3_create_function(db, "gqlite_indexed_access", 2, SQLITE_DETERMINISTIC | SQLITE_UTF8, nullptr, &gqlite_indexed_access, nullptr, nullptr);
     sqlite3_create_function(db, "gqlite_range_access", 3, SQLITE_DETERMINISTIC | SQLITE_UTF8, nullptr, &gqlite_range_access, nullptr, nullptr);
     sqlite3_create_function(db, "gqlite_contains", 2, SQLITE_DETERMINISTIC | SQLITE_UTF8, nullptr, &gqlite_contains, nullptr, nullptr);
     sqlite3_create_function(db, "gqlite_tail", 1, SQLITE_DETERMINISTIC | SQLITE_UTF8, nullptr, &gqlite_tail, nullptr, nullptr);
+    sqlite3_create_function(db, "gqlite_to_integer", 1, SQLITE_DETERMINISTIC | SQLITE_UTF8, nullptr, &gqlite_to_integer, nullptr, nullptr);
   }
 }//END backends/sqlite_ext.cpp
```

### Comparing `gqlitedb-1.0.0/src/gqlite-c.h` & `gqlitedb-1.1.0/src/gqlite-c.h`

 * *Files identical despite different names*

### Comparing `gqlitedb-1.0.0/src/gqlite.h` & `gqlitedb-1.1.0/src/gqlite.h`

 * *Files identical despite different names*

