# Comparing `tmp/referrers-0.5.0.tar.gz` & `tmp/referrers-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "referrers-0.5.0.tar", max compression
+gzip compressed data, was "referrers-0.5.1.tar", max compression
```

## Comparing `referrers-0.5.0.tar` & `referrers-0.5.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-05-07 22:48:31.845692 referrers-0.5.0/LICENSE
--rw-r--r--   0        0        0     7319 2024-05-07 22:48:31.845692 referrers-0.5.0/README.md
--rw-r--r--   0        0        0      372 2024-05-07 22:48:31.845692 referrers-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      130 2024-05-07 22:48:31.845692 referrers-0.5.0/src/referrers/__init__.py
--rw-r--r--   0        0        0    42056 2024-05-07 22:48:31.845692 referrers-0.5.0/src/referrers/impl.py
--rw-r--r--   0        0        0     7852 1970-01-01 00:00:00.000000 referrers-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-17 22:02:23.190553 referrers-0.5.1/LICENSE
+-rw-r--r--   0        0        0     7536 2024-05-17 22:02:23.190553 referrers-0.5.1/README.md
+-rw-r--r--   0        0        0      372 2024-05-17 22:02:23.190553 referrers-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-05-17 22:02:23.190553 referrers-0.5.1/src/referrers/__init__.py
+-rw-r--r--   0        0        0    42056 2024-05-17 22:02:23.190553 referrers-0.5.1/src/referrers/impl.py
+-rw-r--r--   0        0        0     8069 1970-01-01 00:00:00.000000 referrers-0.5.1/PKG-INFO
```

### Comparing `referrers-0.5.0/LICENSE` & `referrers-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `referrers-0.5.0/README.md` & `referrers-0.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: referrers
+Version: 0.5.1
+Summary: Finds the graph of referrers for a Python object
+Author: Neil Ferguson
+Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: networkx (>=3.1.0)
+Description-Content-Type: text/markdown
+
 # Referrers
 
 Referrers is a Python package that helps to answer the question **"what is holding
 a reference to this object?"**, which is useful for debugging memory leaks and other
 issues. It tries to assign a meaningful name to each reference to an object and
 returns a graph of referrers (including indirect referrers).
 
@@ -100,56 +115,63 @@
 For example, to print the referrers of the top 10 largest objects using 
 [Pympler](https://pympler.readthedocs.io/en/latest/):
 
 ```python
 from pympler import muppy
 import referrers
 
