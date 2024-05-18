# Comparing `tmp/langspace-0.1.2.tar.gz` & `tmp/langspace-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langspace-0.1.2.tar", last modified: Sat May 18 00:02:46 2024, max compression
+gzip compressed data, was "langspace-0.1.3.tar", last modified: Sat May 18 15:55:38 2024, max compression
```

## Comparing `langspace-0.1.2.tar` & `langspace-0.1.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.841615 langspace-0.1.2/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)    35149 2023-03-15 12:32:16.000000 langspace-0.1.2/LICENSE
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1558 2024-05-18 00:02:46.841431 langspace-0.1.2/PKG-INFO
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      611 2024-05-17 23:28:54.000000 langspace-0.1.2/README.md
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.835545 langspace-0.1.2/langspace/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-11-21 12:34:00.000000 langspace-0.1.2/langspace/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.836858 langspace-0.1.2/langspace/metrics/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        0 2024-01-26 18:39:47.000000 langspace-0.1.2/langspace/metrics/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      307 2024-05-16 18:37:32.000000 langspace-0.1.2/langspace/metrics/disentanglement.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      111 2024-01-26 18:39:48.000000 langspace-0.1.2/langspace/metrics/interpolation.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.837067 langspace-0.1.2/langspace/models/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      142 2024-03-12 13:00:53.000000 langspace-0.1.2/langspace/models/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.837915 langspace-0.1.2/langspace/ops/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-11-21 12:34:19.000000 langspace-0.1.2/langspace/ops/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      100 2024-02-27 15:35:00.000000 langspace-0.1.2/langspace/ops/arithmetic.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1438 2024-02-27 15:35:00.000000 langspace-0.1.2/langspace/ops/interpolation.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1778 2024-02-27 15:35:00.000000 langspace-0.1.2/langspace/ops/traversal.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.838354 langspace-0.1.2/langspace/probe/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      335 2024-01-20 14:44:57.000000 langspace-0.1.2/langspace/probe/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.838676 langspace-0.1.2/langspace/probe/arithmetic/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3684 2024-03-15 13:21:38.000000 langspace-0.1.2/langspace/probe/arithmetic/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2298 2024-05-17 21:00:54.000000 langspace-0.1.2/langspace/probe/base.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.839137 langspace-0.1.2/langspace/probe/cluster_vis/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     6488 2024-05-17 23:59:06.000000 langspace-0.1.2/langspace/probe/cluster_vis/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      117 2024-03-15 13:04:53.000000 langspace-0.1.2/langspace/probe/cluster_vis/methods.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.839439 langspace-0.1.2/langspace/probe/defmod/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-11-24 11:17:37.000000 langspace-0.1.2/langspace/probe/defmod/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.839568 langspace-0.1.2/langspace/probe/disentanglement/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)    26085 2024-05-17 23:05:26.000000 langspace-0.1.2/langspace/probe/disentanglement/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.840061 langspace-0.1.2/langspace/probe/interpolation/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3637 2024-03-15 13:21:58.000000 langspace-0.1.2/langspace/probe/interpolation/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.840304 langspace-0.1.2/langspace/probe/lingprop/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      979 2024-01-20 14:32:48.000000 langspace-0.1.2/langspace/probe/lingprop/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.840618 langspace-0.1.2/langspace/probe/sts/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      926 2024-01-20 14:34:31.000000 langspace-0.1.2/langspace/probe/sts/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.840901 langspace-0.1.2/langspace/probe/traversal/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4559 2024-03-15 13:23:01.000000 langspace-0.1.2/langspace/probe/traversal/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 00:02:46.841199 langspace-0.1.2/langspace.egg-info/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1558 2024-05-18 00:02:46.000000 langspace-0.1.2/langspace.egg-info/PKG-INFO
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      885 2024-05-18 00:02:46.000000 langspace-0.1.2/langspace.egg-info/SOURCES.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        1 2024-05-18 00:02:46.000000 langspace-0.1.2/langspace.egg-info/dependency_links.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       71 2024-05-18 00:02:46.000000 langspace-0.1.2/langspace.egg-info/requires.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       10 2024-05-18 00:02:46.000000 langspace-0.1.2/langspace.egg-info/top_level.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      795 2024-05-18 00:01:54.000000 langspace-0.1.2/pyproject.toml
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       70 2024-05-16 18:17:28.000000 langspace-0.1.2/requirements.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       38 2024-05-18 00:02:46.841657 langspace-0.1.2/setup.cfg
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     1131 2024-05-18 00:01:59.000000 langspace-0.1.2/setup.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 15:55:38.217871 langspace-0.1.3/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)    35149 2023-03-15 12:32:16.000000 langspace-0.1.3/LICENSE
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1585 2024-05-18 15:55:38.217638 langspace-0.1.3/PKG-INFO
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      611 2024-05-17 23:28:54.000000 langspace-0.1.3/README.md
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 15:55:38.210285 langspace-0.1.3/langspace/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-11-21 12:34:00.000000 langspace-0.1.3/langspace/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 15:55:38.212112 langspace-0.1.3/langspace/metrics/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        0 2024-01-26 18:39:47.000000 langspace-0.1.3/langspace/metrics/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      307 2024-05-16 18:37:32.000000 langspace-0.1.3/langspace/metrics/disentanglement.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      111 2024-01-26 18:39:48.000000 langspace-0.1.3/langspace/metrics/interpolation.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 15:55:38.212378 langspace-0.1.3/langspace/models/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      142 2024-03-12 13:00:53.000000 langspace-0.1.3/langspace/models/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 15:55:38.213239 langspace-0.1.3/langspace/ops/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-11-21 12:34:19.000000 langspace-0.1.3/langspace/ops/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      100 2024-02-27 15:35:00.000000 langspace-0.1.3/langspace/ops/arithmetic.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1438 2024-02-27 15:35:00.000000 langspace-0.1.3/langspace/ops/interpolation.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1778 2024-02-27 15:35:00.000000 langspace-0.1.3/langspace/ops/traversal.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 15:55:38.213712 langspace-0.1.3/langspace/probe/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      335 2024-01-20 14:44:57.000000 langspace-0.1.3/langspace/probe/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 15:55:38.214290 langspace-0.1.3/langspace/probe/arithmetic/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3684 2024-03-15 13:21:38.000000 langspace-0.1.3/langspace/probe/arithmetic/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2298 2024-05-17 21:00:54.000000 langspace-0.1.3/langspace/probe/base.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 15:55:38.215077 langspace-0.1.3/langspace/probe/cluster_vis/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     6734 2024-05-18 00:42:37.000000 langspace-0.1.3/langspace/probe/cluster_vis/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      117 2024-03-15 13:04:53.000000 langspace-0.1.3/langspace/probe/cluster_vis/methods.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 15:55:38.215379 langspace-0.1.3/langspace/probe/defmod/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-11-24 11:17:37.000000 langspace-0.1.3/langspace/probe/defmod/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 15:55:38.215524 langspace-0.1.3/langspace/probe/disentanglement/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)    26178 2024-05-18 00:20:29.000000 langspace-0.1.3/langspace/probe/disentanglement/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 15:55:38.216038 langspace-0.1.3/langspace/probe/interpolation/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3637 2024-03-15 13:21:58.000000 langspace-0.1.3/langspace/probe/interpolation/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 15:55:38.216325 langspace-0.1.3/langspace/probe/lingprop/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      979 2024-01-20 14:32:48.000000 langspace-0.1.3/langspace/probe/lingprop/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 15:55:38.216696 langspace-0.1.3/langspace/probe/sts/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      926 2024-01-20 14:34:31.000000 langspace-0.1.3/langspace/probe/sts/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 15:55:38.217030 langspace-0.1.3/langspace/probe/traversal/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4559 2024-03-15 13:23:01.000000 langspace-0.1.3/langspace/probe/traversal/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-18 15:55:38.217388 langspace-0.1.3/langspace.egg-info/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1585 2024-05-18 15:55:38.000000 langspace-0.1.3/langspace.egg-info/PKG-INFO
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      885 2024-05-18 15:55:38.000000 langspace-0.1.3/langspace.egg-info/SOURCES.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        1 2024-05-18 15:55:38.000000 langspace-0.1.3/langspace.egg-info/dependency_links.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       83 2024-05-18 15:55:38.000000 langspace-0.1.3/langspace.egg-info/requires.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       10 2024-05-18 15:55:38.000000 langspace-0.1.3/langspace.egg-info/top_level.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      795 2024-05-18 15:53:37.000000 langspace-0.1.3/pyproject.toml
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       82 2024-05-18 00:12:54.000000 langspace-0.1.3/requirements.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       38 2024-05-18 15:55:38.217914 langspace-0.1.3/setup.cfg
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     1131 2024-05-18 15:53:41.000000 langspace-0.1.3/setup.py
```

### Comparing `langspace-0.1.2/LICENSE` & `langspace-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `langspace-0.1.2/PKG-INFO` & `langspace-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langspace
-Version: 0.1.2
+Version: 0.1.3
 Summary: LangSpace: Probing Large Language VAEs made simple
 Home-page: 
 Author: ['Danilo S. Carvalho', 'Yingji Zhang']
 Author-email: "Danilo S. Carvalho" <danilo.carvalho@manchester.ac.uk>, Yingji Zhang <yingji.zhang@postgrad.manchester.ac.uk>
 Project-URL: Homepage, https://github.com/neuro-symbolic-ai/LangSpace
 Project-URL: Issues, https://github.com/neuro-symbolic-ai/LangSpace/issues
 Keywords: probing,vae,llm,generative,nlp
@@ -16,14 +16,15 @@
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: transformers
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: pot
+Requires-Dist: yellowbrick
 Requires-Dist: langvae
 Requires-Dist: saf-nlp
 Requires-Dist: saf-datasets
 
 # LangSpace: Probing Large Language VAEs made simple
 
 LangSpace is a Python library for evaluating and probing language models using Variational Autoencoders (VAEs). It provides an easy-to-use interface to perform a variety of analises on pretrained [LangVAE](https://github.com/neuro-symbolic-ai/LangVAE) models.
```

