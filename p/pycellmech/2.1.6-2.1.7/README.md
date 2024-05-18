# Comparing `tmp/pycellmech-2.1.6.tar.gz` & `tmp/pycellmech-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycellmech-2.1.6.tar", last modified: Sat May 18 01:28:11 2024, max compression
+gzip compressed data, was "dist/pycellmech-2.1.7.tar", last modified: Sat May 18 01:44:06 2024, max compression
```

## Comparing `pycellmech-2.1.6.tar` & `pycellmech-2.1.7.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 01:28:11.851161 pycellmech-2.1.6/
--rw-rw-r--   0 janan.arslan (31680)    10513    14649 2024-05-18 00:12:55.000000 pycellmech-2.1.6/LICENSE.txt
--rw-rw-r--   0 janan.arslan (31680)    10513       42 2024-05-18 01:26:47.000000 pycellmech-2.1.6/MANIFEST.in
--rw-r--r--   0 janan.arslan (31680)    10513     7782 2024-05-18 01:28:11.851678 pycellmech-2.1.6/PKG-INFO
--rw-rw-r--   0 janan.arslan (31680)    10513     5873 2024-05-18 00:12:55.000000 pycellmech-2.1.6/README.md
-drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 01:28:11.841201 pycellmech-2.1.6/pycellmech/
-drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 01:28:11.850476 pycellmech-2.1.6/pycellmech/pycellmech.egg-info/
--rw-r--r--   0 janan.arslan (31680)    10513     7782 2024-05-18 01:28:11.000000 pycellmech-2.1.6/pycellmech/pycellmech.egg-info/PKG-INFO
--rw-r--r--   0 janan.arslan (31680)    10513      338 2024-05-18 01:28:11.000000 pycellmech-2.1.6/pycellmech/pycellmech.egg-info/SOURCES.txt
--rw-r--r--   0 janan.arslan (31680)    10513        1 2024-05-18 01:28:11.000000 pycellmech-2.1.6/pycellmech/pycellmech.egg-info/dependency_links.txt
--rw-r--r--   0 janan.arslan (31680)    10513       52 2024-05-18 01:28:11.000000 pycellmech-2.1.6/pycellmech/pycellmech.egg-info/entry_points.txt
--rw-r--r--   0 janan.arslan (31680)    10513       51 2024-05-18 01:28:11.000000 pycellmech-2.1.6/pycellmech/pycellmech.egg-info/requires.txt
--rw-r--r--   0 janan.arslan (31680)    10513        1 2024-05-18 01:28:11.000000 pycellmech-2.1.6/pycellmech/pycellmech.egg-info/top_level.txt
--rw-rw-r--   0 janan.arslan (31680)    10513       79 2024-05-18 01:28:11.853240 pycellmech-2.1.6/setup.cfg
--rw-rw-r--   0 janan.arslan (31680)    10513     1181 2024-05-18 01:28:06.000000 pycellmech-2.1.6/setup.py
+drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 01:44:06.592968 pycellmech-2.1.7/
+-rw-rw-r--   0 janan.arslan (31680)    10513       18 2024-05-18 01:40:03.000000 pycellmech-2.1.7/MANIFEST.in
+-rw-r--r--   0 janan.arslan (31680)    10513     7782 2024-05-18 01:44:06.593385 pycellmech-2.1.7/PKG-INFO
+-rw-rw-r--   0 janan.arslan (31680)    10513     5873 2024-05-18 00:12:55.000000 pycellmech-2.1.7/README.md
+-rw-rw-r--   0 janan.arslan (31680)    10513       79 2024-05-18 01:44:06.594545 pycellmech-2.1.7/setup.cfg
+-rw-rw-r--   0 janan.arslan (31680)    10513     1167 2024-05-18 01:36:38.000000 pycellmech-2.1.7/setup.py
+drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 01:44:06.577788 pycellmech-2.1.7/src/
+drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 01:44:06.585878 pycellmech-2.1.7/src/pycellmech/
+-rw-rw-r--   0 janan.arslan (31680)    10513      140 2024-05-18 01:25:31.000000 pycellmech-2.1.7/src/pycellmech/__init__.py
+-rw-r--r--   0 janan.arslan (31680)    10513      627 2024-05-18 01:32:02.000000 pycellmech-2.1.7/src/pycellmech/cli.py
+-rw-rw-r--   0 janan.arslan (31680)    10513    14907 2024-05-18 00:12:55.000000 pycellmech-2.1.7/src/pycellmech/geometric_shape_features.py
+-rw-rw-r--   0 janan.arslan (31680)    10513     8999 2024-05-18 01:43:54.000000 pycellmech-2.1.7/src/pycellmech/main.py
+-rw-rw-r--   0 janan.arslan (31680)    10513     9396 2024-05-18 00:12:55.000000 pycellmech-2.1.7/src/pycellmech/one_dimensional_features.py
+-rw-rw-r--   0 janan.arslan (31680)    10513    16979 2024-05-18 00:12:55.000000 pycellmech-2.1.7/src/pycellmech/polygonal_shape_features.py
+drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 01:44:06.592347 pycellmech-2.1.7/src/pycellmech.egg-info/
+-rw-r--r--   0 janan.arslan (31680)    10513     7782 2024-05-18 01:44:06.000000 pycellmech-2.1.7/src/pycellmech.egg-info/PKG-INFO
+-rw-r--r--   0 janan.arslan (31680)    10513      471 2024-05-18 01:44:06.000000 pycellmech-2.1.7/src/pycellmech.egg-info/SOURCES.txt
+-rw-r--r--   0 janan.arslan (31680)    10513        1 2024-05-18 01:44:06.000000 pycellmech-2.1.7/src/pycellmech.egg-info/dependency_links.txt
+-rw-r--r--   0 janan.arslan (31680)    10513       52 2024-05-18 01:44:06.000000 pycellmech-2.1.7/src/pycellmech.egg-info/entry_points.txt
+-rw-r--r--   0 janan.arslan (31680)    10513       51 2024-05-18 01:44:06.000000 pycellmech-2.1.7/src/pycellmech.egg-info/requires.txt
+-rw-r--r--   0 janan.arslan (31680)    10513       11 2024-05-18 01:44:06.000000 pycellmech-2.1.7/src/pycellmech.egg-info/top_level.txt
```

### Comparing `pycellmech-2.1.6/PKG-INFO` & `pycellmech-2.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycellmech
-Version: 2.1.6
+Version: 2.1.7
 Summary: A shape-based feature extractor for use in biological and medical studies.
 Home-page: https://github.com/icm-dac/pycellmech
 Author: Janan Arslan
 Author-email: janan.arslan@icm-institute.org
 License: UNKNOWN
 Description: <div align="left">
           <img width="15%" src="/figures/pyrcellmech_logo_v2.png" alt="pycellmech Logo">
