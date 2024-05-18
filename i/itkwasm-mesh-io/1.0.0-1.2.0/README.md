# Comparing `tmp/itkwasm_mesh_io-1.0.0.tar.gz` & `tmp/itkwasm_mesh_io-1.2.0.tar.gz`

## Comparing `itkwasm_mesh_io-1.0.0.tar` & `itkwasm_mesh_io-1.2.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/docs/Makefile
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/docs/conf.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/docs/make.bat
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/docs/requirements.txt
--rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/docs/_static/favicon.png
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/docs/_static/logo.svg
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/_version.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/byu_read_mesh.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/byu_read_mesh_async.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/byu_write_mesh.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/byu_write_mesh_async.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/free_surfer_ascii_read_mesh.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/free_surfer_ascii_read_mesh_async.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/free_surfer_ascii_write_mesh.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/free_surfer_ascii_write_mesh_async.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/free_surfer_binary_read_mesh.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/free_surfer_binary_read_mesh_async.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/free_surfer_binary_write_mesh.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/free_surfer_binary_write_mesh_async.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/obj_read_mesh.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/obj_read_mesh_async.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/obj_write_mesh.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/obj_write_mesh_async.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/off_read_mesh.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/off_read_mesh_async.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/off_write_mesh.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/off_write_mesh_async.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/read_mesh.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/read_mesh_async.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/stl_read_mesh.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/stl_read_mesh_async.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/stl_write_mesh.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/stl_write_mesh_async.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/swc_read_mesh.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/swc_read_mesh_async.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/swc_write_mesh.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/swc_write_mesh_async.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/vtk_poly_data_read_mesh.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/vtk_poly_data_read_mesh_async.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/vtk_poly_data_write_mesh.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/vtk_poly_data_write_mesh_async.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_read_mesh.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_read_mesh_async.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_write_mesh.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_write_mesh_async.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_zstd_read_mesh.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_zstd_read_mesh_async.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_zstd_write_mesh.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_zstd_write_mesh_async.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_ztd_read_mesh.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_ztd_read_mesh_async.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_ztd_write_mesh.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_ztd_write_mesh_async.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/write_mesh.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/write_mesh_async.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/tests/common.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/tests/fixtures.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/tests/test_read_write_mesh.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/tests/test_read_write_mesh_async.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/tests/test_vtk_poly_data.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/tests/test_vtk_poly_data_async.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/.gitignore
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/README.md
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/docs/Makefile
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/docs/conf.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/docs/make.bat
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/docs/requirements.txt
+-rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/docs/_static/favicon.png
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/docs/_static/logo.svg
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/_version.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/byu_read_mesh.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/byu_read_mesh_async.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/byu_write_mesh.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/byu_write_mesh_async.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/free_surfer_ascii_read_mesh.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/free_surfer_ascii_read_mesh_async.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/free_surfer_ascii_write_mesh.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/free_surfer_ascii_write_mesh_async.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/free_surfer_binary_read_mesh.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/free_surfer_binary_read_mesh_async.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/free_surfer_binary_write_mesh.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/free_surfer_binary_write_mesh_async.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/obj_read_mesh.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/obj_read_mesh_async.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/obj_write_mesh.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/obj_write_mesh_async.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/off_read_mesh.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/off_read_mesh_async.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/off_write_mesh.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/off_write_mesh_async.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/read_mesh.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/read_mesh_async.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/stl_read_mesh.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/stl_read_mesh_async.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/stl_write_mesh.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/stl_write_mesh_async.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/swc_read_mesh.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/swc_read_mesh_async.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/swc_write_mesh.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/swc_write_mesh_async.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/vtk_poly_data_read_mesh.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/vtk_poly_data_read_mesh_async.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/vtk_poly_data_write_mesh.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/vtk_poly_data_write_mesh_async.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_read_mesh.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_read_mesh_async.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_write_mesh.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_write_mesh_async.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_zstd_read_mesh.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_zstd_read_mesh_async.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_zstd_write_mesh.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_zstd_write_mesh_async.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_ztd_read_mesh.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_ztd_read_mesh_async.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_ztd_write_mesh.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_ztd_write_mesh_async.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/write_mesh.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/write_mesh_async.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/tests/common.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/tests/fixtures.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/tests/test_read_write_mesh.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/tests/test_read_write_mesh_async.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/tests/test_vtk_poly_data.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/tests/test_vtk_poly_data_async.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/.gitignore
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/README.md
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 itkwasm_mesh_io-1.2.0/PKG-INFO
```

### Comparing `itkwasm_mesh_io-1.0.0/docs/Makefile` & `itkwasm_mesh_io-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/docs/conf.py` & `itkwasm_mesh_io-1.2.0/docs/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 from datetime import date
+import os
 
 project = 'itkwasm-mesh-io'
 copyright = f'{date.today().year}, NumFOCUS'
 author = 'Insight Software Consortium'
 
 extensions = [
     'sphinx.ext.autosummary',
@@ -42,15 +43,16 @@
 }
 
 html_theme = 'furo'
 html_static_path = ['_static']
 html_logo = "_static/logo.svg"
 html_favicon = "_static/favicon.png"
 html_title = f"{project}"
