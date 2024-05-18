# Comparing `tmp/dtw-python-1.4.2.tar.gz` & `tmp/dtw_python-1.4.3-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtw-python-1.4.2.tar", last modified: Tue Mar 19 07:33:27 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

