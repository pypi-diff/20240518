# Comparing `tmp/glidergun-0.5.6.tar.gz` & `tmp/glidergun-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glidergun-0.5.6.tar", last modified: Fri May 17 11:44:34 2024, max compression
+gzip compressed data, was "glidergun-0.5.7.tar", last modified: Fri May 17 22:45:53 2024, max compression
```

## Comparing `glidergun-0.5.6.tar` & `glidergun-0.5.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 11:44:34.257897 glidergun-0.5.6/
--rw-rw-rw-   0        0        0     2832 2024-05-17 11:44:34.255452 glidergun-0.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     2148 2024-04-24 03:01:21.000000 glidergun-0.5.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 11:44:34.226870 glidergun-0.5.6/glidergun/
--rw-rw-rw-   0        0        0      438 2024-05-17 02:12:31.000000 glidergun-0.5.6/glidergun/__init__.py
--rw-rw-rw-   0        0        0    50020 2024-05-17 02:12:30.000000 glidergun-0.5.6/glidergun/_grid.py
--rw-rw-rw-   0        0        0     4200 2024-05-17 11:42:12.000000 glidergun-0.5.6/glidergun/_ipython.py
--rw-rw-rw-   0        0        0     1783 2024-04-24 03:01:21.000000 glidergun-0.5.6/glidergun/_literals.py
--rw-rw-rw-   0        0        0    10367 2024-05-17 02:12:25.000000 glidergun-0.5.6/glidergun/_stack.py
-drwxrwxrwx   0        0        0        0 2024-05-17 11:44:34.255187 glidergun-0.5.6/glidergun.egg-info/
--rw-rw-rw-   0        0        0     2832 2024-05-17 11:44:34.000000 glidergun-0.5.6/glidergun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2024-05-17 11:44:34.000000 glidergun-0.5.6/glidergun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 11:44:34.000000 glidergun-0.5.6/glidergun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-05-17 11:44:34.000000 glidergun-0.5.6/glidergun.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-17 11:44:34.000000 glidergun-0.5.6/glidergun.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      746 2024-05-17 11:43:31.000000 glidergun-0.5.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 11:44:34.257897 glidergun-0.5.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 22:45:53.198145 glidergun-0.5.7/
+-rw-rw-rw-   0        0        0     2832 2024-05-17 22:45:53.197148 glidergun-0.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2148 2024-04-24 03:01:21.000000 glidergun-0.5.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 22:45:53.167365 glidergun-0.5.7/glidergun/
+-rw-rw-rw-   0        0        0      438 2024-05-17 15:49:39.000000 glidergun-0.5.7/glidergun/__init__.py
+-rw-rw-rw-   0        0        0    50082 2024-05-17 15:49:45.000000 glidergun-0.5.7/glidergun/_grid.py
+-rw-rw-rw-   0        0        0     4140 2024-05-17 15:49:49.000000 glidergun-0.5.7/glidergun/_ipython.py
+-rw-rw-rw-   0        0        0     1783 2024-05-17 15:49:52.000000 glidergun-0.5.7/glidergun/_literals.py
+-rw-rw-rw-   0        0        0    10498 2024-05-17 15:49:55.000000 glidergun-0.5.7/glidergun/_stack.py
+drwxrwxrwx   0        0        0        0 2024-05-17 22:45:53.195144 glidergun-0.5.7/glidergun.egg-info/
+-rw-rw-rw-   0        0        0     2832 2024-05-17 22:45:53.000000 glidergun-0.5.7/glidergun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2024-05-17 22:45:53.000000 glidergun-0.5.7/glidergun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 22:45:53.000000 glidergun-0.5.7/glidergun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-17 22:45:53.000000 glidergun-0.5.7/glidergun.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-17 22:45:53.000000 glidergun-0.5.7/glidergun.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      746 2024-05-17 15:28:33.000000 glidergun-0.5.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 22:45:53.198145 glidergun-0.5.7/setup.cfg
```

### Comparing `glidergun-0.5.6/PKG-INFO` & `glidergun-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glidergun
-Version: 0.5.6
+Version: 0.5.7
 Summary: Map Algebra with NumPy
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/glidergun
 Project-URL: Bug Tracker, https://github.com/jshirota/glidergun/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `glidergun-0.5.6/README.md` & `glidergun-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `glidergun-0.5.6/glidergun/_grid.py` & `glidergun-0.5.7/glidergun/_grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -877,14 +877,16 @@
 
     def project(
         self,
         epsg: Union[int, CRS],
         resampling: Union[Resampling, ResamplingMethod] = "nearest",
     ) -> "Grid":
         crs = CRS.from_epsg(epsg) if isinstance(epsg, int) else epsg
