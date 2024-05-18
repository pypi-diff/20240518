# Comparing `tmp/yahist-1.9.5-py3-none-any.whl.zip` & `tmp/yahist-1.9.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 26225 bytes, number of entries: 8
+Zip file size: 26235 bytes, number of entries: 8
 -rw-r--r--  2.0 unx      111 b- defN 21-Feb-26 06:55 yahist/__init__.py
--rw-r--r--  2.0 unx    37774 b- defN 21-Apr-16 08:22 yahist/hist1d.py
--rw-r--r--  2.0 unx    30906 b- defN 21-Apr-02 01:13 yahist/hist2d.py
+-rw-r--r--  2.0 unx    37903 b- defN 21-May-05 23:52 yahist/hist1d.py
+-rw-r--r--  2.0 unx    30893 b- defN 21-May-01 05:57 yahist/hist2d.py
 -rw-r--r--  2.0 unx    18390 b- defN 21-Apr-08 01:34 yahist/utils.py
--rw-r--r--  2.0 unx      735 b- defN 21-Apr-16 08:37 yahist-1.9.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Apr-16 08:37 yahist-1.9.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 21-Apr-16 08:37 yahist-1.9.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      587 b- defN 21-Apr-16 08:37 yahist-1.9.5.dist-info/RECORD
-8 files, 88602 bytes uncompressed, 25217 bytes compressed:  71.5%
+-rw-r--r--  2.0 unx      735 b- defN 21-May-05 23:59 yahist-1.9.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-May-05 23:59 yahist-1.9.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 21-May-05 23:59 yahist-1.9.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      587 b- defN 21-May-05 23:59 yahist-1.9.6.dist-info/RECORD
+8 files, 88718 bytes uncompressed, 25227 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: yahist/hist2d.py
 Comment: 
 
 Filename: yahist/utils.py
 Comment: 
 
-Filename: yahist-1.9.5.dist-info/METADATA
+Filename: yahist-1.9.6.dist-info/METADATA
 Comment: 
 
-Filename: yahist-1.9.5.dist-info/WHEEL
+Filename: yahist-1.9.6.dist-info/WHEEL
 Comment: 
 
-Filename: yahist-1.9.5.dist-info/top_level.txt
+Filename: yahist-1.9.6.dist-info/top_level.txt
 Comment: 
 
-Filename: yahist-1.9.5.dist-info/RECORD
+Filename: yahist-1.9.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yahist/hist1d.py

```diff
@@ -955,45 +955,47 @@
             if is_listlike(obj[k]):
                 obj[k] = np.array(obj[k])
         hnew = cls()
         hnew.__dict__.update(obj)
         return hnew
 
     @classmethod
-    def from_bincounts(cls, counts, bins=None, errors=None):
+    def from_bincounts(cls, counts, bins=None, errors=None, **kwargs):
         """
         Creates histogram object from array of histogrammed counts,
         edges/bins, and optionally errors.
 
         Parameters
         ----------
         counts : array
             Array of bin counts
         bins : array, default None
             Array of bin edges. If not specified for Hist1D,
             uses `bins = np.arange(len(counts)+1)`.
         errors : array, default None
             Array of bin errors (optional)
+        **kwargs
+            Parameters to be passed to `Hist1D`/`Hist2D` constructor.
 
         Returns
         -------
         Hist
         """
-        hnew = cls()
+        hnew = cls(**kwargs)
         counts = np.asarray(counts)
         if cls.__name__ == "Hist1D":
             if bins is None:
                 bins = np.arange(len(counts) + 1)
             else:
                 bins = np.asarray(bins)
 
         hnew._counts = counts.astype(np.float64)
-        hnew._edges = bins
+        hnew._edges = np.asarray(bins)
         if errors is not None:
-            hnew._errors = errors
+            hnew._errors = np.asarray(errors)
         else:
             hnew._errors = hnew._counts ** 0.5
         return hnew
 
     @classmethod
     def from_random(
         cls, which="norm", params=[0.0, 1.0], size=1e5, random_state=None, **kwargs
```

## yahist/hist2d.py

```diff
@@ -106,15 +106,15 @@
 
         result = histogramdd_wrapper((xs, ys), bins, range, weights, overflow, threads,)
 
         counts, (edgesx, edgesy) = result
         counts = counts.T
 
         if weights is not None:
-            sumw2, _ = yahist.utils.histogramdd_wrapper(
+            sumw2, _ = histogramdd_wrapper(
                 (xs, ys), bins, range, weights ** 2, overflow, threads,
             )
             errors = sumw2 ** 0.5
             errors = errors.T
         else:
             errors = counts ** 0.5
```

## Comparing `yahist-1.9.5.dist-info/METADATA` & `yahist-1.9.6.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: yahist
-Version: 1.9.5
+Version: 1.9.6
 Summary: Yet another histogram object with numpy and matplotlib
 Home-page: https://github.com/aminnj/yahist
 Author: Nick Amin
 Author-email: amin.nj@gmail.com
 License: BSD
-Download-URL: https://github.com/aminnj/yahist/tarball/1.9.5
+Download-URL: https://github.com/aminnj/yahist/tarball/1.9.6
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2.7
 Requires-Dist: numpy
```

