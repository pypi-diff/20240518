# Comparing `tmp/opticalpy-1.0.1.tar.gz` & `tmp/opticalpy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opticalpy-1.0.1.tar", last modified: Sat May 18 09:00:16 2024, max compression
+gzip compressed data, was "opticalpy-1.1.0.tar", last modified: Sat May 18 18:54:57 2024, max compression
```

## Comparing `opticalpy-1.0.1.tar` & `opticalpy-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 09:00:16.000000 opticalpy-1.0.1/
--rw-rw-rw-   0        0        0    35823 2024-05-18 07:43:32.000000 opticalpy-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    44369 2024-05-18 09:00:16.000000 opticalpy-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2498 2024-05-18 08:59:30.000000 opticalpy-1.0.1/README.md
--rw-rw-rw-   0        0        0      719 2024-05-18 08:59:47.000000 opticalpy-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-18 09:00:16.000000 opticalpy-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-18 09:00:16.000000 opticalpy-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-18 09:00:16.000000 opticalpy-1.0.1/src/opticalpy/
--rw-rw-rw-   0        0        0      190 2024-05-18 08:33:11.000000 opticalpy-1.0.1/src/opticalpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 09:00:16.000000 opticalpy-1.0.1/src/opticalpy/elems/
--rw-rw-rw-   0        0        0      644 2024-05-18 08:19:58.000000 opticalpy-1.0.1/src/opticalpy/elems/__init__.py
--rw-rw-rw-   0        0        0     4311 2024-05-18 08:43:55.000000 opticalpy-1.0.1/src/opticalpy/elems/beam.py
--rw-rw-rw-   0        0        0     3751 2024-05-18 08:40:50.000000 opticalpy-1.0.1/src/opticalpy/elems/grating.py
--rw-rw-rw-   0        0        0    12887 2024-05-18 08:34:25.000000 opticalpy-1.0.1/src/opticalpy/elems/lens.py
--rw-rw-rw-   0        0        0     2158 2024-05-18 08:01:04.000000 opticalpy-1.0.1/src/opticalpy/elems/material.py
--rw-rw-rw-   0        0        0     7303 2024-05-18 08:34:43.000000 opticalpy-1.0.1/src/opticalpy/elems/mirror.py
--rw-rw-rw-   0        0        0     2749 2024-05-18 08:34:53.000000 opticalpy-1.0.1/src/opticalpy/elems/telescope.py
--rw-rw-rw-   0        0        0     2818 2024-05-18 08:40:00.000000 opticalpy-1.0.1/src/opticalpy/optgroup.py
--rw-rw-rw-   0        0        0     3329 2024-05-18 07:56:43.000000 opticalpy-1.0.1/src/opticalpy/optic.py
--rw-rw-rw-   0        0        0     4867 2024-05-18 08:08:09.000000 opticalpy-1.0.1/src/opticalpy/ray.py
--rw-rw-rw-   0        0        0     1568 2024-05-18 08:39:13.000000 opticalpy-1.0.1/src/opticalpy/scene.py
--rw-rw-rw-   0        0        0     1285 2024-05-18 07:50:30.000000 opticalpy-1.0.1/src/opticalpy/utils.py
--rw-rw-rw-   0        0        0     1139 2024-05-18 08:29:09.000000 opticalpy-1.0.1/src/opticalpy/visualization.py
-drwxrwxrwx   0        0        0        0 2024-05-18 09:00:16.000000 opticalpy-1.0.1/src/opticalpy.egg-info/
--rw-rw-rw-   0        0        0    44369 2024-05-18 09:00:16.000000 opticalpy-1.0.1/src/opticalpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2024-05-18 09:00:16.000000 opticalpy-1.0.1/src/opticalpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 09:00:16.000000 opticalpy-1.0.1/src/opticalpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-18 09:00:16.000000 opticalpy-1.0.1/src/opticalpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 09:00:16.000000 opticalpy-1.0.1/src/opticalpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 18:54:56.000000 opticalpy-1.1.0/
+-rw-rw-rw-   0        0        0    35823 2024-05-18 09:02:46.000000 opticalpy-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0    44369 2024-05-18 18:54:57.000000 opticalpy-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2498 2024-05-18 09:07:48.000000 opticalpy-1.1.0/README.md
+-rw-rw-rw-   0        0        0      746 2024-05-18 18:49:25.000000 opticalpy-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-18 18:54:57.000000 opticalpy-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-18 18:54:56.000000 opticalpy-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-18 18:54:56.000000 opticalpy-1.1.0/src/opticalpy/
+-rw-rw-rw-   0        0        0      190 2024-05-18 09:02:46.000000 opticalpy-1.1.0/src/opticalpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:54:56.000000 opticalpy-1.1.0/src/opticalpy/elems/
+-rw-rw-rw-   0        0        0      682 2024-05-18 18:49:16.000000 opticalpy-1.1.0/src/opticalpy/elems/__init__.py
+-rw-rw-rw-   0        0        0     4311 2024-05-18 09:02:46.000000 opticalpy-1.1.0/src/opticalpy/elems/beam.py
+-rw-rw-rw-   0        0        0     2308 2024-05-18 18:53:17.000000 opticalpy-1.1.0/src/opticalpy/elems/filter.py
+-rw-rw-rw-   0        0        0     3751 2024-05-18 09:02:46.000000 opticalpy-1.1.0/src/opticalpy/elems/grating.py
+-rw-rw-rw-   0        0        0    12887 2024-05-18 09:02:46.000000 opticalpy-1.1.0/src/opticalpy/elems/lens.py
+-rw-rw-rw-   0        0        0     2158 2024-05-18 09:02:46.000000 opticalpy-1.1.0/src/opticalpy/elems/material.py
+-rw-rw-rw-   0        0        0     7303 2024-05-18 18:45:44.000000 opticalpy-1.1.0/src/opticalpy/elems/mirror.py
+-rw-rw-rw-   0        0        0     2749 2024-05-18 09:02:46.000000 opticalpy-1.1.0/src/opticalpy/elems/telescope.py
+-rw-rw-rw-   0        0        0     2818 2024-05-18 09:02:46.000000 opticalpy-1.1.0/src/opticalpy/optgroup.py
+-rw-rw-rw-   0        0        0     3393 2024-05-18 18:48:03.000000 opticalpy-1.1.0/src/opticalpy/optic.py
+-rw-rw-rw-   0        0        0     4867 2024-05-18 09:02:46.000000 opticalpy-1.1.0/src/opticalpy/ray.py
+-rw-rw-rw-   0        0        0     1568 2024-05-18 09:02:46.000000 opticalpy-1.1.0/src/opticalpy/scene.py
+-rw-rw-rw-   0        0        0     1285 2024-05-18 09:02:46.000000 opticalpy-1.1.0/src/opticalpy/utils.py
+-rw-rw-rw-   0        0        0     1139 2024-05-18 09:02:46.000000 opticalpy-1.1.0/src/opticalpy/visualization.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:54:56.000000 opticalpy-1.1.0/src/opticalpy.egg-info/
+-rw-rw-rw-   0        0        0    44369 2024-05-18 18:54:56.000000 opticalpy-1.1.0/src/opticalpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      633 2024-05-18 18:54:56.000000 opticalpy-1.1.0/src/opticalpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 18:54:56.000000 opticalpy-1.1.0/src/opticalpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-18 18:54:56.000000 opticalpy-1.1.0/src/opticalpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-18 18:54:56.000000 opticalpy-1.1.0/src/opticalpy.egg-info/top_level.txt
```

### Comparing `opticalpy-1.0.1/LICENSE` & `opticalpy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.1/PKG-INFO` & `opticalpy-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opticalpy
-Version: 1.0.1
+Version: 1.1.0
 Summary: Exact geometrical optics including dispersion to learn and design optical instruments
 Author-email: Aurélien Genin <aurelien.genin@polytechnique.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `opticalpy-1.0.1/README.md` & `opticalpy-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.1/src/opticalpy/elems/beam.py` & `opticalpy-1.1.0/src/opticalpy/elems/beam.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.1/src/opticalpy/elems/grating.py` & `opticalpy-1.1.0/src/opticalpy/elems/grating.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.1/src/opticalpy/elems/lens.py` & `opticalpy-1.1.0/src/opticalpy/elems/lens.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.1/src/opticalpy/elems/material.py` & `opticalpy-1.1.0/src/opticalpy/elems/material.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.1/src/opticalpy/elems/mirror.py` & `opticalpy-1.1.0/src/opticalpy/elems/mirror.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.1/src/opticalpy/elems/telescope.py` & `opticalpy-1.1.0/src/opticalpy/elems/telescope.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.1/src/opticalpy/optgroup.py` & `opticalpy-1.1.0/src/opticalpy/optgroup.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.1/src/opticalpy/optic.py` & `opticalpy-1.1.0/src/opticalpy/optic.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,25 @@
     def __init__(self, 
                  equations:list, 
                  extent:list[float],
                  scene:None=None,
                  group=None, 
                  origin:np.ndarray|list[float]=[0,0], 
                  rotation:float|u.Quantity=0*u.deg,
-                 label:str|None = None):
+                 label:str|None = None,
+                 color='k'):
         self.raw_equation_x = equations[0]
         self.raw_equation_y = equations[1]
         self.extent : list[float] = extent
         self.origin : np.ndarray = origin if type(origin)==np.ndarray else np.array(origin)
         self.rotation = rotation if type(rotation)==u.Quantity else rotation*u.deg
         self.sin, self.cos = np.sin(self.rotation).value, np.cos(self.rotation).value
         self.equation_x, self.equation_y = self.calc_equation()
         self.label : str|None = label
+        self.color = color
         self.scene = scene
         self.group = group
         if (self.scene is not None) & (self.group is None): self.scene.append(self)
         if self.group is not None: self.group.append(self)
         if self.scene is not None: self.hitbox : list[float] = self.calc_hitbox(self.scene.step)
 
     def calc_equation(self):
@@ -42,15 +44,15 @@
     def plot_hitbox(self, ax) -> None:
         l,r,b,t = self.hitbox
         ax.plot([l,r,r,l,l], [b,b,t,t,b], color='r', ls=':', alpha=0.5)
 
     def __plot__(self, ax) -> None:
         t = np.linspace(self.extent[0], self.extent[1], 100)
         x, y = self.equation_x(t), self.equation_y(t)
-        ax.plot(x, y, color='k')
+        ax.plot(x, y, color=self.color)
 
     def normal_angle(self, t:float) -> u.Quantity:
         equation_dx = grad(self.equation_x)
         equation_dy = grad(self.equation_y)
         normal = np.array([-equation_dy(t), equation_dx(t)])
         normal /= np.linalg.norm(normal)
         normal_angle = np.arctan2(normal[1], normal[0])*u.rad
```