```

### Comparing `pycellmech-2.1.6/README.md` & `pycellmech-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pycellmech-2.1.6/pycellmech/pycellmech.egg-info/PKG-INFO` & `pycellmech-2.1.7/src/pycellmech.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycellmech
-Version: 2.1.6
+Version: 2.1.7
 Summary: A shape-based feature extractor for use in biological and medical studies.
 Home-page: https://github.com/icm-dac/pycellmech
 Author: Janan Arslan
 Author-email: janan.arslan@icm-institute.org
 License: UNKNOWN
 Description: <div align="left">
           <img width="15%" src="/figures/pyrcellmech_logo_v2.png" alt="pycellmech Logo">
```

### Comparing `pycellmech-2.1.6/setup.py` & `pycellmech-2.1.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 readme_path = os.path.join(current_directory, './README.md')
 with open(readme_path, encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="pycellmech",
-    version="2.1.6",
+    version="2.1.7",
     author="Janan Arslan",
     author_email="janan.arslan@icm-institute.org",
     description="A shape-based feature extractor for use in biological and medical studies.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/icm-dac/pycellmech",
-    packages=find_packages(where='pycellmech'),
-    package_dir={'': 'pycellmech'},
+    packages=find_packages(where='src'),
+    package_dir={'': 'src'},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=[
```

