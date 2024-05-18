# Comparing `tmp/crawler_user_agents-0.4.0.tar.gz` & `tmp/crawler_user_agents-0.5.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawler_user_agents-0.4.0.tar", last modified: Sat May 18 08:45:11 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

