# Comparing `tmp/sts_lib-0.31.2.tar.gz` & `tmp/sts_lib-0.32.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sts_lib-0.31.2.tar", last modified: Sun May 12 07:10:18 2024, max compression
+gzip compressed data, was "sts_lib-0.32.0.tar", last modified: Sat May 18 08:31:02 2024, max compression
```

## Comparing `sts_lib-0.31.2.tar` & `sts_lib-0.32.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 07:10:18.248735 sts_lib-0.31.2/
--rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.31.2/LICENSE
--rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.31.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6916 2024-05-12 07:10:18.248735 sts_lib-0.31.2/PKG-INFO
--rw-rw-rw-   0        0        0     5463 2024-04-29 19:01:51.000000 sts_lib-0.31.2/README.md
--rw-rw-rw-   0        0        0     1728 2024-05-12 07:10:18.250746 sts_lib-0.31.2/setup.cfg
--rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.31.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 07:10:18.169152 sts_lib-0.31.2/sts/
--rw-rw-rw-   0        0        0    52886 2024-05-12 07:09:50.000000 sts_lib-0.31.2/sts/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.31.2/sts/__main__.py
--rw-rw-rw-   0        0        0     7551 2024-05-07 18:11:46.000000 sts_lib-0.31.2/sts/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-12 07:10:18.169152 sts_lib-0.31.2/sts/data/
-drwxrwxrwx   0        0        0        0 2024-05-12 07:10:18.178708 sts_lib-0.31.2/sts/data/config/
--rw-rw-rw-   0        0        0      915 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/_default.json
--rw-rw-rw-   0        0        0      608 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/hk2s.json
--rw-rw-rw-   0        0        0      346 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/hk2t.json
--rw-rw-rw-   0        0        0      410 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/jp2t.json
--rw-rw-rw-   0        0        0      419 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/s2hk.json
--rw-rw-rw-   0        0        0      267 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/s2t.json
--rw-rw-rw-   0        0        0      417 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/s2tw.json
--rw-rw-rw-   0        0        0      607 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/s2twp.json
--rw-rw-rw-   0        0        0      247 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/t2hk.json
--rw-rw-rw-   0        0        0      261 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/t2jp.json
--rw-rw-rw-   0        0        0      267 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/t2s.json
--rw-rw-rw-   0        0        0      245 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/t2tw.json
--rw-rw-rw-   0        0        0      606 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/tw2s.json
--rw-rw-rw-   0        0        0      670 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/tw2sp.json
--rw-rw-rw-   0        0        0      344 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/config/tw2t.json
-drwxrwxrwx   0        0        0        0 2024-05-12 07:10:18.189169 sts_lib-0.31.2/sts/data/dictionary/
--rw-rw-rw-   0        0        0      595 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/HKVariants.txt
--rw-rw-rw-   0        0        0     2865 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/HKVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0      103 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/JPShinjitaiCharacters.txt
--rw-rw-rw-   0        0        0     2720 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/JPShinjitaiPhrases.txt
--rw-rw-rw-   0        0        0     3307 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/JPVariants.txt
--rw-rw-rw-   0        0        0    38333 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/STCharacters.txt
--rw-rw-rw-   0        0        0  1053351 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/STPhrases.txt
--rw-rw-rw-   0        0        0    38740 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/TSCharacters.txt
--rw-rw-rw-   0        0        0     5438 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/TSPhrases.txt
--rw-rw-rw-   0        0        0     8014 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/TWPhrasesIT.txt
--rw-rw-rw-   0        0        0     2205 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/TWPhrasesName.txt
--rw-rw-rw-   0        0        0      608 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/TWPhrasesOther.txt
--rw-rw-rw-   0        0        0      351 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/TWVariants.txt
--rw-rw-rw-   0        0        0     1143 2024-05-08 13:34:57.000000 sts_lib-0.31.2/sts/data/dictionary/TWVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0    22659 2024-05-11 09:04:03.000000 sts_lib-0.31.2/sts/data/htmlpage.tpl.html
-drwxrwxrwx   0        0        0        0 2024-05-12 07:10:18.219108 sts_lib-0.31.2/sts/data/scheme/
--rw-rw-rw-   0        0        0    21633 2024-05-11 06:46:32.000000 sts_lib-0.31.2/sts/data/scheme/st_multi.txt
--rw-rw-rw-   0        0        0      436 2024-05-11 06:46:32.000000 sts_lib-0.31.2/sts/data/scheme/ts_multi.txt
--rw-rw-rw-   0        0        0     2108 2024-05-11 06:46:32.000000 sts_lib-0.31.2/sts/data/scheme/variant.txt
-drwxrwxrwx   0        0        0        0 2024-05-12 07:10:18.239124 sts_lib-0.31.2/sts_lib.egg-info/
--rw-rw-rw-   0        0        0     6916 2024-05-12 07:10:18.000000 sts_lib-0.31.2/sts_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1325 2024-05-12 07:10:18.000000 sts_lib-0.31.2/sts_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 07:10:18.000000 sts_lib-0.31.2/sts_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-12 07:10:18.000000 sts_lib-0.31.2/sts_lib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      202 2024-05-12 07:10:18.000000 sts_lib-0.31.2/sts_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-12 07:10:18.000000 sts_lib-0.31.2/sts_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 08:31:02.789052 sts_lib-0.32.0/
+-rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.32.0/LICENSE
+-rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.32.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6916 2024-05-18 08:31:02.789052 sts_lib-0.32.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5463 2024-04-29 19:01:51.000000 sts_lib-0.32.0/README.md
+-rw-rw-rw-   0        0        0     1728 2024-05-18 08:31:02.791027 sts_lib-0.32.0/setup.cfg
+-rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.32.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 08:31:02.545657 sts_lib-0.32.0/sts/
+-rw-rw-rw-   0        0        0    55131 2024-05-18 08:12:48.000000 sts_lib-0.32.0/sts/__init__.py
+-rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.32.0/sts/__main__.py
+-rw-rw-rw-   0        0        0     7551 2024-05-07 18:11:46.000000 sts_lib-0.32.0/sts/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-18 08:31:02.545657 sts_lib-0.32.0/sts/data/
+drwxrwxrwx   0        0        0        0 2024-05-18 08:31:02.586151 sts_lib-0.32.0/sts/data/config/
+-rw-rw-rw-   0        0        0      915 2024-05-16 19:09:29.000000 sts_lib-0.32.0/sts/data/config/_default.json
+-rw-rw-rw-   0        0        0      635 2024-05-18 05:04:31.000000 sts_lib-0.32.0/sts/data/config/hk2s.json
+-rw-rw-rw-   0        0        0      373 2024-05-18 05:04:31.000000 sts_lib-0.32.0/sts/data/config/hk2t.json
+-rw-rw-rw-   0        0        0      437 2024-05-18 05:04:31.000000 sts_lib-0.32.0/sts/data/config/jp2t.json
+-rw-rw-rw-   0        0        0      446 2024-05-18 05:04:31.000000 sts_lib-0.32.0/sts/data/config/s2hk.json
+-rw-rw-rw-   0        0        0      294 2024-05-18 05:04:31.000000 sts_lib-0.32.0/sts/data/config/s2t.json
+-rw-rw-rw-   0        0        0      444 2024-05-18 05:04:31.000000 sts_lib-0.32.0/sts/data/config/s2tw.json
+-rw-rw-rw-   0        0        0      634 2024-05-18 05:04:31.000000 sts_lib-0.32.0/sts/data/config/s2twp.json
+-rw-rw-rw-   0        0        0      274 2024-05-18 05:04:31.000000 sts_lib-0.32.0/sts/data/config/t2hk.json
+-rw-rw-rw-   0        0        0      288 2024-05-18 05:04:31.000000 sts_lib-0.32.0/sts/data/config/t2jp.json
+-rw-rw-rw-   0        0        0      294 2024-05-18 05:04:31.000000 sts_lib-0.32.0/sts/data/config/t2s.json
+-rw-rw-rw-   0        0        0      272 2024-05-18 05:04:31.000000 sts_lib-0.32.0/sts/data/config/t2tw.json
+-rw-rw-rw-   0        0        0      633 2024-05-18 05:04:31.000000 sts_lib-0.32.0/sts/data/config/tw2s.json
+-rw-rw-rw-   0        0        0      697 2024-05-18 05:04:31.000000 sts_lib-0.32.0/sts/data/config/tw2sp.json
+-rw-rw-rw-   0        0        0      371 2024-05-18 05:04:31.000000 sts_lib-0.32.0/sts/data/config/tw2t.json
+drwxrwxrwx   0        0        0        0 2024-05-18 08:31:02.759039 sts_lib-0.32.0/sts/data/dictionary/
+-rw-rw-rw-   0        0        0      595 2024-05-08 13:34:57.000000 sts_lib-0.32.0/sts/data/dictionary/HKVariants.txt
+-rw-rw-rw-   0        0        0     2865 2024-05-08 13:34:57.000000 sts_lib-0.32.0/sts/data/dictionary/HKVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0      103 2024-05-08 13:34:57.000000 sts_lib-0.32.0/sts/data/dictionary/JPShinjitaiCharacters.txt
+-rw-rw-rw-   0        0        0     2720 2024-05-08 13:34:57.000000 sts_lib-0.32.0/sts/data/dictionary/JPShinjitaiPhrases.txt
+-rw-rw-rw-   0        0        0     3307 2024-05-08 13:34:57.000000 sts_lib-0.32.0/sts/data/dictionary/JPVariants.txt
+-rw-rw-rw-   0        0        0    38333 2024-05-08 13:34:57.000000 sts_lib-0.32.0/sts/data/dictionary/STCharacters.txt
+-rw-rw-rw-   0        0        0  1053351 2024-05-08 13:34:57.000000 sts_lib-0.32.0/sts/data/dictionary/STPhrases.txt
+-rw-rw-rw-   0        0        0    38740 2024-05-08 13:34:57.000000 sts_lib-0.32.0/sts/data/dictionary/TSCharacters.txt
+-rw-rw-rw-   0        0        0     5438 2024-05-08 13:34:57.000000 sts_lib-0.32.0/sts/data/dictionary/TSPhrases.txt
+-rw-rw-rw-   0        0        0     8014 2024-05-08 13:34:57.000000 sts_lib-0.32.0/sts/data/dictionary/TWPhrasesIT.txt
+-rw-rw-rw-   0        0        0     2205 2024-05-08 13:34:57.000000 sts_lib-0.32.0/sts/data/dictionary/TWPhrasesName.txt
+-rw-rw-rw-   0        0        0      608 2024-05-08 13:34:57.000000 sts_lib-0.32.0/sts/data/dictionary/TWPhrasesOther.txt
+-rw-rw-rw-   0        0        0      351 2024-05-08 13:34:57.000000 sts_lib-0.32.0/sts/data/dictionary/TWVariants.txt
+-rw-rw-rw-   0        0        0     1143 2024-05-08 13:34:57.000000 sts_lib-0.32.0/sts/data/dictionary/TWVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0    22659 2024-05-18 07:27:32.000000 sts_lib-0.32.0/sts/data/htmlpage.tpl.html
+drwxrwxrwx   0        0        0        0 2024-05-18 08:31:02.769060 sts_lib-0.32.0/sts/data/scheme/
+-rw-rw-rw-   0        0        0    21633 2024-05-18 08:30:03.000000 sts_lib-0.32.0/sts/data/scheme/st_multi.txt
+-rw-rw-rw-   0        0        0      436 2024-05-18 08:30:03.000000 sts_lib-0.32.0/sts/data/scheme/ts_multi.txt
+-rw-rw-rw-   0        0        0     2108 2024-05-18 08:30:03.000000 sts_lib-0.32.0/sts/data/scheme/variant.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 08:31:02.785054 sts_lib-0.32.0/sts_lib.egg-info/
+-rw-rw-rw-   0        0        0     6916 2024-05-18 08:31:02.000000 sts_lib-0.32.0/sts_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1325 2024-05-18 08:31:02.000000 sts_lib-0.32.0/sts_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 08:31:02.000000 sts_lib-0.32.0/sts_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-18 08:31:02.000000 sts_lib-0.32.0/sts_lib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      202 2024-05-18 08:31:02.000000 sts_lib-0.32.0/sts_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-18 08:31:02.000000 sts_lib-0.32.0/sts_lib.egg-info/top_level.txt
```

### Comparing `sts_lib-0.31.2/LICENSE` & `sts_lib-0.32.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.2/PKG-INFO` & `sts_lib-0.32.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.31.2
+Version: 0.32.0
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
```

### Comparing `sts_lib-0.31.2/README.md` & `sts_lib-0.32.0/README.md`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.2/setup.cfg` & `sts_lib-0.32.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.2/sts/__init__.py` & `sts_lib-0.32.0/sts/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python3
-"""An open library for flexible simplified-traditional Chinese text conversion.
-"""
+"""An open library for flexible simplified-traditional Chinese text conversion."""
 import html
 import itertools
 import json
 import math
 import os
 import re
 import sys
@@ -44,15 +43,15 @@
         @_lazyprop.setter
         def _lazyprop(self, value):
             setattr(self, attr_name, value)
 
         return _lazyprop
 
 
-__version__ = '0.31.2'
+__version__ = '0.32.0'
 
 StsDictMatch = namedtuple('StsDictMatch', ['conv', 'start', 'end'])
 StsDictConv = namedtuple('StsDictConv', ['key', 'values'])
 StsConvExclude = namedtuple('StsConvExclude', ['text'])
 
 
 class StreamList(list):
@@ -88,17 +87,61 @@
             return False
         else:
             return True
 
 
 class Unicode():
     """Utilities for Unicode string handling.
+
+    We also allow IVI and VS in an IDS.
     """
-    @staticmethod
-    def composite_length(text, pos):
+    @classmethod
+    def is_valid_ids_hanzi(cls, code):
+        """Test if code is a valid "hanzi" in an IDS.
+
+        IDS := Ideographic | Radical | CJK_Stroke | Private Use
+             | U+FF1F
+             | IDS_UnaryOperator IDS
+             | IDS_BinaryOperator IDS IDS
+             | IDS_TrinaryOperator IDS IDS IDS
+        """
+        return (
+            0x4E00 <= code <= 0x9FFF  # CJK unified
+            or 0x3400 <= code <= 0x4DBF  # Ext-A
+            or 0xF900 <= code <= 0xFAFF  # CJK Compatibility Ideographs
+            or 0x20000 <= code <= 0x3FFFF  # ExtB+ (including CJK Compatibility Ideographs Supplement)
+            or 0x2E80 <= code <= 0x2FDF  # Radical
+            or 0x31C0 <= code <= 0x31EF  # Stroke
+            or 0xE000 <= code <= 0xF8FF or 0xF0000 <= code <= 0x1FFFFF  # Private
+            or code == 0xFF1F  # ？
+            or 0xFE00 <= code <= 0xFE0F or 0xE0100 <= code <= 0xE01EF  # VS (non-standard)
+        )
+
+    @classmethod
+    def is_hanzi(cls, code):
+        """Test if code is a "hanzi" (which prefers no space)."""
+        return (
+            cls.is_valid_ids_hanzi(code)
+            or 0x2FF0 <= code <= 0x33FF  # IDS operator
+                                         # CJK Symbols and Punctuation (including IVI)
+                                         # Hiragana
+                                         # Katakana
+                                         # Bopomofo
+                                         # Hangul Compatibility Jamo
+                                         # Kanbun
+                                         # Bopomofo Extended
+                                         # (CJK Strokes)
+                                         # Katakana Phonetic Extensions
+                                         # Enclosed CJK Letters and Months
+                                         # CJK Compatibility
+            or 0xFF00 <= code <= 0xFFEF  # Halfwidth and Fullwidth Forms
+        )
+
+    @classmethod
+    def composite_length(cls, text, pos):
         """Get the length of the Unicode composite at pos.
 
         A unicode composite is a complex of characters with composers.
         For example, an ideographic description sequence (IDS),
         or a hanzi with a variant selector (VS), etc.
         """
         i = pos
@@ -110,41 +153,30 @@
             code = ord(text[i])
 
             # check if the current char is a prefix composer
             if code == 0x303E:
                 # ideographic variation indicator
                 is_ids = True
                 length += 1
-            elif 0x2FF0 <= code <= 0x2FF1 or 0x2FF4 <= code <= 0x2FFB:
+            elif 0x2FFE <= code <= 0x2FFF:
+                # IDS unary operator
+                is_ids = True
+                length += 1
+            elif 0x2FF0 <= code <= 0x2FF1 or 0x2FF4 <= code <= 0x2FFD or code == 0x31EF:
                 # IDS binary operator
                 is_ids = True
                 length += 2
             elif 0x2FF2 <= code <= 0x2FF3:
                 # IDS trinary operator
                 is_ids = True
                 length += 3
-            elif is_ids and not (
-                0x4E00 <= code <= 0x9FFF  # CJK unified
-                or 0x3400 <= code <= 0x4DBF or 0x20000 <= code <= 0x3FFFF  # Ext-A, ExtB+
-                or 0xF900 <= code <= 0xFAFF or 0x2F800 <= code <= 0x2FA1F  # Compatibility
-                or 0x2E80 <= code <= 0x2FDF  # Radical
-                or 0x31C0 <= code <= 0x31EF  # Stroke
-                or 0xE000 <= code <= 0xF8FF or 0xF0000 <= code <= 0x1FFFFF  # Private
-                or code == 0xFF1F  # ？
-                or 0xFE00 <= code <= 0xFE0F or 0xE0100 <= code <= 0xE01EF  # VS
-            ):
+            elif is_ids and not cls.is_valid_ids_hanzi(code):
                 # check for a valid IDS to avoid a breaking on e.g.:
                 #
                 #     IDS包括⿰⿱⿲⿳⿴⿵⿶⿷⿸⿹⿺⿻，可用於…
-                #
-                # - IDS := Ideographic | Radical | CJK_Stroke | Private Use
-                #        | U+FF1F | IDS_BinaryOperator IDS IDS
-                #        | IDS_TrinaryOperator IDS IDS IDS
-                #
-                # - We also allow IVI and VS in an IDS.
                 break
 
             # check if the next char is a postfix composer
             if i + 1 < total:
                 code = ord(text[i + 1])
                 if 0xFE00 <= code <= 0xFE0F:
                     # variation selectors
@@ -174,16 +206,15 @@
             i += 1
             length -= 1
 
         return i - pos
 
     @classmethod
     def split(cls, text):
-        """Split a text into a list of Unicode composites.
-        """
+        """Split a text into a list of Unicode composites."""
         i = 0
         total = len(text)
         result = []
         while i < total:
             length = cls.composite_length(text, i)
             result.append(text[i:i + length])
             i += length
@@ -206,41 +237,35 @@
     - JSON: which is dumped from the internal data structure.
     """
     def __init__(self, *args, **kwargs):
         self._dict = {}
         self.update(dict(*args, **kwargs))
 
     def __repr__(self):
-        """Implementation of repr(self).
-        """
+        """Implementation of repr(self)."""
         return f'{self.__class__.__name__}({repr(list(self.items()))})'
 
     def __getitem__(self, key):
-        """Implementation of self[key].
-        """
+        """Implementation of self[key]."""
         return self._dict[key]
 
     def __contains__(self, item):
-        """Implementation of "item in self".
-        """
+        """Implementation of "item in self"."""
         return item in self._dict
 
     def __len__(self):
-        """Implementation of len(self).
-        """
+        """Implementation of len(self)."""
         return len(self._dict)
 
     def __iter__(self):
-        """Implementation of iter(self).
-        """
+        """Implementation of iter(self)."""
         return iter(self._dict)
 
     def __eq__(self, other):
-        """Implementation of "==" operator.
-        """
+        """Implementation of "==" operator."""
         if not isinstance(other, (dict, StsDict)):
             return False
 
         # faster check for the same type
         if type(self) is type(other):
             return self._dict == other._dict
 
@@ -253,31 +278,27 @@
             keys.add(key)
         for key in other:
             if key not in keys:
                 return False
         return True
 
     def __delitem__(self, key):
-        """Implementation of del self[key].
-        """
+        """Implementation of del self[key]."""
         del self._dict[key]
 
     def keys(self):
-        """Get a generator of keys.
-        """
+        """Get a generator of keys."""
         yield from self._dict.keys()
 
     def values(self):
-        """Get a generator of values.
-        """
+        """Get a generator of values."""
         yield from self._dict.values()
 
     def items(self):
-        """Get a generator of key-values pairs.
-        """
+        """Get a generator of key-values pairs."""
         yield from self._dict.items()
 
     def add(self, key, values, skip_check=False):
         """Add a key-values pair to this dictionary.
 
         Args:
             values: a string or an iterable of strings.
@@ -525,16 +546,15 @@
             for newkey in conv.apply_enum(key, include_short=True, include_self=True):
                 map_keys.setdefault(newkey, None)
 
         for key in map_keys:
             newkeys = self.apply_enum(key)
             for newkey in newkeys:
                 try:
-                    values = stsdict[newkey]
-                    assert values
+                    assert stsdict[newkey]
                 except (KeyError, AssertionError):
                     pass
                 else:
                     break
             else:
                 continue
 
@@ -656,16 +676,15 @@
 
         if not results:
             results.append(_parts if isinstance(_parts, str) else ''.join(_parts))
 
         return results
 
     def _apply_enum_sub(self, parts, stack, data, include_short=False, include_self=False):
-        """Helper function of apply_enum
-        """
+        """Helper function of apply_enum"""
         (newparts, index, matched) = data
         has_atomic_match = False
         i = math.inf
         while i > index:
             match = self.match(parts, index, i)
 
             if match is None:
@@ -791,58 +810,52 @@
 
     Compared with hash, trie is faster for applying conversion,
     but takes more space and is slower to construct.
 
     NOTE: The internal data format is different from base StsDict.
     """
     def __getitem__(self, key):
-        """Implementation of self[key].
-        """
+        """Implementation of self[key]."""
         trie = self._dict
         try:
             for comp in Unicode.split(key):
                 trie = trie[comp]
             return trie['']
         except KeyError:
             raise KeyError(key)
 
     def __contains__(self, item):
-        """Implementation of "item in self".
-        """
+        """Implementation of "item in self"."""
         try:
             self[item]
         except KeyError:
             return False
         else:
             return True
 
     def __len__(self):
-        """Implementation of len(self).
-        """
+        """Implementation of len(self)."""
         return sum(1 for _ in self)
 
     def __iter__(self):
-        """Implementation of iter(self).
-        """
+        """Implementation of iter(self)."""
         return self.keys()
 
     def __delitem__(self, key):
-        """Implementation of del self[key].
-        """
+        """Implementation of del self[key]."""
         trie = self._dict
         try:
             for comp in Unicode.split(key):
                 trie = trie[comp]
             del trie['']
         except KeyError:
             raise KeyError(key)
 
     def keys(self):
-        """Get a generator of keys.
-        """
+        """Get a generator of keys."""
         trie = self._dict
         stack = [('', trie, iter(trie))]
         while stack:
             key, trie, it = stack[-1]
             for comp in it:
                 if comp == '':
                     yield key
@@ -850,16 +863,15 @@
                     trie = trie[comp]
                     stack.append((key + comp, trie, iter(trie)))
                     break
             else:
                 stack.pop()
 
     def values(self):
-        """Get a generator of values.
-        """
+        """Get a generator of values."""
         trie = self._dict
         stack = [(trie, iter(trie))]
         while stack:
             trie, it = stack[-1]
             for comp in it:
                 if comp == '':
                     yield trie[comp]
@@ -867,16 +879,15 @@
                     trie = trie[comp]
                     stack.append((trie, iter(trie)))
                     break
             else:
                 stack.pop()
 
     def items(self):
-        """Get a generator of key-values pairs.
-        """
+        """Get a generator of key-values pairs."""
         trie = self._dict
         stack = [('', trie, iter(trie))]
         while stack:
             key, trie, it = stack[-1]
             for comp in it:
                 if comp == '':
                     yield key, trie[comp]
@@ -936,16 +947,15 @@
         if match:
             conv = StsDictConv(parts[pos:match_end], match)
             return StsDictMatch(conv, pos, match_end)
         return None
 
 
 class StsMaker():
-    """A class for making dictionary file(s).
-    """
+    """A class for making dictionary file(s)."""
     config_dir = os.path.join(os.path.dirname(__file__), 'data', 'config')
     dictionary_dir = os.path.join(os.path.dirname(__file__), 'data', 'dictionary')
 
     def make(self, config_name, base_dir=None,
              skip_check=False, skip_requires=False, quiet=False):
         """Make dictionary file(s) according to a config.
 
@@ -1080,14 +1090,15 @@
         else:
             for i, src in enumerate(srcs):
                 srcs[i] = self.normalize_dict_scheme(src, config_dir)
 
         mode = dict_scheme.setdefault('mode', 'load')
         dict_scheme['sort'] = bool(dict_scheme.get('sort'))
         dict_scheme['check'] = bool(dict_scheme.get('check'))
+        dict_scheme['auto_space'] = bool(dict_scheme.get('auto_space'))
 
         if mode == 'filter':
             method = dict_scheme.setdefault('method', 'remove_key_values')
             if method not in ('remove_keys', 'remove_key_values'):
                 raise ValueError(f'unknown method for filter: {method}')
 
             try:
@@ -1147,14 +1158,17 @@
         try:
             func = getattr(self, f'_make_dict_mode_{mode}')
         except AttributeError:
             raise ValueError(f'Specified mode is not supported: {mode}')
         else:
             table = func(dict_scheme)
 
+        if dict_scheme['auto_space']:
+            self._make_dict_auto_space(table)
+
         if dest:
             os.makedirs(os.path.dirname(dest), exist_ok=True)
             if format == 'tlist':
                 Trie(table).dumpjson(dest, sort=sort)
             elif format == 'jlist':
                 table.dumpjson(dest, sort=sort)
             else:  # default: list
@@ -1307,14 +1321,39 @@
                 try:
                     t.remove(v)
                 except ValueError:
                     pass
             if not t:
                 del table[k]
 
+    def _make_dict_auto_space(self, table):
+        extra_table = Table()
+        for key, values in table.items():
+            newkey = self._make_dict_auto_space_make_spaced(key)
+            if newkey != key and newkey not in table:
+                newvalues = [self._make_dict_auto_space_make_spaced(v) for v in values]
+                extra_table.add(newkey, newvalues)
+        for key, values in extra_table.items():
+            table.add(key, values, skip_check=True)
+
+    @staticmethod
+    def _make_dict_auto_space_make_spaced(text):
+        last_is_hanzi = None
+        rv = []
+        parts = Unicode.split(text)
+        for part in parts:
+            is_hanzi = all(Unicode.is_hanzi(ord(c)) for c in part)
+            if last_is_hanzi is None:
+                last_is_hanzi = is_hanzi
+            elif last_is_hanzi != is_hanzi:
+                rv.append(' ')
+                last_is_hanzi = is_hanzi
+            rv.append(part)
+        return ''.join(rv)
+
     def get_config_file(self, config, base_dir=None):
         """Calculate the path of a config file.
 
         1. Use it if it's an absolute path.
         2. Assume relative to base_dir or CWD.
         3. Assume relative to default config directory. (basename only; .json omissible)
         4. If not found, return 2.
@@ -1394,16 +1433,15 @@
             if self.check_update(src, mtime):
                 rv = dict_scheme['_updated'] = True
 
         return rv
 
 
 class StsConverter():
-    """Convert a text using an stsdict.
-    """
+    """Convert a text using an stsdict."""
     exclude_return_group_pattern = re.compile(r'^return\d*$')
     template_placeholder_pattern = re.compile(r'%(\w*)%')
     htmlpage_template = os.path.join(os.path.dirname(__file__), 'data', 'htmlpage.tpl.html')
 
     def __init__(self, stsdict):
         """Initialize a converter.
 
@@ -1456,16 +1494,15 @@
             index = end
 
         t = text[index:]
         if t:
             yield from self.table.apply(t)
 
     def convert_formatted(self, text, format=None, exclude=None):
-        """Convert a text and yield each formatted part.
-        """
+        """Convert a text and yield each formatted part."""
         conv = self.convert(text, exclude=exclude)
         format = format if format is not None else 'txt'
         formatter = getattr(self, f'_convert_formatted_{format}')
         yield from formatter(conv)
 
     def _convert_formatted_txt(self, parts):
         for part in parts:
```

