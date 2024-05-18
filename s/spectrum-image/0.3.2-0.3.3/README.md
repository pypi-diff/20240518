# Comparing `tmp/spectrum_image-0.3.2.tar.gz` & `tmp/spectrum_image-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_image-0.3.2.tar", last modified: Sat May 18 00:49:05 2024, max compression
+gzip compressed data, was "spectrum_image-0.3.3.tar", last modified: Sat May 18 00:56:32 2024, max compression
```

## Comparing `spectrum_image-0.3.2.tar` & `spectrum_image-0.3.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-05-18 00:49:05.474372 spectrum_image-0.3.2/
--rw-r--r--   0 sung       (501) staff       (20)    35149 2024-03-12 18:53:01.000000 spectrum_image-0.3.2/LICENSE
--rw-r--r--   0 sung       (501) staff       (20)     1800 2024-05-18 00:49:05.474198 spectrum_image-0.3.2/PKG-INFO
--rw-r--r--   0 sung       (501) staff       (20)      922 2024-04-10 01:05:24.000000 spectrum_image-0.3.2/README.md
--rw-r--r--   0 sung       (501) staff       (20)      981 2024-05-18 00:49:02.000000 spectrum_image-0.3.2/pyproject.toml
--rw-r--r--   0 sung       (501) staff       (20)       38 2024-05-18 00:49:05.474410 spectrum_image-0.3.2/setup.cfg
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-05-18 00:49:05.471704 spectrum_image-0.3.2/src/
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-05-18 00:49:05.472265 spectrum_image-0.3.2/src/spectrum_image/
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-05-18 00:49:05.473650 spectrum_image-0.3.2/src/spectrum_image/EELS/
--rw-r--r--   0 sung       (501) staff       (20)    24186 2024-04-22 03:59:53.000000 spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_LP.py
--rw-r--r--   0 sung       (501) staff       (20)    23464 2024-04-22 04:04:52.000000 spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_SI.py
--rw-r--r--   0 sung       (501) staff       (20)    13359 2024-04-22 03:35:02.000000 spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_bgsub.py
--rw-r--r--   0 sung       (501) staff       (20)      764 2024-04-22 02:26:56.000000 spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_edge.py
--rw-r--r--   0 sung       (501) staff       (20)     1466 2024-03-26 23:43:32.000000 spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_lineshapes.py
--rw-r--r--   0 sung       (501) staff       (20)    12303 2024-04-22 02:15:06.000000 spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_util.py
--rw-r--r--   0 sung       (501) staff       (20)      582 2024-04-22 04:00:49.000000 spectrum_image-0.3.2/src/spectrum_image/EELS/__init__.py
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-05-18 00:49:05.473876 spectrum_image-0.3.2/src/spectrum_image/RIXS/
--rw-r--r--   0 sung       (501) staff       (20)    12352 2024-05-17 20:50:10.000000 spectrum_image-0.3.2/src/spectrum_image/RIXS/RIXS_EM.py
--rw-r--r--   0 sung       (501) staff       (20)      643 2024-04-22 04:42:02.000000 spectrum_image-0.3.2/src/spectrum_image/RIXS/__init__.py
--rw-r--r--   0 sung       (501) staff       (20)      280 2024-03-12 18:53:01.000000 spectrum_image-0.3.2/src/spectrum_image/__init__.py
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-05-18 00:49:05.474017 spectrum_image-0.3.2/src/spectrum_image.egg-info/
--rw-r--r--   0 sung       (501) staff       (20)     1800 2024-05-18 00:49:05.000000 spectrum_image-0.3.2/src/spectrum_image.egg-info/PKG-INFO
--rw-r--r--   0 sung       (501) staff       (20)      604 2024-05-18 00:49:05.000000 spectrum_image-0.3.2/src/spectrum_image.egg-info/SOURCES.txt
--rw-r--r--   0 sung       (501) staff       (20)        1 2024-05-18 00:49:05.000000 spectrum_image-0.3.2/src/spectrum_image.egg-info/dependency_links.txt
--rw-r--r--   0 sung       (501) staff       (20)       52 2024-05-18 00:49:05.000000 spectrum_image-0.3.2/src/spectrum_image.egg-info/requires.txt
--rw-r--r--   0 sung       (501) staff       (20)       15 2024-05-18 00:49:05.000000 spectrum_image-0.3.2/src/spectrum_image.egg-info/top_level.txt
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-05-18 00:56:32.615515 spectrum_image-0.3.3/
+-rw-r--r--   0 sung       (501) staff       (20)    35149 2024-03-12 18:53:01.000000 spectrum_image-0.3.3/LICENSE
+-rw-r--r--   0 sung       (501) staff       (20)     1800 2024-05-18 00:56:32.615326 spectrum_image-0.3.3/PKG-INFO
+-rw-r--r--   0 sung       (501) staff       (20)      922 2024-04-10 01:05:24.000000 spectrum_image-0.3.3/README.md
+-rw-r--r--   0 sung       (501) staff       (20)      981 2024-05-18 00:56:24.000000 spectrum_image-0.3.3/pyproject.toml
+-rw-r--r--   0 sung       (501) staff       (20)       38 2024-05-18 00:56:32.615557 spectrum_image-0.3.3/setup.cfg
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-05-18 00:56:32.612256 spectrum_image-0.3.3/src/
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-05-18 00:56:32.613303 spectrum_image-0.3.3/src/spectrum_image/
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-05-18 00:56:32.614704 spectrum_image-0.3.3/src/spectrum_image/EELS/
+-rw-r--r--   0 sung       (501) staff       (20)    24186 2024-04-22 03:59:53.000000 spectrum_image-0.3.3/src/spectrum_image/EELS/EELS_LP.py
+-rw-r--r--   0 sung       (501) staff       (20)    23464 2024-04-22 04:04:52.000000 spectrum_image-0.3.3/src/spectrum_image/EELS/EELS_SI.py
+-rw-r--r--   0 sung       (501) staff       (20)    13359 2024-04-22 03:35:02.000000 spectrum_image-0.3.3/src/spectrum_image/EELS/EELS_bgsub.py
+-rw-r--r--   0 sung       (501) staff       (20)      764 2024-04-22 02:26:56.000000 spectrum_image-0.3.3/src/spectrum_image/EELS/EELS_edge.py
+-rw-r--r--   0 sung       (501) staff       (20)     1466 2024-03-26 23:43:32.000000 spectrum_image-0.3.3/src/spectrum_image/EELS/EELS_lineshapes.py
+-rw-r--r--   0 sung       (501) staff       (20)    12303 2024-04-22 02:15:06.000000 spectrum_image-0.3.3/src/spectrum_image/EELS/EELS_util.py
+-rw-r--r--   0 sung       (501) staff       (20)      582 2024-04-22 04:00:49.000000 spectrum_image-0.3.3/src/spectrum_image/EELS/__init__.py
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-05-18 00:56:32.614953 spectrum_image-0.3.3/src/spectrum_image/RIXS/
+-rw-r--r--   0 sung       (501) staff       (20)    12474 2024-05-18 00:56:14.000000 spectrum_image-0.3.3/src/spectrum_image/RIXS/RIXS_EM.py
+-rw-r--r--   0 sung       (501) staff       (20)      643 2024-04-22 04:42:02.000000 spectrum_image-0.3.3/src/spectrum_image/RIXS/__init__.py
+-rw-r--r--   0 sung       (501) staff       (20)      280 2024-03-12 18:53:01.000000 spectrum_image-0.3.3/src/spectrum_image/__init__.py
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-05-18 00:56:32.615129 spectrum_image-0.3.3/src/spectrum_image.egg-info/
+-rw-r--r--   0 sung       (501) staff       (20)     1800 2024-05-18 00:56:32.000000 spectrum_image-0.3.3/src/spectrum_image.egg-info/PKG-INFO
+-rw-r--r--   0 sung       (501) staff       (20)      604 2024-05-18 00:56:32.000000 spectrum_image-0.3.3/src/spectrum_image.egg-info/SOURCES.txt
+-rw-r--r--   0 sung       (501) staff       (20)        1 2024-05-18 00:56:32.000000 spectrum_image-0.3.3/src/spectrum_image.egg-info/dependency_links.txt
+-rw-r--r--   0 sung       (501) staff       (20)       52 2024-05-18 00:56:32.000000 spectrum_image-0.3.3/src/spectrum_image.egg-info/requires.txt
+-rw-r--r--   0 sung       (501) staff       (20)       15 2024-05-18 00:56:32.000000 spectrum_image-0.3.3/src/spectrum_image.egg-info/top_level.txt
```

### Comparing `spectrum_image-0.3.2/LICENSE` & `spectrum_image-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.3.2/PKG-INFO` & `spectrum_image-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum_image
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python Package for EELS (Electron Energy Loss Spectroscopy) Analysis
 Author-email: Suk Hyun Sung <sukhsung@umich.edu>, Michale Colletta <mrc297@cornell.edu>, Alex Stangle <astangel@umich.edu>
 Project-URL: Homepage, https://github.com/sukhsung/spectrum-image
 Project-URL: Repository, https://github.com/sukhsung/spectrum-image
 Project-URL: Bug Tracker, https://github.com/sukhsung/spectrum-image/issues
 Keywords: Electron Microscopy,EELS,TEM,STEM,Electron Energy Loss Spectroscopy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spectrum_image-0.3.2/README.md` & `spectrum_image-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.3.2/pyproject.toml` & `spectrum_image-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spectrum_image"
