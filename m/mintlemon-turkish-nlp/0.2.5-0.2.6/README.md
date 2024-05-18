# Comparing `tmp/mintlemon-turkish-nlp-0.2.5.tar.gz` & `tmp/mintlemon-turkish-nlp-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mintlemon-turkish-nlp-0.2.5.tar", last modified: Thu Apr  6 07:06:22 2023, max compression
+gzip compressed data, was "mintlemon-turkish-nlp-0.2.6.tar", last modified: Sat May 18 16:25:48 2024, max compression
```

## Comparing `mintlemon-turkish-nlp-0.2.5.tar` & `mintlemon-turkish-nlp-0.2.6.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-04-06 07:06:22.234216 mintlemon-turkish-nlp-0.2.5/
--rw-r--r--   0 koc        (501) staff       (20)      784 2023-04-03 01:44:04.000000 mintlemon-turkish-nlp-0.2.5/AUTHORS.rst
--rw-r--r--   0 koc        (501) staff       (20)    11357 2023-04-03 01:44:04.000000 mintlemon-turkish-nlp-0.2.5/LICENSE
--rw-r--r--   0 koc        (501) staff       (20)       75 2023-04-03 01:44:04.000000 mintlemon-turkish-nlp-0.2.5/MANIFEST.in
--rw-r--r--   0 koc        (501) staff       (20)     6994 2023-04-06 07:06:22.233448 mintlemon-turkish-nlp-0.2.5/PKG-INFO
--rw-r--r--   0 koc        (501) staff       (20)     5314 2023-04-06 01:20:16.000000 mintlemon-turkish-nlp-0.2.5/README.md
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-04-06 07:06:22.217305 mintlemon-turkish-nlp-0.2.5/mintlemon/
--rw-r--r--   0 koc        (501) staff       (20)      200 2023-04-03 01:44:04.000000 mintlemon-turkish-nlp-0.2.5/mintlemon/__init__.py
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-04-06 07:06:22.220864 mintlemon-turkish-nlp-0.2.5/mintlemon/data/
--rw-r--r--   0 koc        (501) staff       (20)     1565 2023-04-03 01:44:04.000000 mintlemon-turkish-nlp-0.2.5/mintlemon/data/TR_non_breaking_prefixes.txt
--rw-r--r--   0 koc        (501) staff       (20)   159044 2023-04-03 01:44:04.000000 mintlemon-turkish-nlp-0.2.5/mintlemon/data/ascii_to_str_dict.pickle
--rw-r--r--   0 koc        (501) staff       (20)     4260 2023-04-04 03:07:24.000000 mintlemon-turkish-nlp-0.2.5/mintlemon/data/stop_words.txt
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-04-06 07:06:22.225326 mintlemon-turkish-nlp-0.2.5/mintlemon/normalizer/
--rw-r--r--   0 koc        (501) staff       (20)      138 2023-04-03 01:44:04.000000 mintlemon-turkish-nlp-0.2.5/mintlemon/normalizer/__init__.py
--rw-r--r--   0 koc        (501) staff       (20)    15189 2023-04-03 01:44:04.000000 mintlemon-turkish-nlp-0.2.5/mintlemon/normalizer/_builtin.py
--rw-r--r--   0 koc        (501) staff       (20)    10121 2023-04-06 07:05:05.000000 mintlemon-turkish-nlp-0.2.5/mintlemon/normalizer/normalizer.py
--rw-r--r--   0 koc        (501) staff       (20)     3052 2023-04-05 23:54:04.000000 mintlemon-turkish-nlp-0.2.5/mintlemon/normalizer/text_to_root_dtm.py
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-04-06 07:06:22.228211 mintlemon-turkish-nlp-0.2.5/mintlemon/sentence_splitter/
--rw-r--r--   0 koc        (501) staff       (20)       80 2023-04-03 01:44:04.000000 mintlemon-turkish-nlp-0.2.5/mintlemon/sentence_splitter/__init__.py
--rw-r--r--   0 koc        (501) staff       (20)     1820 2023-04-04 02:44:24.000000 mintlemon-turkish-nlp-0.2.5/mintlemon/sentence_splitter/sentence_splitter.py
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-04-06 07:06:22.232312 mintlemon-turkish-nlp-0.2.5/mintlemon_turkish_nlp.egg-info/
--rw-r--r--   0 koc        (501) staff       (20)     6994 2023-04-06 07:06:21.000000 mintlemon-turkish-nlp-0.2.5/mintlemon_turkish_nlp.egg-info/PKG-INFO
--rw-r--r--   0 koc        (501) staff       (20)      656 2023-04-06 07:06:22.000000 mintlemon-turkish-nlp-0.2.5/mintlemon_turkish_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 koc        (501) staff       (20)        1 2023-04-06 07:06:21.000000 mintlemon-turkish-nlp-0.2.5/mintlemon_turkish_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 koc        (501) staff       (20)      133 2023-04-06 07:06:21.000000 mintlemon-turkish-nlp-0.2.5/mintlemon_turkish_nlp.egg-info/requires.txt
--rw-r--r--   0 koc        (501) staff       (20)       10 2023-04-06 07:06:21.000000 mintlemon-turkish-nlp-0.2.5/mintlemon_turkish_nlp.egg-info/top_level.txt
--rw-r--r--   0 koc        (501) staff       (20)     1087 2023-04-03 01:44:04.000000 mintlemon-turkish-nlp-0.2.5/pyproject.toml
--rw-r--r--   0 koc        (501) staff       (20)       38 2023-04-06 07:06:22.234479 mintlemon-turkish-nlp-0.2.5/setup.cfg
--rw-r--r--   0 koc        (501) staff       (20)     2272 2023-04-06 07:05:48.000000 mintlemon-turkish-nlp-0.2.5/setup.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 16:25:48.969881 mintlemon-turkish-nlp-0.2.6/
+-rw-r--r--   0 koc        (501) staff       (20)      784 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.6/AUTHORS.rst
+-rw-r--r--   0 koc        (501) staff       (20)    11357 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.6/LICENSE
+-rw-r--r--   0 koc        (501) staff       (20)       75 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.6/MANIFEST.in
+-rw-r--r--   0 koc        (501) staff       (20)     3823 2024-05-18 16:25:48.969232 mintlemon-turkish-nlp-0.2.6/PKG-INFO
+-rw-r--r--   0 koc        (501) staff       (20)     1772 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.6/README.md
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 16:25:48.955800 mintlemon-turkish-nlp-0.2.6/mintlemon/
+-rw-r--r--   0 koc        (501) staff       (20)      275 2024-02-19 23:15:49.000000 mintlemon-turkish-nlp-0.2.6/mintlemon/__init__.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 16:25:48.958702 mintlemon-turkish-nlp-0.2.6/mintlemon/data/
+-rw-r--r--   0 koc        (501) staff       (20)     1565 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.6/mintlemon/data/TR_non_breaking_prefixes.txt
+-rw-r--r--   0 koc        (501) staff       (20)   159044 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.6/mintlemon/data/ascii_to_str_dict.pickle
+-rw-r--r--   0 koc        (501) staff       (20)     4260 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.6/mintlemon/data/stop_words.txt
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 16:25:48.961379 mintlemon-turkish-nlp-0.2.6/mintlemon/normalizer/
+-rw-r--r--   0 koc        (501) staff       (20)      138 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.6/mintlemon/normalizer/__init__.py
+-rw-r--r--   0 koc        (501) staff       (20)    15189 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.6/mintlemon/normalizer/_builtin.py
+-rw-r--r--   0 koc        (501) staff       (20)    12341 2024-02-16 12:50:56.000000 mintlemon-turkish-nlp-0.2.6/mintlemon/normalizer/normalizer.py
+-rw-r--r--   0 koc        (501) staff       (20)     3025 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.6/mintlemon/normalizer/text_to_root_dtm.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 16:25:48.963007 mintlemon-turkish-nlp-0.2.6/mintlemon/sentence_splitter/
+-rw-r--r--   0 koc        (501) staff       (20)       80 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.6/mintlemon/sentence_splitter/__init__.py
+-rw-r--r--   0 koc        (501) staff       (20)     1592 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.6/mintlemon/sentence_splitter/sentence_splitter.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 16:25:48.964387 mintlemon-turkish-nlp-0.2.6/mintlemon/turkish_spellcheck/
+-rw-r--r--   0 koc        (501) staff       (20)       88 2024-02-19 23:14:58.000000 mintlemon-turkish-nlp-0.2.6/mintlemon/turkish_spellcheck/__init__.py
+-rw-r--r--   0 koc        (501) staff       (20)     4263 2024-02-20 16:36:02.000000 mintlemon-turkish-nlp-0.2.6/mintlemon/turkish_spellcheck/turkish_spellchecker.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 16:25:48.967722 mintlemon-turkish-nlp-0.2.6/mintlemon_turkish_nlp.egg-info/
+-rw-r--r--   0 koc        (501) staff       (20)     3823 2024-05-18 16:25:48.000000 mintlemon-turkish-nlp-0.2.6/mintlemon_turkish_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 koc        (501) staff       (20)      750 2024-05-18 16:25:48.000000 mintlemon-turkish-nlp-0.2.6/mintlemon_turkish_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 koc        (501) staff       (20)        1 2024-05-18 16:25:48.000000 mintlemon-turkish-nlp-0.2.6/mintlemon_turkish_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 koc        (501) staff       (20)      133 2024-05-18 16:25:48.000000 mintlemon-turkish-nlp-0.2.6/mintlemon_turkish_nlp.egg-info/requires.txt
+-rw-r--r--   0 koc        (501) staff       (20)       10 2024-05-18 16:25:48.000000 mintlemon-turkish-nlp-0.2.6/mintlemon_turkish_nlp.egg-info/top_level.txt
+-rw-r--r--   0 koc        (501) staff       (20)     1087 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.6/pyproject.toml
+-rw-r--r--   0 koc        (501) staff       (20)       38 2024-05-18 16:25:48.970010 mintlemon-turkish-nlp-0.2.6/setup.cfg
+-rw-r--r--   0 koc        (501) staff       (20)     2272 2024-05-17 18:34:21.000000 mintlemon-turkish-nlp-0.2.6/setup.py
```

### Comparing `mintlemon-turkish-nlp-0.2.5/AUTHORS.rst` & `mintlemon-turkish-nlp-0.2.6/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.5/LICENSE` & `mintlemon-turkish-nlp-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.5/mintlemon/data/TR_non_breaking_prefixes.txt` & `mintlemon-turkish-nlp-0.2.6/mintlemon/data/TR_non_breaking_prefixes.txt`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.5/mintlemon/data/ascii_to_str_dict.pickle` & `mintlemon-turkish-nlp-0.2.6/mintlemon/data/ascii_to_str_dict.pickle`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.5/mintlemon/data/stop_words.txt` & `mintlemon-turkish-nlp-0.2.6/mintlemon/data/stop_words.txt`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.5/mintlemon/normalizer/_builtin.py` & `mintlemon-turkish-nlp-0.2.6/mintlemon/normalizer/_builtin.py`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.5/mintlemon/normalizer/normalizer.py` & `mintlemon-turkish-nlp-0.2.6/mintlemon/normalizer/normalizer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import re
 import warnings
