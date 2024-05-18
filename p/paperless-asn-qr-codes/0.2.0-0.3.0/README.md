# Comparing `tmp/paperless_asn_qr_codes-0.2.0.tar.gz` & `tmp/paperless_asn_qr_codes-0.3.0.tar.gz`

## Comparing `paperless_asn_qr_codes-0.2.0.tar` & `paperless_asn_qr_codes-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 paperless_asn_qr_codes-0.2.0/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 paperless_asn_qr_codes-0.2.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 paperless_asn_qr_codes-0.2.0/paperless_asn_qr_codes/__init__.py
--rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 paperless_asn_qr_codes-0.2.0/paperless_asn_qr_codes/avery_labels.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 paperless_asn_qr_codes-0.2.0/paperless_asn_qr_codes/main.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 paperless_asn_qr_codes-0.2.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 paperless_asn_qr_codes-0.2.0/LICENSE
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 paperless_asn_qr_codes-0.2.0/README.md
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 paperless_asn_qr_codes-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 paperless_asn_qr_codes-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 paperless_asn_qr_codes-0.3.0/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 paperless_asn_qr_codes-0.3.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 paperless_asn_qr_codes-0.3.0/paperless_asn_qr_codes/__init__.py
+-rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 paperless_asn_qr_codes-0.3.0/paperless_asn_qr_codes/avery_labels.py
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 paperless_asn_qr_codes-0.3.0/paperless_asn_qr_codes/main.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 paperless_asn_qr_codes-0.3.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 paperless_asn_qr_codes-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 paperless_asn_qr_codes-0.3.0/README.md
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 paperless_asn_qr_codes-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 paperless_asn_qr_codes-0.3.0/PKG-INFO
```

### Comparing `paperless_asn_qr_codes-0.2.0/.github/workflows/publish.yaml` & `paperless_asn_qr_codes-0.3.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `paperless_asn_qr_codes-0.2.0/paperless_asn_qr_codes/avery_labels.py` & `paperless_asn_qr_codes-0.3.0/paperless_asn_qr_codes/avery_labels.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,28 +85,47 @@
 }
 
 RETURN_ADDRESS = 5167
 BUSINESS_CARDS = 5371
 
 
 class AveryLabel:
-    def __init__(self, label, debug, **kwargs):
+    def __init__(self, label, debug,
+                 topDown=True, start_pos=None,
+                 **kwargs):
         data = labelInfo[label]
         self.across = data.labels_horizontal
         self.down = data.labels_vertical
         self.size = data.label_size
         self.labelsep = (
             self.size[0] + data.gutter_size[0],
             self.size[1] + data.gutter_size[1],
         )
         self.margins = data.margin
-        self.topDown = True
+        self.topDown = topDown
         self.debug = debug
         self.pagesize = data.pagesize
-        self.position = 0
+
+        #Calculate start offset
+        if isinstance(start_pos, tuple):
+            rows, columns = start_pos
+            # Minimum Value 1 for row/column
+            rows = max(rows, 1)
+            columns = max(columns, 1)
+            if self.topDown:
+                offset = (columns - 1) * self.down + rows - 1
+            else:
+                offset = (rows - 1) * self.across + columns - 1
+        elif start_pos:
+            offset = start_pos - 1
+        else:
+            offset = 0
+        # Limit start position to number of labels - 1
+        self.position = min(offset,  self.across * self.down - 1)
+
         self.__dict__.update(kwargs)
 
     def open(self, filename):
         self.canvas = canvas.Canvas(filename, pagesize=self.pagesize)
         if self.debug:
             self.canvas.setPageCompression(0)
         self.canvas.setLineJoin(1)
```

### Comparing `paperless_asn_qr_codes-0.2.0/paperless_asn_qr_codes/main.py` & `paperless_asn_qr_codes-0.3.0/paperless_asn_qr_codes/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+import re
 
 from reportlab.lib.units import mm
 from reportlab_qrcode import QRCodeImage
 
 from paperless_asn_qr_codes import avery_labels
 
 
@@ -15,39 +16,87 @@
     qr = QRCodeImage(barcode_value, size=y * 0.9)
     qr.drawOn(c, 1 * mm, y * 0.05)
     c.setFont("Helvetica", 2 * mm)
     c.drawString(y, (y - 2 * mm) / 2, barcode_value)
 
 
 def main():
+    # Match the starting position parameter. Allow x:y or n
+    def _start_position(arg):
+        if mat := re.match(r"^(\d{1,2}):(\d{1,2})$", arg):
+            return (int(mat.group(1)), int(mat.group(2)))
+        elif mat := re.match(r"^\d+$", arg):
+            return int(arg)
+        else:
+            raise argparse.ArgumentTypeError("invalid value")
+
     parser = argparse.ArgumentParser(
         prog="paperless-asn-qr-codes",
         description="CLI Tool for generating paperless ASN labels with QR codes",
     )
     parser.add_argument("start_asn", type=int, help="The value of the first ASN")
