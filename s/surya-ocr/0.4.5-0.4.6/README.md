# Comparing `tmp/surya_ocr-0.4.5.tar.gz` & `tmp/surya_ocr-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surya_ocr-0.4.5.tar", max compression
+gzip compressed data, was "surya_ocr-0.4.6.tar", max compression
```

## Comparing `surya_ocr-0.4.5.tar` & `surya_ocr-0.4.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    35085 2024-05-16 22:00:38.015767 surya_ocr-0.4.5/LICENSE
--rw-r--r--   0        0        0    25121 2024-05-16 22:00:38.015767 surya_ocr-0.4.5/README.md
--rw-r--r--   0        0        0     3084 2024-05-16 22:00:38.015767 surya_ocr-0.4.5/detect_layout.py
--rw-r--r--   0        0        0     3314 2024-05-16 22:00:38.015767 surya_ocr-0.4.5/detect_text.py
--rw-r--r--   0        0        0     6909 2024-05-16 22:00:38.015767 surya_ocr-0.4.5/ocr_app.py
--rw-r--r--   0        0        0     4112 2024-05-16 22:00:38.015767 surya_ocr-0.4.5/ocr_text.py
--rw-r--r--   0        0        0     1343 2024-05-16 22:00:38.019767 surya_ocr-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     3720 2024-05-16 22:00:38.019767 surya_ocr-0.4.5/reading_order.py
--rw-r--r--   0        0        0      530 2024-05-16 22:00:38.019767 surya_ocr-0.4.5/run_ocr_app.py
--rw-r--r--   0        0        0      827 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/benchmark/bbox.py
--rw-r--r--   0        0        0     4239 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/benchmark/metrics.py
--rw-r--r--   0        0        0     4971 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/benchmark/tesseract.py
--rw-r--r--   0        0        0      887 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/benchmark/util.py
--rw-r--r--   0        0        0     5460 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/detection.py
--rw-r--r--   0        0        0      603 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/input/langs.py
--rw-r--r--   0        0        0     2268 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/input/load.py
--rw-r--r--   0        0        0     3486 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/input/processing.py
--rw-r--r--   0        0        0     2138 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/languages.py
--rw-r--r--   0        0        0     8598 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/layout.py
--rw-r--r--   0        0        0     5902 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/detection/segformer.py
--rw-r--r--   0        0        0      159 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/ordering/config.py
--rw-r--r--   0        0        0    25734 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/ordering/decoder.py
--rw-r--r--   0        0        0     3670 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/ordering/encoder.py
--rw-r--r--   0        0        0     3902 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/ordering/encoderdecoder.py
--rw-r--r--   0        0        0     1568 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/ordering/model.py
--rw-r--r--   0        0        0     6199 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/ordering/processor.py
--rw-r--r--   0        0        0     1676 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/recognition/config.py
--rw-r--r--   0        0        0    32140 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/recognition/decoder.py
--rw-r--r--   0        0        0     2762 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/recognition/encoder.py
--rw-r--r--   0        0        0     2842 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/recognition/model.py
--rw-r--r--   0        0        0     9296 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/recognition/processor.py
--rw-r--r--   0        0        0     3588 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/recognition/tokenizer.py
--rw-r--r--   0        0        0     4154 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/ocr.py
--rw-r--r--   0        0        0     5848 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/ordering.py
--rw-r--r--   0        0        0     6085 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/postprocessing/affinity.py
--rw-r--r--   0        0        0      853 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/postprocessing/fonts.py
--rw-r--r--   0        0        0     7833 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/postprocessing/heatmap.py
--rw-r--r--   0        0        0     3313 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/postprocessing/math/latex.py
--rw-r--r--   0        0        0     3114 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/postprocessing/math/render.py
--rw-r--r--   0        0        0     4382 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/postprocessing/text.py
--rw-r--r--   0        0        0     1253 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/postprocessing/util.py
--rw-r--r--   0        0        0     3882 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/recognition.py
--rw-r--r--   0        0        0     4529 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/schema.py
--rw-r--r--   0        0        0     3615 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/settings.py
--rw-r--r--   0        0        0    26457 1970-01-01 00:00:00.000000 surya_ocr-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0    35085 2024-05-17 22:04:10.543151 surya_ocr-0.4.6/LICENSE
+-rw-r--r--   0        0        0    25008 2024-05-17 22:04:10.543151 surya_ocr-0.4.6/README.md
+-rw-r--r--   0        0        0     3084 2024-05-17 22:04:10.543151 surya_ocr-0.4.6/detect_layout.py
+-rw-r--r--   0        0        0     3314 2024-05-17 22:04:10.543151 surya_ocr-0.4.6/detect_text.py
+-rw-r--r--   0        0        0     6909 2024-05-17 22:04:10.543151 surya_ocr-0.4.6/ocr_app.py
+-rw-r--r--   0        0        0     4112 2024-05-17 22:04:10.543151 surya_ocr-0.4.6/ocr_text.py
+-rw-r--r--   0        0        0     1344 2024-05-17 22:04:10.547151 surya_ocr-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     3720 2024-05-17 22:04:10.547151 surya_ocr-0.4.6/reading_order.py
+-rw-r--r--   0        0        0      616 2024-05-17 22:04:10.547151 surya_ocr-0.4.6/run_ocr_app.py
+-rw-r--r--   0        0        0      827 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/benchmark/bbox.py
+-rw-r--r--   0        0        0     4239 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/benchmark/metrics.py
+-rw-r--r--   0        0        0     4971 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/benchmark/tesseract.py
+-rw-r--r--   0        0        0      887 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/benchmark/util.py
+-rw-r--r--   0        0        0     5315 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/detection.py
+-rw-r--r--   0        0        0      603 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/input/langs.py
+-rw-r--r--   0        0        0     2268 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/input/load.py
+-rw-r--r--   0        0        0     3763 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/input/processing.py
+-rw-r--r--   0        0        0     2138 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/languages.py
+-rw-r--r--   0        0        0     8603 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/layout.py
+-rw-r--r--   0        0        0     5901 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/model/detection/segformer.py
+-rw-r--r--   0        0        0      159 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/model/ordering/config.py
+-rw-r--r--   0        0        0    25734 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/model/ordering/decoder.py
+-rw-r--r--   0        0        0     3670 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/model/ordering/encoder.py
+-rw-r--r--   0        0        0     3902 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/model/ordering/encoderdecoder.py
+-rw-r--r--   0        0        0     1567 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/model/ordering/model.py
+-rw-r--r--   0        0        0     6199 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/model/ordering/processor.py
+-rw-r--r--   0        0        0     1676 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/model/recognition/config.py
+-rw-r--r--   0        0        0    32140 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/model/recognition/decoder.py
+-rw-r--r--   0        0        0     2762 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/model/recognition/encoder.py
+-rw-r--r--   0        0        0     2841 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/model/recognition/model.py
+-rw-r--r--   0        0        0     9296 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/model/recognition/processor.py
+-rw-r--r--   0        0        0     3588 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/model/recognition/tokenizer.py
+-rw-r--r--   0        0        0     4875 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/ocr.py
+-rw-r--r--   0        0        0     5838 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/ordering.py
+-rw-r--r--   0        0        0     5806 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/postprocessing/affinity.py
+-rw-r--r--   0        0        0      853 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/postprocessing/fonts.py
+-rw-r--r--   0        0        0     7785 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/postprocessing/heatmap.py
+-rw-r--r--   0        0        0     3313 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/postprocessing/math/latex.py
+-rw-r--r--   0        0        0     3114 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/postprocessing/math/render.py
+-rw-r--r--   0        0        0     4382 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/postprocessing/text.py
+-rw-r--r--   0        0        0     1253 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/postprocessing/util.py
+-rw-r--r--   0        0        0     3883 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/recognition.py
+-rw-r--r--   0        0        0     4490 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/schema.py
+-rw-r--r--   0        0        0     3685 2024-05-17 22:04:10.691152 surya_ocr-0.4.6/surya/settings.py
+-rw-r--r--   0        0        0    26351 1970-01-01 00:00:00.000000 surya_ocr-0.4.6/PKG-INFO
```

### Comparing `surya_ocr-0.4.5/LICENSE` & `surya_ocr-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/README.md` & `surya_ocr-0.4.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -139,16 +139,14 @@
 
 - `bboxes` - detected bounding boxes for text
   - `bbox` - the axis-aligned rectangle for the text line in (x1, y1, x2, y2) format.  (x1, y1) is the top left corner, and (x2, y2) is the bottom right corner.
   - `polygon` - the polygon for the text line in (x1, y1), (x2, y2), (x3, y3), (x4, y4) format.  The points are in clockwise order from the top left.
   - `confidence` - the confidence of the model in the detected text (0-1)
 - `vertical_lines` - vertical lines detected in the document
   - `bbox` - the axis-aligned line coordinates.
