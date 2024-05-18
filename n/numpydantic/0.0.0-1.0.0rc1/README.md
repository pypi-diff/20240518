# Comparing `tmp/numpydantic-0.0.0.tar.gz` & `tmp/numpydantic-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpydantic-0.0.0.tar", max compression
+gzip compressed data, was "numpydantic-1.0.0rc1.tar", last modified: Sat May 18 01:21:16 2024, max compression
```

## Comparing `numpydantic-0.0.0.tar` & `numpydantic-1.0.0rc1.tar`

### file list

```diff
@@ -1,5 +1,34 @@
--rw-r--r--   0        0        0     1071 2024-02-02 01:53:21.226339 numpydantic-0.0.0/LICENSE
--rw-r--r--   0        0        0       94 2024-02-02 01:53:21.226466 numpydantic-0.0.0/README.md
--rw-r--r--   0        0        0        2 2024-02-02 01:53:45.747824 numpydantic-0.0.0/numpydantic/__init__.py
--rw-r--r--   0        0        0      382 2024-02-02 01:54:22.114280 numpydantic-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 numpydantic-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-02-02 01:53:21.226339 numpydantic-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     3919 2024-04-03 23:31:57.506716 numpydantic-1.0.0rc1/README.md
+-rw-r--r--   0        0        0     2056 2024-05-18 01:21:16.860265 numpydantic-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-04-04 03:21:40.424457 numpydantic-1.0.0rc1/src/numpydantic/.DS_Store
+-rw-r--r--   0        0        0      316 2024-04-23 02:35:29.607872 numpydantic-1.0.0rc1/src/numpydantic/__init__.py
+-rw-r--r--   0        0        0     2759 2024-05-16 05:09:35.686033 numpydantic-1.0.0rc1/src/numpydantic/dtype.py
+-rw-r--r--   0        0        0      197 2024-04-23 02:36:10.489339 numpydantic-1.0.0rc1/src/numpydantic/exceptions.py
+-rw-r--r--   0        0        0      443 2024-05-09 05:06:59.484309 numpydantic-1.0.0rc1/src/numpydantic/interface/__init__.py
+-rw-r--r--   0        0        0     1543 2024-05-18 00:28:09.845192 numpydantic-1.0.0rc1/src/numpydantic/interface/dask.py
+-rw-r--r--   0        0        0     6497 2024-05-18 00:28:27.564833 numpydantic-1.0.0rc1/src/numpydantic/interface/hdf5.py
+-rw-r--r--   0        0        0     6302 2024-05-18 01:08:19.698258 numpydantic-1.0.0rc1/src/numpydantic/interface/interface.py
+-rw-r--r--   0        0        0     1550 2024-05-18 00:53:46.935649 numpydantic-1.0.0rc1/src/numpydantic/interface/numpy.py
+-rw-r--r--   0        0        0       47 2024-04-23 02:47:24.151838 numpydantic-1.0.0rc1/src/numpydantic/interface/xarray.py
+-rw-r--r--   0        0        0     4153 2024-05-18 00:34:12.796438 numpydantic-1.0.0rc1/src/numpydantic/interface/zarr.py
+-rw-r--r--   0        0        0     1470 2024-05-18 01:05:09.799203 numpydantic-1.0.0rc1/src/numpydantic/maps.py
+-rw-r--r--   0        0        0     2117 2024-05-18 01:15:56.425468 numpydantic-1.0.0rc1/src/numpydantic/meta.py
+-rw-r--r--   0        0        0     2138 2024-05-15 21:39:17.388265 numpydantic-1.0.0rc1/src/numpydantic/monkeypatch.py
+-rw-r--r--   0        0        0     4919 2024-05-18 00:33:09.966148 numpydantic-1.0.0rc1/src/numpydantic/ndarray.py
+-rw-r--r--   0        0        0      542 2024-05-18 01:13:43.173698 numpydantic-1.0.0rc1/src/numpydantic/ndarray.pyi
+-rw-r--r--   0        0        0     6693 2024-05-18 01:03:52.283638 numpydantic-1.0.0rc1/src/numpydantic/schema.py
+-rw-r--r--   0        0        0      678 2024-05-09 03:26:26.479741 numpydantic-1.0.0rc1/src/numpydantic/types.py
+-rw-r--r--   0        0        0        0 2024-04-03 22:50:41.167226 numpydantic-1.0.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0     4836 2024-05-17 23:36:02.073010 numpydantic-1.0.0rc1/tests/conftest.py
+-rw-r--r--   0        0        0     4021 2024-05-16 03:05:17.922915 numpydantic-1.0.0rc1/tests/fixtures.py
+-rw-r--r--   0        0        0        0 2024-04-09 00:54:38.999742 numpydantic-1.0.0rc1/tests/test_interface/__init__.py
+-rw-r--r--   0        0        0     1043 2024-05-09 05:06:59.486862 numpydantic-1.0.0rc1/tests/test_interface/conftest.py
+-rw-r--r--   0        0        0     1379 2024-05-14 22:28:23.749257 numpydantic-1.0.0rc1/tests/test_interface/test_dask.py
+-rw-r--r--   0        0        0     3249 2024-05-17 23:51:17.657048 numpydantic-1.0.0rc1/tests/test_interface/test_hdf5.py
+-rw-r--r--   0        0        0     2853 2024-05-18 01:13:40.285516 numpydantic-1.0.0rc1/tests/test_interface/test_interface.py
+-rw-r--r--   0        0        0      870 2024-05-17 23:59:26.685569 numpydantic-1.0.0rc1/tests/test_interface/test_numpy.py
+-rw-r--r--   0        0        0     3912 2024-05-18 00:39:30.448720 numpydantic-1.0.0rc1/tests/test_interface/test_zarr.py
+-rw-r--r--   0        0        0      881 2024-05-16 05:26:37.839232 numpydantic-1.0.0rc1/tests/test_meta.py
+-rw-r--r--   0        0        0     5714 2024-05-18 01:05:33.062349 numpydantic-1.0.0rc1/tests/test_ndarray.py
+-rw-r--r--   0        0        0     5564 1970-01-01 00:00:00.000000 numpydantic-1.0.0rc1/PKG-INFO
```

### Comparing `numpydantic-0.0.0/LICENSE` & `numpydantic-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

