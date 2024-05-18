# Comparing `tmp/pycellmech-2.1.0.tar.gz` & `tmp/pycellmech-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycellmech-2.1.0.tar", last modified: Sat May 18 00:30:36 2024, max compression
+gzip compressed data, was "dist/pycellmech-2.1.1.tar", last modified: Sat May 18 00:37:28 2024, max compression
```

## Comparing `pycellmech-2.1.0.tar` & `pycellmech-2.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 00:30:36.041329 pycellmech-2.1.0/
--rw-rw-r--   0 janan.arslan (31680)    10513       34 2024-05-18 00:12:55.000000 pycellmech-2.1.0/MANIFEST.in
--rw-r--r--   0 janan.arslan (31680)    10513      508 2024-05-18 00:30:36.041504 pycellmech-2.1.0/PKG-INFO
-drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 00:30:36.040967 pycellmech-2.1.0/pycellmech.egg-info/
--rw-r--r--   0 janan.arslan (31680)    10513      508 2024-05-18 00:30:35.000000 pycellmech-2.1.0/pycellmech.egg-info/PKG-INFO
--rw-r--r--   0 janan.arslan (31680)    10513      199 2024-05-18 00:30:35.000000 pycellmech-2.1.0/pycellmech.egg-info/SOURCES.txt
--rw-r--r--   0 janan.arslan (31680)    10513        1 2024-05-18 00:30:35.000000 pycellmech-2.1.0/pycellmech.egg-info/dependency_links.txt
--rw-r--r--   0 janan.arslan (31680)    10513       51 2024-05-18 00:30:35.000000 pycellmech-2.1.0/pycellmech.egg-info/requires.txt
--rw-r--r--   0 janan.arslan (31680)    10513        1 2024-05-18 00:30:35.000000 pycellmech-2.1.0/pycellmech.egg-info/top_level.txt
--rw-rw-r--   0 janan.arslan (31680)    10513       79 2024-05-18 00:30:36.043511 pycellmech-2.1.0/setup.cfg
--rw-rw-r--   0 janan.arslan (31680)    10513     1030 2024-05-18 00:30:29.000000 pycellmech-2.1.0/setup.py
+drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 00:37:28.027123 pycellmech-2.1.1/
+-rw-rw-r--   0 janan.arslan (31680)    10513       34 2024-05-18 00:12:55.000000 pycellmech-2.1.1/MANIFEST.in
+-rw-r--r--   0 janan.arslan (31680)    10513      508 2024-05-18 00:37:28.027309 pycellmech-2.1.1/PKG-INFO
+drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 00:37:28.026711 pycellmech-2.1.1/pycellmech.egg-info/
+-rw-r--r--   0 janan.arslan (31680)    10513      508 2024-05-18 00:37:27.000000 pycellmech-2.1.1/pycellmech.egg-info/PKG-INFO
+-rw-r--r--   0 janan.arslan (31680)    10513      199 2024-05-18 00:37:27.000000 pycellmech-2.1.1/pycellmech.egg-info/SOURCES.txt
+-rw-r--r--   0 janan.arslan (31680)    10513        1 2024-05-18 00:37:27.000000 pycellmech-2.1.1/pycellmech.egg-info/dependency_links.txt
+-rw-r--r--   0 janan.arslan (31680)    10513       56 2024-05-18 00:37:27.000000 pycellmech-2.1.1/pycellmech.egg-info/requires.txt
+-rw-r--r--   0 janan.arslan (31680)    10513        1 2024-05-18 00:37:27.000000 pycellmech-2.1.1/pycellmech.egg-info/top_level.txt
+-rw-rw-r--   0 janan.arslan (31680)    10513       79 2024-05-18 00:37:28.028981 pycellmech-2.1.1/setup.cfg
+-rw-rw-r--   0 janan.arslan (31680)    10513     1035 2024-05-18 00:36:26.000000 pycellmech-2.1.1/setup.py
```

### Comparing `pycellmech-2.1.0/setup.py` & `pycellmech-2.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 
 # Read the README.md file
 with open(os.path.join(current_directory, '../README.md'), encoding='utf-8') as f:
     long_description = f.read()    
 
 setup(
     name="pycellmech",
-    version="2.1.0",
+    version="2.1.1",
     author="Janan Arslan",
     author_email="janan.arslan@icm-institute.org",
     description="A shape-based feature extractor for medical and biological studies",
     long_description_content_type="text/markdown",
     url="https://github.com/icm-dac/pycellmech",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=[
-        "matplotlib"
-        "numpy"
-        "math"
-        "opencv-python"
-        "pandas"
+        "matplotlib",
+        "numpy",
+        "math",
+        "opencv-python",
+        "pandas",
         "scikit-learn"
     ],
     include_package_data=True,
 )
```