### Comparing `sts_lib-0.31.2/sts/cli.py` & `sts_lib-0.32.0/sts/cli.py`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.2/sts/data/config/_default.json` & `sts_lib-0.32.0/sts/data/config/_default.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.2/sts/data/config/hk2s.json` & `sts_lib-0.32.0/sts/data/config/hk2s.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'dicts'": "{0: {'auto_space': True}}"}*

```diff
@@ -1,10 +1,11 @@
 {
     "dicts": [
         {
+            "auto_space": true,
             "file": "../dictionary/hk2s.tlist",
             "mode": "join",
             "src": [
                 {
                     "mode": "load",
                     "src": [
                         "../dictionary/HKVariantsRevPhrases.txt",
```

### Comparing `sts_lib-0.31.2/sts/data/config/s2twp.json` & `sts_lib-0.32.0/sts/data/config/tw2sp.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.765625%*

 * *Differences: {"'dicts'": "{0: {'file': '../dictionary/tw2sp.tlist', 'src': {0: {'src': "*

 * *            "['../dictionary/TWPhrasesRev.list', '../dictionary/TWVariantsRevPhrases.txt', "*

 * *            "'../dictionary/TWVariantsRev.list']}, 1: {'src': ['../dictionary/TSPhrases.txt', "*

 * *            "'../dictionary/TSCharacters.txt']}}, 'auto_space': True}}",*

 * * "'name'": "'Traditional Chinese (Taiwan standard) to Simplified Chinese (with phrases)'"}*

