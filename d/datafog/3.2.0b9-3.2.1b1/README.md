# Comparing `tmp/datafog-3.2.0b9.tar.gz` & `tmp/datafog-3.2.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-3.2.0b9.tar", last modified: Mon May 13 19:45:36 2024, max compression
+gzip compressed data, was "datafog-3.2.1b1.tar", last modified: Sat May 18 00:01:25 2024, max compression
```

## Comparing `datafog-3.2.0b9.tar` & `datafog-3.2.1b1.tar`

### file list

```diff
@@ -1,19 +1,39 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:45:36.964847 datafog-3.2.0b9/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-13 14:18:11.000000 datafog-3.2.0b9/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     6510 2024-05-13 19:45:36.964714 datafog-3.2.0b9/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     5289 2024-05-13 14:50:51.000000 datafog-3.2.0b9/README.md
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:45:36.963432 datafog-3.2.0b9/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-13 19:21:21.000000 datafog-3.2.0b9/datafog/__about__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      821 2024-05-13 19:44:16.000000 datafog-3.2.0b9/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      222 2024-05-13 18:39:10.000000 datafog-3.2.0b9/datafog/config.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2892 2024-05-13 19:44:17.000000 datafog-3.2.0b9/datafog/main.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:45:36.964228 datafog-3.2.0b9/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     6510 2024-05-13 19:45:36.000000 datafog-3.2.0b9/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      274 2024-05-13 19:45:36.000000 datafog-3.2.0b9/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-13 19:45:36.000000 datafog-3.2.0b9/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)      159 2024-05-13 19:45:36.000000 datafog-3.2.0b9/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        8 2024-05-13 19:45:36.000000 datafog-3.2.0b9/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-13 19:45:36.964893 datafog-3.2.0b9/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1920 2024-05-13 19:45:31.000000 datafog-3.2.0b9/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:45:36.964355 datafog-3.2.0b9/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)     2905 2024-05-13 19:44:48.000000 datafog-3.2.0b9/tests/test_main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 00:01:25.251688 datafog-3.2.1b1/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-17 23:38:08.000000 datafog-3.2.1b1/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     7966 2024-05-18 00:01:25.251544 datafog-3.2.1b1/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6742 2024-05-17 23:38:08.000000 datafog-3.2.1b1/README.md
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 00:01:25.248324 datafog-3.2.1b1/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-17 23:39:53.000000 datafog-3.2.1b1/datafog/__about__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      862 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      222 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/config.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     3275 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 00:01:25.249143 datafog-3.2.1b1/datafog/processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      350 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/processing/__init__.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 00:01:25.249736 datafog-3.2.1b1/datafog/processing/image_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      146 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/processing/image_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2872 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/processing/image_processing/donut_processor.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      787 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/processing/image_processing/image_downloader.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      297 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/processing/image_processing/pytesseract_processor.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 00:01:25.250107 datafog-3.2.1b1/datafog/processing/spark_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       69 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/processing/spark_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2225 2024-05-17 23:57:03.000000 datafog-3.2.1b1/datafog/processing/spark_processing/pyspark_udfs.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 00:01:25.250402 datafog-3.2.1b1/datafog/processing/text_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       51 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/processing/text_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1300 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/processing/text_processing/spacy_pii_annotator.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 00:01:25.250939 datafog-3.2.1b1/datafog/services/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      118 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/services/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1802 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/services/image_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1035 2024-05-17 23:47:08.000000 datafog-3.2.1b1/datafog/services/spark_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      633 2024-05-17 23:38:08.000000 datafog-3.2.1b1/datafog/services/text_service.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 00:01:25.249000 datafog-3.2.1b1/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     7966 2024-05-18 00:01:25.000000 datafog-3.2.1b1/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      906 2024-05-18 00:01:25.000000 datafog-3.2.1b1/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-18 00:01:25.000000 datafog-3.2.1b1/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)      144 2024-05-18 00:01:25.000000 datafog-3.2.1b1/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       14 2024-05-18 00:01:25.000000 datafog-3.2.1b1/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-18 00:01:25.251742 datafog-3.2.1b1/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1944 2024-05-17 23:57:53.000000 datafog-3.2.1b1/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 00:01:25.251321 datafog-3.2.1b1/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2024-05-17 23:38:08.000000 datafog-3.2.1b1/tests/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2447 2024-05-17 23:38:08.000000 datafog-3.2.1b1/tests/test_image_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2945 2024-05-17 23:38:08.000000 datafog-3.2.1b1/tests/test_main.py
```

### Comparing `datafog-3.2.0b9/LICENSE` & `datafog-3.2.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-3.2.0b9/PKG-INFO` & `datafog-3.2.1b1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,7 @@
-Metadata-Version: 2.1
-Name: datafog
-Version: 3.2.0b9
-Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
-Home-page: https://datafog.ai
-Author: DataFog
-Author-email: hi@datafog.ai
-Maintainer: DataFog
-Maintainer-email: hi@datafog.ai
-License: MIT
-Project-URL: Homepage, https://datafog.ai
-Project-URL: Documentation, https://docs.datafog.ai
-Project-URL: Discord, https://discord.gg/bzDth394R4
-Project-URL: Twitter, https://twitter.com/datafoginc
-Project-URL: GitHub, https://github.com/datafog/datafog-python
-Keywords: pii,redaction,nlp,rag,retrieval augmented generation
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: tox
-Classifier: Framework :: Pytest
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <a href="https://www.datafog.ai"><img src="public/colorlogo.png" alt="DataFog logo"></a>
 </p>
 
 <p align="center">
     <b>Open-source DevSecOps for Generative AI Systems</b>. <br />
 </p>