-version = "0.3.2"
+version = "0.3.3"
 dependencies = [
   "numpy",
   "matplotlib",
   "jupyterlab",
   "ipympl",
   "scipy",
   "tqdm",
```

### Comparing `spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_LP.py` & `spectrum_image-0.3.3/src/spectrum_image/EELS/EELS_LP.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_SI.py` & `spectrum_image-0.3.3/src/spectrum_image/EELS/EELS_SI.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_bgsub.py` & `spectrum_image-0.3.3/src/spectrum_image/EELS/EELS_bgsub.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_edge.py` & `spectrum_image-0.3.3/src/spectrum_image/EELS/EELS_edge.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_lineshapes.py` & `spectrum_image-0.3.3/src/spectrum_image/EELS/EELS_lineshapes.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.3.2/src/spectrum_image/EELS/EELS_util.py` & `spectrum_image-0.3.3/src/spectrum_image/EELS/EELS_util.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.3.2/src/spectrum_image/EELS/__init__.py` & `spectrum_image-0.3.3/src/spectrum_image/EELS/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.3.2/src/spectrum_image/RIXS/RIXS_EM.py` & `spectrum_image-0.3.3/src/spectrum_image/RIXS/RIXS_EM.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,17 +130,19 @@
             self.ui['roi2'].set_active( False )
 
 
         # Check for integration flip
         if self.ui['ck_roisetting'].get_status()[1]:
             self.int_dir = 1
             self.ui['ck_roisetting'].labels[1].set_text('Integrate E-inc')
+            self.ax['spec'].set_xlabel('Energy Loss (eV)')
         else:
             self.int_dir = 0
             self.ui['ck_roisetting'].labels[1].set_text('Integrate E-loss')
+            self.ax['spec'].set_xlabel('Incident Energy (eV)')
 
         self.int_dir = int(self.ui['ck_roisetting'].get_status()[1])
         self.on_change_roi1()
         # self.on_change_roi2()
 
 
     def on_change_roi1(self):
```

### Comparing `spectrum_image-0.3.2/src/spectrum_image/RIXS/__init__.py` & `spectrum_image-0.3.3/src/spectrum_image/RIXS/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.3.2/src/spectrum_image.egg-info/PKG-INFO` & `spectrum_image-0.3.3/src/spectrum_image.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum_image
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python Package for EELS (Electron Energy Loss Spectroscopy) Analysis
 Author-email: Suk Hyun Sung <sukhsung@umich.edu>, Michale Colletta <mrc297@cornell.edu>, Alex Stangle <astangel@umich.edu>
 Project-URL: Homepage, https://github.com/sukhsung/spectrum-image
 Project-URL: Repository, https://github.com/sukhsung/spectrum-image
 Project-URL: Bug Tracker, https://github.com/sukhsung/spectrum-image/issues
 Keywords: Electron Microscopy,EELS,TEM,STEM,Electron Energy Loss Spectroscopy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spectrum_image-0.3.2/src/spectrum_image.egg-info/SOURCES.txt` & `spectrum_image-0.3.3/src/spectrum_image.egg-info/SOURCES.txt`

 * *Files identical despite different names*

