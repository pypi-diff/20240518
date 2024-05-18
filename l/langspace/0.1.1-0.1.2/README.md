# Comparing `tmp/langspace-0.1.1.tar.gz` & `tmp/langspace-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langspace-0.1.1.tar", last modified: Fri May 17 23:38:50 2024, max compression
+gzip compressed data, was "langspace-0.1.2.tar", last modified: Sat May 18 00:02:46 2024, max compression
```

## Comparing `langspace-0.1.1.tar` & `langspace-0.1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-17 23:38:50.696007 langspace-0.1.1/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)    35149 2023-03-15 12:32:16.000000 langspace-0.1.1/LICENSE
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1558 2024-05-17 23:38:50.695781 langspace-0.1.1/PKG-INFO
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      611 2024-05-17 23:28:54.000000 langspace-0.1.1/README.md
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-17 23:38:50.689193 langspace-0.1.1/langspace/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-11-21 12:34:00.000000 langspace-0.1.1/langspace/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-17 23:38:50.690811 langspace-0.1.1/langspace/metrics/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        0 2024-01-26 18:39:47.000000 langspace-0.1.1/langspace/metrics/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      307 2024-05-16 18:37:32.000000 langspace-0.1.1/langspace/metrics/disentanglement.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      111 2024-01-26 18:39:48.000000 langspace-0.1.1/langspace/metrics/interpolation.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-17 23:38:50.691060 langspace-0.1.1/langspace/models/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      142 2024-03-12 13:00:53.000000 langspace-0.1.1/langspace/models/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-17 23:38:50.691877 langspace-0.1.1/langspace/ops/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-11-21 12:34:19.000000 langspace-0.1.1/langspace/ops/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      100 2024-02-27 15:35:00.000000 langspace-0.1.1/langspace/ops/arithmetic.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1438 2024-02-27 15:35:00.000000 langspace-0.1.1/langspace/ops/interpolation.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1778 2024-02-27 15:35:00.000000 langspace-0.1.1/langspace/ops/traversal.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-17 23:38:50.692311 langspace-0.1.1/langspace/probe/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      335 2024-01-20 14:44:57.000000 langspace-0.1.1/langspace/probe/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-17 23:38:50.692670 langspace-0.1.1/langspace/probe/arithmetic/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3684 2024-03-15 13:21:38.000000 langspace-0.1.1/langspace/probe/arithmetic/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2298 2024-05-17 21:00:54.000000 langspace-0.1.1/langspace/probe/base.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-17 23:38:50.693254 langspace-0.1.1/langspace/probe/cluster_vis/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     6486 2024-05-17 23:33:17.000000 langspace-0.1.1/langspace/probe/cluster_vis/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      117 2024-03-15 13:04:53.000000 langspace-0.1.1/langspace/probe/cluster_vis/methods.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-17 23:38:50.693568 langspace-0.1.1/langspace/probe/defmod/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-11-24 11:17:37.000000 langspace-0.1.1/langspace/probe/defmod/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-17 23:38:50.693720 langspace-0.1.1/langspace/probe/disentanglement/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)    26085 2024-05-17 23:05:26.000000 langspace-0.1.1/langspace/probe/disentanglement/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-17 23:38:50.694271 langspace-0.1.1/langspace/probe/interpolation/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3637 2024-03-15 13:21:58.000000 langspace-0.1.1/langspace/probe/interpolation/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-17 23:38:50.694553 langspace-0.1.1/langspace/probe/lingprop/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      979 2024-01-20 14:32:48.000000 langspace-0.1.1/langspace/probe/lingprop/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-17 23:38:50.694892 langspace-0.1.1/langspace/probe/sts/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      926 2024-01-20 14:34:31.000000 langspace-0.1.1/langspace/probe/sts/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-17 23:38:50.695201 langspace-0.1.1/langspace/probe/traversal/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4559 2024-03-15 13:23:01.000000 langspace-0.1.1/langspace/probe/traversal/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-17 23:38:50.695549 langspace-0.1.1/langspace.egg-info/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1558 2024-05-17 23:38:50.000000 langspace-0.1.1/langspace.egg-info/PKG-INFO
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      885 2024-05-17 23:38:50.000000 langspace-0.1.1/langspace.egg-info/SOURCES.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        1 2024-05-17 23:38:50.000000 langspace-0.1.1/langspace.egg-info/dependency_links.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       71 2024-05-17 23:38:50.000000 langspace-0.1.1/langspace.egg-info/requires.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       10 2024-05-17 23:38:50.000000 langspace-0.1.1/langspace.egg-info/top_level.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      795 2024-05-17 23:23:17.000000 langspace-0.1.1/pyproject.toml
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       70 2024-05-16 18:17:28.000000 langspace-0.1.1/requirements.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       38 2024-05-17 23:38:50.696055 langspace-0.1.1/setup.cfg
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     1131 2024-05-17 23:20:55.000000 langspace-0.1.1/setup.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.841615 langspace-0.1.2/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)    35149 2023-03-15 12:32:16.000000 langspace-0.1.2/LICENSE
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1558 2024-05-18 00:02:46.841431 langspace-0.1.2/PKG-INFO
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      611 2024-05-17 23:28:54.000000 langspace-0.1.2/README.md
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.835545 langspace-0.1.2/langspace/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-11-21 12:34:00.000000 langspace-0.1.2/langspace/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.836858 langspace-0.1.2/langspace/metrics/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        0 2024-01-26 18:39:47.000000 langspace-0.1.2/langspace/metrics/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      307 2024-05-16 18:37:32.000000 langspace-0.1.2/langspace/metrics/disentanglement.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      111 2024-01-26 18:39:48.000000 langspace-0.1.2/langspace/metrics/interpolation.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.837067 langspace-0.1.2/langspace/models/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      142 2024-03-12 13:00:53.000000 langspace-0.1.2/langspace/models/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.837915 langspace-0.1.2/langspace/ops/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-11-21 12:34:19.000000 langspace-0.1.2/langspace/ops/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      100 2024-02-27 15:35:00.000000 langspace-0.1.2/langspace/ops/arithmetic.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1438 2024-02-27 15:35:00.000000 langspace-0.1.2/langspace/ops/interpolation.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1778 2024-02-27 15:35:00.000000 langspace-0.1.2/langspace/ops/traversal.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.838354 langspace-0.1.2/langspace/probe/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      335 2024-01-20 14:44:57.000000 langspace-0.1.2/langspace/probe/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.838676 langspace-0.1.2/langspace/probe/arithmetic/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3684 2024-03-15 13:21:38.000000 langspace-0.1.2/langspace/probe/arithmetic/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2298 2024-05-17 21:00:54.000000 langspace-0.1.2/langspace/probe/base.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.839137 langspace-0.1.2/langspace/probe/cluster_vis/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     6488 2024-05-17 23:59:06.000000 langspace-0.1.2/langspace/probe/cluster_vis/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      117 2024-03-15 13:04:53.000000 langspace-0.1.2/langspace/probe/cluster_vis/methods.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.839439 langspace-0.1.2/langspace/probe/defmod/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-11-24 11:17:37.000000 langspace-0.1.2/langspace/probe/defmod/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.839568 langspace-0.1.2/langspace/probe/disentanglement/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)    26085 2024-05-17 23:05:26.000000 langspace-0.1.2/langspace/probe/disentanglement/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.840061 langspace-0.1.2/langspace/probe/interpolation/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3637 2024-03-15 13:21:58.000000 langspace-0.1.2/langspace/probe/interpolation/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.840304 langspace-0.1.2/langspace/probe/lingprop/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      979 2024-01-20 14:32:48.000000 langspace-0.1.2/langspace/probe/lingprop/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.840618 langspace-0.1.2/langspace/probe/sts/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      926 2024-01-20 14:34:31.000000 langspace-0.1.2/langspace/probe/sts/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.840901 langspace-0.1.2/langspace/probe/traversal/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4559 2024-03-15 13:23:01.000000 langspace-0.1.2/langspace/probe/traversal/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.841199 langspace-0.1.2/langspace.egg-info/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1558 2024-05-18 00:02:46.000000 langspace-0.1.2/langspace.egg-info/PKG-INFO
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      885 2024-05-18 00:02:46.000000 langspace-0.1.2/langspace.egg-info/SOURCES.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        1 2024-05-18 00:02:46.000000 langspace-0.1.2/langspace.egg-info/dependency_links.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       71 2024-05-18 00:02:46.000000 langspace-0.1.2/langspace.egg-info/requires.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       10 2024-05-18 00:02:46.000000 langspace-0.1.2/langspace.egg-info/top_level.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      795 2024-05-18 00:01:54.000000 langspace-0.1.2/pyproject.toml
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       70 2024-05-16 18:17:28.000000 langspace-0.1.2/requirements.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       38 2024-05-18 00:02:46.841657 langspace-0.1.2/setup.cfg
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     1131 2024-05-18 00:01:59.000000 langspace-0.1.2/setup.py
```

### Comparing `langspace-0.1.1/LICENSE` & `langspace-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langspace-0.1.1/PKG-INFO` & `langspace-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langspace
-Version: 0.1.1
+Version: 0.1.2
 Summary: LangSpace: Probing Large Language VAEs made simple
 Home-page: 
 Author: ['Danilo S. Carvalho', 'Yingji Zhang']
 Author-email: "Danilo S. Carvalho" <danilo.carvalho@manchester.ac.uk>, Yingji Zhang <yingji.zhang@postgrad.manchester.ac.uk>
 Project-URL: Homepage, https://github.com/neuro-symbolic-ai/LangSpace
 Project-URL: Issues, https://github.com/neuro-symbolic-ai/LangSpace/issues
 Keywords: probing,vae,llm,generative,nlp