### Comparing `langspace-0.1.2/README.md` & `langspace-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `langspace-0.1.2/langspace/ops/interpolation.py` & `langspace-0.1.3/langspace/ops/interpolation.py`

 * *Files identical despite different names*

### Comparing `langspace-0.1.2/langspace/ops/traversal.py` & `langspace-0.1.3/langspace/ops/traversal.py`

 * *Files identical despite different names*

### Comparing `langspace-0.1.2/langspace/probe/arithmetic/__init__.py` & `langspace-0.1.3/langspace/probe/arithmetic/__init__.py`

 * *Files identical despite different names*

### Comparing `langspace-0.1.2/langspace/probe/base.py` & `langspace-0.1.3/langspace/probe/base.py`

 * *Files identical despite different names*

### Comparing `langspace-0.1.2/langspace/probe/cluster_vis/__init__.py` & `langspace-0.1.3/langspace/probe/cluster_vis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,17 +125,24 @@
         args:
             Inputs:
                 list: [[s1, label], [s2, label], ..., [sn, label]]
                 E.g., [["the appalachian mountains are a kind of mountain", label1], ["the appalachian mountains are a kind of mountain", label2]]
             Return:
                 save image.png
         """
+
+        if (isinstance(list(self.data[:1])[0], Sentence)):
+            data = [[sent.surface, " ".join([tok.annotations[annotation] for tok in sent.tokens])]
+                    for sent in self.data]
+        else:
+            data = self.data
+
         latent_all, label_all = [], []
-        for data_batch in tqdm([self.data[i * self.batch_size: (i + 1) * self.batch_size]
-                           for i in range(math.ceil(self.sample_size / self.batch_size))], desc="Encoding"):
+        for data_batch in tqdm([data[i * self.batch_size: (i + 1) * self.batch_size]
+                                for i in range(math.ceil(self.sample_size / self.batch_size))], desc="Encoding"):
             latent_all.append(self.encoding([d[0] for d in data_batch]))
             label_all.extend([d[1] for d in data_batch])
 
         latent_all = torch.cat(latent_all)
         classes = list(set(label_all))
 
         # Create the visualizer and draw the vectors
```

### Comparing `langspace-0.1.2/langspace/probe/disentanglement/__init__.py` & `langspace-0.1.3/langspace/probe/disentanglement/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -490,25 +490,25 @@
 
             # print(model.feature_importances_.shape) 256
 
         r = np.array(r)
 
         for i in range(0, r.shape[1]):
             p = r[:, i]
-            p = p / np.sum(p)
+            p = p / np.sum(p) if (np.sum(p) > 1e-7) else 0.0
             h_k_p = self.entropy(p) / np.log(r.shape[0])
             disentanglement.append(1 - h_k_p)
 
         disentanglement = np.array(disentanglement)
-        weight = np.sum(r, axis=0) / np.sum(r)
+        weight = np.sum(r, axis=0) / np.sum(r) if (np.sum(r) > 1e-7) else 0.0
         # print("Disentanglement Score: {:.4f}".format(np.sum(weight * disentanglement)))
 
         for j in range(0, r.shape[0]):
             p = r[j, :]
-            p = p / np.sum(p)
+            p = p / np.sum(p) if (np.sum(p) > 1e-7) else 0.0
             h_d_p = self.entropy(p) / np.log(r.shape[1])
             completeness.append(1 - h_d_p)
 
         completeness = np.array(completeness)
         # print("Completeness Score: {:.4f}".format(np.mean(completeness)))
 
         informativeness = np.array(informativeness)
```

### Comparing `langspace-0.1.2/langspace/probe/interpolation/__init__.py` & `langspace-0.1.3/langspace/probe/interpolation/__init__.py`

 * *Files identical despite different names*

### Comparing `langspace-0.1.2/langspace/probe/lingprop/__init__.py` & `langspace-0.1.3/langspace/probe/lingprop/__init__.py`

 * *Files identical despite different names*

### Comparing `langspace-0.1.2/langspace/probe/sts/__init__.py` & `langspace-0.1.3/langspace/probe/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `langspace-0.1.2/langspace/probe/traversal/__init__.py` & `langspace-0.1.3/langspace/probe/traversal/__init__.py`

 * *Files identical despite different names*

### Comparing `langspace-0.1.2/langspace.egg-info/PKG-INFO` & `langspace-0.1.3/langspace.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langspace
-Version: 0.1.2
+Version: 0.1.3
 Summary: LangSpace: Probing Large Language VAEs made simple
 Home-page: 
 Author: ['Danilo S. Carvalho', 'Yingji Zhang']
 Author-email: "Danilo S. Carvalho" <danilo.carvalho@manchester.ac.uk>, Yingji Zhang <yingji.zhang@postgrad.manchester.ac.uk>
 Project-URL: Homepage, https://github.com/neuro-symbolic-ai/LangSpace
 Project-URL: Issues, https://github.com/neuro-symbolic-ai/LangSpace/issues
 Keywords: probing,vae,llm,generative,nlp
@@ -16,14 +16,15 @@
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: transformers
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: pot
+Requires-Dist: yellowbrick
 Requires-Dist: langvae
 Requires-Dist: saf-nlp
 Requires-Dist: saf-datasets
 
 # LangSpace: Probing Large Language VAEs made simple
 
 LangSpace is a Python library for evaluating and probing language models using Variational Autoencoders (VAEs). It provides an easy-to-use interface to perform a variety of analises on pretrained [LangVAE](https://github.com/neuro-symbolic-ai/LangVAE) models.
```

### Comparing `langspace-0.1.2/langspace.egg-info/SOURCES.txt` & `langspace-0.1.3/langspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langspace-0.1.2/pyproject.toml` & `langspace-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "langspace"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Danilo S. Carvalho", email="danilo.carvalho@manchester.ac.uk" },
   { name="Yingji Zhang", email="yingji.zhang@postgrad.manchester.ac.uk" }
 ]
 description = "LangSpace: Probing Large Language VAEs made simple"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `langspace-0.1.2/setup.py` & `langspace-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     install_requires = [str(x).strip() for x in all_reqs]
 
     return install_requires
 
 
 setup(
     name='LangSpace',
-    version='0.1.2',
+    version='0.1.3',
     packages=['langspace', 'langspace.ops', 'langspace.probe', 'langspace.probe.sts', 'langspace.probe.defmod',
               'langspace.probe.lingprop', 'langspace.probe.traversal', 'langspace.probe.arithmetic',
               'langspace.probe.cluster_vis', 'langspace.probe.interpolation', 'langspace.probe.disentanglement',
               'langspace.models', 'langspace.metrics'],
     url='',
     license='',
     author=['Danilo S. Carvalho', 'Yingji Zhang'],
```