-    parser.add_argument("output_file", type=str, default="labels.pdf", help="The output file to write to (default: labels.pdf)")
+    parser.add_argument(
+        "output_file",
+        type=str,
+        default="labels.pdf",
+        help="The output file to write to (default: labels.pdf)",
+    )
     parser.add_argument(
         "--format", "-f", choices=avery_labels.labelInfo.keys(), default="averyL4731"
     )
     parser.add_argument(
-        "--digits", "-d", default=7, help="Number of digits in the ASN (default: 7, produces 'ASN0000001')", type=int
+        "--digits",
+        "-d",
+        default=7,
+        help="Number of digits in the ASN (default: 7, produces 'ASN0000001')",
+        type=int,
     )
     parser.add_argument(
         "--border",
         "-b",
         action="store_true",
         help="Display borders around labels, useful for debugging the printer alignment",
     )
+    parser.add_argument(
+        "--row-wise",
+        "-r",
+        action="store_false",
+        help="Increment the ASNs row-wise, go from left to right",
+    )
+    parser.add_argument(
+        "--num-labels",
+        "-n",
+        type=int,
+        help="Number of labels to be printed on the sheet",
+    )
+    parser.add_argument(
+        "--pages",
+        "-p",
+        type=int,
+        default=1,
+        help="Number of pages to be printed, ignored if NUM_LABELS is set (default: 1)",
+    )
+    parser.add_argument(
+        "--start-position",
+        "-s",
+        type=_start_position,
+        help="Define the starting position on the sheet, eighter as ROW:COLUMN or COUNT, both starting from 1 (default: 1:1 or 1)",
+    )
+
     args = parser.parse_args()
     global startASN
     global digits
     startASN = int(args.start_asn)
     digits = int(args.digits)