+        if crs.wkt == self.crs.wkt:
+            return self
         transform, width, height = calculate_default_transform(
             self.crs, crs, self.width, self.height, *self.extent
         )
         return self._reproject(
             transform,
             crs,
             width,
```

### Comparing `glidergun-0.5.6/glidergun/_ipython.py` & `glidergun-0.5.7/glidergun/_ipython.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,19 +23,17 @@
 
         obj = obj.to_uint8_range()
 
         if isinstance(obj, Grid):
             plt.imshow(obj.data, cmap=color)
 
         elif isinstance(obj, Stack):
-            rgb = [
-                obj.grids[i - 1].data for i in (color if color else (1, 2, 3))]
+            rgb = [obj.grids[i - 1].data for i in (color if color else (1, 2, 3))]
             alpha = np.where(np.isfinite(rgb[0] + rgb[1] + rgb[2]), 255, 0)
-            plt.imshow(
-                np.dstack([*[np.asanyarray(g, "uint8") for g in rgb], alpha]))
+            plt.imshow(np.dstack([*[np.asanyarray(g, "uint8") for g in rgb], alpha]))
 
         plt.savefig(buffer, bbox_inches="tight", pad_inches=0)
         plt.close(figure)
         image = b64encode(buffer.getvalue()).decode()
         return f"data:image/png;base64, {image}"
 
 
@@ -52,25 +50,25 @@
     **kwargs,
 ):
     import folium
     import jinja2
 
     obj_4326 = obj.project(4326)
 
-    extent = Extent(obj_4326.xmin, max(obj_4326.ymin, -80),
-                    obj_4326.xmax, min(obj_4326.ymax, 80))
+    extent = Extent(
+        obj_4326.xmin, max(obj_4326.ymin, -85), obj_4326.xmax, min(obj_4326.ymax, 85)
+    )
 
     if obj_4326.extent != extent:
         obj_4326 = obj.clip(extent)
 
     obj_3857 = obj_4326.project(3857)
 
     figure = folium.Figure(width=str(width), height=height)
-    bounds = [[obj_4326.ymin, obj_4326.xmin],
-              [obj_4326.ymax, obj_4326.xmax]]
+    bounds = [[obj_4326.ymin, obj_4326.xmin], [obj_4326.ymax, obj_4326.xmax]]
 
     if folium_map is None:
         if basemap:
             tile_layer = folium.TileLayer(basemap, attr=attribution)
         else:
             tile_layer = folium.TileLayer(
                 tiles="https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/tile/{z}/{y}/{x}",
@@ -111,16 +109,15 @@
             thumbnail = _thumbnail(obj, obj._cmap)
             extent = obj.extent
         elif isinstance(obj, Stack):
             thumbnail = _thumbnail(obj, obj._rgb)
             extent = obj.extent
         return f'<div>{description}</div><img src="{thumbnail}" /><div>{extent}</div>'
 
-    # type: ignore
-    formatter = ipython.display_formatter.formatters["text/html"]
+    formatter = ipython.display_formatter.formatters["text/html"]  # type: ignore
     formatter.for_type(Grid, html)
     formatter.for_type(Stack, html)
     formatter.for_type(
         tuple,
         lambda items: (
             f"""
             <table>
```

### Comparing `glidergun-0.5.6/glidergun/_literals.py` & `glidergun-0.5.7/glidergun/_literals.py`

 * *Files identical despite different names*

### Comparing `glidergun-0.5.6/glidergun/_stack.py` & `glidergun-0.5.7/glidergun/_stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,18 @@
 
     def pca(self, n_components: int = 3):
         return stack(*pca(n_components, *self.grids))
 
     def project(
         self, epsg: Union[int, CRS], resampling: Resampling = Resampling.nearest
     ):
-        return self.each(lambda g: g.project(epsg, resampling))
+        crs = CRS.from_epsg(epsg) if isinstance(epsg, int) else epsg
+        if crs.wkt == self.crs.wkt:
+            return self
+        return self.each(lambda g: g.project(crs, resampling))
 
     def resample(
         self,
         cell_size: Union[Tuple[float, float], float],
         resampling: Resampling = Resampling.nearest,
     ):
         return self.each(lambda g: g.resample(cell_size, resampling))
```

### Comparing `glidergun-0.5.6/glidergun.egg-info/PKG-INFO` & `glidergun-0.5.7/glidergun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glidergun
-Version: 0.5.6
+Version: 0.5.7
 Summary: Map Algebra with NumPy
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/glidergun
 Project-URL: Bug Tracker, https://github.com/jshirota/glidergun/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `glidergun-0.5.6/pyproject.toml` & `glidergun-0.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "glidergun"
-version = "0.5.6"
+version = "0.5.7"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "Map Algebra with NumPy"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