```diff
@@ -1,28 +1,30 @@
 {
     "dicts": [
         {
-            "file": "../dictionary/s2twp.tlist",
+            "auto_space": true,
+            "file": "../dictionary/tw2sp.tlist",
             "mode": "join",
             "src": [
                 {
                     "mode": "load",
                     "src": [
-                        "../dictionary/STPhrases.txt",
-                        "../dictionary/STCharacters.txt"
+                        "../dictionary/TWPhrasesRev.list",
+                        "../dictionary/TWVariantsRevPhrases.txt",
+                        "../dictionary/TWVariantsRev.list"
                     ]
                 },
                 {
                     "mode": "load",
                     "src": [
-                        "../dictionary/TWPhrases.list",
-                        "../dictionary/TWVariants.txt"
+                        "../dictionary/TSPhrases.txt",
+                        "../dictionary/TSCharacters.txt"
                     ]
                 }
             ]
         }
     ],
-    "name": "Simplified Chinese to Traditional Chinese (Taiwan standard, with phrases)",
+    "name": "Traditional Chinese (Taiwan standard) to Simplified Chinese (with phrases)",
     "requires": [
         "_default.json"
     ]
 }
```

### Comparing `sts_lib-0.31.2/sts/data/config/tw2s.json` & `sts_lib-0.32.0/sts/data/config/s2twp.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.765625%*

 * *Differences: {"'dicts'": "{0: {'file': '../dictionary/s2twp.tlist', 'src': {0: {'src': "*

 * *            "['../dictionary/STPhrases.txt', '../dictionary/STCharacters.txt']}, 1: {'src': "*

 * *            "['../dictionary/TWPhrases.list', '../dictionary/TWVariants.txt']}}, 'auto_space': "*

 * *            'True}}',*

 * * "'name'": "'Simplified Chinese to Traditional Chinese (Taiwan standard, with phrases)'"}*