-from typing import List
+from typing import List, Optional, Dict, Set, Union
 from pathlib import Path
 from ._builtin import DeasciifierBuiltin, NormBuiltin
-import pandas as pd
 
 ST_WR_PATH = str(Path(__file__).parent.parent / "data/stop_words.txt")
 
 class Normalizer:
+    
+    STOP_WORDS = None
+        
     @staticmethod
     def lower_case(text: str) -> str:
         """
         Converts a string of text to lowercase for Turkish language.
 
         This function handles all Turkish characters which are not handled properly by python lower() method,
         e.g., "İ" -> "i", "I" -> "ı", "Ğ" -> "ğ", "Ü" -> "ü", "Ö" -> "ö", "Ş" -> "ş", "Ç" -> "ç".
@@ -61,87 +63,94 @@
         output : str
             Text stripped from punctuations.
             
         Example:
         --------
         >>> from mintlemon import Normalizer
         >>> Normalizer.remove_punctuations("#Merhaba, Dünya! ! # $ % &'()*+,-./:; <= >?@ [\]^_`{|}~) ")
-        'Dünya'
+        'Merhaba Dünya'
         """
-        text = re.sub(r'\s*#\w+', '', text) # remove hashtags
-        text = re.sub(r"(@\[A-Za-z0-9]+)|([^0-9A-Za-zğüşıöçĞÜŞİÖÇ0-9 \t])|(\w+:\/\/\S+)|^rt|http.+?", '', text) # punctuations removed except #,@
-
-        return text.strip()
+        text = re.sub(r"[^\w\sğüşıöçĞÜŞİÖÇ.,']", "", text)  
+        text = re.sub(r"\s+", " ", text) 
+        
+        return text.strip()  
 
     @staticmethod