-- `horizontal_lines` - horizontal lines detected in the document
-  - `bbox` - the axis-aligned line coordinates.
 - `page` - the page number in the file
 - `image_bbox` - the bbox for the image in (x1, y1, x2, y2) format.  (x1, y1) is the top left corner, and (x2, y2) is the bottom right corner.  All line bboxes will be contained within this bbox.
 
 **Performance tips**
 
 Setting the `DETECTOR_BATCH_SIZE` env var properly will make a big difference when using a GPU.  Each batch item will use `280MB` of VRAM, so very high batch sizes are possible.  The default is a batch size `32`, which will use about 9GB of VRAM.  Depending on your CPU core count, it might help, too - the default CPU batch size is `2`.
```

### Comparing `surya_ocr-0.4.5/detect_layout.py` & `surya_ocr-0.4.6/detect_layout.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/detect_text.py` & `surya_ocr-0.4.6/detect_text.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/ocr_app.py` & `surya_ocr-0.4.6/ocr_app.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/ocr_text.py` & `surya_ocr-0.4.6/ocr_text.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/pyproject.toml` & `surya_ocr-0.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "surya-ocr"
-version = "0.4.5"
+version = "0.4.6"
 description = "OCR, layout, reading order, and line detection in 90+ languages"
 authors = ["Vik Paruchuri <vik.paruchuri@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/VikParuchuri/surya"
 keywords = ["ocr", "pdf", "text detection", "text recognition"]
 packages = [
@@ -17,16 +17,16 @@
     "run_ocr_app.py",
     "detect_layout.py",
     "reading_order.py",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13,!=3.9.7"
-transformers = "4.36.2"
-torch = "^2.2.2"
+transformers = "^4.41.0"
+torch = "^2.3.0"
 pydantic = "^2.5.3"
 pydantic-settings = "^2.1.0"
 python-dotenv = "^1.0.0"
 pillow = "^10.2.0"
 pypdfium2 = "^4.25.0"
 opencv-python = "^4.9.0.80"
 tabulate = "^0.9.0"
```

### Comparing `surya_ocr-0.4.5/reading_order.py` & `surya_ocr-0.4.6/reading_order.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/benchmark/bbox.py` & `surya_ocr-0.4.6/surya/benchmark/bbox.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/benchmark/metrics.py` & `surya_ocr-0.4.6/surya/benchmark/metrics.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/benchmark/tesseract.py` & `surya_ocr-0.4.6/surya/benchmark/tesseract.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/benchmark/util.py` & `surya_ocr-0.4.6/surya/benchmark/util.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/detection.py` & `surya_ocr-0.4.6/surya/detection.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import torch
 import numpy as np
 from PIL import Image
 
 from surya.model.detection.segformer import SegformerForRegressionMask
 from surya.postprocessing.heatmap import get_and_clean_boxes
-from surya.postprocessing.affinity import get_vertical_lines, get_horizontal_lines
+from surya.postprocessing.affinity import get_vertical_lines
 from surya.input.processing import prepare_image, split_image, get_total_splits
 from surya.schema import TextDetectionResult
 from surya.settings import settings
 from tqdm import tqdm
 from concurrent.futures import ProcessPoolExecutor
 import torch.nn.functional as F
 
@@ -105,31 +105,29 @@
     heatmap, affinity_map = preds
     heat_img = Image.fromarray((heatmap * 255).astype(np.uint8))
     aff_img = Image.fromarray((affinity_map * 255).astype(np.uint8))
     affinity_size = list(reversed(affinity_map.shape))
     heatmap_size = list(reversed(heatmap.shape))
     bboxes = get_and_clean_boxes(heatmap, heatmap_size, orig_sizes)
     vertical_lines = get_vertical_lines(affinity_map, affinity_size, orig_sizes)
-    horizontal_lines = get_horizontal_lines(affinity_map, affinity_size, orig_sizes)
 
     result = TextDetectionResult(
         bboxes=bboxes,
         vertical_lines=vertical_lines,
-        horizontal_lines=horizontal_lines,
         heatmap=heat_img,
         affinity_map=aff_img,
         image_bbox=[0, 0, orig_sizes[0], orig_sizes[1]]
     )
     return result
 
 
 def batch_text_detection(images: List, model, processor, batch_size=None) -> List[TextDetectionResult]:
     preds, orig_sizes = batch_detection(images, model, processor, batch_size=batch_size)
     results = []
-    if len(images) == 1: # Ensures we don't parallelize with streamlit
+    if settings.IN_STREAMLIT: # Ensures we don't parallelize with streamlit
         for i in range(len(images)):
             result = parallel_get_lines(preds[i], orig_sizes[i])
             results.append(result)
     else:
         with ProcessPoolExecutor(max_workers=settings.DETECTOR_POSTPROCESSING_CPU_WORKERS) as executor:
             results = list(executor.map(parallel_get_lines, preds, orig_sizes))
```

### Comparing `surya_ocr-0.4.5/surya/input/langs.py` & `surya_ocr-0.4.6/surya/input/langs.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/input/load.py` & `surya_ocr-0.4.6/surya/input/load.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/input/processing.py` & `surya_ocr-0.4.6/surya/input/processing.py`

 * *Files 18% similar despite different names*

```diff
@@ -76,35 +76,42 @@
     for bbox in bboxes:
         line = image.crop((bbox[0], bbox[1], bbox[2], bbox[3]))
         lines.append(line)
     return lines
 
 
 def slice_polys_from_image(image: Image.Image, polys):
+    image_array = np.array(image)
     lines = []
     for idx, poly in enumerate(polys):
-        lines.append(slice_and_pad_poly(image, poly, idx))
+        lines.append(slice_and_pad_poly(image, image_array, poly, idx))
     return lines
 
 
-def slice_and_pad_poly(image: Image.Image, coordinates, idx):
+def slice_and_pad_poly(image: Image.Image, image_array: np.array, coordinates, idx):
     # Create a mask for the polygon
     mask = Image.new('L', image.size, 0)
 
-    # coordinates must be in tuple form for PIL
+    # Draw polygon onto mask
     coordinates = [(corner[0], corner[1]) for corner in coordinates]
     ImageDraw.Draw(mask).polygon(coordinates, outline=1, fill=1)
     bbox = mask.getbbox()
+
+    if bbox is None:
+        return None
+
     mask = np.array(mask)
 
-    # Extract the polygonal area from the image
-    polygon_image = np.array(image)
+    # We mask out anything not in the polygon
+    polygon_image = image_array.copy()
     polygon_image[mask == 0] = settings.RECOGNITION_PAD_VALUE
-    polygon_image = Image.fromarray(polygon_image)
 
-    rectangle = Image.new('RGB', (bbox[2] - bbox[0], bbox[3] - bbox[1]), 'white')
+    # Crop out the bbox, and ensure we pad the area outside the polygon with the pad value
+    cropped_polygon = polygon_image[bbox[1]:bbox[3], bbox[0]:bbox[2]]
+    rectangle = np.full((bbox[3] - bbox[1], bbox[2] - bbox[0], 3), settings.RECOGNITION_PAD_VALUE, dtype=np.uint8)
+    rectangle[:, :] = cropped_polygon
 
     # Paste the polygon into the rectangle
-    rectangle.paste(polygon_image.crop(bbox), (0, 0))
+    rectangle_image = Image.fromarray(rectangle)
 
-    return rectangle
+    return rectangle_image
```

### Comparing `surya_ocr-0.4.5/surya/languages.py` & `surya_ocr-0.4.6/surya/languages.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/layout.py` & `surya_ocr-0.4.6/surya/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 
 
 def batch_layout_detection(images: List, model, processor, detection_results: Optional[List[TextDetectionResult]] = None, batch_size=None) -> List[LayoutResult]:
     preds, orig_sizes = batch_detection(images, model, processor, batch_size=batch_size)
     id2label = model.config.id2label
 
     results = []
-    if len(images) == 1: # Ensures we don't parallelize with streamlit
+    if settings.IN_STREAMLIT: # Ensures we don't parallelize with streamlit
         for i in range(len(images)):
             result = parallel_get_regions(preds[i], orig_sizes[i], id2label, detection_results[i] if detection_results else None)
             results.append(result)
     else:
         futures = []
         with ProcessPoolExecutor(max_workers=settings.DETECTOR_POSTPROCESSING_CPU_WORKERS) as executor:
             for i in range(len(images)):
```

### Comparing `surya_ocr-0.4.5/surya/model/detection/segformer.py` & `surya_ocr-0.4.6/surya/model/detection/segformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def load_model(checkpoint=settings.DETECTOR_MODEL_CHECKPOINT, device=settings.TORCH_DEVICE_DETECTION, dtype=settings.MODEL_DTYPE_DETECTION):
     config = SegformerConfig.from_pretrained(checkpoint)
     model = SegformerForRegressionMask.from_pretrained(checkpoint, torch_dtype=dtype, config=config)
     if "mps" in device:
         print("Warning: MPS may have poor results. This is a bug with MPS, see here - https://github.com/pytorch/pytorch/issues/84936")
     model = model.to(device)
     model = model.eval()
-    print(f"Loading detection model {checkpoint} on device {device} with dtype {dtype}")
+    print(f"Loaded detection model {checkpoint} on device {device} with dtype {dtype}")
     return model
 
 
 def load_processor(checkpoint=settings.DETECTOR_MODEL_CHECKPOINT):
     processor = SegformerImageProcessor.from_pretrained(checkpoint)
     return processor
```

### Comparing `surya_ocr-0.4.5/surya/model/ordering/decoder.py` & `surya_ocr-0.4.6/surya/model/ordering/decoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/model/ordering/encoder.py` & `surya_ocr-0.4.6/surya/model/ordering/encoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/model/ordering/encoderdecoder.py` & `surya_ocr-0.4.6/surya/model/ordering/encoderdecoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/model/ordering/model.py` & `surya_ocr-0.4.6/surya/model/ordering/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,9 +26,9 @@
 
     model = OrderVisionEncoderDecoderModel.from_pretrained(checkpoint, config=config, torch_dtype=dtype)
     assert isinstance(model.decoder, MBartOrder)
     assert isinstance(model.encoder, VariableDonutSwinModel)
 
     model = model.to(device)
     model = model.eval()
-    print(f"Loading reading order model {checkpoint} on device {device} with dtype {dtype}")
+    print(f"Loaded reading order model {checkpoint} on device {device} with dtype {dtype}")
     return model
```

### Comparing `surya_ocr-0.4.5/surya/model/ordering/processor.py` & `surya_ocr-0.4.6/surya/model/ordering/processor.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/model/recognition/config.py` & `surya_ocr-0.4.6/surya/model/recognition/config.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/model/recognition/decoder.py` & `surya_ocr-0.4.6/surya/model/recognition/decoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/model/recognition/encoder.py` & `surya_ocr-0.4.6/surya/model/recognition/encoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/model/recognition/model.py` & `surya_ocr-0.4.6/surya/model/recognition/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     model = LangVisionEncoderDecoderModel.from_pretrained(checkpoint, config=config, torch_dtype=dtype)
     assert isinstance(model.decoder, MBartMoE)
     assert isinstance(model.encoder, VariableDonutSwinModel)
 
     model = model.to(device)
     model = model.eval()
-    print(f"Loading recognition model {checkpoint} on device {device} with dtype {dtype}")
+    print(f"Loaded recognition model {checkpoint} on device {device} with dtype {dtype}")
     return model
 
 
 class LangVisionEncoderDecoderModel(VisionEncoderDecoderModel):
     def prepare_inputs_for_generation(
             self, input_ids, decoder_langs=None, past_key_values=None, attention_mask=None, use_cache=None, encoder_outputs=None, **kwargs
     ):
```

### Comparing `surya_ocr-0.4.5/surya/model/recognition/processor.py` & `surya_ocr-0.4.6/surya/model/recognition/processor.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/model/recognition/tokenizer.py` & `surya_ocr-0.4.6/surya/model/recognition/tokenizer.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/ocr.py` & `surya_ocr-0.4.6/surya/ocr.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from collections import defaultdict
+from concurrent.futures import ProcessPoolExecutor
 from typing import List
 from tqdm import tqdm
 
 import torch
 from PIL import Image
 
 from surya.detection import batch_text_detection
 from surya.input.processing import slice_polys_from_image, slice_bboxes_from_image
 from surya.postprocessing.text import truncate_repetitions, sort_text_lines
 from surya.recognition import batch_recognition
 from surya.schema import TextLine, OCRResult
+from surya.settings import settings
 
 
 def run_recognition(images: List[Image.Image], langs: List[List[str]], rec_model, rec_processor, bboxes: List[List[List[int]]] = None, polygons: List[List[List[List[int]]]] = None, batch_size=None) -> List[OCRResult]:
     # Polygons need to be in corner format - [[x1, y1], [x2, y2], [x3, y3], [x4, y4]], bboxes in [x1, y1, x2, y2] format
     assert bboxes is not None or polygons is not None
     assert len(images) == len(langs), "You need to pass in one list of languages for each image"
     slice_map = []
@@ -56,28 +58,46 @@
             image_bbox=[0, 0, image.size[0], image.size[1]]
         )
         predictions_by_image.append(pred)
 
     return predictions_by_image
 
 
+def parallel_slice_polys(det_pred, image):
+    polygons = [p.polygon for p in det_pred.bboxes]
+    slices = slice_polys_from_image(image, polygons)
+    return slices
+
+
 def run_ocr(images: List[Image.Image], langs: List[List[str]], det_model, det_processor, rec_model, rec_processor, batch_size=None) -> List[OCRResult]:
     det_predictions = batch_text_detection(images, det_model, det_processor)
     if det_model.device.type == "cuda":
         torch.cuda.empty_cache() # Empty cache from first model run
 
-    slice_map = []
     all_slices = []
+
+    if settings.IN_STREAMLIT:
+        all_slices = [parallel_slice_polys(det_pred, image) for det_pred, image in zip(det_predictions, images)]
+    else:
+        futures = []
+        with ProcessPoolExecutor(max_workers=settings.DETECTOR_POSTPROCESSING_CPU_WORKERS) as executor:
+            for image_idx in range(len(images)):
+                future = executor.submit(parallel_slice_polys, det_predictions[image_idx], images[image_idx])
+                futures.append(future)
+
+            for future in futures:
+                all_slices.append(future.result())
+
+    slice_map = []
     all_langs = []
-    for idx, (image, det_pred, lang) in enumerate(zip(images, det_predictions, langs)):
-        polygons = [p.polygon for p in det_pred.bboxes]
-        slices = slice_polys_from_image(image, polygons)
-        slice_map.append(len(slices))
-        all_slices.extend(slices)
-        all_langs.extend([lang] * len(slices))
+    for idx, (slice, lang) in enumerate(zip(all_slices, langs)):
+        slice_map.append(len(slice))
+        all_langs.extend([lang] * len(slice))
+
+    all_slices = [slice for sublist in all_slices for slice in sublist]
 
     rec_predictions, confidence_scores = batch_recognition(all_slices, all_langs, rec_model, rec_processor, batch_size=batch_size)
 
     predictions_by_image = []
     slice_start = 0
     for idx, (image, det_pred, lang) in enumerate(zip(images, det_predictions, langs)):
         slice_end = slice_start + slice_map[idx]
```

### Comparing `surya_ocr-0.4.5/surya/ordering.py` & `surya_ocr-0.4.6/surya/ordering.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from copy import deepcopy
-from typing import List, Optional
+from typing import List
 import torch
 from PIL import Image
 
 from surya.model.ordering.encoderdecoder import OrderVisionEncoderDecoderModel
 from surya.schema import OrderBox, OrderResult
 from surya.settings import settings
 from tqdm import tqdm
```

### Comparing `surya_ocr-0.4.5/surya/postprocessing/affinity.py` & `surya_ocr-0.4.6/surya/postprocessing/affinity.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,8 @@
 
     vertical_lines = [line for i, line in enumerate(vertical_lines) if i not in to_remove]
 
     if len(vertical_lines) > 0:
         # Always start with top left of page
         vertical_lines[0].bbox[1] = 0
 
-    return vertical_lines
-
-
-def get_horizontal_lines(affinity_map, processor_size, image_size) -> List[ColumnLine]:
-    horizontal_lines = get_detected_lines(affinity_map, horizontal=True)
-    for line in horizontal_lines:
-        line.rescale_bbox(processor_size, image_size)
-    return horizontal_lines
+    return vertical_lines
```

### Comparing `surya_ocr-0.4.5/surya/postprocessing/fonts.py` & `surya_ocr-0.4.6/surya/postprocessing/fonts.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/postprocessing/heatmap.py` & `surya_ocr-0.4.6/surya/postprocessing/heatmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,16 +81,16 @@
     # prepare data
     img_h, img_w = linemap.shape
 
     text_threshold, low_text = get_dynamic_thresholds(linemap, text_threshold, low_text)
 
     ret, text_score = cv2.threshold(linemap, low_text, 1, cv2.THRESH_BINARY)
 
-    text_score_comb = np.clip(text_score, 0, 1)
-    label_count, labels, stats, centroids = cv2.connectedComponentsWithStats(text_score_comb.astype(np.uint8), connectivity=4)
+    text_score_comb = np.clip(text_score, 0, 1).astype(np.uint8)
+    label_count, labels, stats, centroids = cv2.connectedComponentsWithStats(text_score_comb, connectivity=4)
 
     det = []
     confidences = []
     max_confidence = 0
     for k in range(1, label_count):
         # size filtering
         size = stats[k, cv2.CC_STAT_AREA]
@@ -136,17 +136,16 @@
             box = np.array([[l, t], [r, t], [r, b], [l, b]], dtype=np.float32)
 
         # make clock-wise order
         startidx = box.sum(axis=1).argmin()
         box = np.roll(box, 4-startidx, 0)
         box = np.array(box)
 
-        mask = np.zeros_like(linemap).astype(np.uint8)
-        cv2.fillPoly(mask, [np.int32(box)], 255)
-        mask = mask.astype(np.float32) / 255
+        mask = np.zeros_like(linemap, dtype=np.uint8)
+        cv2.fillPoly(mask, [np.int32(box)], 1)
 
         roi = np.where(mask == 1, linemap, 0)
         confidence = np.mean(roi[roi != 0])
 
         if confidence > max_confidence:
             max_confidence = confidence
```

### Comparing `surya_ocr-0.4.5/surya/postprocessing/math/latex.py` & `surya_ocr-0.4.6/surya/postprocessing/math/latex.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/postprocessing/math/render.py` & `surya_ocr-0.4.6/surya/postprocessing/math/render.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/postprocessing/text.py` & `surya_ocr-0.4.6/surya/postprocessing/text.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/postprocessing/util.py` & `surya_ocr-0.4.6/surya/postprocessing/util.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.5/surya/recognition.py` & `surya_ocr-0.4.6/surya/recognition.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     if batch_size is None:
         batch_size = get_batch_size()
 
     images = [image.convert("RGB") for image in images]
 
     output_text = []
     confidences = []
+
     for i in tqdm(range(0, len(images), batch_size), desc="Recognizing Text"):
         batch_langs = languages[i:i+batch_size]
         has_math = ["_math" in lang for lang in batch_langs]
         batch_images = images[i:i+batch_size]
         model_inputs = processor(text=[""] * len(batch_langs), images=batch_images, lang=batch_langs)
 
         batch_pixel_values = model_inputs["pixel_values"]
```

### Comparing `surya_ocr-0.4.5/surya/schema.py` & `surya_ocr-0.4.6/surya/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,14 @@
     languages: List[str]
     image_bbox: List[float]
 
 
 class TextDetectionResult(BaseModel):
     bboxes: List[PolygonBox]
     vertical_lines: List[ColumnLine]
-    horizontal_lines: List[ColumnLine]
     heatmap: Any
     affinity_map: Any
     image_bbox: List[float]
 
 
 class LayoutResult(BaseModel):
     bboxes: List[LayoutBox]
```

### Comparing `surya_ocr-0.4.5/surya/settings.py` & `surya_ocr-0.4.6/surya/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 
 
 class Settings(BaseSettings):
     # General
     TORCH_DEVICE: Optional[str] = None
     IMAGE_DPI: int = 96
+    IN_STREAMLIT: bool = False # Whether we're running in streamlit
 
     # Paths
     DATA_DIR: str = "data"
     RESULT_DIR: str = "results"
     BASE_DIR: str = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
     FONT_DIR: str = os.path.join(BASE_DIR, "static", "fonts")
 
@@ -65,15 +66,15 @@
         "all": os.path.join(FONT_DIR, "GoNotoCurrent-Regular.ttf"),
         "zh": os.path.join(FONT_DIR, "GoNotoCJKCore.ttf"),
         "ja": os.path.join(FONT_DIR, "GoNotoCJKCore.ttf"),
         "ko": os.path.join(FONT_DIR, "GoNotoCJKCore.ttf"),
     }
     RECOGNITION_FONT_DL_BASE: str = "https://github.com/satbyy/go-noto-universal/releases/download/v7.0"
     RECOGNITION_BENCH_DATASET_NAME: str = "vikp/rec_bench"