```

### Comparing `langspace-0.1.1/README.md` & `langspace-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `langspace-0.1.1/langspace/ops/interpolation.py` & `langspace-0.1.2/langspace/ops/interpolation.py`

 * *Files identical despite different names*

### Comparing `langspace-0.1.1/langspace/ops/traversal.py` & `langspace-0.1.2/langspace/ops/traversal.py`

 * *Files identical despite different names*

### Comparing `langspace-0.1.1/langspace/probe/arithmetic/__init__.py` & `langspace-0.1.2/langspace/probe/arithmetic/__init__.py`

 * *Files identical despite different names*

### Comparing `langspace-0.1.1/langspace/probe/base.py` & `langspace-0.1.2/langspace/probe/base.py`

 * *Files identical despite different names*

### Comparing `langspace-0.1.1/langspace/probe/cluster_vis/__init__.py` & `langspace-0.1.2/langspace/probe/cluster_vis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import numpy as np
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from tqdm import tqdm
 from yellowbrick.features import PCA
 from yellowbrick.text import UMAPVisualizer
 
-mpl.use('TkAgg')  # !IMPORTANT
+# mpl.use('TkAgg')  # !IMPORTANT
 
 
 class ClusterVisualizationProbe(LatentSpaceProbe):
     """
     Class for visualisation (PCA, T-SNE, UMAP) of the latent space of a language VAE.
     """
     def __init__(self, model: LangVAE, data: Iterable[Tuple[Union[str, Sentence], Union[str, int]]], sample_size: int,
```

### Comparing `langspace-0.1.1/langspace/probe/disentanglement/__init__.py` & `langspace-0.1.2/langspace/probe/disentanglement/__init__.py`

 * *Files identical despite different names*

### Comparing `langspace-0.1.1/langspace/probe/interpolation/__init__.py` & `langspace-0.1.2/langspace/probe/interpolation/__init__.py`

 * *Files identical despite different names*

### Comparing `langspace-0.1.1/langspace/probe/lingprop/__init__.py` & `langspace-0.1.2/langspace/probe/lingprop/__init__.py`

 * *Files identical despite different names*

### Comparing `langspace-0.1.1/langspace/probe/sts/__init__.py` & `langspace-0.1.2/langspace/probe/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `langspace-0.1.1/langspace/probe/traversal/__init__.py` & `langspace-0.1.2/langspace/probe/traversal/__init__.py`

 * *Files identical despite different names*

### Comparing `langspace-0.1.1/langspace.egg-info/PKG-INFO` & `langspace-0.1.2/langspace.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langspace
-Version: 0.1.1
+Version: 0.1.2
 Summary: LangSpace: Probing Large Language VAEs made simple
 Home-page: 
 Author: ['Danilo S. Carvalho', 'Yingji Zhang']
 Author-email: "Danilo S. Carvalho" <danilo.carvalho@manchester.ac.uk>, Yingji Zhang <yingji.zhang@postgrad.manchester.ac.uk>
 Project-URL: Homepage, https://github.com/neuro-symbolic-ai/LangSpace
 Project-URL: Issues, https://github.com/neuro-symbolic-ai/LangSpace/issues
 Keywords: probing,vae,llm,generative,nlp
```

### Comparing `langspace-0.1.1/langspace.egg-info/SOURCES.txt` & `langspace-0.1.2/langspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langspace-0.1.1/pyproject.toml` & `langspace-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "langspace"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Danilo S. Carvalho", email="danilo.carvalho@manchester.ac.uk" },
   { name="Yingji Zhang", email="yingji.zhang@postgrad.manchester.ac.uk" }
 ]
 description = "LangSpace: Probing Large Language VAEs made simple"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `langspace-0.1.1/setup.py` & `langspace-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     install_requires = [str(x).strip() for x in all_reqs]
 
     return install_requires
 
 
 setup(
     name='LangSpace',
-    version='0.1.1',
+    version='0.1.2',
     packages=['langspace', 'langspace.ops', 'langspace.probe', 'langspace.probe.sts', 'langspace.probe.defmod',
               'langspace.probe.lingprop', 'langspace.probe.traversal', 'langspace.probe.arithmetic',
               'langspace.probe.cluster_vis', 'langspace.probe.interpolation', 'langspace.probe.disentanglement',
               'langspace.models', 'langspace.metrics'],
     url='',
     license='',
     author=['Danilo S. Carvalho', 'Yingji Zhang'],
```

