# Comparing `tmp/pyspatialml-0.21.tar.gz` & `tmp/pyspatialml-0.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspatialml-0.21.tar", last modified: Sat Aug  6 16:57:03 2022, max compression
+gzip compressed data, was "pyspatialml-0.22.0.tar", max compression
```

## Comparing `pyspatialml-0.21.tar` & `pyspatialml-0.22.0.tar`

### file list

```diff
@@ -1,83 +1,52 @@
-drwxr-xr-x   0 stevenpawley   (501) staff       (20)        0 2022-08-06 16:57:03.111324 pyspatialml-0.21/
--rw-r--r--   0 stevenpawley   (501) staff       (20)    35141 2022-01-30 04:05:23.000000 pyspatialml-0.21/LICENSE
--rw-r--r--   0 stevenpawley   (501) staff       (20)       52 2022-01-30 04:05:23.000000 pyspatialml-0.21/MANIFEST.in
--rw-r--r--   0 stevenpawley   (501) staff       (20)    17560 2022-08-06 16:57:03.111012 pyspatialml-0.21/PKG-INFO
--rw-r--r--   0 stevenpawley   (501) staff       (20)    17226 2022-08-03 05:43:21.000000 pyspatialml-0.21/README.md
-drwxr-xr-x   0 stevenpawley   (501) staff       (20)        0 2022-08-06 16:57:03.065794 pyspatialml-0.21/pyspatialml/
--rw-r--r--   0 stevenpawley   (501) staff       (20)       64 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/__init__.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)      618 2022-08-03 05:43:21.000000 pyspatialml-0.21/pyspatialml/_extraction.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     8831 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/_plotting.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     8184 2022-08-03 05:43:21.000000 pyspatialml-0.21/pyspatialml/_prediction.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     4227 2022-08-03 05:43:21.000000 pyspatialml-0.21/pyspatialml/_rasterbase.py
-drwxr-xr-x   0 stevenpawley   (501) staff       (20)        0 2022-08-06 16:57:03.103372 pyspatialml-0.21/pyspatialml/datasets/
--rw-r--r--   0 stevenpawley   (501) staff       (20)        0 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/__init__.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)    33305 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/chnl_dist.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)    33297 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/dem.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)    33300 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/dist.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)    70166 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/extracted_pixels.txt
--rw-r--r--   0 stevenpawley   (501) staff       (20)    33285 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/ffreq.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)    33286 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/landimg2.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)    33286 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/landimg3.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)    33286 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/landimg4.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)   870707 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/landsat96_labelled_pixels.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)   160290 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/landsat96_points.dbf
--rw-r--r--   0 stevenpawley   (501) staff       (20)      536 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/landsat96_points.prj
--rw-r--r--   0 stevenpawley   (501) staff       (20)    28100 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/landsat96_points.shp
--rw-r--r--   0 stevenpawley   (501) staff       (20)     8100 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/landsat96_points.shx
--rw-r--r--   0 stevenpawley   (501) staff       (20)     8938 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/landsat96_polygons.dbf
--rw-r--r--   0 stevenpawley   (501) staff       (20)      493 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/landsat96_polygons.prj
--rw-r--r--   0 stevenpawley   (501) staff       (20)     4756 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/landsat96_polygons.shp
--rw-r--r--   0 stevenpawley   (501) staff       (20)      372 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/landsat96_polygons.shx
--rw-r--r--   0 stevenpawley   (501) staff       (20)  4336805 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/landsat_multiband.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)   869907 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/lsat7_2000_10.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)   869907 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/lsat7_2000_20.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)   869907 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/lsat7_2000_30.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)   869905 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/lsat7_2000_40.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)   869905 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/lsat7_2000_50.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)   435771 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/lsat7_2000_70.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)    25062 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/meuse.dbf
--rw-r--r--   0 stevenpawley   (501) staff       (20)      434 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/meuse.prj
--rw-r--r--   0 stevenpawley   (501) staff       (20)      967 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/meuse.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     4440 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/meuse.shp
--rw-r--r--   0 stevenpawley   (501) staff       (20)     1340 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/meuse.shx
--rw-r--r--   0 stevenpawley   (501) staff       (20)    33327 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/mrvbf.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)      889 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/nc.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)    33293 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/rsp.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)    33307 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/slope.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)    33285 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/soil.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)   869411 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/strata.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)    33319 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/datasets/twi.tif
--rw-r--r--   0 stevenpawley   (501) staff       (20)     7989 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/preprocessing.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)    95090 2022-08-03 05:43:21.000000 pyspatialml-0.21/pyspatialml/raster.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)    17819 2022-08-03 05:43:21.000000 pyspatialml-0.21/pyspatialml/rasterlayer.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     1185 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/rasterstats.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)    13361 2022-08-03 05:43:21.000000 pyspatialml-0.21/pyspatialml/transformers.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     1438 2022-01-30 04:05:23.000000 pyspatialml-0.21/pyspatialml/vector.py
-drwxr-xr-x   0 stevenpawley   (501) staff       (20)        0 2022-08-06 16:57:03.067117 pyspatialml-0.21/pyspatialml.egg-info/
--rw-r--r--   0 stevenpawley   (501) staff       (20)    17560 2022-08-06 16:57:03.000000 pyspatialml-0.21/pyspatialml.egg-info/PKG-INFO
--rw-r--r--   0 stevenpawley   (501) staff       (20)     2239 2022-08-06 16:57:03.000000 pyspatialml-0.21/pyspatialml.egg-info/SOURCES.txt
--rw-r--r--   0 stevenpawley   (501) staff       (20)        1 2022-08-06 16:57:03.000000 pyspatialml-0.21/pyspatialml.egg-info/dependency_links.txt
--rw-r--r--   0 stevenpawley   (501) staff       (20)      129 2022-08-06 16:57:03.000000 pyspatialml-0.21/pyspatialml.egg-info/requires.txt
--rw-r--r--   0 stevenpawley   (501) staff       (20)       18 2022-08-06 16:57:03.000000 pyspatialml-0.21/pyspatialml.egg-info/top_level.txt
--rw-r--r--   0 stevenpawley   (501) staff       (20)       38 2022-08-06 16:57:03.111420 pyspatialml-0.21/setup.cfg
--rw-r--r--   0 stevenpawley   (501) staff       (20)     1185 2022-08-06 16:56:52.000000 pyspatialml-0.21/setup.py
-drwxr-xr-x   0 stevenpawley   (501) staff       (20)        0 2022-08-06 16:57:03.110589 pyspatialml-0.21/tests/
--rw-r--r--   0 stevenpawley   (501) staff       (20)        0 2022-01-30 04:05:23.000000 pyspatialml-0.21/tests/__init__.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)      799 2022-08-03 05:43:21.000000 pyspatialml-0.21/tests/test_alter.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     3048 2022-01-30 04:05:23.000000 pyspatialml-0.21/tests/test_append.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     2377 2022-01-30 04:05:23.000000 pyspatialml-0.21/tests/test_apply.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     1915 2022-08-03 05:43:21.000000 pyspatialml-0.21/tests/test_band_names.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     1260 2022-01-30 04:05:23.000000 pyspatialml-0.21/tests/test_crop.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     1887 2022-01-30 04:05:23.000000 pyspatialml-0.21/tests/test_drop.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     4342 2022-01-30 04:05:23.000000 pyspatialml-0.21/tests/test_extract.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     3501 2022-01-30 04:05:23.000000 pyspatialml-0.21/tests/test_indexing.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     3811 2022-01-30 04:05:23.000000 pyspatialml-0.21/tests/test_initiation.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     2160 2022-01-30 04:05:23.000000 pyspatialml-0.21/tests/test_intersect.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     2957 2022-01-30 04:05:23.000000 pyspatialml-0.21/tests/test_mask.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     1255 2022-01-30 04:05:23.000000 pyspatialml-0.21/tests/test_plotting.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     8009 2022-01-30 04:05:23.000000 pyspatialml-0.21/tests/test_prediction.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     4101 2022-01-30 04:05:23.000000 pyspatialml-0.21/tests/test_rename.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     1486 2022-08-03 05:43:21.000000 pyspatialml-0.21/tests/test_sample.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     1218 2022-01-30 04:05:23.000000 pyspatialml-0.21/tests/test_stats.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)     2018 2022-01-30 04:05:23.000000 pyspatialml-0.21/tests/test_tocrs.py
--rw-r--r--   0 stevenpawley   (501) staff       (20)      735 2022-01-30 04:05:23.000000 pyspatialml-0.21/tests/test_write.py
+-rw-r--r--   0        0        0    35141 2024-05-18 03:17:44.578611 pyspatialml-0.22.0/LICENSE
+-rw-r--r--   0        0        0    17229 2024-05-18 04:48:00.485702 pyspatialml-0.22.0/README.md
+-rw-r--r--   0        0        0      700 2024-05-18 15:27:58.682263 pyspatialml-0.22.0/pyproject.toml
+-rw-r--r--   0        0        0       64 2024-05-18 03:17:44.595025 pyspatialml-0.22.0/pyspatialml/__init__.py
+-rw-r--r--   0        0        0      618 2024-05-18 04:03:54.249762 pyspatialml-0.22.0/pyspatialml/_extraction.py
+-rw-r--r--   0        0        0     8831 2024-05-18 04:03:54.249907 pyspatialml-0.22.0/pyspatialml/_plotting.py
+-rw-r--r--   0        0        0     8184 2024-05-18 03:17:44.595549 pyspatialml-0.22.0/pyspatialml/_prediction.py
+-rw-r--r--   0        0        0     4227 2024-05-18 03:17:44.595630 pyspatialml-0.22.0/pyspatialml/_rasterbase.py
+-rw-r--r--   0        0        0        0 2024-05-18 03:17:44.595692 pyspatialml-0.22.0/pyspatialml/datasets/__init__.py
+-rw-r--r--   0        0        0    33305 2024-05-18 03:17:44.595866 pyspatialml-0.22.0/pyspatialml/datasets/chnl_dist.tif
+-rw-r--r--   0        0        0    33297 2024-05-18 03:17:44.595974 pyspatialml-0.22.0/pyspatialml/datasets/dem.tif
+-rw-r--r--   0        0        0    33300 2024-05-18 03:17:44.596068 pyspatialml-0.22.0/pyspatialml/datasets/dist.tif
+-rw-r--r--   0        0        0    70166 2024-05-18 04:48:00.487953 pyspatialml-0.22.0/pyspatialml/datasets/extracted_pixels.txt
+-rw-r--r--   0        0        0    33285 2024-05-18 03:17:44.596336 pyspatialml-0.22.0/pyspatialml/datasets/ffreq.tif
+-rw-r--r--   0        0        0    33286 2024-05-18 03:17:44.596453 pyspatialml-0.22.0/pyspatialml/datasets/landimg2.tif
+-rw-r--r--   0        0        0    33286 2024-05-18 03:17:44.596625 pyspatialml-0.22.0/pyspatialml/datasets/landimg3.tif
+-rw-r--r--   0        0        0    33286 2024-05-18 03:17:44.596794 pyspatialml-0.22.0/pyspatialml/datasets/landimg4.tif
+-rw-r--r--   0        0        0   870707 2024-05-18 03:17:44.598175 pyspatialml-0.22.0/pyspatialml/datasets/landsat96_labelled_pixels.tif
+-rw-r--r--   0        0        0   160290 2024-05-18 03:17:44.598833 pyspatialml-0.22.0/pyspatialml/datasets/landsat96_points.dbf
+-rw-r--r--   0        0        0      536 2024-05-18 04:48:00.498623 pyspatialml-0.22.0/pyspatialml/datasets/landsat96_points.prj
+-rw-r--r--   0        0        0    28100 2024-05-18 03:17:44.599051 pyspatialml-0.22.0/pyspatialml/datasets/landsat96_points.shp
+-rw-r--r--   0        0        0     8100 2024-05-18 03:17:44.599156 pyspatialml-0.22.0/pyspatialml/datasets/landsat96_points.shx
+-rw-r--r--   0        0        0     8938 2024-05-18 03:17:44.599287 pyspatialml-0.22.0/pyspatialml/datasets/landsat96_polygons.dbf
+-rw-r--r--   0        0        0      493 2024-05-18 04:48:00.498908 pyspatialml-0.22.0/pyspatialml/datasets/landsat96_polygons.prj
+-rw-r--r--   0        0        0     4756 2024-05-18 03:17:44.599434 pyspatialml-0.22.0/pyspatialml/datasets/landsat96_polygons.shp
+-rw-r--r--   0        0        0      372 2024-05-18 03:17:44.599484 pyspatialml-0.22.0/pyspatialml/datasets/landsat96_polygons.shx
+-rw-r--r--   0        0        0  4336805 2024-05-18 03:17:44.605376 pyspatialml-0.22.0/pyspatialml/datasets/landsat_multiband.tif
+-rw-r--r--   0        0        0   869907 2024-05-18 03:17:44.606729 pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_10.tif
+-rw-r--r--   0        0        0   869907 2024-05-18 03:17:44.608015 pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_20.tif
+-rw-r--r--   0        0        0   869907 2024-05-18 03:17:44.609461 pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_30.tif
+-rw-r--r--   0        0        0   869905 2024-05-18 03:17:44.610714 pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_40.tif
+-rw-r--r--   0        0        0   869905 2024-05-18 03:17:44.612145 pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_50.tif
+-rw-r--r--   0        0        0   435771 2024-05-18 03:17:44.613062 pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_70.tif
+-rw-r--r--   0        0        0    25062 2024-05-18 03:17:44.613170 pyspatialml-0.22.0/pyspatialml/datasets/meuse.dbf
+-rw-r--r--   0        0        0      434 2024-05-18 04:48:00.499193 pyspatialml-0.22.0/pyspatialml/datasets/meuse.prj
+-rw-r--r--   0        0        0      967 2024-05-18 04:48:00.499299 pyspatialml-0.22.0/pyspatialml/datasets/meuse.py
+-rw-r--r--   0        0        0     4440 2024-05-18 03:17:44.613379 pyspatialml-0.22.0/pyspatialml/datasets/meuse.shp
+-rw-r--r--   0        0        0     1340 2024-05-18 03:17:44.613445 pyspatialml-0.22.0/pyspatialml/datasets/meuse.shx
+-rw-r--r--   0        0        0    33327 2024-05-18 03:17:44.613547 pyspatialml-0.22.0/pyspatialml/datasets/mrvbf.tif
+-rw-r--r--   0        0        0      889 2024-05-18 04:48:00.499394 pyspatialml-0.22.0/pyspatialml/datasets/nc.py
+-rw-r--r--   0        0        0    33293 2024-05-18 03:17:44.613729 pyspatialml-0.22.0/pyspatialml/datasets/rsp.tif
+-rw-r--r--   0        0        0    33307 2024-05-18 03:17:44.613836 pyspatialml-0.22.0/pyspatialml/datasets/slope.tif
+-rw-r--r--   0        0        0    33285 2024-05-18 03:17:44.613952 pyspatialml-0.22.0/pyspatialml/datasets/soil.tif
+-rw-r--r--   0        0        0   869411 2024-05-18 03:17:44.614915 pyspatialml-0.22.0/pyspatialml/datasets/strata.tif
+-rw-r--r--   0        0        0    33319 2024-05-18 03:17:44.615036 pyspatialml-0.22.0/pyspatialml/datasets/twi.tif
+-rw-r--r--   0        0        0     8137 2024-05-18 04:48:00.499521 pyspatialml-0.22.0/pyspatialml/preprocessing.py
+-rw-r--r--   0        0        0    95089 2024-05-18 04:48:00.499896 pyspatialml-0.22.0/pyspatialml/raster.py
+-rw-r--r--   0        0        0    17937 2024-05-18 04:48:00.500055 pyspatialml-0.22.0/pyspatialml/rasterlayer.py
+-rw-r--r--   0        0        0     1185 2024-05-18 03:17:44.615450 pyspatialml-0.22.0/pyspatialml/rasterstats.py
+-rw-r--r--   0        0        0    15649 2024-05-18 03:17:44.615583 pyspatialml-0.22.0/pyspatialml/transformers.py
+-rw-r--r--   0        0        0     1438 2024-05-18 03:17:44.615642 pyspatialml-0.22.0/pyspatialml/vector.py
+-rw-r--r--   0        0        0    18404 1970-01-01 00:00:00.000000 pyspatialml-0.22.0/PKG-INFO
```

### Comparing `pyspatialml-0.21/LICENSE` & `pyspatialml-0.22.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/PKG-INFO` & `pyspatialml-0.22.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: pyspatialml
-Version: 0.21
-Summary: Machine learning for GIS spatial modelling
-Home-page: https://github.com/stevenpawley/pyspatialml
-Author: Steven Pawley
-Author-email: steven.pawley@gmail.com
-License: GNU
-Keywords: GIS
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Codecov test coverage](https://codecov.io/gh/stevenpawley/pyspatialml/branch/master/graph/badge.svg)](https://codecov.io/gh/stevenpawley/pyspatialml?branch=master)
 
 # Pyspatialml
 Machine learning classification and regression modelling for spatial raster data.
 
 ## Description
 `Pyspatialml` is a Python module for applying scikit-learn machine learning models to 'stacks' of raster datasets.
@@ -230,15 +217,15 @@
 
 ```
 stack.plot()
 ```
 
 ### Integration with Pandas
 
-Data from a Raster object can converted into a Pandas dataframe, with each pixel representing by a row, and columns
+Data from a Raster object can be converted into a Pandas dataframe, with each pixel representing by a row, and columns
 reflecting the x, y coordinates and the values of each RasterLayer in the Raster object:
 
 ```
 df = stack.to_pandas(max_pixels=50000, resampling='nearest')
 df.head()
 ```
```

### Comparing `pyspatialml-0.21/README.md` & `pyspatialml-0.22.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: pyspatialml
+Version: 0.22.0
+Summary: Machine learning classification and regression modelling for spatial raster data.
+Home-page: https://stevenpawley.github.io/Pyspatialml/
+License: GPL-3.0-or-later
+Author: Steven Pawley
+Author-email: dr.stevenpawley@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: affine (>=2.4.0,<3.0.0)
+Requires-Dist: geopandas (>=0.14.4,<0.15.0)
+Requires-Dist: matplotlib (>=3.9.0,<4.0.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: rasterio (>=1.3.10,<2.0.0)
+Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
+Requires-Dist: scipy (>=1.13.0,<2.0.0)
+Requires-Dist: shapely (>=2.0.4,<3.0.0)
+Requires-Dist: tqdm (>=4.66.4,<5.0.0)
+Project-URL: Repository, https://github.com/stevenpawley/Pyspatialml
+Description-Content-Type: text/markdown
+
 [![Codecov test coverage](https://codecov.io/gh/stevenpawley/pyspatialml/branch/master/graph/badge.svg)](https://codecov.io/gh/stevenpawley/pyspatialml?branch=master)
 
 # Pyspatialml
 Machine learning classification and regression modelling for spatial raster data.
 
 ## Description
 `Pyspatialml` is a Python module for applying scikit-learn machine learning models to 'stacks' of raster datasets.
@@ -217,15 +245,15 @@
 
 ```
 stack.plot()
 ```
 
 ### Integration with Pandas
 
-Data from a Raster object can converted into a Pandas dataframe, with each pixel representing by a row, and columns
+Data from a Raster object can be converted into a Pandas dataframe, with each pixel representing by a row, and columns
 reflecting the x, y coordinates and the values of each RasterLayer in the Raster object:
 
 ```
 df = stack.to_pandas(max_pixels=50000, resampling='nearest')
 df.head()
 ```
 
@@ -426,7 +454,8 @@
 # generate 5 random points in a single polygon
 random_points = [get_random_point_in_polygon(training_py.geometry[0]) for i in range(5)]
 
 # convert to a GeoDataFrame
 random_points = geopandas.GeoDataFrame(
   geometry=geopandas.GeoSeries(random_points))
 ```
+
```

### Comparing `pyspatialml-0.21/pyspatialml/_extraction.py` & `pyspatialml-0.22.0/pyspatialml/_extraction.py`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/_plotting.py` & `pyspatialml-0.22.0/pyspatialml/_plotting.py`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/_prediction.py` & `pyspatialml-0.22.0/pyspatialml/_prediction.py`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/_rasterbase.py` & `pyspatialml-0.22.0/pyspatialml/_rasterbase.py`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/chnl_dist.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/chnl_dist.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/dem.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/dem.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/dist.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/dist.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/extracted_pixels.txt` & `pyspatialml-0.22.0/pyspatialml/datasets/extracted_pixels.txt`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/ffreq.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/ffreq.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/landimg2.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/landimg2.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/landimg3.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/landimg3.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/landimg4.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/landimg4.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/landsat96_labelled_pixels.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/landsat96_labelled_pixels.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/landsat96_points.dbf` & `pyspatialml-0.22.0/pyspatialml/datasets/landsat96_points.dbf`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/landsat96_points.prj` & `pyspatialml-0.22.0/pyspatialml/datasets/landsat96_points.prj`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/landsat96_points.shp` & `pyspatialml-0.22.0/pyspatialml/datasets/landsat96_points.shp`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/landsat96_points.shx` & `pyspatialml-0.22.0/pyspatialml/datasets/landsat96_points.shx`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/landsat96_polygons.dbf` & `pyspatialml-0.22.0/pyspatialml/datasets/landsat96_polygons.dbf`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/landsat96_polygons.shp` & `pyspatialml-0.22.0/pyspatialml/datasets/landsat96_polygons.shp`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/landsat_multiband.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/landsat_multiband.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/lsat7_2000_10.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_10.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/lsat7_2000_20.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_20.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/lsat7_2000_30.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_30.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/lsat7_2000_40.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_40.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/lsat7_2000_50.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_50.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/lsat7_2000_70.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/lsat7_2000_70.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/meuse.dbf` & `pyspatialml-0.22.0/pyspatialml/datasets/meuse.dbf`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/meuse.py` & `pyspatialml-0.22.0/pyspatialml/datasets/meuse.py`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/meuse.shp` & `pyspatialml-0.22.0/pyspatialml/datasets/meuse.shp`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/meuse.shx` & `pyspatialml-0.22.0/pyspatialml/datasets/meuse.shx`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/mrvbf.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/mrvbf.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/nc.py` & `pyspatialml-0.22.0/pyspatialml/datasets/nc.py`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/rsp.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/rsp.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/slope.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/slope.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/soil.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/soil.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/strata.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/strata.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/datasets/twi.tif` & `pyspatialml-0.22.0/pyspatialml/datasets/twi.tif`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/preprocessing.py` & `pyspatialml-0.22.0/pyspatialml/preprocessing.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,15 +99,18 @@
     meta["dtype"] = xyarrays.dtype
 
     with rasterio.open(file_path, "w", **meta) as dst:
         dst.write(xyarrays)
 
     new_raster = Raster(file_path)
     names = ["x_coordinates", "y_coordinates"]
-    new_raster.rename({old: new for old, new in zip(new_raster.names, names)})
+    new_raster.rename(
+        {old: new for old, new in zip(new_raster.names, names)},
+        in_place=True
+    )
 
     return new_raster
 
 
 def rotated_coordinates(layer, file_path, n_angles=8, driver="GTiff"):
     """Generate 2d arrays with n_angles rotated coordinates.
 
@@ -144,15 +147,16 @@
     meta["count"] = n_angles
     meta["dtype"] = grids_directional.dtype
     with rasterio.open(file_path, "w", **meta) as dst:
         dst.write(grids_directional)
 
     new_raster = Raster(file_path)
     names = ["angle_" + str(i + 1) for i in range(n_angles)]
-    new_raster.rename({old: new for old, new in zip(new_raster.names, names)})
+    new_raster.rename({old: new for old, new in zip(new_raster.names, names)},
+                      in_place=True)
 
     return new_raster
 
 
 def distance_to_corners(layer, file_path, driver="GTiff"):
     """Generate buffer distances to corner and centre coordinates of raster
     extent.
@@ -190,15 +194,16 @@
     meta["count"] = 5
     meta["dtype"] = arr.dtype
 
     with rasterio.open(file_path, "w", **meta) as dst:
         dst.write(arr)
 
     new_raster = Raster(file_path)
-    new_raster.rename({old: new for old, new in zip(new_raster.names, names)})
+    new_raster.rename({old: new for old, new in zip(new_raster.names, names)},
+                      in_place=True)
 
     return new_raster
 
 
 def _grid_distance(shape, rows, cols):
     """Generate buffer distances to x,y coordinates.
     Parameters
@@ -276,10 +281,11 @@
     meta["dtype"] = arr.dtype
 
     with rasterio.open(file_path, "w", **meta) as dst:
         dst.write(arr)
 
     names = ["dist_sample" + str(i + 1) for i in range(len(rows))]
     new_raster = Raster(file_path)
-    new_raster.rename({old: new for old, new in zip(new_raster.names, names)})
+    new_raster.rename({old: new for old, new in zip(new_raster.names, names)},
+                      in_place=True)
 
     return new_raster
```

### Comparing `pyspatialml-0.21/pyspatialml/raster.py` & `pyspatialml-0.22.0/pyspatialml/raster.py`

 * *Files 0% similar despite different names*

```diff
@@ -2556,15 +2556,15 @@
         # lookup pixel values at row, col positons by chunk
         windows = [w for w in self.block_shapes(*self.block_shape)]
         data_gen = (self.read(window=w, masked=True) for w in windows)
         t = tqdm(windows, total=len(windows), disable=not progress)
 
         dtype = np.find_common_type([np.float32], self.dtypes)
         X = np.ma.zeros((self.count, 0), dtype=dtype)
-        pixel_indices = np.zeros(0, dtype=np.int)
+        pixel_indices = np.zeros(0, dtype="int")
 
         for w, data, pbar in zip(windows, data_gen, t):
             res, chunk_pixels = extract_by_chunk(data, w, rowcol_idx, pixel_index)
             X = np.ma.concatenate((X, res), axis=1)
             pixel_indices = np.concatenate((pixel_indices, chunk_pixels))
 
         X = X.transpose((1, 0))
```

### Comparing `pyspatialml-0.21/pyspatialml/rasterlayer.py` & `pyspatialml-0.22.0/pyspatialml/rasterlayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         """
 
         driver = self.driver
 
         if isinstance(other, RasterLayer):
             result = function(self.read(masked=True), other.read(masked=True))
         else:
-            result = function(self.read(masked=True))
+            result = function(self.read(masked=True), other)
 
         nodata = get_nodata_value(result.dtype)
 
         # open output file with updated metadata
         meta = self.meta.copy()
         meta.update(driver=driver, count=1, dtype=result.dtype, nodata=nodata)
 
@@ -432,14 +432,20 @@
                     "Invalid resampling method. Resampling "
                     "method must be one of {0}:".format(resampling_methods)
                 )
 
             kwargs["resampling"] = rasterio.enums.Resampling[kwargs["resampling"]]
 
         return self.ds.read(indexes=self.bidx, **kwargs)
+    
+    def seek(self, offset, whence=None):
+        return self
+    
+    def tell(self):
+        return self
 
     def write(self, file_path, driver="GTiff", dtype=None, nodata=None, **kwargs):
         """Write method for a single RasterLayer.
 
         Parameters
         ----------
         file_path : str (opt)
```

### Comparing `pyspatialml-0.21/pyspatialml/rasterstats.py` & `pyspatialml-0.22.0/pyspatialml/rasterstats.py`

 * *Files identical despite different names*

### Comparing `pyspatialml-0.21/pyspatialml/transformers.py` & `pyspatialml-0.22.0/pyspatialml/transformers.py`

 * *Files 6% similar despite different names*

```diff
@@ -366,9 +366,83 @@
 
     # predict and replace mask
     result = transformer.transform(flat_pixels)
 
     # reshape the prediction from a 1D into 3D array [band, row, col]
     result = result.reshape((n_features, rows, cols))
     result = np.ma.masked_array(data=result, mask=mask, copy=True)
-    
+
     return result
+
+
+class AspectTransformer(BaseEstimator, TransformerMixin):
+    """Transformer to decompose aspect maps into northerness and easterness"""
+
+    def __init__(self):
+        self._quadrants = None
+        self._reverse = np.array([0.0, 360.0])
+
+    def _dir_from_comp(self, X):
+        return np.rad2deg(np.arctan2(X[:, 1], X[:, 0]))
+
+    def fit(self, X, y=None):
+        return self
+
+    def fit_transform(self, X, y=None):
+        return self.transform(X, y)
+
+    def transform(self, X, y=None):
+        """Takes a vector of floating point numbers, assumed to be aspect in degrees
+        and returns an array with two dimensions with the strength of the easterly and
+        northernly direction
+
+        Parameters
+        ----------
+        X : array-like of sample {n_samples, n_features}
+            New samples for the prediction.
+
+        y : None
+            Not used.
+
+        Returns
+        -------
+        ndarray : 2d array with the sin and cosine components of the original
+            data.
+        """
+        # ensure that X is a ndarray
+        if isinstance(X, list):
+            X = np.asarray(X)
+
+        # store quadrant so that inverse can be found
+        condlist = [np.logical_and(X >= 0, X <= 180), np.logical_and(X > 180, X < 360)]
+        choicelist = np.arange(0, 2)
+        self._quadrants = np.select(condlist, choicelist)
+
+        radians = np.deg2rad(X)
+        easterness = np.cos(radians)
+        northerness = np.sin(radians)
+
+        return np.column_stack([easterness, northerness])
+
+    def inverse_transform(self, X, y=None):
+        """Takes a vector with two columns containing the strength of the easterly and
+        northernly directions and returns a array with a single dimension with the
+        azimuth in degrees
+
+        Because the quadrant is not known, this function only returns the azimuth
+        relative to a northernly direction
+
+        Parameters
+        ----------
+        X : array-like of sample {n_samples, n_features}
+            New samples for the prediction.
+
+        y : None
+            Not used.
+
+        Returns
+        -------
+        ndarray : 2d array with the azimuth.
+        """
+        inverse = self._dir_from_comp(X)
+        inverse = np.abs(inverse + self._reverse[self._quadrants])
+        return inverse
```

### Comparing `pyspatialml-0.21/pyspatialml/vector.py` & `pyspatialml-0.22.0/pyspatialml/vector.py`

 * *Files identical despite different names*

