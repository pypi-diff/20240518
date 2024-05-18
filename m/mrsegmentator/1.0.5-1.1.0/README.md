# Comparing `tmp/mrsegmentator-1.0.5.tar.gz` & `tmp/mrsegmentator-1.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrsegmentator-1.0.5.tar", last modified: Mon May 13 12:59:48 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

