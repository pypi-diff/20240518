# Comparing `tmp/chromophile-1.0.3.tar.gz` & `tmp/chromophile-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromophile-1.0.3.tar", last modified: Tue Sep 19 03:28:29 2023, max compression
+gzip compressed data, was "chromophile-1.0.5.tar", last modified: Sat May 18 02:58:18 2024, max compression
```

## Comparing `chromophile-1.0.3.tar` & `chromophile-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 krh        (501) staff       (20)        0 2023-09-19 03:28:29.094533 chromophile-1.0.3/
--rw-r--r--   0 krh        (501) staff       (20)     7048 2023-09-18 02:48:22.000000 chromophile-1.0.3/LICENSE.txt
--rw-r--r--   0 krh        (501) staff       (20)       31 2023-09-18 02:48:22.000000 chromophile-1.0.3/MANIFEST.in
--rw-r--r--   0 krh        (501) staff       (20)    10800 2023-09-19 03:28:29.094367 chromophile-1.0.3/PKG-INFO
--rw-r--r--   0 krh        (501) staff       (20)     1995 2023-09-18 02:48:22.000000 chromophile-1.0.3/README.rst
-drwxr-xr-x   0 krh        (501) staff       (20)        0 2023-09-19 03:28:29.091134 chromophile-1.0.3/chromophile/
--rw-r--r--   0 krh        (501) staff       (20)     9900 2023-09-18 02:48:22.000000 chromophile-1.0.3/chromophile/__init__.py
--rw-r--r--   0 krh        (501) staff       (20)    48864 2023-09-18 02:48:22.000000 chromophile-1.0.3/chromophile/_cmaps.dat
-drwxr-xr-x   0 krh        (501) staff       (20)        0 2023-09-19 03:28:29.093337 chromophile-1.0.3/chromophile.egg-info/
--rw-r--r--   0 krh        (501) staff       (20)    10800 2023-09-19 03:28:29.000000 chromophile-1.0.3/chromophile.egg-info/PKG-INFO
--rw-r--r--   0 krh        (501) staff       (20)      272 2023-09-19 03:28:29.000000 chromophile-1.0.3/chromophile.egg-info/SOURCES.txt
--rw-r--r--   0 krh        (501) staff       (20)        1 2023-09-19 03:28:29.000000 chromophile-1.0.3/chromophile.egg-info/dependency_links.txt
--rw-r--r--   0 krh        (501) staff       (20)       12 2023-09-19 03:28:29.000000 chromophile-1.0.3/chromophile.egg-info/top_level.txt
--rw-r--r--   0 krh        (501) staff       (20)      866 2023-09-18 02:48:22.000000 chromophile-1.0.3/pyproject.toml
--rw-r--r--   0 krh        (501) staff       (20)      147 2023-09-19 03:28:29.094990 chromophile-1.0.3/setup.cfg
-drwxr-xr-x   0 krh        (501) staff       (20)        0 2023-09-19 03:28:29.093645 chromophile-1.0.3/tests/
--rw-r--r--   0 krh        (501) staff       (20)     3386 2023-09-18 02:48:22.000000 chromophile-1.0.3/tests/test_chromophile.py
+drwxr-xr-x   0 krh        (501) staff       (20)        0 2024-05-18 02:58:18.145429 chromophile-1.0.5/
+-rw-r--r--   0 krh        (501) staff       (20)     7048 2024-05-17 05:15:20.000000 chromophile-1.0.5/LICENSE.txt
+-rw-r--r--   0 krh        (501) staff       (20)       31 2024-05-17 05:15:20.000000 chromophile-1.0.5/MANIFEST.in
+-rw-r--r--   0 krh        (501) staff       (20)    10800 2024-05-18 02:58:18.145299 chromophile-1.0.5/PKG-INFO
+-rw-r--r--   0 krh        (501) staff       (20)     1995 2024-05-17 05:15:20.000000 chromophile-1.0.5/README.rst
+drwxr-xr-x   0 krh        (501) staff       (20)        0 2024-05-18 02:58:18.142135 chromophile-1.0.5/chromophile/
+-rw-r--r--   0 krh        (501) staff       (20)     9900 2024-05-17 05:15:20.000000 chromophile-1.0.5/chromophile/__init__.py
+-rw-r--r--   0 krh        (501) staff       (20)    48864 2024-05-17 05:15:20.000000 chromophile-1.0.5/chromophile/_cmaps.dat
+drwxr-xr-x   0 krh        (501) staff       (20)        0 2024-05-18 02:58:18.144921 chromophile-1.0.5/chromophile.egg-info/
+-rw-r--r--   0 krh        (501) staff       (20)    10800 2024-05-18 02:58:18.000000 chromophile-1.0.5/chromophile.egg-info/PKG-INFO
+-rw-r--r--   0 krh        (501) staff       (20)      272 2024-05-18 02:58:18.000000 chromophile-1.0.5/chromophile.egg-info/SOURCES.txt
+-rw-r--r--   0 krh        (501) staff       (20)        1 2024-05-18 02:58:18.000000 chromophile-1.0.5/chromophile.egg-info/dependency_links.txt
+-rw-r--r--   0 krh        (501) staff       (20)       12 2024-05-18 02:58:18.000000 chromophile-1.0.5/chromophile.egg-info/top_level.txt
+-rw-r--r--   0 krh        (501) staff       (20)      866 2024-05-17 05:15:20.000000 chromophile-1.0.5/pyproject.toml
+-rw-r--r--   0 krh        (501) staff       (20)      147 2024-05-18 02:58:18.145842 chromophile-1.0.5/setup.cfg
+drwxr-xr-x   0 krh        (501) staff       (20)        0 2024-05-18 02:58:18.144304 chromophile-1.0.5/tests/
+-rw-r--r--   0 krh        (501) staff       (20)     3386 2024-05-17 05:15:20.000000 chromophile-1.0.5/tests/test_chromophile.py
```

### Comparing `chromophile-1.0.3/LICENSE.txt` & `chromophile-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chromophile-1.0.3/PKG-INFO` & `chromophile-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromophile
-Version: 1.0.3
+Version: 1.0.5
 Summary: Color maps for continuous quantitative data
 Author-email: Kyle Hofmann <kyle.hofmann@gmail.com>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
             CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