+html_baseurl = os.environ.get("SPHINX_BASE_URL", "")
 
 # Furo options
 html_theme_options = {
     "top_of_page_button": "edit",
     "source_repository": "https://github.com/InsightSoftwareConsortium/itk-wasm",
     "source_branch": "main",
-    "source_directory": "docs",
+    "source_directory": "packages/mesh-io/python/itkwasm-mesh-io/docs",
 }
```

### Comparing `itkwasm_mesh_io-1.0.0/docs/index.md` & `itkwasm_mesh_io-1.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/docs/make.bat` & `itkwasm_mesh_io-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/docs/_static/favicon.png` & `itkwasm_mesh_io-1.2.0/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/__init__.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/__init__.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/byu_read_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/byu_read_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/byu_read_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/byu_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/byu_write_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/byu_write_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/byu_write_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/byu_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/free_surfer_ascii_read_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/free_surfer_ascii_read_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/free_surfer_ascii_read_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/free_surfer_ascii_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/free_surfer_ascii_write_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/free_surfer_ascii_write_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/free_surfer_ascii_write_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/free_surfer_ascii_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/free_surfer_binary_read_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/free_surfer_binary_read_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/free_surfer_binary_read_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/free_surfer_binary_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/free_surfer_binary_write_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/free_surfer_binary_write_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/free_surfer_binary_write_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/free_surfer_binary_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/obj_read_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/obj_read_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/obj_read_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/obj_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/obj_write_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/obj_write_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/obj_write_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/obj_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/off_read_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/off_read_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/off_read_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/off_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/off_write_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/off_write_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/off_write_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/off_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/read_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/read_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/read_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/stl_read_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/stl_read_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/stl_read_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/stl_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/stl_write_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/stl_write_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/stl_write_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/stl_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/swc_read_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/swc_read_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/swc_read_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/swc_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/swc_write_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/swc_write_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/swc_write_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/swc_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/vtk_poly_data_read_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/vtk_poly_data_read_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/vtk_poly_data_read_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/vtk_poly_data_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/vtk_poly_data_write_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/vtk_poly_data_write_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/vtk_poly_data_write_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/vtk_poly_data_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_read_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_read_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_read_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_write_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_write_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_write_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_zstd_read_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_zstd_read_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_zstd_read_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_zstd_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_zstd_write_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_zstd_write_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_zstd_write_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_zstd_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_ztd_read_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_ztd_read_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_ztd_read_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_ztd_read_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_ztd_write_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_ztd_write_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/wasm_ztd_write_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/wasm_ztd_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/write_mesh.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/write_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/itkwasm_mesh_io/write_mesh_async.py` & `itkwasm_mesh_io-1.2.0/itkwasm_mesh_io/write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/tests/fixtures.py` & `itkwasm_mesh_io-1.2.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/tests/test_read_write_mesh.py` & `itkwasm_mesh_io-1.2.0/tests/test_read_write_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/tests/test_read_write_mesh_async.py` & `itkwasm_mesh_io-1.2.0/tests/test_read_write_mesh_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/tests/test_vtk_poly_data.py` & `itkwasm_mesh_io-1.2.0/tests/test_vtk_poly_data.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/tests/test_vtk_poly_data_async.py` & `itkwasm_mesh_io-1.2.0/tests/test_vtk_poly_data_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/pyproject.toml` & `itkwasm_mesh_io-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_io-1.0.0/PKG-INFO` & `itkwasm_mesh_io-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: itkwasm-mesh-io
-Version: 1.0.0
+Version: 1.2.0
 Summary: Input and output for scientific and medical image file formats.
 Project-URL: Home, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 License-Expression: Apache-2.0
 Keywords: emscripten,itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
```