@@ -54,105 +23,135 @@
 
 DataFog is an open-source DevSecOps platform that lets you scan and redact Personally Identifiable Information (PII) out of your Generative AI applications.
 
 ### Core Problem
 
 ![image](https://github.com/DataFog/datafog-python/assets/61345237/57fba4e5-21cc-458f-ac6a-6fbbb70a8de1)
 
-
 ### How it works
 
 ![image](https://github.com/DataFog/datafog-python/assets/61345237/91f4634a-8a9f-4621-81bc-09930feda78a)
 
-
 ## Installation
 
 DataFog can be installed via pip:
 
 ```bash
 pip install datafog
 ```
 
-## Examples - Updated for v3.1
 
-### Base case: PII annotation of text-files
+## Getting Started
 
-```
-from datafog import OCRPIIAnnotator, TextPIIAnnotator
-import json
-import requests
+The DataFog library provides functionality for text and image processing, including PII (Personally Identifiable Information) annotation and OCR (Optical Character Recognition) capabilities.
 
-response = requests.get('https://gist.githubusercontent.com/sidmohan0/1aa3ec38b4e6594d3c34b113f2e0962d/raw/42e57146197be0f85a5901cd1dcdd9ad15b31bab/sotu_2023.txt')
-response.raise_for_status()  # Ensure the request was successful
-text = response.text
-# print(text)
-text_annotator = TextPIIAnnotator()
-annotated_text = text_annotator.run(text, output_path=f"sotu_2023_output.json")
-print("Annotated Text:", annotated_text)
-```
+### Installation
 
-### OCR Reference Set (Images)
+To install the DataFog library, use the following command:
 
 ```
-image_set = {
-    "medical_invoice": "https://s3.amazonaws.com/thumbnails.venngage.com/template/dc377004-1c2d-49f2-8ddf-d63f11c8d9c2.png",
-    "sales_receipt": "https://templates.invoicehome.com/sales-receipt-template-us-classic-white-750px.png",
-    "press_release": "https://newsroom.cisco.com/c/dam/r/newsroom/en/us/assets/a/y2023/m09/cisco_splunk_1200x675_v3.png",
-    "insurance_claim_scanned_form": "https://www.pdffiller.com/preview/101/35/101035394.png",
-    "scanned_internal_record": "https://www.pdffiller.com/preview/435/972/435972694.png",
-    "executive_email": "https://pbs.twimg.com/media/GM3-wpeWkAAP-cX.jpg"
-}
+pip install datafog
+```
+
+### Usage
+
+The [Getting Started notebook](/datafog-python/examples/getting_started.ipynb)  features a standalone Colab notebook. 
+
+
+#### Text PII Annotation
+
+To annotate PII in a given text, lets start with a set of clinical notes:
 
 ```
+!git clone https://gist.github.com/b43b72693226422bac5f083c941ecfdb.git
+# Define the directory path
+folder_path = 'clinical_notes/'
 
-### OCR text extraction from images + PII annotation
+# List all files in the directory
+file_list = os.listdir(folder_path)
+text_files = sorted([file for file in file_list if file.endswith('.txt')])
 
-with this, you can then run the following steps:
+with open(os.path.join(folder_path, text_files[0]), 'r') as file:
+    clinical_note = file.read()
 
+display(Markdown(clinical_note))
 ```
-from datafog import OCRPIIAnnotator, TextPIIAnnotator
-import json
+which looks like this:
+```
+
+**Date:** April 10, 2024
+
+**Patient:** Emily Johnson, 35 years old
 
-image_url = image_set["executive_email"]
+**MRN:** 00987654
 
-annotator = OCRPIIAnnotator()
-annotated_text = annotator.run(image_url, output_path=f"executive_email_output.json")
-print("Annotated Text:", annotated_text)
+**Chief Complaint:** "I've been experiencing severe back pain and numbness in my legs."
+
+**History of Present Illness:** The patient is a 35-year-old who presents with a 2-month history of worsening back pain, numbness in both legs, and occasional tingling sensations. The patient reports working as a freelance writer and has been experiencing increased stress due to tight deadlines and financial struggles.
+
+**Past Medical History:** Hypothyroidism
+
+**Social History:**
+The patient shares a small apartment with two roommates and relies on public transportation. They mention feeling overwhelmed with work and personal responsibilities, often sacrificing sleep to meet deadlines. The patient expresses concern over the high cost of healthcare and the need for affordable medication options.
+
+**Review of Systems:** Denies fever, chest pain, or shortness of breath. Reports occasional headaches.
+
+**Physical Examination:**
+- General: Appears tired but is alert and oriented.
+- Vitals: BP 128/80, HR 72, Temp 98.6°F, Resp 14/min
+
+**Assessment/Plan:**
+- Continue to monitor blood pressure and thyroid function.
+- Discuss affordable medication options with a pharmacist.
+- Refer to a social worker to address housing concerns and access to healthcare services.
+- Encourage the patient to engage with community support groups for social support.
+- Schedule a follow-up appointment in 4 weeks or sooner if symptoms worsen.
+
+**Comments:** The patient's health concerns are compounded by socioeconomic factors, including employment status, housing stability, and access to healthcare. Addressing these social determinants of health is crucial for improving the patient's overall well-being.
 
 ```
 
-and the output should look like this:
+we can then set up our pipeline to accept these files
 
 ```
-Annotated Text: {'DATE_TIME': ['Wednesday', 'June 12, 2019'], 'LOC': [], 'NRP': [], 'ORG': [], 'PER': ['Kevin Scott Sent', 'Satya Nadella', 'Bill Gates Subject', 'Thoughts']}
+async def run_text_pipeline_demo():
+  results = await datafog.run_text_pipeline(texts)
+  print("Text Pipeline Results:", results)
+  return results
 
+
+texts = [clinical_note]
+loop = asyncio.get_event_loop()
+results = loop.run_until_complete(run_text_pipeline_demo())
 ```
 
-### With PySpark
 
-Note: as of 3.1.0, you'll need to start the Spark session by instancing the DataFog class as shown below
+Note: The DataFog library uses asynchronous programming, so make sure to use the `async`/`await` syntax when calling the appropriate methods.
 
-```
-from datafog import DataFog
-from datafog.pii_annotation import ImageProcessor
-datafog = DataFog()
+#### OCR PII Annotation
 
-# let's process the images that we shared above
-processed_images = [(name, ImageProcessor().download_image(url=image_url)) for name, image_url in image_set.items()]
+Let's use a image (which could easily be a converted or scanned PDF)
 
-from datafog.pii_annotation import SparkService
-parsed_images = [(name, ImageProcessor().parse_image(img)) for name, img in processed_images]
+![Executive Email](https://pbs.twimg.com/media/GM3-wpeWkAAP-cX.jpg)
+
+```
+datafog = DataFog(operations='extract_text')
+url_list = ['https://pbs.twimg.com/media/GM3-wpeWkAAP-cX.jpg']
 
-df = SparkService().spark.createDataFrame(parsed_images, ["image_name", "parsed_data"])
+async def run_ocr_pipeline_demo():
+  results = await datafog.run_ocr_pipeline(url_list)
+  print("OCR Pipeline Results:", results)
 
-# Display DataFrame
-df.show(truncate=False)
+loop = asyncio.get_event_loop()
+loop.run_until_complete(run_ocr_pipeline_demo())
 
 ```
 
+You'll notice that we use async functions liberally throughout the SDK - given the nature of the functions we're providing and the extension of DataFog into API/other formats, this allows the functions to be more easily adapted for those uses. 
+
 ## Contributing
 
 DataFog is a community-driven **open-source** platform and we've been fortunate to have a small and growing contributor base. We'd love to hear ideas, feedback, suggestions for improvement - anything on your mind about what you think can be done to make DataFog better! Join our [Discord](https://discord.gg/bzDth394R4) and join our growing community.
 
 ### Dev Notes
 
 - Justfile commands:
@@ -169,9 +168,7 @@
 
 ```
 
 ## License
 
 This software is published under the [MIT
 license](https://en.wikipedia.org/wiki/MIT_License).
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,71 +1,71 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.2.0b9 Summary: Scan, redact, and
-manage PII in your documents before they get uploaded to a Retrieval Augmented
-Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
-email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
-License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
-Documentation, https://docs.datafog.ai Project-URL: Discord, https://
-discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
-Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
-pii,redaction,nlp,rag,retrieval augmented generation Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Classifier: Framework :: tox
-Classifier: Framework :: Pytest Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
-:: Information Technology Classifier: Intended Audience :: System
-Administrators Requires-Python: >=3.10 Description-Content-Type: text/markdown
-License-File: LICENSE
                                 _[_D_a_t_a_F_o_g_ _l_o_g_o_]
                OOppeenn--ssoouurrccee DDeevvSSeeccOOppss ffoorr GGeenneerraattiivvee AAII SSyysstteemmss.
   _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _p_y_v_e_r_s_i_o_n_s_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]_[_C_o_d_e
                      _s_t_y_l_e_:_ _b_l_a_c_k_]_[_c_o_d_e_c_o_v_]_[_G_i_t_H_u_b_ _I_s_s_u_e_s_]
 ## Overview ### What is DataFog? DataFog is an open-source DevSecOps platform
 that lets you scan and redact Personally Identifiable Information (PII) out of
 your Generative AI applications. ### Core Problem ![image](https://github.com/
 DataFog/datafog-python/assets/61345237/57fba4e5-21cc-458f-ac6a-6fbbb70a8de1)
 ### How it works ![image](https://github.com/DataFog/datafog-python/assets/
 61345237/91f4634a-8a9f-4621-81bc-09930feda78a) ## Installation DataFog can be
