# Comparing `tmp/pycellmech-2.1.2.tar.gz` & `tmp/pycellmech-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycellmech-2.1.2.tar", last modified: Sat May 18 00:42:33 2024, max compression
+gzip compressed data, was "dist/pycellmech-2.1.3.tar", last modified: Sat May 18 00:52:57 2024, max compression
```

## Comparing `pycellmech-2.1.2.tar` & `pycellmech-2.1.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 00:42:33.946275 pycellmech-2.1.2/
--rw-rw-r--   0 janan.arslan (31680)    10513       34 2024-05-18 00:12:55.000000 pycellmech-2.1.2/MANIFEST.in
--rw-r--r--   0 janan.arslan (31680)    10513      508 2024-05-18 00:42:33.946468 pycellmech-2.1.2/PKG-INFO
-drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 00:42:33.945889 pycellmech-2.1.2/pycellmech.egg-info/
--rw-r--r--   0 janan.arslan (31680)    10513      508 2024-05-18 00:42:33.000000 pycellmech-2.1.2/pycellmech.egg-info/PKG-INFO
--rw-r--r--   0 janan.arslan (31680)    10513      199 2024-05-18 00:42:33.000000 pycellmech-2.1.2/pycellmech.egg-info/SOURCES.txt
--rw-r--r--   0 janan.arslan (31680)    10513        1 2024-05-18 00:42:33.000000 pycellmech-2.1.2/pycellmech.egg-info/dependency_links.txt
--rw-r--r--   0 janan.arslan (31680)    10513       51 2024-05-18 00:42:33.000000 pycellmech-2.1.2/pycellmech.egg-info/requires.txt
--rw-r--r--   0 janan.arslan (31680)    10513        1 2024-05-18 00:42:33.000000 pycellmech-2.1.2/pycellmech.egg-info/top_level.txt
--rw-rw-r--   0 janan.arslan (31680)    10513       79 2024-05-18 00:42:33.948508 pycellmech-2.1.2/setup.cfg
--rw-rw-r--   0 janan.arslan (31680)    10513     1019 2024-05-18 00:42:21.000000 pycellmech-2.1.2/setup.py
+drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 00:52:57.547329 pycellmech-2.1.3/
+-rw-rw-r--   0 janan.arslan (31680)    10513       34 2024-05-18 00:12:55.000000 pycellmech-2.1.3/MANIFEST.in
+-rw-r--r--   0 janan.arslan (31680)    10513      508 2024-05-18 00:52:57.547605 pycellmech-2.1.3/PKG-INFO
+drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 00:52:57.546617 pycellmech-2.1.3/pycellmech.egg-info/
+-rw-r--r--   0 janan.arslan (31680)    10513      508 2024-05-18 00:52:57.000000 pycellmech-2.1.3/pycellmech.egg-info/PKG-INFO
+-rw-r--r--   0 janan.arslan (31680)    10513      236 2024-05-18 00:52:57.000000 pycellmech-2.1.3/pycellmech.egg-info/SOURCES.txt
+-rw-r--r--   0 janan.arslan (31680)    10513        1 2024-05-18 00:52:57.000000 pycellmech-2.1.3/pycellmech.egg-info/dependency_links.txt
+-rw-r--r--   0 janan.arslan (31680)    10513       52 2024-05-18 00:52:57.000000 pycellmech-2.1.3/pycellmech.egg-info/entry_points.txt
+-rw-r--r--   0 janan.arslan (31680)    10513       51 2024-05-18 00:52:57.000000 pycellmech-2.1.3/pycellmech.egg-info/requires.txt
+-rw-r--r--   0 janan.arslan (31680)    10513        1 2024-05-18 00:52:57.000000 pycellmech-2.1.3/pycellmech.egg-info/top_level.txt
+-rw-rw-r--   0 janan.arslan (31680)    10513       79 2024-05-18 00:52:57.551549 pycellmech-2.1.3/setup.cfg
+-rw-rw-r--   0 janan.arslan (31680)    10513     1131 2024-05-18 00:52:51.000000 pycellmech-2.1.3/setup.py
```

### Comparing `pycellmech-2.1.2/setup.py` & `pycellmech-2.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read the README.md file
 with open(os.path.join(current_directory, '../README.md'), encoding='utf-8') as f:
     long_description = f.read()    
 
 setup(
     name="pycellmech",
-    version="2.1.2",
+    version="2.1.3",
     author="Janan Arslan",
     author_email="janan.arslan@icm-institute.org",
     description="A shape-based feature extractor for medical and biological studies",
     long_description_content_type="text/markdown",
     url="https://github.com/icm-dac/pycellmech",
     packages=find_packages(),
     classifiers=[
@@ -27,8 +27,13 @@
         "matplotlib",
         "numpy",
         "opencv-python",
         "pandas",
         "scikit-learn"
     ],
     include_package_data=True,
+    entry_points={
+        'console_scripts': [
+            'pycellmech=pycellmech.cli:main',
+        ],
+    },
 )
```