```diff
@@ -1,28 +1,29 @@
 {
     "dicts": [
         {
-            "file": "../dictionary/tw2s.tlist",
+            "auto_space": true,
+            "file": "../dictionary/s2twp.tlist",
             "mode": "join",
             "src": [
                 {
                     "mode": "load",
                     "src": [
-                        "../dictionary/TWVariantsRevPhrases.txt",
-                        "../dictionary/TWVariantsRev.list"
+                        "../dictionary/STPhrases.txt",
+                        "../dictionary/STCharacters.txt"
                     ]
                 },
                 {
                     "mode": "load",
                     "src": [
-                        "../dictionary/TSPhrases.txt",
-                        "../dictionary/TSCharacters.txt"
+                        "../dictionary/TWPhrases.list",
+                        "../dictionary/TWVariants.txt"
                     ]
                 }
             ]
         }
     ],
-    "name": "Traditional Chinese (Taiwan standard) to Simplified Chinese",
+    "name": "Simplified Chinese to Traditional Chinese (Taiwan standard, with phrases)",
     "requires": [
         "_default.json"
     ]
 }
```

### Comparing `sts_lib-0.31.2/sts/data/config/tw2sp.json` & `sts_lib-0.32.0/sts/data/config/tw2s.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7699652777777777%*

 * *Differences: {"'dicts'": "{0: {'file': '../dictionary/tw2s.tlist', 'src': {0: {'src': {delete: [0]}}}, "*

 * *            "'auto_space': True}}",*

 * * "'name'": "'Traditional Chinese (Taiwan standard) to Simplified Chinese'"}*

