# Comparing `tmp/snowflake_connector_python_nightly-2024.5.10.tar.gz` & `tmp/snowflake_connector_python_nightly-2024.5.18-cp38-cp38-macosx_10_14_universal2.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake_connector_python_nightly-2024.5.10.tar", last modified: Fri May 10 04:06:44 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