-    label = avery_labels.AveryLabel(args.format, args.border)
-    label.open(args.output_file)
-    # by default, we render all labels possible on a single sheet
-    count = (
-        avery_labels.labelInfo[args.format].labels_horizontal
-        * avery_labels.labelInfo[args.format].labels_vertical
+    label = avery_labels.AveryLabel(
+        args.format, args.border, topDown=args.row_wise, start_pos=args.start_position
     )
+    label.open(args.output_file)
+
+    # If defined use parameter for number of labels
+    if args.num_labels:
+        count = args.num_labels
+    else:
+        # Otherwise number of pages*labels - offset
+        count = args.pages * label.across * label.down - label.position
     label.render(render, count)
     label.close()
```

### Comparing `paperless_asn_qr_codes-0.2.0/LICENSE` & `paperless_asn_qr_codes-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paperless_asn_qr_codes-0.2.0/README.md` & `paperless_asn_qr_codes-0.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -9,28 +9,37 @@
 ```console
 pip install paperless-asn-qr-codes
 ```
 
 ## Usage
 
 ```
-usage: paperless-asn-qr-codes [-h] [--format {averyL4731,avery5160,avery5161,avery5163,avery5167,avery5371}] [--border] start_asn output_file
+usage: paperless-asn-qr-codes [-h] [--format {averyL4731,avery5160,avery5161,avery5163,avery5167,avery5371}] [--digits DIGITS] [--border] [--row-wise] [--num-labels NUM_LABELS] [--pages PAGES]
+                              [--start-position START_POSITION]
+                              start_asn output_file
 
 CLI Tool for generating paperless ASN labels with QR codes
 
 positional arguments:
   start_asn             The value of the first ASN
   output_file           The output file to write to (default: labels.pdf)
 
 options:
   -h, --help            show this help message and exit
   --format {averyL4731,avery5160,avery5161,avery5163,avery5167,avery5371}, -f {averyL4731,avery5160,avery5161,avery5163,avery5167,avery5371}
   --digits DIGITS, -d DIGITS
                         Number of digits in the ASN (default: 7, produces 'ASN0000001')
   --border, -b          Display borders around labels, useful for debugging the printer alignment
+  --row-wise, -r        Increment the ASNs row-wise, go from left to right
+  --num-labels NUM_LABELS, -n NUM_LABELS
+                        Number of labels to be printed on the sheet
+  --pages PAGES, -p PAGES
+                        Number of pages to be printed, ignored if NUM_LABELS is set (default: 1)
+  --start-position START_POSITION, -s START_POSITION
+                        Define the starting position on the sheet, eighter as ROW:COLUMN or COUNT, both starting from 1 (default: 1:1 or 1)
 ```
 
 ### Mandatory arguments
 
 - `<start_asn>`: The value of the first ASN to generate
 
 ### Optional arguments
@@ -39,14 +48,18 @@
 
 ---
 
 - `-h`, `--help`: Shows the help message
 - `-f`, `--format`: Selects the format of the output sheet (see [Supported Sheets](#supported-sheets))
 - `-d`, `--digits`: Specifies the number of digits in the ASN (e.g. for the default number 7, the ASN will look like 'ASN0000001')
 - `-b`, `--border`: Generates the borders around the labels to help debug alignment issues (see [Tips & Tricks](#tips--tricks))
+- `-r`, `--row-wise`: Increments the labels from left to right instead of top to bottom
+- `-n`, `--num-labels`: Number of lables to be printed on the sheet
+- `-p`, `--pages`: Number of pages to be generated, ignored if -n is present.
+- `-s`, `--start-position`: Positon of first label to be printed, eighter defined as ROW:COLUMN or NUMBER. Starting from 1 eg. to use the whole sheet it would be 1:1 or 1. Useful if you have a partly used sheet from using `-n`.
 
 ## Supported Sheets
 Some different sheet types are supported with the `-f`/`--format` argument, however, not all are tested.
 
 The default is Avery L4731.
 
 Currently tested and known working are:
```

### Comparing `paperless_asn_qr_codes-0.2.0/pyproject.toml` & `paperless_asn_qr_codes-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "argparse",
   "reportlab",
   "reportlab_qrcode"
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/entropia/paperless-asn-qr-codes#readme"
```

### Comparing `paperless_asn_qr_codes-0.2.0/PKG-INFO` & `paperless_asn_qr_codes-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: paperless-asn-qr-codes
-Version: 0.2.0
+Version: 0.3.0
 Summary: Code for generating paperless ASN labels with QR codes
 Project-URL: Documentation, https://github.com/entropia/paperless-asn-qr-codes#readme
 Project-URL: Issues, https://github.com/entropia/paperless-asn-qr-codes/issues
 Project-URL: Source, https://github.com/entropia/paperless-asn-qr-codes
 Author-email: Jan Christian Grünhage <jan.christian@gruenhage.xyz>, margau <dev@marvingaube.de>
 License-Expression: GPL-3.0
 License-File: LICENSE
@@ -12,15 +12,14 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
-Requires-Dist: argparse
 Requires-Dist: reportlab
 Requires-Dist: reportlab-qrcode
 Description-Content-Type: text/markdown
 
 # paperless-asn-qr-codes
 
 `paperless-asn-qr-codes` is a command line utility for generating ASN labels
@@ -32,28 +31,37 @@
 ```console
 pip install paperless-asn-qr-codes
 ```
 
 ## Usage
 
 ```
-usage: paperless-asn-qr-codes [-h] [--format {averyL4731,avery5160,avery5161,avery5163,avery5167,avery5371}] [--border] start_asn output_file
+usage: paperless-asn-qr-codes [-h] [--format {averyL4731,avery5160,avery5161,avery5163,avery5167,avery5371}] [--digits DIGITS] [--border] [--row-wise] [--num-labels NUM_LABELS] [--pages PAGES]
+                              [--start-position START_POSITION]
+                              start_asn output_file
 
 CLI Tool for generating paperless ASN labels with QR codes
 
 positional arguments:
   start_asn             The value of the first ASN
   output_file           The output file to write to (default: labels.pdf)
 
 options:
   -h, --help            show this help message and exit
   --format {averyL4731,avery5160,avery5161,avery5163,avery5167,avery5371}, -f {averyL4731,avery5160,avery5161,avery5163,avery5167,avery5371}
   --digits DIGITS, -d DIGITS
                         Number of digits in the ASN (default: 7, produces 'ASN0000001')
   --border, -b          Display borders around labels, useful for debugging the printer alignment
+  --row-wise, -r        Increment the ASNs row-wise, go from left to right
+  --num-labels NUM_LABELS, -n NUM_LABELS
+                        Number of labels to be printed on the sheet
+  --pages PAGES, -p PAGES
+                        Number of pages to be printed, ignored if NUM_LABELS is set (default: 1)
+  --start-position START_POSITION, -s START_POSITION
+                        Define the starting position on the sheet, eighter as ROW:COLUMN or COUNT, both starting from 1 (default: 1:1 or 1)
 ```
 
 ### Mandatory arguments
 
 - `<start_asn>`: The value of the first ASN to generate
 
 ### Optional arguments
@@ -62,14 +70,18 @@
 
 ---
 
 - `-h`, `--help`: Shows the help message
 - `-f`, `--format`: Selects the format of the output sheet (see [Supported Sheets](#supported-sheets))
 - `-d`, `--digits`: Specifies the number of digits in the ASN (e.g. for the default number 7, the ASN will look like 'ASN0000001')
 - `-b`, `--border`: Generates the borders around the labels to help debug alignment issues (see [Tips & Tricks](#tips--tricks))
+- `-r`, `--row-wise`: Increments the labels from left to right instead of top to bottom
+- `-n`, `--num-labels`: Number of lables to be printed on the sheet
+- `-p`, `--pages`: Number of pages to be generated, ignored if -n is present.
+- `-s`, `--start-position`: Positon of first label to be printed, eighter defined as ROW:COLUMN or NUMBER. Starting from 1 eg. to use the whole sheet it would be 1:1 or 1. Useful if you have a partly used sheet from using `-n`.
 
 ## Supported Sheets
 Some different sheet types are supported with the `-f`/`--format` argument, however, not all are tested.
 
 The default is Avery L4731.
 
 Currently tested and known working are:
```