-top_10_objects = (muppy.sort(muppy.get_objects()))[-10:]
-top_10_objects.reverse()
-
-for obj in top_10_objects:
-    print(
-        referrers.get_referrer_graph(
-            obj,
-            exclude_object_ids=[id(top_10_objects)],
+def main():
+    top_10_objects = (muppy.sort(muppy.get_objects()))[-10:]
+    top_10_objects.reverse()
+    
+    for obj in top_10_objects:
+        print(
+            referrers.get_referrer_graph(
+                obj,
+                exclude_object_ids=[id(top_10_objects)],
+            )
         )
-    )
-
-
+        
+if __name__ == "__main__":
+    main()
 ```
 
 Note that this example sets the `search_for_untracked_objects` flag to `True` to try to find
 referrers for objects that are not tracked by the garbage collector. It also sets
 `exclude_object_ids` to exclude the `top_10_objects` variable from the graph.
 
 Here's how to find the referrers of all objects that have been created
 between two points in time:
 
 ```python
 import referrers
 from pympler import summary, muppy
 
-o1 = muppy.get_objects()
-my_dict = {'a': [1]}
-o2 = muppy.get_objects()
-
-o1_ids = {id(obj) for obj in o1}
-o2_ids = {id(obj): obj for obj in o2}
-diff = [obj for obj_id, obj in o2_ids.items() if obj_id not in o1_ids]
-
-summary.print_(summary.get_diff(summary.summarize(o1), summary.summarize(o2)))
-
-for obj in diff:
-    print(
-        referrers.get_referrer_graph(
-            obj,
-            exclude_object_ids=[id(o1), id(o2), id(diff), id(o2_ids)],
+def main():
+    o1 = muppy.get_objects()
+    my_dict = {'a': [1]}
+    o2 = muppy.get_objects()
+    
+    o1_ids = {id(obj) for obj in o1}
+    o2_ids = {id(obj): obj for obj in o2}
+    diff = [obj for obj_id, obj in o2_ids.items() if obj_id not in o1_ids]
+    
+    summary.print_(summary.get_diff(summary.summarize(o1), summary.summarize(o2)))
+    
+    for obj in diff:
+        print(
+            referrers.get_referrer_graph(
+                obj,
+                exclude_object_ids=[id(o1), id(o2), id(diff), id(o2_ids)],
+            )
         )
-    )
+
+if __name__ == '__main__':
+    main()
+
 ```
 
 This will print a summary of the objects that have been created between o1 and o2,
 as well as the variable names that reference these objects. This can be useful for finding
 memory leaks.
 
 ## Integration with NetworkX
@@ -267,7 +289,8 @@
     └─╼ ParentClass.member_variable (instance attribute) (id=4482048576)
         └─╼ my_func.local_variable (local) (id=4482048576)
 ```
 
 ## Source
 
 See [https://github.com/nfergu/referrers](https://github.com/nfergu/referrers) for the Github repo.
+
```

### Comparing `referrers-0.5.0/src/referrers/impl.py` & `referrers-0.5.1/src/referrers/impl.py`

 * *Files identical despite different names*

### Comparing `referrers-0.5.0/PKG-INFO` & `referrers-0.5.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: referrers
-Version: 0.5.0
-Summary: Finds the graph of referrers for a Python object
-Author: Neil Ferguson
-Requires-Python: >=3.8
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: networkx (>=3.1.0)
-Description-Content-Type: text/markdown
-
 # Referrers
 
 Referrers is a Python package that helps to answer the question **"what is holding
 a reference to this object?"**, which is useful for debugging memory leaks and other
 issues. It tries to assign a meaningful name to each reference to an object and
 returns a graph of referrers (including indirect referrers).
 
@@ -115,56 +100,63 @@
 For example, to print the referrers of the top 10 largest objects using 
 [Pympler](https://pympler.readthedocs.io/en/latest/):
 
 ```python
 from pympler import muppy
 import referrers
 
-top_10_objects = (muppy.sort(muppy.get_objects()))[-10:]
-top_10_objects.reverse()
-
-for obj in top_10_objects:
-    print(
-        referrers.get_referrer_graph(
-            obj,
-            exclude_object_ids=[id(top_10_objects)],
+def main():
+    top_10_objects = (muppy.sort(muppy.get_objects()))[-10:]
+    top_10_objects.reverse()
+    
+    for obj in top_10_objects:
+        print(
+            referrers.get_referrer_graph(
+                obj,
+                exclude_object_ids=[id(top_10_objects)],
+            )
         )
-    )
-
-
+        
+if __name__ == "__main__":
+    main()
 ```
 
 Note that this example sets the `search_for_untracked_objects` flag to `True` to try to find
 referrers for objects that are not tracked by the garbage collector. It also sets
 `exclude_object_ids` to exclude the `top_10_objects` variable from the graph.
 
 Here's how to find the referrers of all objects that have been created
 between two points in time:
 
 ```python
 import referrers
 from pympler import summary, muppy
 
-o1 = muppy.get_objects()
-my_dict = {'a': [1]}
-o2 = muppy.get_objects()
-
-o1_ids = {id(obj) for obj in o1}
-o2_ids = {id(obj): obj for obj in o2}
-diff = [obj for obj_id, obj in o2_ids.items() if obj_id not in o1_ids]
-
-summary.print_(summary.get_diff(summary.summarize(o1), summary.summarize(o2)))
-
-for obj in diff:
-    print(
-        referrers.get_referrer_graph(
-            obj,
-            exclude_object_ids=[id(o1), id(o2), id(diff), id(o2_ids)],
+def main():
+    o1 = muppy.get_objects()
+    my_dict = {'a': [1]}
+    o2 = muppy.get_objects()
+    
+    o1_ids = {id(obj) for obj in o1}
+    o2_ids = {id(obj): obj for obj in o2}
+    diff = [obj for obj_id, obj in o2_ids.items() if obj_id not in o1_ids]
+    
+    summary.print_(summary.get_diff(summary.summarize(o1), summary.summarize(o2)))
+    
+    for obj in diff:
+        print(
+            referrers.get_referrer_graph(
+                obj,
+                exclude_object_ids=[id(o1), id(o2), id(diff), id(o2_ids)],
+            )
         )
-    )
+
+if __name__ == '__main__':
+    main()
+
 ```
 
 This will print a summary of the objects that have been created between o1 and o2,
 as well as the variable names that reference these objects. This can be useful for finding
 memory leaks.
 
 ## Integration with NetworkX
@@ -282,8 +274,7 @@
     └─╼ ParentClass.member_variable (instance attribute) (id=4482048576)
         └─╼ my_func.local_variable (local) (id=4482048576)
 ```
 
 ## Source
 
 See [https://github.com/nfergu/referrers](https://github.com/nfergu/referrers) for the Github repo.
-
```