-    def remove_accent_marks(text: str) -> str:
+    def remove_accent_marks(text: str, accent_mapping: Optional[Dict[str, str]] = None) -> str:
         """
         Removes accent marks from the given string.
 
         Parameters
         ----------
         text : str
             Input text.
 
+        accent_mapping: dict, optional
+            A dictionary mapping accented characters to their unaccented equivalents.
+            If not provided, a default mapping for some common accents in Turkish will be used.
+
         Returns
         -------
         text : str
             Text stripped from accent marks.
 
         Example:
         --------
         >>> from mintlemon import Normalizer
         >>> Normalizer.remove_accent_marks("merhâbâ")
         'merhaba'
-        """
-        accent_marks = {
-            "â": "a",
-            "ô": "o",
-            "î": "i",
-            "ê": "e",
-            "û": "u",
-            "Â": "A",
-            "Ô": "O",
-            "Î": "İ",
-            "Ê": "E",
-            "Û": "U",
-        }
-        for mark, letter in accent_marks.items():
+
+        >>> accent_mapping = {"ä": "a", "ö": "o", "ü": "u"}
+        >>> Normalizer.remove_accent_marks("früchtë", accent_mapping)
+        'fruchte'
+        """
+        if accent_mapping is None:
+            accent_mapping = {
+                "â": "a",
+                "ô": "o",
+                "î": "i",
+                "ê": "e",
+                "û": "u",
+                "Â": "A",
+                "Ô": "O",
+                "Î": "İ",
+                "Ê": "E",
+                "Û": "U",
+            }
+
+        for mark, letter in accent_mapping.items():
             text = text.replace(mark, letter)
         return text
 
     @staticmethod
-    def convert_text_numbers(text):
+    def num_to_tr_text(text):
         """