```

### Comparing `chromophile-1.0.3/README.rst` & `chromophile-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `chromophile-1.0.3/chromophile/__init__.py` & `chromophile-1.0.5/chromophile/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 objects.  They are also displayed in the online documentation.
 """
 
 import importlib.resources
 import itertools
 
 
-__version__ = '1.0.3'
+__version__ = '1.0.5'
 __all__ = ('cmap', 'palette')
 
 _INDEX = (
     ('cp_cyc_isolum_dark', 360),
     ('cp_cyc_isolum_light', 360),
     ('cp_cyc_isolum_wide', 360),
     ('cp_cyc_red_cyan_valley', 360),
```

### Comparing `chromophile-1.0.3/chromophile/_cmaps.dat` & `chromophile-1.0.5/chromophile/_cmaps.dat`

 * *Files identical despite different names*

### Comparing `chromophile-1.0.3/chromophile.egg-info/PKG-INFO` & `chromophile-1.0.5/chromophile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromophile
-Version: 1.0.3
+Version: 1.0.5
 Summary: Color maps for continuous quantitative data
 Author-email: Kyle Hofmann <kyle.hofmann@gmail.com>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
             CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
```

### Comparing `chromophile-1.0.3/pyproject.toml` & `chromophile-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.9"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chromophile"
-version = "1.0.3"
+version = "1.0.5"
 authors = [
   { name="Kyle Hofmann", email="kyle.hofmann@gmail.com" },
 ]
 description = "Color maps for continuous quantitative data"
 readme = "README.rst"
 license = { file="LICENSE.txt" }
 requires-python = ">=3.7"
```

### Comparing `chromophile-1.0.3/tests/test_chromophile.py` & `chromophile-1.0.5/tests/test_chromophile.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     ('cp_lemon_lime', 'cp_seq_green_yellow_cw'),
     ('cp_red', 'cp_seq_red_pink_cw1'),
     ('cp_orange', 'cp_seq_red_yellow_ccw'),
     )
 
 
 def test_version():
-    assert cp.__version__ == '1.0.3'
+    assert cp.__version__ == '1.0.5'
 
 
 def test_palette_cmap_name_consistency():
     _ = pytest.importorskip("matplotlib")
     for name in cp.palette.keys():
         assert name in cp.cmap.keys()
     for name in cp.cmap.keys():
```