```diff
@@ -1,29 +1,29 @@
 {
     "dicts": [
         {
-            "file": "../dictionary/tw2sp.tlist",
+            "auto_space": true,
+            "file": "../dictionary/tw2s.tlist",
             "mode": "join",
             "src": [
                 {
                     "mode": "load",
                     "src": [
-                        "../dictionary/TWPhrasesRev.list",
                         "../dictionary/TWVariantsRevPhrases.txt",
                         "../dictionary/TWVariantsRev.list"
                     ]
                 },
                 {
                     "mode": "load",
                     "src": [
                         "../dictionary/TSPhrases.txt",
                         "../dictionary/TSCharacters.txt"
                     ]
                 }
             ]
         }
     ],
-    "name": "Traditional Chinese (Taiwan standard) to Simplified Chinese (with phrases)",
+    "name": "Traditional Chinese (Taiwan standard) to Simplified Chinese",
     "requires": [
         "_default.json"
     ]
 }
```

### Comparing `sts_lib-0.31.2/sts/data/dictionary/HKVariants.txt` & `sts_lib-0.32.0/sts/data/dictionary/HKVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.2/sts/data/dictionary/HKVariantsRevPhrases.txt` & `sts_lib-0.32.0/sts/data/dictionary/HKVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.2/sts/data/dictionary/JPShinjitaiPhrases.txt` & `sts_lib-0.32.0/sts/data/dictionary/JPShinjitaiPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.2/sts/data/dictionary/JPVariants.txt` & `sts_lib-0.32.0/sts/data/dictionary/JPVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.2/sts/data/dictionary/STCharacters.txt` & `sts_lib-0.32.0/sts/data/dictionary/STCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.2/sts/data/dictionary/STPhrases.txt` & `sts_lib-0.32.0/sts/data/dictionary/STPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.2/sts/data/dictionary/TSCharacters.txt` & `sts_lib-0.32.0/sts/data/dictionary/TSCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.2/sts/data/dictionary/TSPhrases.txt` & `sts_lib-0.32.0/sts/data/dictionary/TSPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.2/sts/data/dictionary/TWPhrasesIT.txt` & `sts_lib-0.32.0/sts/data/dictionary/TWPhrasesIT.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.2/sts/data/dictionary/TWPhrasesName.txt` & `sts_lib-0.32.0/sts/data/dictionary/TWPhrasesName.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.2/sts/data/dictionary/TWPhrasesOther.txt` & `sts_lib-0.32.0/sts/data/dictionary/TWPhrasesOther.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.2/sts/data/dictionary/TWVariantsRevPhrases.txt` & `sts_lib-0.32.0/sts/data/dictionary/TWVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.2/sts/data/htmlpage.tpl.html` & `sts_lib-0.32.0/sts/data/htmlpage.tpl.html`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.2/sts/data/scheme/st_multi.txt` & `sts_lib-0.32.0/sts/data/scheme/st_multi.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.2/sts/data/scheme/variant.txt` & `sts_lib-0.32.0/sts/data/scheme/variant.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.31.2/sts_lib.egg-info/PKG-INFO` & `sts_lib-0.32.0/sts_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.31.2
+Version: 0.32.0
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
```

### Comparing `sts_lib-0.31.2/sts_lib.egg-info/SOURCES.txt` & `sts_lib-0.32.0/sts_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