-        Convert numbers in a text to words in Turkish language
+        Converts numbers in a text to their Turkish text equivalents within the TurkNorm package.
 
-        This function converts numbers in a given text to words in Turkish language.
-        The function uses regular expressions to find and extract numbers in the text,
-        and then uses the number_to_word function to convert the numbers to words.
-        If the number is too large, a warning is issued. If the decimal number is represented by a period,
-        a warning is issued. (because in Turkish language decimal number is represented by comma.)
-        The last text where numbers were converted to words is returned.
+        This method identifies and converts numerical values found in the given text into their
+        corresponding Turkish words, adhering to Turkish numerical expression standards. It alerts
+        for numbers exceeding processing capacity or when decimal numbers are improperly formatted.
+        The output is the original text with numbers converted to their Turkish word equivalents.
 
         Parameters
         ----------
         text : str
-            The text containing numbers to be converted to words
+            The input text containing numerical values to be converted.
 
         Returns
         -------
         text : str
-            The text with the numbers converted to words in Turkish language
+            The text with numerical values converted to Turkish words.
 
-        Example:
-        --------
+        Example
+        -------
         >>> from mintlemon import Normalizer
-        >>> Normalizer.convert_text_numbers("Evi 1000000 TL Değerinde! Çok güzel bir evi var ama 3,5 ay boyunca satamamışlar...")
-        'Evi bir milyon TL Değerinde! Çok güzel bir evi var ama üç virgül beş ay boyunca satamamışlar...
+        >>> Normalizer.num_to_tr_text("Evi 1000000 TL Değerinde! Çok güzel bir evi var ama 3,5 ay boyunca satamamışlar...")
+        'Evi bir milyon TL Değerinde! Çok güzel bir evi var ama üç virgül beş ay boyunca satamamışlar...'
         """
-
         def convert_number(match):
             number = float(match.group(0).replace(",", "."))
             if number >= 1e21:
                 return warnings.warn(
                     "The number is too big to convert it to words in Turkish language."
                 )
             elif number == int(number):
@@ -150,15 +159,15 @@
                 return warnings.warn(
                     "In Turkish language, decimal numbers are expressed with commas."
                 )
 
         return re.sub(
             r"[-+]?\d*.\d+|\d+", convert_number, text.replace(",", " virgül ")
         ).lstrip()
-
+        
     @staticmethod
     def deasciify(input: List[str]) -> List[str]:
         """
         Deasciifies the given text for Turkish.
 
         Parameters
         ----------
