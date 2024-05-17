# Comparing `tmp/marker_pdf-0.2.6.tar.gz` & `tmp/marker_pdf-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marker_pdf-0.2.6.tar", max compression
+gzip compressed data, was "marker_pdf-0.2.7.tar", max compression
```

## Comparing `marker_pdf-0.2.6.tar` & `marker_pdf-0.2.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    35101 2024-05-16 22:46:38.271131 marker_pdf-0.2.6/LICENSE
--rw-r--r--   0        0        0    12609 2024-05-16 22:46:38.271131 marker_pdf-0.2.6/README.md
--rwxr-xr-x   0        0        0      638 2024-05-16 22:46:38.271131 marker_pdf-0.2.6/chunk_convert.py
--rwxr-xr-x   0        0        0     1151 2024-05-16 22:46:38.271131 marker_pdf-0.2.6/chunk_convert.sh
--rwxr-xr-x   0        0        0     4853 2024-05-16 22:46:38.271131 marker_pdf-0.2.6/convert.py
--rwxr-xr-x   0        0        0     1246 2024-05-16 22:46:38.271131 marker_pdf-0.2.6/convert_single.py
--rw-r--r--   0        0        0     1376 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/benchmark/scoring.py
--rw-r--r--   0        0        0      231 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/cleaners/bullets.py
--rw-r--r--   0        0        0     4457 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/cleaners/code.py
--rw-r--r--   0        0        0      950 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/cleaners/fontstyle.py
--rw-r--r--   0        0        0     2766 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/cleaners/headers.py
--rw-r--r--   0        0        0     2456 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/cleaners/headings.py
--rw-r--r--   0        0        0      248 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/cleaners/text.py
--rw-r--r--   0        0        0     5172 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/convert.py
--rw-r--r--   0        0        0     2450 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/debug/data.py
--rw-r--r--   0        0        0     7884 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/equations/equations.py
--rw-r--r--   0        0        0     1549 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/equations/inference.py
--rw-r--r--   0        0        0     2594 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/images/extract.py
--rw-r--r--   0        0        0      473 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/images/save.py
--rw-r--r--   0        0        0     1928 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/layout/layout.py
--rw-r--r--   0        0        0     2516 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/layout/order.py
--rw-r--r--   0        0        0      396 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/logger.py
--rw-r--r--   0        0        0     3121 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/models.py
--rw-r--r--   0        0        0      888 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/ocr/detection.py
--rw-r--r--   0        0        0     2468 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/ocr/heuristics.py
--rw-r--r--   0        0        0     1223 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/ocr/lang.py
--rw-r--r--   0        0        0     5742 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/ocr/recognition.py
--rw-r--r--   0        0        0     2180 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/ocr/tesseract.py
--rw-r--r--   0        0        0      258 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/ocr/utils.py
--rw-r--r--   0        0        0     1266 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/output.py
--rw-r--r--   0        0        0     3932 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/pdf/extract_text.py
--rw-r--r--   0        0        0      817 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/pdf/images.py
--rw-r--r--   0        0        0     2442 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/pdf/utils.py
--rw-r--r--   0        0        0     4134 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/postprocessors/editor.py
--rw-r--r--   0        0        0     7226 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/postprocessors/markdown.py
--rw-r--r--   0        0        0     4977 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/postprocessors/t5.py
--rw-r--r--   0        0        0     2849 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/schema/bbox.py
--rw-r--r--   0        0        0     3259 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/schema/block.py
--rw-r--r--   0        0        0      502 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/schema/merged.py
--rw-r--r--   0        0        0     1618 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/schema/page.py
--rw-r--r--   0        0        0     4238 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/settings.py
--rw-r--r--   0        0        0     3384 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/tables/cells.py
--rw-r--r--   0        0        0     7178 2024-05-16 22:46:38.283131 marker_pdf-0.2.6/marker/tables/table.py
--rw-r--r--   0        0        0     1128 2024-05-16 22:46:38.283131 marker_pdf-0.2.6/marker/tables/utils.py
--rw-r--r--   0        0        0      156 2024-05-16 22:46:38.283131 marker_pdf-0.2.6/marker/utils.py
--rw-r--r--   0        0        0     1338 2024-05-16 22:46:38.283131 marker_pdf-0.2.6/pyproject.toml
--rw-r--r--   0        0        0    14231 1970-01-01 00:00:00.000000 marker_pdf-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    35101 2024-05-17 22:57:52.928438 marker_pdf-0.2.7/LICENSE
+-rw-r--r--   0        0        0    12609 2024-05-17 22:57:52.928438 marker_pdf-0.2.7/README.md
+-rwxr-xr-x   0        0        0      638 2024-05-17 22:57:52.928438 marker_pdf-0.2.7/chunk_convert.py
+-rwxr-xr-x   0        0        0     1151 2024-05-17 22:57:52.928438 marker_pdf-0.2.7/chunk_convert.sh
+-rwxr-xr-x   0        0        0     4853 2024-05-17 22:57:52.928438 marker_pdf-0.2.7/convert.py
+-rwxr-xr-x   0        0        0     1246 2024-05-17 22:57:52.928438 marker_pdf-0.2.7/convert_single.py
+-rw-r--r--   0        0        0     1376 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/benchmark/scoring.py
+-rw-r--r--   0        0        0      231 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/cleaners/bullets.py
+-rw-r--r--   0        0        0     4457 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/cleaners/code.py
+-rw-r--r--   0        0        0      950 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/cleaners/fontstyle.py
+-rw-r--r--   0        0        0     2766 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/cleaners/headers.py
+-rw-r--r--   0        0        0     2456 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/cleaners/headings.py
+-rw-r--r--   0        0        0      248 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/cleaners/text.py
+-rw-r--r--   0        0        0     5172 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/convert.py
+-rw-r--r--   0        0        0     2450 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/debug/data.py
+-rw-r--r--   0        0        0     7884 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/equations/equations.py
+-rw-r--r--   0        0        0     1549 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/equations/inference.py
+-rw-r--r--   0        0        0     2594 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/images/extract.py
+-rw-r--r--   0        0        0      473 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/images/save.py
+-rw-r--r--   0        0        0     1928 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/layout/layout.py
+-rw-r--r--   0        0        0     2516 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/layout/order.py
+-rw-r--r--   0        0        0      396 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/logger.py
+-rw-r--r--   0        0        0     3121 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/models.py
+-rw-r--r--   0        0        0      888 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/ocr/detection.py
+-rw-r--r--   0        0        0     2468 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/ocr/heuristics.py
+-rw-r--r--   0        0        0     1223 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/ocr/lang.py
+-rw-r--r--   0        0        0     5742 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/ocr/recognition.py
+-rw-r--r--   0        0        0     2180 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/ocr/tesseract.py
+-rw-r--r--   0        0        0      258 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/ocr/utils.py
+-rw-r--r--   0        0        0     1266 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/output.py
+-rw-r--r--   0        0        0     3932 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/pdf/extract_text.py
+-rw-r--r--   0        0        0      817 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/pdf/images.py
+-rw-r--r--   0        0        0     2442 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/pdf/utils.py
+-rw-r--r--   0        0        0     4134 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/postprocessors/editor.py
+-rw-r--r--   0        0        0     7226 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/postprocessors/markdown.py
+-rw-r--r--   0        0        0     4977 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/postprocessors/t5.py
+-rw-r--r--   0        0        0     2849 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/schema/bbox.py
+-rw-r--r--   0        0        0     3259 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/schema/block.py
+-rw-r--r--   0        0        0      502 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/schema/merged.py
+-rw-r--r--   0        0        0     1618 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/schema/page.py
+-rw-r--r--   0        0        0     4238 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/settings.py
+-rw-r--r--   0        0        0     3384 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/tables/cells.py
+-rw-r--r--   0        0        0     7178 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/tables/table.py
+-rw-r--r--   0        0        0     1128 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/tables/utils.py
+-rw-r--r--   0        0        0      156 2024-05-17 22:57:52.936438 marker_pdf-0.2.7/marker/utils.py
+-rw-r--r--   0        0        0     1270 2024-05-17 22:57:52.940438 marker_pdf-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0    14231 1970-01-01 00:00:00.000000 marker_pdf-0.2.7/PKG-INFO
```

### Comparing `marker_pdf-0.2.6/LICENSE` & `marker_pdf-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/README.md` & `marker_pdf-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/chunk_convert.py` & `marker_pdf-0.2.7/chunk_convert.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/chunk_convert.sh` & `marker_pdf-0.2.7/chunk_convert.sh`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/convert.py` & `marker_pdf-0.2.7/convert.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/convert_single.py` & `marker_pdf-0.2.7/convert_single.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/benchmark/scoring.py` & `marker_pdf-0.2.7/marker/benchmark/scoring.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/cleaners/code.py` & `marker_pdf-0.2.7/marker/cleaners/code.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/cleaners/fontstyle.py` & `marker_pdf-0.2.7/marker/cleaners/fontstyle.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/cleaners/headers.py` & `marker_pdf-0.2.7/marker/cleaners/headers.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/cleaners/headings.py` & `marker_pdf-0.2.7/marker/cleaners/headings.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/convert.py` & `marker_pdf-0.2.7/marker/convert.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/debug/data.py` & `marker_pdf-0.2.7/marker/debug/data.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/equations/equations.py` & `marker_pdf-0.2.7/marker/equations/equations.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/equations/inference.py` & `marker_pdf-0.2.7/marker/equations/inference.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/images/extract.py` & `marker_pdf-0.2.7/marker/images/extract.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/layout/layout.py` & `marker_pdf-0.2.7/marker/layout/layout.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/layout/order.py` & `marker_pdf-0.2.7/marker/layout/order.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/models.py` & `marker_pdf-0.2.7/marker/models.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/ocr/detection.py` & `marker_pdf-0.2.7/marker/ocr/detection.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/ocr/heuristics.py` & `marker_pdf-0.2.7/marker/ocr/heuristics.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/ocr/lang.py` & `marker_pdf-0.2.7/marker/ocr/lang.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/ocr/recognition.py` & `marker_pdf-0.2.7/marker/ocr/recognition.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/ocr/tesseract.py` & `marker_pdf-0.2.7/marker/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/output.py` & `marker_pdf-0.2.7/marker/output.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/pdf/extract_text.py` & `marker_pdf-0.2.7/marker/pdf/extract_text.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/pdf/images.py` & `marker_pdf-0.2.7/marker/pdf/images.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/pdf/utils.py` & `marker_pdf-0.2.7/marker/pdf/utils.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/postprocessors/editor.py` & `marker_pdf-0.2.7/marker/postprocessors/editor.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/postprocessors/markdown.py` & `marker_pdf-0.2.7/marker/postprocessors/markdown.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/postprocessors/t5.py` & `marker_pdf-0.2.7/marker/postprocessors/t5.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/schema/bbox.py` & `marker_pdf-0.2.7/marker/schema/bbox.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/schema/block.py` & `marker_pdf-0.2.7/marker/schema/block.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/schema/page.py` & `marker_pdf-0.2.7/marker/schema/page.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/settings.py` & `marker_pdf-0.2.7/marker/settings.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/tables/cells.py` & `marker_pdf-0.2.7/marker/tables/cells.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/tables/table.py` & `marker_pdf-0.2.7/marker/tables/table.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/marker/tables/utils.py` & `marker_pdf-0.2.7/marker/tables/utils.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.6/pyproject.toml` & `marker_pdf-0.2.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "marker-pdf"
-version = "0.2.6"
+version = "0.2.7"
 description = "Convert PDF to markdown with high speed and accuracy."
 authors = ["Vik Paruchuri <github@vikas.sh>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/VikParuchuri/marker"
 keywords = ["pdf", "markdown", "ocr", "nlp"]
 packages = [
@@ -19,25 +19,25 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13,!=3.9.7"
 scikit-learn = "^1.3.2"
 Pillow = "^10.1.0"
 pydantic = "^2.4.2"
 pydantic-settings = "^2.0.3"
-transformers = "^4.36.2" # 4.36.2 needed because issues with donut models and later versions
+transformers = "^4.36.2"
 numpy = "^1.26.1"
 python-dotenv = "^1.0.0"
 torch = "^2.2.2" # Issue with torch 2.3.0 and vision models - https://github.com/pytorch/pytorch/issues/121834
 ray = "^2.20.0"
 tqdm = "^4.66.1"
 tabulate = "^0.9.0"
 ftfy = "^6.1.1"
-texify = "^0.1.8"
+texify = "^0.1.9"
 rapidfuzz = "^3.8.1"
-surya-ocr = "^0.4.3"
+surya-ocr = "^0.4.6"
 filetype = "^1.2.0"
 regex = "^2024.4.28"
 pdftext = "^0.3.7"
 grpcio = "^1.63.0"
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
```