### Comparing `opticalpy-1.0.1/src/opticalpy/ray.py` & `opticalpy-1.1.0/src/opticalpy/ray.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.1/src/opticalpy/scene.py` & `opticalpy-1.1.0/src/opticalpy/scene.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.1/src/opticalpy/utils.py` & `opticalpy-1.1.0/src/opticalpy/utils.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.1/src/opticalpy/visualization.py` & `opticalpy-1.1.0/src/opticalpy/visualization.py`

 * *Files identical despite different names*

### Comparing `opticalpy-1.0.1/src/opticalpy.egg-info/PKG-INFO` & `opticalpy-1.1.0/src/opticalpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opticalpy
-Version: 1.0.1
+Version: 1.1.0
 Summary: Exact geometrical optics including dispersion to learn and design optical instruments
 Author-email: Aurélien Genin <aurelien.genin@polytechnique.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `opticalpy-1.0.1/src/opticalpy.egg-info/SOURCES.txt` & `opticalpy-1.1.0/src/opticalpy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,12 +11,13 @@
 src/opticalpy.egg-info/PKG-INFO
 src/opticalpy.egg-info/SOURCES.txt
 src/opticalpy.egg-info/dependency_links.txt
 src/opticalpy.egg-info/requires.txt
 src/opticalpy.egg-info/top_level.txt
 src/opticalpy/elems/__init__.py
 src/opticalpy/elems/beam.py
+src/opticalpy/elems/filter.py
 src/opticalpy/elems/grating.py
 src/opticalpy/elems/lens.py
 src/opticalpy/elems/material.py
 src/opticalpy/elems/mirror.py
 src/opticalpy/elems/telescope.py
```