@@ -177,147 +186,184 @@
         'O sırada bahçede çiçekleri kokluyorduk. Herşey bahçıvanın ıslık çalmasıyla yaşandı...'
         """
         deasciifier = DeasciifierBuiltin(input)
         result = deasciifier.convert_to_turkish()
         return result
 
     @staticmethod
-    def normalize_turkish_chars(text):
+    def normalize_chars(text, translation_table=None):
         """
-        Normalize Turkish characters in the given text.
+        Normalize characters in the given text based on the provided translation table.
 
         Parameters
         ----------
         text : str
             The text to be normalized.
 
+        translation_table : dict or str.maketrans, optional
+            The translation table that defines the mapping of characters to be replaced.
+            If not provided, it defaults to the mapping of Turkish characters to their ASCII equivalents.
+
         Returns
         -------
         str
-            The normalized text with Turkish characters replaced by their ASCII equivalents.
+            The normalized text with characters replaced based on the translation table.
 
         Examples
         --------
-        >>> normalize_turkish_chars("Bir gün İstanbul'da çay içtik.")
-        'Bir gun Istanbul\'da cay ictik.'
-
-        >>> normalize_turkish_chars("Gazi Üniversitesi'ne hoş geldiniz.")
-        'Gazi Universitesi\'ne hos geldiniz.'
+        Default Turkish normalization:
+        >>> normalize_chars("Bir gün İstanbul'da çay içtik.")
+        'Bir gun Istanbul'da cay ictik.'
+
+        >>> normalize_chars("Gazi Üniversitesi'ne hoş geldiniz.")
+        'Gazi Universitesi'ne hos geldiniz.'
+
+        Custom translation for Azerbaijani language:
+        >>> azerbaijani_table = str.maketrans("ƏəĞğÇçŞşÜüÖöİı", "AaGgCcSsUuOoIi")
+        >>> normalize_chars("Mən Ağcabədi şəhərində yaşayıram.", azerbaijani_table)
+        'Men Agcabedi seherinde yasayiram.'
         """
-        translationTable = str.maketrans("ğĞıİöÖüÜşŞçÇ", "gGiIoOuUsScC")
-        result = text.translate(translationTable)
+        if translation_table is None:
+            translation_table = str.maketrans("ğĞıİöÖüÜşŞçÇ", "gGiIoOuUsScC")
+
+        result = text.translate(translation_table)
         return result
 
     @staticmethod
-    def remove_numbers(text):
+    def remove_numbers(text, remove_signed=True, remove_decimal=True):
         """
         Removes numerical expressions from a given text.
 
         This function removes all numerical expressions from a given text, including
-        integers, decimals, and signed integers/decimals.
+        integers, decimals, and signed integers/decimals based on the parameters.
 
         Parameters
         ----------
         text : str
             The text to remove numerical expressions from
 
+        remove_signed : bool, optional
+            Whether to remove signed integers/decimals from the text.
+            By default, it is set to True.
+
+        remove_decimal : bool, optional
+            Whether to remove decimal numbers from the text.
+            By default, it is set to True.
+
         Returns
         -------
         cleaned_text : str
             The cleaned text without any numerical expressions
 
         Example
         -------
