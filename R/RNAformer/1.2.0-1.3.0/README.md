# Comparing `tmp/rnaformer-1.2.0.tar.gz` & `tmp/rnaformer-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnaformer-1.2.0.tar", last modified: Mon Apr 22 14:38:14 2024, max compression
+gzip compressed data, was "rnaformer-1.3.0.tar", last modified: Sat May 18 10:35:32 2024, max compression
```

## Comparing `rnaformer-1.2.0.tar` & `rnaformer-1.3.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-22 14:38:14.754991 rnaformer-1.2.0/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)    11347 2024-04-10 11:44:16.000000 rnaformer-1.2.0/LICENSE
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      124 2024-04-17 13:09:53.000000 rnaformer-1.2.0/MANIFEST.in
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4970 2024-04-22 14:38:14.750991 rnaformer-1.2.0/PKG-INFO
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4381 2024-04-22 14:37:55.000000 rnaformer-1.2.0/README.md
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-22 14:38:14.742991 rnaformer-1.2.0/RNAformer/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-17 13:15:35.000000 rnaformer-1.2.0/RNAformer/__init__.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-22 14:38:14.746991 rnaformer-1.2.0/RNAformer/model/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3594 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/model/RNAformer.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     2020 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/model/RNAformer_block.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      755 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/model/RNAformer_stack.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/model/__init__.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-22 14:38:14.746991 rnaformer-1.2.0/RNAformer/module/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/module/__init__.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)    13307 2024-04-22 14:11:45.000000 rnaformer-1.2.0/RNAformer/module/axial_attention.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      940 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/module/axial_dropout.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3788 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/module/embedding.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3371 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/module/feed_forward.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-22 14:38:14.746991 rnaformer-1.2.0/RNAformer/pl_module/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/pl_module/__init__.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)    11243 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/pl_module/datamodule_rna.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     9104 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/pl_module/rna_folding_trainer.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-22 14:38:14.750991 rnaformer-1.2.0/RNAformer/utils/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      164 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/utils/__init__.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4062 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/utils/configuration.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-22 14:38:14.750991 rnaformer-1.2.0/RNAformer/utils/data/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/utils/data/__init__.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     5800 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/utils/data/rna.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     6566 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/utils/eval_predictions.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      890 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/utils/folder_manager.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3656 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/utils/group_parameters.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-22 14:38:14.750991 rnaformer-1.2.0/RNAformer/utils/handler/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/utils/handler/__init__.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     2145 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/utils/handler/base_handler.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3478 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/utils/handler/checkpoint.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     1480 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/utils/handler/folder.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     2461 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/utils/instantiate.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3780 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/utils/logger.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-22 14:38:14.750991 rnaformer-1.2.0/RNAformer/utils/optim/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/utils/optim/__init__.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     1067 2024-04-10 11:44:16.000000 rnaformer-1.2.0/RNAformer/utils/optim/lr_schedule.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-22 14:38:14.750991 rnaformer-1.2.0/RNAformer.egg-info/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4970 2024-04-22 14:38:14.000000 rnaformer-1.2.0/RNAformer.egg-info/PKG-INFO
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     2097 2024-04-22 14:38:14.000000 rnaformer-1.2.0/RNAformer.egg-info/SOURCES.txt
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        1 2024-04-22 14:38:14.000000 rnaformer-1.2.0/RNAformer.egg-info/dependency_links.txt
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)       10 2024-04-22 14:38:14.000000 rnaformer-1.2.0/RNAformer.egg-info/top_level.txt
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      626 2024-04-22 14:38:08.000000 rnaformer-1.2.0/pyproject.toml
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)       38 2024-04-22 14:38:14.754991 rnaformer-1.2.0/setup.cfg
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      286 2024-04-22 14:37:48.000000 rnaformer-1.2.0/setup.py
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-18 10:35:32.754878 rnaformer-1.3.0/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)    11347 2024-04-10 11:44:16.000000 rnaformer-1.3.0/LICENSE
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)      124 2024-04-17 13:09:53.000000 rnaformer-1.3.0/MANIFEST.in
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     5722 2024-05-18 10:35:32.754878 rnaformer-1.3.0/PKG-INFO
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4381 2024-04-22 14:37:55.000000 rnaformer-1.3.0/README.md
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-18 10:35:32.750878 rnaformer-1.3.0/RNAformer/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-17 13:15:35.000000 rnaformer-1.3.0/RNAformer/__init__.py
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-18 10:35:32.754878 rnaformer-1.3.0/RNAformer/model/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3594 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/model/RNAformer.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     2020 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/model/RNAformer_block.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)      755 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/model/RNAformer_stack.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/model/__init__.py
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-18 10:35:32.754878 rnaformer-1.3.0/RNAformer/module/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/module/__init__.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)    13307 2024-04-22 14:11:45.000000 rnaformer-1.3.0/RNAformer/module/axial_attention.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)      940 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/module/axial_dropout.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3788 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/module/embedding.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3371 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/module/feed_forward.py
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-18 10:35:32.754878 rnaformer-1.3.0/RNAformer/pl_module/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/pl_module/__init__.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)    11243 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/pl_module/datamodule_rna.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     9104 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/pl_module/rna_folding_trainer.py
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-18 10:35:32.754878 rnaformer-1.3.0/RNAformer/utils/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)      164 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/utils/__init__.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4062 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/utils/configuration.py
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-18 10:35:32.754878 rnaformer-1.3.0/RNAformer/utils/data/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/utils/data/__init__.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     5800 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/utils/data/rna.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     6566 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/utils/eval_predictions.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)      890 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/utils/folder_manager.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3656 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/utils/group_parameters.py
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-18 10:35:32.754878 rnaformer-1.3.0/RNAformer/utils/handler/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/utils/handler/__init__.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     2145 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/utils/handler/base_handler.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3478 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/utils/handler/checkpoint.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     1480 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/utils/handler/folder.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     2461 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/utils/instantiate.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3780 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/utils/logger.py
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-18 10:35:32.754878 rnaformer-1.3.0/RNAformer/utils/optim/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/utils/optim/__init__.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     1067 2024-04-10 11:44:16.000000 rnaformer-1.3.0/RNAformer/utils/optim/lr_schedule.py
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-18 10:35:32.754878 rnaformer-1.3.0/RNAformer.egg-info/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     5722 2024-05-18 10:35:32.000000 rnaformer-1.3.0/RNAformer.egg-info/PKG-INFO
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     2129 2024-05-18 10:35:32.000000 rnaformer-1.3.0/RNAformer.egg-info/SOURCES.txt
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)        1 2024-05-18 10:35:32.000000 rnaformer-1.3.0/RNAformer.egg-info/dependency_links.txt
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)      303 2024-05-18 10:35:32.000000 rnaformer-1.3.0/RNAformer.egg-info/requires.txt
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)       10 2024-05-18 10:35:32.000000 rnaformer-1.3.0/RNAformer.egg-info/top_level.txt
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     1214 2024-05-18 10:35:29.000000 rnaformer-1.3.0/pyproject.toml
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)       38 2024-05-18 10:35:32.754878 rnaformer-1.3.0/setup.cfg
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)      286 2024-04-22 14:37:48.000000 rnaformer-1.3.0/setup.py
```

### Comparing `rnaformer-1.2.0/LICENSE` & `rnaformer-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/PKG-INFO` & `rnaformer-1.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: RNAformer
-Version: 1.2.0
-Summary: RNAformer: a simple single-sequence-based deep learning model for RNA secondary structure prediction.
-Author: Frederic Runge, Rolf Backofen, Frank Hutter
-Author-email: "Joerg K.H. Franke" <frankej@cs.uni-freiburg.de>, Ryan Koeksal <koeksalr@informatik.uni-freiburg.de>
-Project-URL: Homepage, https://github.com/automl/RNAformer
-Project-URL: Issues, https://github.com/automl/RNAformer/issues
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # RNAformer
 
 This repository contains the source code to the preprint [*RNAformer: A Simple Yet Effective Deep Learning Model for RNA Secondary Structure Prediction*](https://www.biorxiv.org/content/10.1101/2024.02.12.579881v1)  and to the preceding workshop paper 
 [*Scalable Deep Learning for RNA Secondary Structure Prediction*](https://arxiv.org/abs/2307.10073) 
 presented at the 2023 ICML Workshop on Computational Biology.
 
 ### Abstract
```

### Comparing `rnaformer-1.2.0/RNAformer/model/RNAformer.py` & `rnaformer-1.3.0/RNAformer/model/RNAformer.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/RNAformer/model/RNAformer_block.py` & `rnaformer-1.3.0/RNAformer/model/RNAformer_block.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/RNAformer/model/RNAformer_stack.py` & `rnaformer-1.3.0/RNAformer/model/RNAformer_stack.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/RNAformer/module/axial_attention.py` & `rnaformer-1.3.0/RNAformer/module/axial_attention.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/RNAformer/module/axial_dropout.py` & `rnaformer-1.3.0/RNAformer/module/axial_dropout.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/RNAformer/module/embedding.py` & `rnaformer-1.3.0/RNAformer/module/embedding.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/RNAformer/module/feed_forward.py` & `rnaformer-1.3.0/RNAformer/module/feed_forward.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/RNAformer/pl_module/datamodule_rna.py` & `rnaformer-1.3.0/RNAformer/pl_module/datamodule_rna.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/RNAformer/pl_module/rna_folding_trainer.py` & `rnaformer-1.3.0/RNAformer/pl_module/rna_folding_trainer.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/RNAformer/utils/configuration.py` & `rnaformer-1.3.0/RNAformer/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/RNAformer/utils/data/rna.py` & `rnaformer-1.3.0/RNAformer/utils/data/rna.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/RNAformer/utils/eval_predictions.py` & `rnaformer-1.3.0/RNAformer/utils/eval_predictions.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/RNAformer/utils/folder_manager.py` & `rnaformer-1.3.0/RNAformer/utils/folder_manager.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/RNAformer/utils/group_parameters.py` & `rnaformer-1.3.0/RNAformer/utils/group_parameters.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/RNAformer/utils/handler/base_handler.py` & `rnaformer-1.3.0/RNAformer/utils/handler/base_handler.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/RNAformer/utils/handler/checkpoint.py` & `rnaformer-1.3.0/RNAformer/utils/handler/checkpoint.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/RNAformer/utils/handler/folder.py` & `rnaformer-1.3.0/RNAformer/utils/handler/folder.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/RNAformer/utils/instantiate.py` & `rnaformer-1.3.0/RNAformer/utils/instantiate.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/RNAformer/utils/logger.py` & `rnaformer-1.3.0/RNAformer/utils/logger.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/RNAformer/utils/optim/lr_schedule.py` & `rnaformer-1.3.0/RNAformer/utils/optim/lr_schedule.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.2.0/RNAformer.egg-info/PKG-INFO` & `rnaformer-1.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,42 @@
 Metadata-Version: 2.1
 Name: RNAformer
-Version: 1.2.0
+Version: 1.3.0
 Summary: RNAformer: a simple single-sequence-based deep learning model for RNA secondary structure prediction.
 Author: Frederic Runge, Rolf Backofen, Frank Hutter
 Author-email: "Joerg K.H. Franke" <frankej@cs.uni-freiburg.de>, Ryan Koeksal <koeksalr@informatik.uni-freiburg.de>
+Maintainer-email: Ryan Koeksal <koeksalr@informatik.uni-freiburg.de>, "Joerg K.H. Franke" <frankej@cs.uni-freiburg.de>
 Project-URL: Homepage, https://github.com/automl/RNAformer
 Project-URL: Issues, https://github.com/automl/RNAformer/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: torch==2.1.0
+Requires-Dist: torchvision==0.16.0
+Requires-Dist: torchaudio==2.1.0
+Requires-Dist: tqdm
+Requires-Dist: pyyaml
+Requires-Dist: pyaml
+Requires-Dist: numpy
+Requires-Dist: packaging
+Requires-Dist: wheel
+Requires-Dist: tabulate
+Requires-Dist: scipy
+Requires-Dist: pandas==2.0.2
+Requires-Dist: scikit-learn==1.3.0
+Requires-Dist: matplotlib==3.7.2
+Requires-Dist: polars
+Requires-Dist: loralib==0.1.2
+Requires-Dist: tensorboard==2.13.0
+Requires-Dist: transformers==4.30.2
+Requires-Dist: datasets==2.13.1
+Requires-Dist: pytorch-lightning==2.0.4
+Requires-Dist: deepspeed==0.9.5
+Requires-Dist: rotary-embedding-torch
 
 # RNAformer
 
 This repository contains the source code to the preprint [*RNAformer: A Simple Yet Effective Deep Learning Model for RNA Secondary Structure Prediction*](https://www.biorxiv.org/content/10.1101/2024.02.12.579881v1)  and to the preceding workshop paper 
 [*Scalable Deep Learning for RNA Secondary Structure Prediction*](https://arxiv.org/abs/2307.10073) 
 presented at the 2023 ICML Workshop on Computational Biology.
```

### Comparing `rnaformer-1.2.0/RNAformer.egg-info/SOURCES.txt` & `rnaformer-1.3.0/RNAformer.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 ./RNAformer/utils/handler/folder.py
 ./RNAformer/utils/optim/__init__.py
 ./RNAformer/utils/optim/lr_schedule.py
 RNAformer/__init__.py
 RNAformer.egg-info/PKG-INFO
 RNAformer.egg-info/SOURCES.txt
 RNAformer.egg-info/dependency_links.txt
+RNAformer.egg-info/requires.txt
 RNAformer.egg-info/top_level.txt
 RNAformer/model/RNAformer.py
 RNAformer/model/RNAformer_block.py
 RNAformer/model/RNAformer_stack.py
 RNAformer/model/__init__.py
 RNAformer/module/__init__.py
 RNAformer/module/axial_attention.py
```

