# Comparing `tmp/lephare-0.1.8.tar.gz` & `tmp/lephare-0.1.9-cp312-cp312-macosx_10_15_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lephare-0.1.8.tar", last modified: Thu May 16 20:34:36 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

