# Comparing `tmp/openaiisrich-0.3.0-py3-none-any.whl.zip` & `tmp/openaiisrich-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2140 bytes, number of entries: 6
--rw-r--r--  2.0 unx      435 b- defN 24-May-18 10:59 openaiisrich/__init__.py
--rw-r--r--  2.0 unx     1770 b- defN 24-May-18 10:59 openaiisrich/openai-pricing.json
--rw-r--r--  2.0 unx      650 b- defN 24-May-18 10:59 openaiisrich-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-18 10:59 openaiisrich-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-May-18 10:59 openaiisrich-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      486 b- defN 24-May-18 10:59 openaiisrich-0.3.0.dist-info/RECORD
-6 files, 3446 bytes uncompressed, 1254 bytes compressed:  63.6%
+Zip file size: 2141 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      435 b- defN 24-May-18 11:00 openaiisrich/__init__.py
+-rw-r--r--  2.0 unx     1810 b- defN 24-May-18 11:00 openaiisrich/openai-pricing.json
+-rw-r--r--  2.0 unx      650 b- defN 24-May-18 11:01 openaiisrich-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-18 11:01 openaiisrich-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-May-18 11:01 openaiisrich-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      486 b- defN 24-May-18 11:01 openaiisrich-0.4.0.dist-info/RECORD
+6 files, 3486 bytes uncompressed, 1255 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: openaiisrich/__init__.py
 Comment: 
 
 Filename: openaiisrich/openai-pricing.json
 Comment: 
 
-Filename: openaiisrich-0.3.0.dist-info/METADATA
+Filename: openaiisrich-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: openaiisrich-0.3.0.dist-info/WHEEL
+Filename: openaiisrich-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: openaiisrich-0.3.0.dist-info/top_level.txt
+Filename: openaiisrich-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: openaiisrich-0.3.0.dist-info/RECORD
+Filename: openaiisrich-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openaiisrich/openai-pricing.json

### Pretty-printed

 * *Similarity: 0.9855072463768115%*

 * *Differences: {"'gpt-4o'": "{'per_tokens': 1000}", "'gpt-4o-2024-05-13'": "{'per_tokens': 1000}"}*

```diff
@@ -77,18 +77,20 @@
     "gpt-4-turbo-preview": {
         "completion": 0.03,
         "per_tokens": 1000,
         "prompt": 0.01
     },
     "gpt-4o": {
         "completion": 0.015,
+        "per_tokens": 1000,
         "prompt": 0.005
     },
     "gpt-4o-2024-05-13": {
         "completion": 0.015,
+        "per_tokens": 1000,
         "prompt": 0.005
     },
     "text-ada-001": {
         "per_tokens": 1000,
         "prompt": 0.0004
     },
     "text-babbage-001": {
```

## Comparing `openaiisrich-0.3.0.dist-info/METADATA` & `openaiisrich-0.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openaiisrich
-Version: 0.3.0
+Version: 0.4.0
 Author-email: Martin Monperrus <martin.monperrus@gnieh.org>
 Description-Content-Type: text/markdown
 
 # openaiisrich
 
 openai is rich -- pricing information of openai models as JSON, incl. prompt and completion costs (`n_context_tokens_total`, `n_generated_tokens_total`).
```

