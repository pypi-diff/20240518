# Comparing `tmp/openaiisrich-0.1-py3-none-any.whl.zip` & `tmp/openaiisrich-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2007 bytes, number of entries: 6
--rw-r--r--  2.0 unx      437 b- defN 24-May-18 10:42 openaiisrich/__init__.py
--rw-r--r--  2.0 unx     1651 b- defN 24-May-18 10:42 openaiisrich/openai-pricing.json
--rw-r--r--  2.0 unx      469 b- defN 24-May-18 10:42 openaiisrich-0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-18 10:42 openaiisrich-0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-May-18 10:42 openaiisrich-0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      478 b- defN 24-May-18 10:42 openaiisrich-0.1.dist-info/RECORD
-6 files, 3140 bytes uncompressed, 1137 bytes compressed:  63.8%
+Zip file size: 2026 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      435 b- defN 24-May-18 10:46 openaiisrich/__init__.py
+-rw-r--r--  2.0 unx     1651 b- defN 24-May-18 10:46 openaiisrich/openai-pricing.json
+-rw-r--r--  2.0 unx      471 b- defN 24-May-18 10:46 openaiisrich-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-18 10:46 openaiisrich-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-May-18 10:46 openaiisrich-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      486 b- defN 24-May-18 10:46 openaiisrich-0.2.0.dist-info/RECORD
+6 files, 3148 bytes uncompressed, 1140 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: openaiisrich/__init__.py
 Comment: 
 
 Filename: openaiisrich/openai-pricing.json
 Comment: 
 
-Filename: openaiisrich-0.1.dist-info/METADATA
+Filename: openaiisrich-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: openaiisrich-0.1.dist-info/WHEEL
+Filename: openaiisrich-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: openaiisrich-0.1.dist-info/top_level.txt
+Filename: openaiisrich-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: openaiisrich-0.1.dist-info/RECORD
+Filename: openaiisrich-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openaiisrich/__init__.py

```diff
@@ -5,9 +5,9 @@
     
 def load_json():
   return json.loads(resources.read_text(openaiisrich,"openai-pricing.json"))
 
 DATA = load_json()
 
 def cost(model, n_prompt_tokens, n_completion_tokens):
-  model_pricing = DATA["model"]
+  model_pricing = DATA[model]
   return n_prompt_tokens/model_pricing["per_tokens"]*model_pricing["prompt"] + n_completion_tokens/model_pricing["per_tokens"]*model_pricing["completion"]
```