-    RECOGNITION_PAD_VALUE: int = 0 # Should be 0 or 255
+    RECOGNITION_PAD_VALUE: int = 255 # Should be 0 or 255
 
     # Layout
     LAYOUT_MODEL_CHECKPOINT: str = "vikp/surya_layout2"
     LAYOUT_BENCH_DATASET_NAME: str = "vikp/publaynet_bench"
 
     # Ordering
     ORDER_MODEL_CHECKPOINT: str = "vikp/surya_order"
```

### Comparing `surya_ocr-0.4.5/PKG-INFO` & `surya_ocr-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surya-ocr
-Version: 0.4.5
+Version: 0.4.6
 Summary: OCR, layout, reading order, and line detection in 90+ languages
 Home-page: https://github.com/VikParuchuri/surya
 License: GPL-3.0-or-later
 Keywords: ocr,pdf,text detection,text recognition
 Author: Vik Paruchuri
 Author-email: vik.paruchuri@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
@@ -19,16 +19,16 @@
 Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.1.0,<3.0.0)
 Requires-Dist: pypdfium2 (>=4.25.0,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
-Requires-Dist: torch (>=2.2.2,<3.0.0)
-Requires-Dist: transformers (==4.36.2)
+Requires-Dist: torch (>=2.3.0,<3.0.0)
+Requires-Dist: transformers (>=4.41.0,<5.0.0)
 Project-URL: Repository, https://github.com/VikParuchuri/surya
 Description-Content-Type: text/markdown
 
 # Surya
 
 Surya is a document OCR toolkit that does:
 
@@ -169,16 +169,14 @@
 
 - `bboxes` - detected bounding boxes for text
   - `bbox` - the axis-aligned rectangle for the text line in (x1, y1, x2, y2) format.  (x1, y1) is the top left corner, and (x2, y2) is the bottom right corner.
   - `polygon` - the polygon for the text line in (x1, y1), (x2, y2), (x3, y3), (x4, y4) format.  The points are in clockwise order from the top left.
   - `confidence` - the confidence of the model in the detected text (0-1)
 - `vertical_lines` - vertical lines detected in the document
   - `bbox` - the axis-aligned line coordinates.
-- `horizontal_lines` - horizontal lines detected in the document
-  - `bbox` - the axis-aligned line coordinates.
 - `page` - the page number in the file
 - `image_bbox` - the bbox for the image in (x1, y1, x2, y2) format.  (x1, y1) is the top left corner, and (x2, y2) is the bottom right corner.  All line bboxes will be contained within this bbox.
 
 **Performance tips**
 
 Setting the `DETECTOR_BATCH_SIZE` env var properly will make a big difference when using a GPU.  Each batch item will use `280MB` of VRAM, so very high batch sizes are possible.  The default is a batch size `32`, which will use about 9GB of VRAM.  Depending on your CPU core count, it might help, too - the default CPU batch size is `2`.
```