+        >>> from mintlemon import Normalizer
+        >>> normalize = Normalizer()
         >>> text = "Bu cümle 12.34 ile başlıyor ve 56 ile bitiyor. 2,5 +3,5 -3,4 ile ilgili bir şeyler söyleyebiliriz."
-        >>> remove_numbers(text)
-        'Bu cümle ile başlıyor ve ile bitiyor. ile ilgili bir şeyler söyleyebiliriz.'
+        >>> normalize.remove_numbers(text)
+        'Bu cümle ile başlıyor ve ile bitiyor. İle ilgili bir şeyler söyleyebiliriz.'
         """
-        return re.sub(r"(?<!\d)[-+]?\d*\.?\d+(?!\d)\s*", "", text)
+        if remove_signed and remove_decimal:
+            pattern = r"(?<!\d)[-+]?\d*\.?\d+(?!\d)"
+        elif remove_signed:
+            pattern = r"(?<!\d)[-+]?\d+(?!\d)"
+        elif remove_decimal:
+            pattern = r"\d*\.?\d+"
+        else:
+            pattern = r"\d+"
 
-    @staticmethod
-    def remove_more_space(text: str) -> str:
-        """
-        Removes extra spaces from the given text.
+        cleaned_text = re.sub(pattern, "", text)
 
-        Parameters
-        ----------
-        text : str
-            The text to remove extra spaces from.
+        cleaned_text = re.sub(r"\s*,\s*", " ", cleaned_text)
+        cleaned_text = re.sub(r"\s+", " ", cleaned_text)
 
-        Returns
-        -------
-        str
-            The cleaned text without extra spaces.
+        cleaned_text = re.sub(r"^,", "", cleaned_text).strip()
 
-        Example
-        -------
-        >>> text = "Ahmet Selam,  Nerelerdeydin? Seni ÇOOOOK      ÖZLEDİK!!!"
-        >>> remove_more_space(text)
-        'Ahmet Selam, Nerelerdeydin? Seni ÇOOOOK ÖZLEDİK!!!'
-        """
-        return " ".join(text.split())
+        return cleaned_text
 
-    def drop_empty_values(df, column_text) -> pd.DataFrame:
+    @classmethod
+    def remove_stopwords(cls, text: str, stopwords: Union[Set[str], List[str]] = None) -> str:
         """
-        Drop the rows from the given dataframe where the specified column_text is empty.
+        Removes stop words from the given text.
 
         Parameters
         ----------
-        df : pandas.DataFrame
-            The dataframe to be processed
-        column_text : str
-            The name of the column to be checked for empty values
+        text : str
+            The input text.
+        stopwords : Union[Set[str], List[str]], optional
+            A set or list of words to remove from the text.
+            If not provided, it defaults to the stop words loaded from the file.
 
         Returns
         -------
-        pandas.DataFrame
-            The cleaned dataframe without the rows containing empty column_text values
+        str
+            The cleaned text with stop words removed.
 
-        Example
-        -------
-        >>> data = {'id': [1, 2, 3, 4, 5],
-                    'name': ['Şeyma', 'Murat', 'Elif', 'Tarık Kaan', 'Erdinç'],
-                    'text': ['Bilgisayar Mühendisi', 'Doç. Dr', '', 'Yazılım Mühendisi', '']}
-        >>> df = pd.DataFrame(data)
-        >>> cleaned_df = drop_empty_values(df, 'text')
-        >>> cleaned_df
-
-        id      name             text
-        0   1   Şeyma      Bilgisayar Mühendisi
-        2   3   Murat      Doç. Dr
-        3   4   Tarık Kaan Yazılım Mühendisi
-        """
-        cleaned_df = df[df[column_text] != ""]
+        Examples
+        --------
+        >>> from mintlemon import Normalizer
 
-        return cleaned_df
+        # Example 1: Using default stop words list
+        text = "Bu bir örnek cümle, gereksiz kelimeleri çıkarmak istiyorum."
+        cleaned_text = Normalizer.remove_stopwords(text)
+        print(cleaned_text)
+        # Output: "örnek cümle, gereksiz kelimeleri çıkarmak."
+
+        # Example 2: Providing custom stop words list
+        custom_stopwords = ["bir", "gereksiz"]
+        cleaned_text = Normalizer.remove_stopwords(text, stopwords=custom_stopwords)
+        print(cleaned_text)
+        # Output: "Bu örnek cümle, kelimeleri çıkarmak."
+        """
+        if stopwords is None:
+            cls.load_stopwords(ST_WR_PATH)
+            stopwords = cls.STOP_WORDS
+        elif isinstance(stopwords, list):
+            stopwords = set(stopwords)
 