-installed via pip: ```bash pip install datafog ``` ## Examples - Updated for
-v3.1 ### Base case: PII annotation of text-files ``` from datafog import
-OCRPIIAnnotator, TextPIIAnnotator import json import requests response =
-requests.get('https://gist.githubusercontent.com/sidmohan0/
-1aa3ec38b4e6594d3c34b113f2e0962d/raw/42e57146197be0f85a5901cd1dcdd9ad15b31bab/
-sotu_2023.txt') response.raise_for_status() # Ensure the request was successful
-text = response.text # print(text) text_annotator = TextPIIAnnotator()
-annotated_text = text_annotator.run(text, output_path=f"sotu_2023_output.json")
-print("Annotated Text:", annotated_text) ``` ### OCR Reference Set (Images) ```
-image_set = { "medical_invoice": "https://s3.amazonaws.com/
-thumbnails.venngage.com/template/dc377004-1c2d-49f2-8ddf-d63f11c8d9c2.png",
-"sales_receipt": "https://templates.invoicehome.com/sales-receipt-template-us-
-classic-white-750px.png", "press_release": "https://newsroom.cisco.com/c/dam/r/
-newsroom/en/us/assets/a/y2023/m09/cisco_splunk_1200x675_v3.png",
-"insurance_claim_scanned_form": "https://www.pdffiller.com/preview/101/35/
-101035394.png", "scanned_internal_record": "https://www.pdffiller.com/preview/
-435/972/435972694.png", "executive_email": "https://pbs.twimg.com/media/GM3-
-wpeWkAAP-cX.jpg" } ``` ### OCR text extraction from images + PII annotation
-with this, you can then run the following steps: ``` from datafog import
-OCRPIIAnnotator, TextPIIAnnotator import json image_url = image_set
-["executive_email"] annotator = OCRPIIAnnotator() annotated_text =
-annotator.run(image_url, output_path=f"executive_email_output.json") print
-("Annotated Text:", annotated_text) ``` and the output should look like this:
-``` Annotated Text: {'DATE_TIME': ['Wednesday', 'June 12, 2019'], 'LOC': [],
-'NRP': [], 'ORG': [], 'PER': ['Kevin Scott Sent', 'Satya Nadella', 'Bill Gates
-Subject', 'Thoughts']} ``` ### With PySpark Note: as of 3.1.0, you'll need to
-start the Spark session by instancing the DataFog class as shown below ``` from
-datafog import DataFog from datafog.pii_annotation import ImageProcessor
-datafog = DataFog() # let's process the images that we shared above
-processed_images = [(name, ImageProcessor().download_image(url=image_url)) for
-name, image_url in image_set.items()] from datafog.pii_annotation import
-SparkService parsed_images = [(name, ImageProcessor().parse_image(img)) for
-name, img in processed_images] df = SparkService().spark.createDataFrame
-(parsed_images, ["image_name", "parsed_data"]) # Display DataFrame df.show
-(truncate=False) ``` ## Contributing DataFog is a community-driven **open-
-source** platform and we've been fortunate to have a small and growing
-contributor base. We'd love to hear ideas, feedback, suggestions for
-improvement - anything on your mind about what you think can be done to make
-DataFog better! Join our [Discord](https://discord.gg/bzDth394R4) and join our
-growing community. ### Dev Notes - Justfile commands: - `just format` to apply
-formatting. - `just lint` to check formatting and style. ### Testing To run the
-datafog unit tests, check out this repository and do ``` tox ``` ## License
-This software is published under the [MIT license](https://en.wikipedia.org/
-wiki/MIT_License).
+installed via pip: ```bash pip install datafog ``` ## Getting Started The
+DataFog library provides functionality for text and image processing, including
+PII (Personally Identifiable Information) annotation and OCR (Optical Character
+Recognition) capabilities. ### Installation To install the DataFog library, use
+the following command: ``` pip install datafog ``` ### Usage The [Getting
+Started notebook](/datafog-python/examples/getting_started.ipynb) features a
+standalone Colab notebook. #### Text PII Annotation To annotate PII in a given
+text, lets start with a set of clinical notes: ``` !git clone https://
+gist.github.com/b43b72693226422bac5f083c941ecfdb.git # Define the directory
+path folder_path = 'clinical_notes/' # List all files in the directory
+file_list = os.listdir(folder_path) text_files = sorted([file for file in
+file_list if file.endswith('.txt')]) with open(os.path.join(folder_path,
+text_files[0]), 'r') as file: clinical_note = file.read() display(Markdown
+(clinical_note)) ``` which looks like this: ``` **Date:** April 10, 2024
+**Patient:** Emily Johnson, 35 years old **MRN:** 00987654 **Chief Complaint:**
+"I've been experiencing severe back pain and numbness in my legs." **History of
+Present Illness:** The patient is a 35-year-old who presents with a 2-month
+history of worsening back pain, numbness in both legs, and occasional tingling
+sensations. The patient reports working as a freelance writer and has been
+experiencing increased stress due to tight deadlines and financial struggles.
+**Past Medical History:** Hypothyroidism **Social History:** The patient shares
+a small apartment with two roommates and relies on public transportation. They
+mention feeling overwhelmed with work and personal responsibilities, often
+sacrificing sleep to meet deadlines. The patient expresses concern over the
+high cost of healthcare and the need for affordable medication options.
+**Review of Systems:** Denies fever, chest pain, or shortness of breath.
+Reports occasional headaches. **Physical Examination:** - General: Appears
+tired but is alert and oriented. - Vitals: BP 128/80, HR 72, Temp 98.6Â°F, Resp
+14/min **Assessment/Plan:** - Continue to monitor blood pressure and thyroid
+function. - Discuss affordable medication options with a pharmacist. - Refer to
+a social worker to address housing concerns and access to healthcare services.
+- Encourage the patient to engage with community support groups for social
+support. - Schedule a follow-up appointment in 4 weeks or sooner if symptoms
+worsen. **Comments:** The patient's health concerns are compounded by
+socioeconomic factors, including employment status, housing stability, and
+access to healthcare. Addressing these social determinants of health is crucial
+for improving the patient's overall well-being. ``` we can then set up our
+pipeline to accept these files ``` async def run_text_pipeline_demo(): results
+= await datafog.run_text_pipeline(texts) print("Text Pipeline Results:",
+results) return results texts = [clinical_note] loop = asyncio.get_event_loop()
+results = loop.run_until_complete(run_text_pipeline_demo()) ``` Note: The
+DataFog library uses asynchronous programming, so make sure to use the `async`/
+`await` syntax when calling the appropriate methods. #### OCR PII Annotation
+Let's use a image (which could easily be a converted or scanned PDF) !
+[Executive Email](https://pbs.twimg.com/media/GM3-wpeWkAAP-cX.jpg) ``` datafog
+= DataFog(operations='extract_text') url_list = ['https://pbs.twimg.com/media/
+GM3-wpeWkAAP-cX.jpg'] async def run_ocr_pipeline_demo(): results = await
+datafog.run_ocr_pipeline(url_list) print("OCR Pipeline Results:", results) loop
+= asyncio.get_event_loop() loop.run_until_complete(run_ocr_pipeline_demo()) ```
+You'll notice that we use async functions liberally throughout the SDK - given
+the nature of the functions we're providing and the extension of DataFog into
+API/other formats, this allows the functions to be more easily adapted for
+those uses. ## Contributing DataFog is a community-driven **open-source**
+platform and we've been fortunate to have a small and growing contributor base.
+We'd love to hear ideas, feedback, suggestions for improvement - anything on
+your mind about what you think can be done to make DataFog better! Join our
+[Discord](https://discord.gg/bzDth394R4) and join our growing community. ###
+Dev Notes - Justfile commands: - `just format` to apply formatting. - `just
+lint` to check formatting and style. ### Testing To run the datafog unit tests,
+check out this repository and do ``` tox ``` ## License This software is
+published under the [MIT license](https://en.wikipedia.org/wiki/MIT_License).
```

### Comparing `datafog-3.2.0b9/datafog/__init__.py` & `datafog-3.2.1b1/datafog/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-from .main import (DataFog
-    # DataFog, OCRPIIAnnotator, TextPIIAnnotator
-)
+from .config import OperationType
+from .main import DataFog, OCRPIIAnnotator, TextPIIAnnotator
 from .processing.image_processing.donut_processor import DonutProcessor
 from .processing.image_processing.image_downloader import ImageDownloader
 from .processing.image_processing.pytesseract_processor import PytesseractProcessor
 from .processing.text_processing.spacy_pii_annotator import SpacyPIIAnnotator
-
-
 from .services.image_service import ImageService
 from .services.spark_service import SparkService
 from .services.text_service import TextService
-from .config import OperationType
+
+# from .__about__ import __version__
 
 __all__ = [
     "DonutProcessor",
     "DataFog",
     "ImageService",
     "OCRPIIAnnotator",
     "OperationType",
     "SparkService",
     "TextPIIAnnotator",
     "TextService",
     "SpacyPIIAnnotator",
     "ImageDownloader",
     "PytesseractProcessor",
-]
+    # "__version__",
+]
```

### Comparing `datafog-3.2.0b9/datafog/main.py` & `datafog-3.2.1b1/datafog/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 import asyncio
+import importlib
 import json
+import subprocess
+import sys
 from typing import List
 
 import aiohttp
 
 from .config import OperationType
+from .processing.image_processing.donut_processor import DonutProcessor
+from .processing.text_processing.spacy_pii_annotator import SpacyPIIAnnotator
 from .services.image_service import ImageService
 from .services.spark_service import SparkService
 from .services.text_service import TextService
 
 
-
 class DataFog:
-    def __init__(self, operations: List[OperationType] = [OperationType.ANNOTATE_PII]):
-        self.image_service = ImageService()
-        self.text_service = TextService()
-        self.spark_service = SparkService()
+    def __init__(
+        self,
+        image_service=ImageService(),
+        text_service=TextService(),
+        spark_service=None,
+        operations: List[OperationType] = [OperationType.ANNOTATE_PII],
+    ):
+        self.image_service = image_service
+        self.text_service = text_service
+        self.spark_service: SparkService = spark_service
         self.operations: List[OperationType] = operations
 
     async def run_ocr_pipeline(self, image_urls: List[str]):
         """Run the OCR pipeline asynchronously."""
         extracted_text = await self.image_service.ocr_extract(image_urls)
         if OperationType.ANNOTATE_PII in self.operations:
             annotated_text = await self.text_service.batch_annotate_texts(
@@ -32,54 +42,55 @@
         """Run the text pipeline asynchronously."""
         if OperationType.ANNOTATE_PII in self.operations:
             annotated_text = await self.text_service.batch_annotate_texts(texts)
             return annotated_text
         return texts
 
 
-# class OCRPIIAnnotator:
-#     def __init__(self):
-#         self.spark_processor: SparkService = None
-#         self.image_service = DonutProcessor()
-#         self.text_annotator = SpacyPIIAnnotator.create()
-
-#     def run(self, image_url, output_path=None):
-#         try:
-#             # Download and process the image to extract text
-#             downloaded_image = self.image_service.download_image(image_url)
-#             extracted_text = self.image_service.parse_image(downloaded_image)
-
-#             # Annotate the extracted text for PII
-#             annotated_text = self.text_annotator.annotate(extracted_text)
-
-#             # Optionally, output the results to a JSON file
-#             if output_path:
-#                 with open(output_path, "w") as f:
-#                     json.dump(annotated_text, f)
-
-#             return annotated_text
-
-#         finally:
-#             # Ensure Spark resources are released
-#             # self.spark_processor.spark.stop()
-#             pass
-
-
-# class TextPIIAnnotator:
-#     def __init__(self):
-#         self.text_annotator = SpacyPIIAnnotator.create()
-#         self.spark_processor: SparkService = None
-
-#     def run(self, text, output_path=None):
-#         try:
-#             annotated_text = self.text_annotator.annotate(text)
-
-#             # Optionally, output the results to a JSON file
-#             if output_path:
-#                 with open(output_path, "w") as f:
-#                     json.dump(annotated_text, f)
-
-#             return annotated_text
-
-#         finally:
-#             # Ensure Spark resources are released
-#             pass
+class OCRPIIAnnotator:
+    def __init__(self):
+        self.image_service = ImageService(use_donut=True, use_tesseract=False)
+        self.text_annotator = SpacyPIIAnnotator.create()
+        self.spark_service: SparkService = None
+
+    async def run(self, image_urls: List[str], output_path=None):
+        try:
+            # Download and process the image to extract text
+            # downloaded_images = await self.image_service.download_images(image_urls)
+            # extracted_texts = await self.image_service.ocr_extract(downloaded_images)
+
+            # # Annotate the extracted text for PII
+            # annotated_texts = [self.text_annotator.annotate(text) for text in extracted_texts]
+
+            # # Optionally, output the results to a JSON file
+            # if output_path:
+            #     with open(output_path, "w") as f:
+            #         json.dump(annotated_texts, f)
+
+            # return annotated_texts
+            pass
+
+        finally:
+            # Ensure Spark resources are released
+            # self.spark_processor.spark.stop()
+            pass
+
+
+class TextPIIAnnotator:
+    def __init__(self):
+        self.text_annotator = SpacyPIIAnnotator.create()
+        self.spark_processor: SparkService = None
+
+    def run(self, text, output_path=None):
+        try:
+            annotated_text = self.text_annotator.annotate(text)
+
+            # Optionally, output the results to a JSON file
+            if output_path:
+                with open(output_path, "w") as f:
+                    json.dump(annotated_text, f)
+
+            return annotated_text
+
+        finally:
+            # Ensure Spark resources are released
+            pass
```

### Comparing `datafog-3.2.0b9/setup.py` & `datafog-3.2.1b1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from setuptools import setup
+from setuptools import find_packages, setup
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "3.2.0b9"
+    return "3.2.1b1"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
     "GitHub": "https://github.com/datafog/datafog-python",
 }
 
 
 setup(
     name="datafog",
     version=__version__(),
-    author="DataFog",
-    author_email="hi@datafog.ai",
+    author="Sid Mohan",
+    author_email="sid@datafog.ai",
     description="Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages=["datafog"],
+    packages=find_packages(),
     install_requires=[
         "pandas",
         "Requests==2.31.0",
         "spacy==3.4.4",
         "en_spacy_pii_fast==0.0.0",
         # "transformers==4.40.1",
         # "torch==2.2.2",
-        "pyspark==3.4.1",
+        # "pyspark==3.4.1",
         "pydantic==1.10.8",
         "Pillow",
         "sentencepiece",
         "protobuf",
         "pytesseract",
         "aiohttp",
         "pytest-asyncio",
```

### Comparing `datafog-3.2.0b9/tests/test_main.py` & `datafog-3.2.1b1/tests/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 import aiohttp
 import pytest
 
 from datafog import (
     DataFog,
     ImageService,
-    # OCRPIIAnnotator,
+    OCRPIIAnnotator,
     OperationType,
     SparkService,
-    # TextPIIAnnotator,
+    TextPIIAnnotator,
     TextService,
 )
 
 
 def search_nested_dict(d, target):
     """Recursively search for a target value in nested dictionaries."""
     if isinstance(d, dict):
@@ -24,30 +24,31 @@
                 return True
             elif isinstance(value, dict):
                 if search_nested_dict(value, target):
                     return True
     return False
 
 
-# def test_textpii_annotator():
-#     """Test the PII annotation functionality."""
-#     text = "John Doe lives at 1234 Elm St, Springfield."
-#     text_annotator = TextPIIAnnotator()
-#     annotated_text = text_annotator.run(text)
-#     assert "Springfield" in annotated_text["LOC"], "PII not annotated correctly."
+def test_textpii_annotator():
+    """Test the PII annotation functionality."""
+    text = "John Doe lives at 1234 Elm St, Springfield."
+    text_annotator = TextPIIAnnotator()
+    annotated_text = text_annotator.run(text)
+    assert "Springfield" in annotated_text["LOC"], "PII not annotated correctly."
 
 
-# def test_donut_processor():
+# @pytest.mark.asyncio
+# async def test_donut_processor():
 #     """Test the PII annotation functionality for the donutprocessor."""
 #     with open("tests/image_set.json", "r") as f:
 #         image_set = json.load(f)
 #         image_url = image_set["executive_email"]
-#     annotator = OCRPIIAnnotator()
-#     annotated_text = annotator.run(image_url)
-#     assert "Satya Nadella" in annotated_text["PER"], "PII not annotated correctly."
+#     ocr_annotator = OCRPIIAnnotator()
+#     annotated_text = await ocr_annotator.run([image_url])
+#     assert "Satya Nadella" in annotated_text[0].get("PER", []), "PII not annotated correctly."
 
 
 @pytest.mark.asyncio
 async def test_datafog_text_annotation():
     """Test DataFog class for text annotation."""
     text = ["Joe Biden is the President of the United States."]
     datafog = DataFog()
```

