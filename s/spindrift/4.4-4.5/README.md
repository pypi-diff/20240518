# Comparing `tmp/spindrift-4.4-py3-none-any.whl.zip` & `tmp/spindrift-4.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15276 bytes, number of entries: 11
--rw-rw-r--  2.0 unx       59 b- defN 24-Jan-05 05:38 spindrift/__init__.py
+Zip file size: 15376 bytes, number of entries: 11
+-rw-rw-r--  2.0 unx       59 b- defN 24-May-18 02:36 spindrift/__init__.py
 -rw-rw-r--  2.0 unx     3369 b- defN 24-Jan-05 05:39 spindrift/cli.py
 -rw-rw-r--  2.0 unx      518 b- defN 24-Jan-05 05:39 spindrift/compat.py
--rw-rw-r--  2.0 unx    39047 b- defN 24-Jan-05 05:39 spindrift/packager.py
+-rw-rw-r--  2.0 unx    39419 b- defN 24-May-18 02:34 spindrift/packager.py
 -rw-rw-r--  2.0 unx     4145 b- defN 24-Jan-05 05:39 spindrift/wsgi.py
--rwxrwxr-x  2.0 unx      102 b- defN 24-Jan-05 05:40 spindrift-4.4.data/scripts/spindrift
--rw-r--r--  2.0 unx     1062 b- defN 24-Jan-05 05:40 spindrift-4.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx      999 b- defN 24-Jan-05 05:40 spindrift-4.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Jan-05 05:40 spindrift-4.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 24-Jan-05 05:40 spindrift-4.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      854 b- defN 24-Jan-05 05:40 spindrift-4.4.dist-info/RECORD
-11 files, 50257 bytes uncompressed, 13840 bytes compressed:  72.5%
+-rwxrwxr-x  2.0 unx      102 b- defN 24-May-18 02:37 spindrift-4.5.data/scripts/spindrift
+-rw-r--r--  2.0 unx     1062 b- defN 24-May-18 02:37 spindrift-4.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      999 b- defN 24-May-18 02:37 spindrift-4.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-18 02:37 spindrift-4.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 24-May-18 02:37 spindrift-4.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      854 b- defN 24-May-18 02:37 spindrift-4.5.dist-info/RECORD
+11 files, 50629 bytes uncompressed, 13940 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: spindrift/packager.py
 Comment: 
 
 Filename: spindrift/wsgi.py
 Comment: 
 
-Filename: spindrift-4.4.data/scripts/spindrift
+Filename: spindrift-4.5.data/scripts/spindrift
 Comment: 
 
-Filename: spindrift-4.4.dist-info/LICENSE
+Filename: spindrift-4.5.dist-info/LICENSE
 Comment: 
 
-Filename: spindrift-4.4.dist-info/METADATA
+Filename: spindrift-4.5.dist-info/METADATA
 Comment: 
 
-Filename: spindrift-4.4.dist-info/WHEEL
+Filename: spindrift-4.5.dist-info/WHEEL
 Comment: 
 
-Filename: spindrift-4.4.dist-info/top_level.txt
+Filename: spindrift-4.5.dist-info/top_level.txt
 Comment: 
 
-Filename: spindrift-4.4.dist-info/RECORD
+Filename: spindrift-4.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spindrift/__init__.py

```diff
@@ -1,3 +1,3 @@
 # Copyright 2017-2024, Ryan P. Kelly.
 
-__version__ = "4.4"
+__version__ = "4.5"
```

## spindrift/packager.py

```diff
@@ -1173,28 +1173,44 @@
         spindrift_wsgi_output_path = os.path.join(
             spindrift_output_path,
             "wsgi.py",
         )
         shutil.copyfile(wsgi_path, spindrift_wsgi_output_path)
 
 
+def indent_entry(entry, indent="        ")
+
+    ret_fp = io.StringIO()
+    entry_fp = io.StringIO(entry)
+
+    for line in entry_fp:
+        ret_fp.write(indent + line)
+
+    return ret_fp.getvalue()
+
+
 def write_flask_shim(path, entry):
     index_path = os.path.join(path, "index.py")
     with open(index_path, "w") as fp:
         fp.write("import spindrift.wsgi\n")
-        fp.write(entry)
         #fp.write("import sys\n")
         #fp.write("import logging\n")
         #fp.write("ch = logging.StreamHandler(sys.stdout)\n")
         #fp.write("ch.setLevel(logging.DEBUG)\n")
         #fp.write("formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')\n")
         #fp.write("ch.setFormatter(formatter)\n")
         #fp.write("logging.getLogger().addHandler(ch)\n")
         fp.write("\n")
+        fp.write("app = None\n")
+        fp.write("\n")
         fp.write("def handler(event, context):\n")
+        fp.write("    global app\n")
+        fp.write("    if app is None:\n")
+        fp.write(indent_entry(entry))
+        fp.write("\n")
         fp.write("    return spindrift.wsgi.handler(app, event, context)\n")
 
 
 def write_eb_shim(path, entry):
     index_path = os.path.join(path, "application.py")
     with open(index_path, "w") as fp:
         fp.write(entry)
```

## Comparing `spindrift-4.4.dist-info/LICENSE` & `spindrift-4.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `spindrift-4.4.dist-info/METADATA` & `spindrift-4.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spindrift
-Version: 4.4
+Version: 4.5
 Summary: package python applications for AWS Lambda, AWS Elastic Beanstalk, AWS Batch (Docker)
 Home-page: https://github.com/f0rk/spindrift
 Author: Ryan P. Kelly
 Author-email: ryan@ryankelly.us
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