-    @staticmethod
-    def remove_stopwords(text: str, stop_words_file: str = ST_WR_PATH) -> str:
+        cleaned_text = " ".join(word for word in text.split() if word.lower() not in stopwords)
+        return cleaned_text
+
+    @classmethod
+    def load_stopwords(cls, stop_words_source: Union[str, Set[str], List[str]]) -> None:
         """
-        Removes stop words from the given text.
+        Loads stop words from a file or a set/list of words.
 
         Parameters
         ----------
-        text : str
-            The text to remove stop words from.
-        stop_words_file : str
-            The path to the file containing the stop words. Default is the path defined in the library.
+        stop_words_source : Union[str, Set[str], List[str]]
+            The path to the file containing the stop words
+            or a set/list of stop words.
 
         Returns
         -------
-        str
-            The cleaned text without stop words.
+        None
 
-        Example
-        -------
-        >>> text = "Bu cümledeki bazı gereksiz kelimeleri çıkarmak istiyorum."
-        >>> remove_stopwords(text)
-        'cümledeki gereksiz kelimeleri çıkarmak istiyorum.'
-        """
-        with open(stop_words_file, "r", encoding="utf-8") as f:
-            stop_words = set(f.read().split())
-
-        cleaned_text = " ".join(
-            word for word in text.split() if word.lower() not in stop_words
-        )
+        Raises
+        ------
+        ValueError
+            If stop_words_source is not a valid type.
 
-        return cleaned_text
+        Examples
+        --------
+        >>> from mintlemon import Normalizer
+
+        # Example 1: Load stop words from file
+        Normalizer.load_stopwords("stop_words.txt")
+
+        # Example 2: Load stop words from a set
+        stop_words_set = {"bu", "bir"}
+        Normalizer.load_stopwords(stop_words_set)
+
+        # Example 3: Load stop words from a list
+        stop_words_list = ["bazı", "istiyorum"]
+        Normalizer.load_stopwords(stop_words_list)
+        """
+        if isinstance(stop_words_source, str):
+            with open(stop_words_source, "r", encoding="utf-8") as f:
+                cls.STOP_WORDS = set(f.read().split())
+        elif isinstance(stop_words_source, (set, list)):
+            cls.STOP_WORDS = set(stop_words_source)
+        else:
+            raise ValueError(
+                "stop_words_source must be a path to a file (str), a set of words (set), or a list of words (list)."
+            )
```

### Comparing `mintlemon-turkish-nlp-0.2.5/mintlemon/normalizer/text_to_root_dtm.py` & `mintlemon-turkish-nlp-0.2.6/mintlemon/normalizer/text_to_root_dtm.py`

 * *Files 7% similar despite different names*

```diff
@@ -81,17 +81,14 @@
         >>> df = pd.DataFrame({'text': ['bu bir örnek metindir', 'başka bir örnek metin']})
         >>> vectorizer = TextRootDTMVectorizer(df, 'text')
         >>> vectorizer.fit_transform()
         """
         processed_texts = []
         for text in self.dataframe[self.column_name]:
             words = nltk.word_tokenize(text)
-            processed_words = []
-            for word in words:
-                root = self._analyze_word(word)
-                if root:
-                    processed_words.append(root)
+            processed_words = [self._analyze_word(word) for word in words]
+            processed_words = [root for root in processed_words if root is not None]
             processed_texts.append(" ".join(processed_words))
 
         X = self.vectorizer.fit_transform(processed_texts)
 
