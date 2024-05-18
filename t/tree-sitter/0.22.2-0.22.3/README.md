# Comparing `tmp/tree-sitter-0.22.2.tar.gz` & `tmp/tree_sitter-0.22.3-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-sitter-0.22.2.tar", last modified: Thu May 16 19:10:27 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