### Comparing `marker_pdf-0.2.6/PKG-INFO` & `marker_pdf-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marker-pdf
-Version: 0.2.6
+Version: 0.2.7
 Summary: Convert PDF to markdown with high speed and accuracy.
 Home-page: https://github.com/VikParuchuri/marker
 License: GPL-3.0-or-later
 Keywords: pdf,markdown,ocr,nlp
 Author: Vik Paruchuri
 Author-email: github@vikas.sh
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
@@ -23,17 +23,17 @@
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.0.3,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rapidfuzz (>=3.8.1,<4.0.0)
 Requires-Dist: ray (>=2.20.0,<3.0.0)
 Requires-Dist: regex (>=2024.4.28,<2025.0.0)
 Requires-Dist: scikit-learn (>=1.3.2,<2.0.0)
-Requires-Dist: surya-ocr (>=0.4.3,<0.5.0)
+Requires-Dist: surya-ocr (>=0.4.6,<0.5.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
-Requires-Dist: texify (>=0.1.8,<0.2.0)
+Requires-Dist: texify (>=0.1.9,<0.2.0)
 Requires-Dist: torch (>=2.2.2,<3.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Requires-Dist: transformers (>=4.36.2,<5.0.0)
 Project-URL: Repository, https://github.com/VikParuchuri/marker
 Description-Content-Type: text/markdown
 
 # Marker
```