-        return pd.DataFrame(X.toarray(), columns=self.vectorizer.get_feature_names_out())
+        return pd.DataFrame(X.toarray(), columns=self.vectorizer.get_feature_names_out())
```

### Comparing `mintlemon-turkish-nlp-0.2.5/mintlemon/sentence_splitter/sentence_splitter.py` & `mintlemon-turkish-nlp-0.2.6/mintlemon/sentence_splitter/sentence_splitter.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,41 +11,35 @@
     Methods:
     --------
     split_sentences(text: str) : List[str]
         Split the given text into sentences by considering Turkish non-breaking prefixes.
     """
     def __init__(self) -> None:
         with open(PATH, "r", encoding="utf-8") as file:
-            non_breaking_prefixes_tr = file.read().splitlines()
-        self.prefixes = non_breaking_prefixes_tr
+            self.non_breaking_prefixes_tr = file.read().splitlines()
+        self.prefix_pattern = r"(?:^|\s)(" + "|".join(self.non_breaking_prefixes_tr) + r")\."
 
     def split_sentences(self, text: str) -> List[str]:
         """
         Split the given text into sentences by considering Turkish non-breaking prefixes.
 
-        Parameters:
-        -----------
+        Parameters
+        ----------
         text : str
             The input text to be split into sentences.
 
-        Returns:
-        --------
+        Returns
+        -------
         sentences : list
             A list of sentences
 
-        Example:
+        Examples
         --------
         >>> from mintlemon import SentenceSplitter
         >>> splitter = SentenceSplitter()
         >>> text = "Bu cümle bir örnektir. Bu cümle de bir örnektir!"
         >>> splitter.split_sentences(text)
         Output: ["Bu cümle bir örnektir.", "Bu cümle de bir örnektir!"]
         """
-        # Create a regex pattern for prefixes
-        prefix_pattern = "(" + "|".join(self.prefixes) + r")\."
-        # Replace all prefixes followed by a period with the prefix
-        text = re.sub(prefix_pattern, r"\1", text)
-        # Use the regular expression to split the text into sentences
-        sentences = re.split(r"(?<=[.!?])\s", text)
-
-        return sentences
+        text = re.sub(self.prefix_pattern, r"\1", text)
 
+        return re.split(r"(?<=[.!?])\s", text)
```

### Comparing `mintlemon-turkish-nlp-0.2.5/mintlemon_turkish_nlp.egg-info/SOURCES.txt` & `mintlemon-turkish-nlp-0.2.6/mintlemon_turkish_nlp.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -10,12 +10,14 @@
 mintlemon/data/stop_words.txt
 mintlemon/normalizer/__init__.py
 mintlemon/normalizer/_builtin.py
 mintlemon/normalizer/normalizer.py
 mintlemon/normalizer/text_to_root_dtm.py
 mintlemon/sentence_splitter/__init__.py
 mintlemon/sentence_splitter/sentence_splitter.py
+mintlemon/turkish_spellcheck/__init__.py
+mintlemon/turkish_spellcheck/turkish_spellchecker.py
 mintlemon_turkish_nlp.egg-info/PKG-INFO
 mintlemon_turkish_nlp.egg-info/SOURCES.txt
 mintlemon_turkish_nlp.egg-info/dependency_links.txt
 mintlemon_turkish_nlp.egg-info/requires.txt
 mintlemon_turkish_nlp.egg-info/top_level.txt
```

### Comparing `mintlemon-turkish-nlp-0.2.5/pyproject.toml` & `mintlemon-turkish-nlp-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.5/setup.py` & `mintlemon-turkish-nlp-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def get_long_description():
     with open("README.md", "r", encoding="utf-8") as f:
         return f.read()
 
 setup(
     name="mintlemon-turkish-nlp",
-    version = "0.2.5",
+    version = "0.2.6",
     description="Mint & Lemon Turkish NLP Library developed by Mint & Lemon Development Team.",
     author="Mint&Lemon",
     license="Apache License, Version 2.0",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/Teknofest-Nane-Limon/mintlemon-turkish-nlp",
     project_urls={
```

