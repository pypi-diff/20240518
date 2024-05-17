# Comparing `tmp/hypernetx-2.2.0.tar.gz` & `tmp/hypernetx-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypernetx-2.2.0.tar", last modified: Sat Mar  2 00:03:15 2024, max compression
+gzip compressed data, was "hypernetx-2.3.0.tar", max compression
```

## Comparing `hypernetx-2.2.0.tar` & `hypernetx-2.3.0.tar`

### file list

```diff
@@ -1,52 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:03:15.750184 hypernetx-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-02 00:03:12.000000 hypernetx-2.2.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-03-02 00:03:12.000000 hypernetx-2.2.0/LONG_DESCRIPTION.rst
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-02 00:03:12.000000 hypernetx-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-03-02 00:03:15.750184 hypernetx-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13445 2024-03-02 00:03:12.000000 hypernetx-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:03:15.738184 hypernetx-2.2.0/hypernetx/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:03:15.742184 hypernetx-2.2.0/hypernetx/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40022 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/algorithms/contagion.py
--rw-r--r--   0 runner    (1001) docker     (127)     8678 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/algorithms/generative_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    24278 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/algorithms/homology_mod2.py
--rw-r--r--   0 runner    (1001) docker     (127)    18981 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/algorithms/hypergraph_modularity.py
--rw-r--r--   0 runner    (1001) docker     (127)     7821 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/algorithms/laplacians_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/algorithms/s_centrality_measures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:03:15.742184 hypernetx-2.2.0/hypernetx/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74018 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/classes/entityset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9915 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/classes/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    83488 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/classes/hypergraph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:03:15.742184 hypernetx-2.2.0/hypernetx/drawing/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/drawing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16140 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/drawing/rubber_band.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/drawing/two_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/drawing/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/read_write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:03:15.742184 hypernetx-2.2.0/hypernetx/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/reports/descriptive_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:03:15.746184 hypernetx-2.2.0/hypernetx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/utils/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/utils/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:03:15.746184 hypernetx-2.2.0/hypernetx/utils/toys/
--rw-r--r--   0 runner    (1001) docker     (127)    26129 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/utils/toys/HarryPotter_Characters.csv
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/utils/toys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/utils/toys/gene_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/utils/toys/harrypotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14357 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/utils/toys/lesmis.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-02 00:03:12.000000 hypernetx-2.2.0/hypernetx/utils/toys/transmission_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 00:03:15.746184 hypernetx-2.2.0/hypernetx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-03-02 00:03:15.000000 hypernetx-2.2.0/hypernetx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-02 00:03:15.000000 hypernetx-2.2.0/hypernetx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 00:03:15.000000 hypernetx-2.2.0/hypernetx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-02 00:03:15.000000 hypernetx-2.2.0/hypernetx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-02 00:03:15.000000 hypernetx-2.2.0/hypernetx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-02 00:03:12.000000 hypernetx-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-03-02 00:03:15.750184 hypernetx-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-02 00:03:12.000000 hypernetx-2.2.0/setup.py
+-rw-r--r--   0        0        0     1531 2024-05-17 22:20:35.008500 hypernetx-2.3.0/LICENSE.rst
+-rw-r--r--   0        0        0    14282 2024-05-17 22:20:35.008500 hypernetx-2.3.0/README.md
+-rw-r--r--   0        0        0      394 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/__init__.py
+-rw-r--r--   0        0        0     2539 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/algorithms/__init__.py
+-rw-r--r--   0        0        0    39968 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/algorithms/contagion.py
+-rw-r--r--   0        0        0     8678 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/algorithms/generative_models.py
+-rw-r--r--   0        0        0    24278 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/algorithms/homology_mod2.py
+-rw-r--r--   0        0        0    18956 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/algorithms/hypergraph_modularity.py
+-rw-r--r--   0        0        0     7821 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/algorithms/laplacians_clustering.py
+-rw-r--r--   0        0        0     9964 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/algorithms/s_centrality_measures.py
+-rw-r--r--   0        0        0      237 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/classes/__init__.py
+-rw-r--r--   0        0        0    13259 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/classes/factory.py
+-rw-r--r--   0        0        0     9852 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/classes/hyp_view.py
+-rw-r--r--   0        0        0    98452 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/classes/hypergraph.py
+-rw-r--r--   0        0        0     7443 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/classes/incidence_store.py
+-rw-r--r--   0        0        0    10028 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/classes/property_store.py
+-rw-r--r--   0        0        0      151 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/drawing/__init__.py
+-rw-r--r--   0        0        0    16790 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/drawing/rubber_band.py
+-rw-r--r--   0        0        0     5612 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/drawing/two_column.py
+-rw-r--r--   0        0        0     3406 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/drawing/util.py
+-rw-r--r--   0        0        0      426 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/exception.py
+-rw-r--r--   0        0        0      379 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/read_write.py
+-rw-r--r--   0        0        0      491 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/reports/__init__.py
+-rw-r--r--   0        0        0    11393 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/reports/descriptive_stats.py
+-rw-r--r--   0        0        0      720 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/utils/__init__.py
+-rw-r--r--   0        0        0     2430 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/utils/decorators.py
+-rw-r--r--   0        0        0     5122 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/utils/extras.py
+-rw-r--r--   0        0        0     1423 2024-05-17 22:20:35.016500 hypernetx-2.3.0/hypernetx/utils/log.py
+-rw-r--r--   0        0        0   165566 2024-05-17 22:20:35.020500 hypernetx-2.3.0/hypernetx/utils/toys/ChungLuTransmissionData.csv
+-rw-r--r--   0        0        0   116969 2024-05-17 22:20:35.020500 hypernetx-2.3.0/hypernetx/utils/toys/GoT.pkl
+-rw-r--r--   0        0        0     7925 2024-05-17 22:20:35.020500 hypernetx-2.3.0/hypernetx/utils/toys/HarryPotterHypergraph.p
+-rw-r--r--   0        0        0    26129 2024-05-17 22:20:35.020500 hypernetx-2.3.0/hypernetx/utils/toys/HarryPotter_Characters.csv
+-rw-r--r--   0        0        0      409 2024-05-17 22:20:35.020500 hypernetx-2.3.0/hypernetx/utils/toys/__init__.py
+-rw-r--r--   0        0        0  1736336 2024-05-17 22:20:35.024500 hypernetx-2.3.0/hypernetx/utils/toys/disGene.txt
+-rw-r--r--   0        0        0      353 2024-05-17 22:20:35.024500 hypernetx-2.3.0/hypernetx/utils/toys/gene_data.py
+-rw-r--r--   0        0        0     3809 2024-05-17 22:20:35.024500 hypernetx-2.3.0/hypernetx/utils/toys/harrypotter.py
+-rw-r--r--   0        0        0    14357 2024-05-17 22:20:35.024500 hypernetx-2.3.0/hypernetx/utils/toys/lesmis.py
+-rw-r--r--   0        0        0      552 2024-05-17 22:20:35.024500 hypernetx-2.3.0/hypernetx/utils/toys/transmission_problem.py
+-rw-r--r--   0        0        0     2408 2024-05-17 22:20:35.028500 hypernetx-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0    15209 1970-01-01 00:00:00.000000 hypernetx-2.3.0/PKG-INFO
```

### Comparing `hypernetx-2.2.0/LICENSE.rst` & `hypernetx-2.3.0/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _license:
 
 License
 =======
 
 HyperNetX
 
-Copyright 2018, 2023, Battelle Memorial Institute
+Copyright 2018, 2023, 2024, Battelle Memorial Institute
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer.
```

### Comparing `hypernetx-2.2.0/README.md` & `hypernetx-2.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-<img src="docs/source/images/harrypotter_basic_hyp.png" align="right" width="300pt">
-
 HyperNetX
 ==========
+<img src="docs/source/images/harrypotter_basic_hyp.png" align="right" width="300pt">
+
 [![Pytest](https://github.com/pnnl/HyperNetX/actions/workflows/ci.yml/badge.svg)](https://github.com/pnnl/HyperNetX/actions/workflows/ci.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
-
+[![CITATION.cff](https://github.com/pnnl/HyperNetX/actions/workflows/cff.yml/badge.svg)](https://github.com/pnnl/HyperNetX/actions/workflows/cff.yml)
 
 The HyperNetX library provides classes and methods for the analysis
 and visualization of complex network data modeled as hypergraphs.
 The library generalizes traditional graph metrics.
 
 HypernetX was developed by the Pacific Northwest National Laboratory for the
 Hypernets project as part of its High Performance Data Analytics (HPDA) program.
@@ -24,93 +24,89 @@
 
 The code in this repository is intended to support researchers modeling data
 as hypergraphs. We have a growing community of users and contributors.
 Documentation is available at: https://pnnl.github.io/HyperNetX
 
 For questions and comments contact the developers directly at: hypernetx@pnnl.gov
 
-New Features in Version 2.0
-===========================
+Summary - Release highlights - HNX 2.3
+--------------------------------------
 
-HNX 2.0 now accepts metadata as core attributes of the edges and nodes of a
-hypergraph. While the library continues to accept lists, dictionaries and
-dataframes as basic inputs for hypergraph constructions, both cell
-properties and edge and node properties can now be easily added for
-retrieval as object attributes.
-
-The core library has been rebuilt to take advantage of the flexibility and speed of Pandas Dataframes.
-Dataframes offer the ability to store and easily access hypergraph metadata. Metadata can be used for filtering objects, and characterize their
-distributions by their attributes.
+HyperNetX 2.3. is the latest, stable release. The core library has been refactored to take better advantage
+of Pandas Dataframes, improve readability and maintainability, address bugs, and make it easier to change.
+New features have been added, most notably the ability to add and remove edges, nodes, and incidences.
 
-**Version 2.0 is not backwards compatible. Objects constructed using version
-1.x can be imported from their incidence dictionaries.**
+**Version 2.3 is not backwards compatible. Objects constructed using earlier versions
+can be imported using their incidence dictionaries and/or property datafames.**
 
 What's New
-----------
-1. The Hypergraph constructor now accepts nested dictionaries with incidence cell properties, pandas.DataFrames, and 2-column Numpy arrays.
-1. Additional constructors accept incidence matrices and incidence dataframes.
-1. Hypergraph constructors accept cell, edge, and node metadata.
-1. Metadata available as attributes on the cells, edges, and nodes.
-1. User-defined cell weights and default weights available to incidence matrix.
-1. Meta data persists with restrictions and removals.
-1. Meta data persists onto s-linegraphs as node attributes of Networkx graphs.
-1. New hnxwidget available using  `pip install hnxwidget`.
+~~~~~~~~~~~~~~~~~~~~~~~~~
+#. Hypergraph now supports adding and removing edges, nodes, and incidences
+#. Hypergraph also supports the sum, difference, union, and intersection of a Hypergraph to another Hypergraph
+#. New factory methods to support the Hypergraph constructor
+#. EntitySet has been replaced by HypergraphView
+#. IncidenceStore and PropertyStore are new classes that maintain the structure and attributes of a Hypergraph
+#. Hypergraph constructors accept cell, edge, and node metadata.
 
 
 What's Changed
+~~~~~~~~~~~~~~~~~~~~~~~~~
+#. HNX now requires Python ^3.10,<=3.12
+#. HNX core libraries have been updated
+#. Updated tutorials
 --------------
 1. The `static` and `dynamic` distinctions no longer exist. All hypergraphs use the same underlying data structure, supported by Pandas dataFrames. All hypergraphs maintain a `state_dict` to avoid repeating computations.
 1. Methods for adding nodes and hyperedges are currently not supported.
 1. The `nwhy` optimizations are no longer supported.
 1. Entity and EntitySet classes are being moved to the background. The Hypergraph constructor does not accept either.
 
 
 
-Tutorials
-=========
+Tutorials Available for Colab
+=============================
 
 Google Colab
 ------------
 
 
-<a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Tutorial%201%20-%20HNX%20Basics.ipynb" target="_blank">
+<a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Basic%201%20-%20HNX%20Basics.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
-    <span >Tutorial 1 - HNX Basics</span>
+    <span >Basic 1 - HNX Basics</span>
 </a>
-<br>
+</br>
 
-<a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Tutorial%202%20-%20Visualization%20Methods.ipynb" target="_blank">
+<a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Basic%202%20-%20Visualization%20Methods.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
-    <span >Tutorial 2 - Visualization Methods</span>
+    <span >Basic 2 - Visualization Methods</span>
 </a>
-<br>
+</br>
 
-<a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Tutorial%203%20-%20LesMis%20Case%20Study.ipynb" target="_blank">
+<a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Basic%203%20-%20LesMis%20Case%20Study.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
-    <span >Tutorial 3 - LesMis Case Study</span>
+    <span >Basic 3 - LesMis Case Study</span>
 </a>
-<br>
+</br>
 
-<a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Tutorial%204%20-%20LesMis%20Visualizations-BookTour.ipynb" target="_blank">
+<a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Basic%204%20-%20LesMis%20Visualizations-BookTour.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
-    <span >Tutorial 4 - LesMis Visualizations-Book Tour</span>
+    <span >Basic 4 - LesMis Visualizations-Book Tour</span>
 </a>
-<br>
+</br>
 
-<a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/Tutorial%205%20-%20s-Centrality.ipynb" target="_blank">
+<a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Basic%205%20-%20HNX%20attributed%20hypergraph.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
-    <span >Tutorial 5 - s-Centrality</span>
+    <span >Basic 5 - HNX attributed hypergraph</span>
 </a>
-<br>
+</br>
 
-<a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/advanced/Tutorial%206%20-%20Homology%20mod%202%20for%20TriLoop%20Example.ipynb" target="_blank">
+<a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Basic%206%20-%20Hypergraph%20Arithmetic.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
-    <span >Tutorial 6 - Homology mod2 for TriLoop Example</span>
+    <span >Basic 6 - Hypergraph Arithmetic.ipynb</span>
 </a>
-<br>
+</br>
 
 
 Jupyter Notebooks
 -----------------
 
 Additional tutorials that can be run as Jupyter Notebooks are found under [tutorials](./tutorials).
 
@@ -186,46 +182,88 @@
 ----------------------
 
 Ensure that you have [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) installed.
 
 ```shell
 git clone https://github.com/pnnl/HyperNetX.git
 cd HyperNetX
+
+# Create a virtual environment
 make venv
 source venv-hnx/bin/activate
-pip install .
+
+# install required dependencies
+make install
 ```
 
 Development
 ===========
 
 Install an editable version
----------------------------
-
 ```
 pip install -e .
 ```
 
-Install an editable version with supported applications
--------------------------------------------------------
+Install additional dependencies to support testing and jupyter notebooks:
+```
+pip install -r requirements.txt
+```
+
+You can also install all these requirements in one Make target:
 
-```shell
-pip install -e .['all']
+```
+make install
+```
+
+Poetry
+======
+
+This library uses [Poetry](https://python-poetry.org/docs/) to manage dependencies and packaging. Poetry can also be
+used to manage your environment for development.
+
+Prerequisites
+-------------
+
+* [Install Poetry](https://python-poetry.org/docs/#installation)
+
+
+Configure Poetry
+----------------
+
+[Configure your Poetry](https://python-poetry.org/docs/configuration/) to create the virtual environment in your project directory:
+```
+poetry config virtualenvs.in-project true
+
+# check the poetry configuration
+poetry config --list
+```
+
+Set up virtual environment
+----------------------------
+
+Create and activate a virtual environment.
+```
+poetry shell
+```
+
+NOTE: If you plan to use Poetry to manage your virtual environment, you can activate the virtual environment
+using poerty: `poetry shell`. Another option is to directly
 
-# for zsh users
-pip install -e .'[all]'
+Install required dependencies and HyperNetX in editable mode.
+```
+poetry install
 ```
 
 Install support for testing
 -----------------------------
 
 > ℹ️ **NOTE:** This project has a pytest configuration file named 'pytest.ini'. By default, pytest will use those configuration settings to run tests.
 
 ```shell
-make test-deps
+poetry install --with test
 
 # run tests
 python -m pytest
 
 # run tests and show coverage report
 python -m pytest --cov=hypernetx
 
@@ -233,40 +271,36 @@
 coverage html
 open htmlcov/index.html
 ```
 
 Install support for tutorials
 -----------------------------
 
-``` shell
-make tutorial-deps
+```
+poetry install --with tutorials
 
 # open Jupyter notebooks in a browser
 make tutorials
 ```
 
-
-
-
-
 Code Quality
 ------------
 HyperNetX uses a number of tools to maintain code quality:
 
 * Pylint
 * Black
 
 Before using these tools, ensure that you install Pylint in your environment:
 
-```shell
-make lint-deps
+```
+poetry install --with lint
 ```
 
-
-### Pylint
+Pylint
+------
 
 [Pylint](https://pylint.pycqa.org/en/latest/index.html) is a static code analyzer for Python-based projects. From the [Pylint docs](https://pylint.pycqa.org/en/latest/index.html#what-is-pylint):
 
 > Pylint analyses your code without actually running it. It checks for errors, enforces a coding standard, looks for code smells, and can make suggestions about how the code could be refactored. Pylint can infer actual values from your code using its internal code representation (astroid). If your code is import logging as argparse, Pylint will know that argparse.error(...) is in fact a logging call and not an argparse call.
 
 To run Pylint and view the results of Pylint, run the following command:
 
@@ -278,45 +312,39 @@
 
 ```shell
 pylint hypernetx --output=pylint-results.txt
 ```
 
 For more information on configuration, see https://pylint.pycqa.org/en/latest/user_guide/configuration/index.html
 
-### Black
-
+Black
+-----
 [Black](https://black.readthedocs.io/en/stable/) is a PEP 8 compliant formatter for Python-based project. This tool is highly opinionated about how Python should be formatted and will automagically reformat your code.
 
 
 ```shell
-make format-deps
 black hypernetx
 ```
 
 Documentation
-===============
+-------------
 
-Build and view documentation locally
----------------------------
+Build and view documentation locally:
 
 ```
-make docs-deps
+poetry install --with docs
 cd docs
 make html
 open docs/build/html/index.html
 ```
 
-Editing documentation
-----------------------
-
 When editing documentation, you can auto-rebuild the documentation locally so that you can view your document changes
 live on the browser without having to rebuild every time you have a change.
 
 ```
-make docs-deps
 cd docs
 make livehtml
 ```
 
 This make script will run in the foreground on your terminal. You should see the following:
 
 ```shell
@@ -349,23 +377,23 @@
 
 # Get the status of the workflow
 gh run list --workflow=ci.yml --repo pnnl/HyperNetX
 ```
 
 
 Versioning
-----------
+==========
 
 This project uses [`commitizen`](https://github.com/commitizen-tools/commitizen) to manage versioning.
 The files where "version" will be updated are listed in the '.cz.toml' file. To create a new version and the associated tag,
 run the following commands:
 
 ```shell
 # Install commitizen tool to environment
-make version-deps
+pip install commitizen
 
 # Updates version; values for '--increment' can be MAJOR, MINOR, or PATCH
 # Autocreates a tag and commit for the updated version
 cz bump  --increment MAJOR  --dry-run
 cz bump  --increment MAJOR
 ```
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
-[docs/source/images/harrypotter_basic_hyp.png]HyperNetX ========== [![Pytest]
+HyperNetX ========== [docs/source/images/harrypotter_basic_hyp.png][![Pytest]
 (https://github.com/pnnl/HyperNetX/actions/workflows/ci.yml/badge.svg)](https:/
 /github.com/pnnl/HyperNetX/actions/workflows/ci.yml) [![Code style: black]
 (https://img.shields.io/badge/code%20style-black-000000.svg)](https://
 github.com/psf/black) [![linting: pylint](https://img.shields.io/badge/linting-
-pylint-yellowgreen)](https://github.com/PyCQA/pylint) The HyperNetX library
+pylint-yellowgreen)](https://github.com/PyCQA/pylint) [![CITATION.cff](https://
+github.com/pnnl/HyperNetX/actions/workflows/cff.yml/badge.svg)](https://
+github.com/pnnl/HyperNetX/actions/workflows/cff.yml) The HyperNetX library
 provides classes and methods for the analysis and visualization of complex
 network data modeled as hypergraphs. The library generalizes traditional graph
 metrics. HypernetX was developed by the Pacific Northwest National Laboratory
 for the Hypernets project as part of its High Performance Data Analytics (HPDA)
 program. PNNL is operated by Battelle Memorial Institute under Contract DE-
 ACO5-76RL01830. * Principal Developer and Designer: Brenda Praggastis *
 Development Team: Audun Myers, Mark Bonicillo * Visualization: Dustin Arendt,
@@ -15,48 +17,44 @@
 Kritzstein * Principal Contributors (Design, Theory, Code): Sinan Aksoy, Dustin
 Arendt, Mark Bonicillo, Helen Jenne, Cliff Joslyn, Nicholas Landry, Audun
 Myers, Christopher Potvin, Brenda Praggastis, Emilie Purvine, Greg Roek, Mirah
 Shi, Francois Theberge, Ji Young Yun The code in this repository is intended to
 support researchers modeling data as hypergraphs. We have a growing community
 of users and contributors. Documentation is available at: https://
 pnnl.github.io/HyperNetX For questions and comments contact the developers
-directly at: hypernetx@pnnl.gov New Features in Version 2.0
-=========================== HNX 2.0 now accepts metadata as core attributes of
-the edges and nodes of a hypergraph. While the library continues to accept
-lists, dictionaries and dataframes as basic inputs for hypergraph
-constructions, both cell properties and edge and node properties can now be
-easily added for retrieval as object attributes. The core library has been
-rebuilt to take advantage of the flexibility and speed of Pandas Dataframes.
-Dataframes offer the ability to store and easily access hypergraph metadata.
-Metadata can be used for filtering objects, and characterize their
-distributions by their attributes. **Version 2.0 is not backwards compatible.
-Objects constructed using version 1.x can be imported from their incidence
-dictionaries.** What's New ---------- 1. The Hypergraph constructor now accepts
-nested dictionaries with incidence cell properties, pandas.DataFrames, and 2-
-column Numpy arrays. 1. Additional constructors accept incidence matrices and
-incidence dataframes. 1. Hypergraph constructors accept cell, edge, and node
-metadata. 1. Metadata available as attributes on the cells, edges, and nodes.
-1. User-defined cell weights and default weights available to incidence matrix.
-1. Meta data persists with restrictions and removals. 1. Meta data persists
-onto s-linegraphs as node attributes of Networkx graphs. 1. New hnxwidget
-available using `pip install hnxwidget`. What's Changed -------------- 1. The
-`static` and `dynamic` distinctions no longer exist. All hypergraphs use the
-same underlying data structure, supported by Pandas dataFrames. All hypergraphs
+directly at: hypernetx@pnnl.gov Summary - Release highlights - HNX 2.3 --------
+------------------------------ HyperNetX 2.3. is the latest, stable release.
+The core library has been refactored to take better advantage of Pandas
+Dataframes, improve readability and maintainability, address bugs, and make it
+easier to change. New features have been added, most notably the ability to add
+and remove edges, nodes, and incidences. **Version 2.3 is not backwards
+compatible. Objects constructed using earlier versions can be imported using
+their incidence dictionaries and/or property datafames.** What's New
+~~~~~~~~~~~~~~~~~~~~~~~~~ #. Hypergraph now supports adding and removing edges,
+nodes, and incidences #. Hypergraph also supports the sum, difference, union,
+and intersection of a Hypergraph to another Hypergraph #. New factory methods
+to support the Hypergraph constructor #. EntitySet has been replaced by
+HypergraphView #. IncidenceStore and PropertyStore are new classes that
+maintain the structure and attributes of a Hypergraph #. Hypergraph
+constructors accept cell, edge, and node metadata. What's Changed
+~~~~~~~~~~~~~~~~~~~~~~~~~ #. HNX now requires Python ^3.10,<=3.12 #. HNX core
+libraries have been updated #. Updated tutorials -------------- 1. The `static`
+and `dynamic` distinctions no longer exist. All hypergraphs use the same
+underlying data structure, supported by Pandas dataFrames. All hypergraphs
 maintain a `state_dict` to avoid repeating computations. 1. Methods for adding
 nodes and hyperedges are currently not supported. 1. The `nwhy` optimizations
 are no longer supported. 1. Entity and EntitySet classes are being moved to the
 background. The Hypergraph constructor does not accept either. Tutorials
-========= Google Colab ------------ _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_T_u_t_o_r_i_a_l_ _1_ _-_ _H_N_X_ _B_a_s_i_c_s_ 
-_[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_T_u_t_o_r_i_a_l_ _2_ _-_ _V_i_s_u_a_l_i_z_a_t_i_o_n_ _M_e_t_h_o_d_s_ 
-_[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_T_u_t_o_r_i_a_l_ _3_ _-_ _L_e_s_M_i_s_ _C_a_s_e_ _S_t_u_d_y_ 
-_[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_T_u_t_o_r_i_a_l_ _4_ _-_ _L_e_s_M_i_s_ _V_i_s_u_a_l_i_z_a_t_i_o_n_s_-_B_o_o_k_ _T_o_u_r_ 
-_[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_T_u_t_o_r_i_a_l_ _5_ _-_ _s_-_C_e_n_t_r_a_l_i_t_y_ 
-_[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_T_u_t_o_r_i_a_l_ _6_ _-_ _H_o_m_o_l_o_g_y_ _m_o_d_2_ _f_o_r_ _T_r_i_L_o_o_p_ _E_x_a_m_p_l_e_ 
-Jupyter Notebooks ----------------- Additional tutorials that can be run as
-Jupyter Notebooks are found under [tutorials](./tutorials). Installation
+Available for Colab ============================= Google Colab ------------
+_[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_B_a_s_i_c_ _1_ _-_ _H_N_X_ _B_a_s_i_c_s_ _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_B_a_s_i_c_ _2_ _-_ _V_i_s_u_a_l_i_z_a_t_i_o_n
+_M_e_t_h_o_d_s_ _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_B_a_s_i_c_ _3_ _-_ _L_e_s_M_i_s_ _C_a_s_e_ _S_t_u_d_y_ _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_B_a_s_i_c_ _4_ _-
+_L_e_s_M_i_s_ _V_i_s_u_a_l_i_z_a_t_i_o_n_s_-_B_o_o_k_ _T_o_u_r_ _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_B_a_s_i_c_ _5_ _-_ _H_N_X_ _a_t_t_r_i_b_u_t_e_d
+_h_y_p_e_r_g_r_a_p_h_ _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_B_a_s_i_c_ _6_ _-_ _H_y_p_e_r_g_r_a_p_h_ _A_r_i_t_h_m_e_t_i_c_._i_p_y_n_b_ Jupyter
+Notebooks ----------------- Additional tutorials that can be run as Jupyter
+Notebooks are found under [tutorials](./tutorials). Installation
 ==================== The recommended installation method for most users is to
 create a virtual environment and install HyperNetX from PyPi. HyperNetX may be
 cloned or forked from [Github](https://github.com/pnnl/HyperNetX).
 Prerequisites ------------- HyperNetX officially supports Python 3.8, 3.9, 3.10
 and 3.11. Create a virtual environment ---------------------------- ### Using
 venv ```shell python -m venv venv-hnx source venv-hnx/bin/activate ``` ###
 Using Anaconda ```shell conda create -n venv-hnx python=3.11 -y conda activate
@@ -66,78 +64,90 @@
 ```shell .\env-hnx\Scripts\activate ``` To deactivate your environment, use:
 ```shell .\env-hnx\Scripts\deactivate ``` Installing HyperNetX
 ==================== Regardless of how you install HyperNetX, ensure that your
 environment is activated and that you are running Python >=3.8. Installing from
 PyPi -------------------- ```shell pip install hypernetx ``` Installing from
 Source ---------------------- Ensure that you have [git](https://git-scm.com/
 book/en/v2/Getting-Started-Installing-Git) installed. ```shell git clone https:
-//github.com/pnnl/HyperNetX.git cd HyperNetX make venv source venv-hnx/bin/
-activate pip install . ``` Development =========== Install an editable version
---------------------------- ``` pip install -e . ``` Install an editable
-version with supported applications -------------------------------------------
------------- ```shell pip install -e .['all'] # for zsh users pip install -e .'
-[all]' ``` Install support for testing ----------------------------- > â¹ï¸
-**NOTE:** This project has a pytest configuration file named 'pytest.ini'. By
-default, pytest will use those configuration settings to run tests. ```shell
-make test-deps # run tests python -m pytest # run tests and show coverage
+//github.com/pnnl/HyperNetX.git cd HyperNetX # Create a virtual environment
+make venv source venv-hnx/bin/activate # install required dependencies make
+install ``` Development =========== Install an editable version ``` pip install
+-e . ``` Install additional dependencies to support testing and jupyter
+notebooks: ``` pip install -r requirements.txt ``` You can also install all
+these requirements in one Make target: ``` make install ``` Poetry ====== This
+library uses [Poetry](https://python-poetry.org/docs/) to manage dependencies
+and packaging. Poetry can also be used to manage your environment for
+development. Prerequisites ------------- * [Install Poetry](https://python-
+poetry.org/docs/#installation) Configure Poetry ---------------- [Configure
+your Poetry](https://python-poetry.org/docs/configuration/) to create the
+virtual environment in your project directory: ``` poetry config
+virtualenvs.in-project true # check the poetry configuration poetry config --
+list ``` Set up virtual environment ---------------------------- Create and
+activate a virtual environment. ``` poetry shell ``` NOTE: If you plan to use
+Poetry to manage your virtual environment, you can activate the virtual
+environment using poerty: `poetry shell`. Another option is to directly Install
+required dependencies and HyperNetX in editable mode. ``` poetry install ```
+Install support for testing ----------------------------- > â¹ï¸ **NOTE:**
+This project has a pytest configuration file named 'pytest.ini'. By default,
+pytest will use those configuration settings to run tests. ```shell poetry
+install --with test # run tests python -m pytest # run tests and show coverage
 report python -m pytest --cov=hypernetx # Generate an HTML code coverage report
 and view it on a browser coverage html open htmlcov/index.html ``` Install
-support for tutorials ----------------------------- ``` shell make tutorial-
-deps # open Jupyter notebooks in a browser make tutorials ``` Code Quality ----
--------- HyperNetX uses a number of tools to maintain code quality: * Pylint *
-Black Before using these tools, ensure that you install Pylint in your
-environment: ```shell make lint-deps ``` ### Pylint [Pylint](https://
+support for tutorials ----------------------------- ``` poetry install --with
+tutorials # open Jupyter notebooks in a browser make tutorials ``` Code Quality
+------------ HyperNetX uses a number of tools to maintain code quality: *
+Pylint * Black Before using these tools, ensure that you install Pylint in your
+environment: ``` poetry install --with lint ``` Pylint ------ [Pylint](https://
 pylint.pycqa.org/en/latest/index.html) is a static code analyzer for Python-
 based projects. From the [Pylint docs](https://pylint.pycqa.org/en/latest/
 index.html#what-is-pylint): > Pylint analyses your code without actually
 running it. It checks for errors, enforces a coding standard, looks for code
 smells, and can make suggestions about how the code could be refactored. Pylint
 can infer actual values from your code using its internal code representation
 (astroid). If your code is import logging as argparse, Pylint will know that
 argparse.error(...) is in fact a logging call and not an argparse call. To run
 Pylint and view the results of Pylint, run the following command: ```shell
 pylint hypernetx ``` You can also run Pylint on the command line to generate a
 report on the quality of the codebase and save it to a file named "pylint-
 results.txt": ```shell pylint hypernetx --output=pylint-results.txt ``` For
 more information on configuration, see https://pylint.pycqa.org/en/latest/
-user_guide/configuration/index.html ### Black [Black](https://
+user_guide/configuration/index.html Black ----- [Black](https://
 black.readthedocs.io/en/stable/) is a PEP 8 compliant formatter for Python-
 based project. This tool is highly opinionated about how Python should be
-formatted and will automagically reformat your code. ```shell make format-deps
-black hypernetx ``` Documentation =============== Build and view documentation
-locally --------------------------- ``` make docs-deps cd docs make html open
-docs/build/html/index.html ``` Editing documentation ---------------------
-- When editing documentation, you can auto-rebuild the documentation locally so
-that you can view your document changes live on the browser without having to
-rebuild every time you have a change. ``` make docs-deps cd docs make livehtml
-``` This make script will run in the foreground on your terminal. You should
-see the following: ```shell The HTML pages are in docs/html. [I 230324 09:50:48
-server:335] Serving on http://127.0.0.1:8000 [I 230324 09:50:48 handlers:62]
-Start watching changes [I 230324 09:50:48 handlers:64] Start detecting changes
-[I 230324 09:50:54 handlers:135] Browser Connected: http://127.0.0.1:8000/
+formatted and will automagically reformat your code. ```shell black hypernetx
+``` Documentation ------------- Build and view documentation locally: ```
+poetry install --with docs cd docs make html open docs/build/html/index.html
+``` When editing documentation, you can auto-rebuild the documentation locally
+so that you can view your document changes live on the browser without having
+to rebuild every time you have a change. ``` cd docs make livehtml ``` This
+make script will run in the foreground on your terminal. You should see the
+following: ```shell The HTML pages are in docs/html. [I 230324 09:50:48 server:
+335] Serving on http://127.0.0.1:8000 [I 230324 09:50:48 handlers:62] Start
+watching changes [I 230324 09:50:48 handlers:64] Start detecting changes [I
+230324 09:50:54 handlers:135] Browser Connected: http://127.0.0.1:8000/
 install.html [I 230324 09:51:02 handlers:135] Browser Connected: http://
 127.0.0.1:8000/ ``` Click on `http://127.0.0.1:8000/install.html` to open the
 docs on your browser. Since this will auto-rebuild, every time you change a
 document file, it will automatically render on your browser, allowing you to
 verify your document changes. Continuous Integration ======================
 This project runs Continuous Integration (CI) using GitHub Actions. Normally,
 CI runs on pull requests, pushes to certain branches, and other events.
 Maintainers of the GitHub repository can manually trigger CI using [GitHub CLI]
 (https://cli.github.com/). See instructions below on how to manually trigger CI
 on GitHub Actions: ```commandline # login to Github gh auth login --with-token
 < ~/.ssh/tokens/ # Trigger CI gh workflow run ci.yml --repo pnnl/HyperNetX --
 ref --field triggeredBy="" # Get the status of the workflow gh run list --
-workflow=ci.yml --repo pnnl/HyperNetX ``` Versioning ---------- This project
+workflow=ci.yml --repo pnnl/HyperNetX ``` Versioning ========== This project
 uses [`commitizen`](https://github.com/commitizen-tools/commitizen) to manage
 versioning. The files where "version" will be updated are listed in the
 '.cz.toml' file. To create a new version and the associated tag, run the
-following commands: ```shell # Install commitizen tool to environment make
-version-deps # Updates version; values for '--increment' can be MAJOR, MINOR,
-or PATCH # Autocreates a tag and commit for the updated version cz bump --
-increment MAJOR --dry-run cz bump --increment MAJOR ``` Notice ====== This
+following commands: ```shell # Install commitizen tool to environment pip
+install commitizen # Updates version; values for '--increment' can be MAJOR,
+MINOR, or PATCH # Autocreates a tag and commit for the updated version cz bump
+--increment MAJOR --dry-run cz bump --increment MAJOR ``` Notice ====== This
 material was prepared as an account of work sponsored by an agency of the
 United States Government. Neither the United States Government nor the United
 States Department of Energy, nor Battelle, nor any of their employees, nor any
 jurisdiction or organization that has cooperated in the development of these
 materials, makes any warranty, express or implied, or assumes any legal
 liability or responsibility for the accuracy, completeness, or usefulness or
 any information, apparatus, product, software, or process disclosed, or
```

### Comparing `hypernetx-2.2.0/hypernetx/algorithms/__init__.py` & `hypernetx-2.3.0/hypernetx/algorithms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     "get_pi",
     "norm_lap",
     "spec_clus",
     # generative_models API's
     "erdos_renyi_hypergraph",
     "chung_lu_hypergraph",
     "dcsbm_hypergraph",
-    # s_centreality_measures API's
+    # s_centrality_measures API's
     "s_betweenness_centrality",
     "s_harmonic_closeness_centrality",
     "s_harmonic_centrality",
     "s_closeness_centrality",
     "s_eccentricity",
     # hypergraph_modularity API's
     "dict2part",
```

### Comparing `hypernetx-2.2.0/hypernetx/algorithms/contagion.py` & `hypernetx-2.3.0/hypernetx/algorithms/contagion.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     """
 
     try:
         from celluloid import Camera
     except ModuleNotFoundError as e:
         raise Exception(
             f"If you need to use {__name__}, please install additional packages by running the "
-            f"following command: pip install .['all']"
+            f"following command: pip install celluloid"
         ) from e
 
     nodeState = defaultdict(lambda: "S")
 
     camera = Camera(fig)
 
     for t in sorted(list(transition_events.keys())):
@@ -304,14 +304,15 @@
         return True
     else:
         return random.choice([False, True])
 
 
 # Auxiliary functions
 
+
 # The ListDict class is copied from Joel Miller's Github repository Mathematics-of-Epidemics-on-Networks
 class _ListDict_(object):
     r"""
     The Gillespie algorithm will involve a step that samples a random element
     from a set based on its weight.  This is awkward in Python.
 
     So I'm introducing a new class based on a stack overflow answer by
@@ -533,15 +534,15 @@
     if rho is not None and initial_infecteds is not None:
         raise Exception("Cannot define both initial_infecteds and rho")
 
     if initial_infecteds is None:
         if rho is None:
             initial_number = 1
         else:
-            initial_number = int(round(H.number_of_nodes() * rho))
+            initial_number = int(round(len(H.nodes) * rho))
         initial_infecteds = random.sample(list(H.nodes), initial_number)
     else:
         # check to make sure that the initially infected nodes are in the hypergraph
         initial_infecteds = list(set(H.nodes).intersection(set(initial_infecteds)))
 
     if initial_recovereds is None:
         initial_recovereds = []
@@ -563,21 +564,21 @@
     for node in initial_recovereds:
         status[node] = "R"
         if return_full_data:
             transition_events[tmin].append(("R", node))
 
     I = [len(initial_infecteds)]
     R = [len(initial_recovereds)]
-    S = [H.number_of_nodes() - I[-1] - R[-1]]
+    S = [len(H.nodes) - I[-1] - R[-1]]
 
     t = tmin
     times = [t]
     newStatus = status.copy()
 
-    edge_neighbors = lambda node: H.edges.memberships[node]
+    edge_neighbors = lambda node: H.nodes.memberships[node]
 
     while t < tmax and I[-1] != 0:
         # Initialize the next step with the same numbers of S, I, and R as the last step before computing the changes
         S.append(S[-1])
         I.append(I[-1])
         R.append(R[-1])
 
@@ -695,15 +696,15 @@
     if rho is not None and initial_infecteds is not None:
         raise Exception("Cannot define both initial_infecteds and rho")
 
     if initial_infecteds is None:
         if rho is None:
             initial_number = 1
         else:
-            initial_number = int(round(H.number_of_nodes() * rho))
+            initial_number = int(round(len(H.nodes) * rho))
         initial_infecteds = random.sample(list(H.nodes), initial_number)
     else:
         # check to make sure that the initially infected nodes are in the hypergraph
         initial_infecteds = list(set(H.nodes).intersection(set(initial_infecteds)))
 
     status = defaultdict(lambda: "S")
 
@@ -713,21 +714,21 @@
 
     for node in initial_infecteds:
         status[node] = "I"
         if return_full_data:
             transition_events[tmin].append(("I", node, None))
 
     I = [len(initial_infecteds)]
-    S = [H.number_of_nodes() - I[-1]]
+    S = [len(H.nodes) - I[-1]]
 
     t = tmin
     times = [t]
     newStatus = status.copy()
 
-    edge_neighbors = lambda node: H.edges.memberships[node]
+    edge_neighbors = lambda node: H.nodes.memberships[node]
 
     while t < tmax and I[-1] != 0:
         # Initialize the next step with the same numbers of S, I, and R as the last step before computing the changes
         S.append(S[-1])
         I.append(I[-1])
         if return_full_data:
             transition_events[t + dt] = list()
@@ -839,15 +840,15 @@
     if rho is not None and initial_infecteds is not None:
         raise Exception("Cannot define both initial_infecteds and rho")
 
     if initial_infecteds is None:
         if rho is None:
             initial_number = 1
         else:
-            initial_number = int(round(H.number_of_nodes() * rho))
+            initial_number = int(round(len(H.nodes) * rho))
         initial_infecteds = random.sample(list(H.nodes), initial_number)
     else:
         # check to make sure that the initially infected nodes are in the hypergraph
         initial_infecteds = list(set(H.nodes).intersection(set(initial_infecteds)))
 
     if initial_recovereds is None:
         initial_recovereds = []
@@ -863,17 +864,17 @@
         status[node] = "I"
 
     for node in initial_recovereds:
         status[node] = "R"
 
     I = [len(initial_infecteds)]
     R = [len(initial_recovereds)]
-    S = [H.number_of_nodes() - I[-1] - R[-1]]
+    S = [len(H.nodes) - I[-1] - R[-1]]
 
-    edge_neighbors = lambda node: H.edges.memberships[node]
+    edge_neighbors = lambda node: H.nodes.memberships[node]
 
     t = tmin
     times = [t]
 
     infecteds = _ListDict_()
 
     infectious_edges = dict()
@@ -1038,31 +1039,31 @@
     if rho is not None and initial_infecteds is not None:
         raise Exception("Cannot define both initial_infecteds and rho")
 
     if initial_infecteds is None:
         if rho is None:
             initial_number = 1
         else:
-            initial_number = int(round(H.number_of_nodes() * rho))
+            initial_number = int(round(len(H.nodes) * rho))
         initial_infecteds = random.sample(list(H.nodes), initial_number)
     else:
         # check to make sure that the initially infected nodes are in the hypergraph
         initial_infecteds = list(set(H.nodes).intersection(set(initial_infecteds)))
 
     status = defaultdict(lambda: "S")
 
     size_dist = np.unique(H.edge_size_dist())
 
     for node in initial_infecteds:
         status[node] = "I"
 
     I = [len(initial_infecteds)]
-    S = [H.number_of_nodes() - I[-1]]
+    S = [len(H.nodes) - I[-1]]
 
-    edge_neighbors = lambda node: H.edges.memberships[node]
+    edge_neighbors = lambda node: H.nodes.memberships[node]
 
     t = tmin
     times = [t]
 
     infecteds = _ListDict_()
 
     infectious_edges = dict()
```

### Comparing `hypernetx-2.2.0/hypernetx/algorithms/generative_models.py` & `hypernetx-2.3.0/hypernetx/algorithms/generative_models.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.2.0/hypernetx/algorithms/homology_mod2.py` & `hypernetx-2.3.0/hypernetx/algorithms/homology_mod2.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.2.0/hypernetx/algorithms/hypergraph_modularity.py` & `hypernetx-2.3.0/hypernetx/algorithms/hypergraph_modularity.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 # wcd: weight function (ex: strict, majority, linear)
 def modularity(HG, A, wdc=linear):
     """
     Computes modularity of hypergraph HG with respect to partition A.
 
     Parameters
     ----------
-    HG : Hypergraph
+    HG : hnx.Hypergraph
         The hypergraph with some precomputed attributes via: precompute_attributes(HG)
     A : list of sets
         Partition of the vertices in HG
     wdc : func, optional
         Hyperparameter for hypergraph modularity [2]_
 
     Note
@@ -175,15 +175,15 @@
 
     ## all same weight
     if uniq:
         _ctr = Counter([(Counter(l).most_common(1)[0][1], len(l)) for l in L])
         EC = sum([wdc(k[1], k[0]) * _ctr[k] for k in _ctr.keys() if k[0] > k[1] / 2])
     else:
         _keys = [(Counter(l).most_common(1)[0][1], len(l)) for l in L]
-        _vals = list(HG.edge_props["weight"])  ## Thanks Brenda!!
+        _vals = list(HG.edges.dataframe["weight"])
         _df = pd.DataFrame(zip(_keys, _vals), columns=["key", "val"])
         _df = _df.groupby(by="key").sum()
         EC = sum(
             [wdc(k[1], k[0]) * v[0] for (k, v) in _df.iterrows() if k[0] > k[1] / 2]
         )
 
     ## Degree Tax
@@ -210,15 +210,15 @@
 
     if uniq:
         for d in Ctr.keys():
             Cnt = Ctr[d]
             for c in np.arange(int(np.floor(d / 2 + 1)), d + 1):
                 for Vol in VolA:
                     DT += Cnt * wdc(d, c) * binom.pmf(c, d, Vol)
-        return (EC - DT) / HG.number_of_edges()
+        return (EC - DT) / len(HG.edges)
     else:
         for d in range(len(Ctr)):
             Cnt = Ctr[d]
             for c in np.arange(int(np.floor(d / 2 + 1)), d + 1):
                 for Vol in VolA:
                     DT += Cnt * wdc(d, c) * binom.pmf(c, d, Vol)
         return (EC - DT) / S
@@ -226,15 +226,15 @@
 
 def conductance(H, A):
     """
     Computes conductance [4] of hypergraph HG with respect to partition A.
 
     Parameters
     ----------
-    H : Hypergraph
+    H : hnx.Hypergraph
         The hypergraph
     A : set
         Partition of the vertices in H
 
     Returns
     -------
     : float
@@ -261,15 +261,15 @@
 def two_section(HG):
     """
     Creates a random walk based [1]_ 2-section igraph Graph with transition weights defined by the
     weights of the hyperedges.
 
     Parameters
     ----------
-    HG : Hypergraph
+    HG : hnx.Hypergraph
 
     Returns
     -------
      : igraph.Graph
        The 2-section graph built from HG
     """
 
@@ -300,15 +300,15 @@
 
 def kumar(HG, delta=0.01, verbose=False):
     """
     Compute a partition of the vertices in hypergraph HG as per Kumar's algorithm [1]_
 
     Parameters
     ----------
-    HG : Hypergraph
+    HG : hnx.Hypergraph
 
     delta : float, optional
         convergence stopping criterion
 
     Returns
     -------
     : list of sets
@@ -334,15 +334,15 @@
         # re-weight
         diff = 0
         for e in HG.edges:
             edge = HG.edges[e]
             reweight = (
                 sum([1 / (1 + HG.size(e, c)) for c in CH])
                 * (HG.size(e) + len(CH))
-                / HG.number_of_edges()
+                / len(HG.edges)
             )
             diff = max(diff, 0.5 * abs(edge.weight - reweight))
             edge.weight = 0.5 * edge.weight + 0.5 * reweight
         if verbose:
             print("pass completed, max edge weight difference:", diff)
 
         # re-run louvain
@@ -393,15 +393,15 @@
         for v in list(np.random.permutation(list(H.nodes))):
             dct_A_v = dct_A[v]
             H_id = [H.incidence_dict[x] for x in H.nodes[v].memberships]
             L = [[dct_A[i] for i in x] for x in H_id]
 
             ## ec portion before move
             _keys = [(Counter(l).most_common(1)[0][1], len(l)) for l in L]
-            _vals = [H.edge_props["weight"][x] for x in H.nodes[v].memberships]
+            _vals = [H.edges[x].weight for x in H.nodes[v].memberships]
             _df = pd.DataFrame(zip(_keys, _vals), columns=["key", "val"])
             _df = _df.groupby(by="key").sum()
             ec = sum(
                 [
                     wdc(k[1], k[0]) * val[0]
                     for (k, val) in _df.iterrows()
                     if k[0] > k[1] / 2
@@ -421,15 +421,15 @@
             best_del_q = 0
             best_dt = 0
             for m in set([i for x in L for i in x]) - {dct_A_v}:
                 dct_A[v] = m
                 L = [[dct_A[i] for i in x] for x in H_id]
                 ## EC
                 _keys = [(Counter(l).most_common(1)[0][1], len(l)) for l in L]
-                _vals = [H.edge_props["weight"][x] for x in H.nodes[v].memberships]
+                _vals = [H.edges[x].weight for x in H.nodes[v].memberships]
                 _df = pd.DataFrame(zip(_keys, _vals), columns=["key", "val"])
                 _df = _df.groupby(by="key").sum()
                 ecp = sum(
                     [
                         wdc(k[1], k[0]) * val[0]
                         for (k, val) in _df.iterrows()
                         if k[0] > k[1] / 2
@@ -565,17 +565,17 @@
     ----
     This is a very simple algorithm that tries moving nodes between communities to improve hypergraph modularity.
     It requires an initial non-trivial partition which can be obtained for example via graph clustering on the 2-section of HG,
     or via Kumar's algorithm.
 
     Parameters
     ----------
-    HG : Hypergraph
+    HG : hnx.Hypergraph
 
-    L : list of sets
+    A : list of sets
       some initial partition of the vertices in HG
 
     wdc : func, optional
         Hyperparameter for hypergraph modularity [2]_
 
     delta : float, optional
             convergence stopping criterion
```

### Comparing `hypernetx-2.2.0/hypernetx/algorithms/laplacians_clustering.py` & `hypernetx-2.3.0/hypernetx/algorithms/laplacians_clustering.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.2.0/hypernetx/algorithms/s_centrality_measures.py` & `hypernetx-2.3.0/hypernetx/algorithms/s_centrality_measures.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,28 +147,25 @@
 def s_closeness_centrality(H, s=1, edges=True, return_singletons=True, source=None):
     r"""
     In a connected component the reciprocal of the sum of the distance between an
     edge(node) and all other edges(nodes) in the component times the number of edges(nodes)
     in the component minus 1.
 
     $V$ = the set of vertices in the linegraph.
-    $n = |V|$
+    $n = \|V\|$
     $d$ = shortest path distance
 
     .. math::
 
         C(u) = \frac{n - 1}{\sum_{v \neq u \in V} d(v, u)}
 
-
     Parameters
     ----------
     H : hnx.Hypergraph
-
     s : int, optional
-
     edges : bool, optional
         Indicates if method should compute edge linegraph (default) or node linegraph.
     return_singletons : bool, optional
         Indicates if method should return values for singleton components.
     source : str, optional
         Identifier of node or edge of interest for computing centrality
 
@@ -239,15 +236,14 @@
 
     Returns
     -------
     dict or float
         returns the s-harmonic closeness centrality value of the edges, a number between 0 and 1 inclusive.
         If source=None a dictionary of values for each s-edge in H is returned.
         If source then a single value is returned.
-
     """
 
     # func = partial(nx.harmonic_centrality)
     # result = _s_centrality(
     #     func,
     #     H,
     #     s=s,
```

### Comparing `hypernetx-2.2.0/hypernetx/classes/hypergraph.py` & `hypernetx-2.3.0/hypernetx/classes/hypergraph.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,183 +1,195 @@
 # Copyright © 2018 Battelle Memorial Institute
 # All rights reserved.
 from __future__ import annotations
 
 import warnings
-
-warnings.filterwarnings("default", category=DeprecationWarning)
-
-from copy import deepcopy
 from collections import defaultdict
-from collections.abc import Sequence, Iterable
-from typing import Optional, Any, TypeVar, Union, Mapping, Hashable
+from typing import TypeVar, Union
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 from networkx.algorithms import bipartite
 from scipy.sparse import coo_matrix, csr_matrix
 
-from hypernetx.classes import EntitySet
 from hypernetx.exception import HyperNetXError
-from hypernetx.utils.decorators import warn_nwhy
-from hypernetx.classes.helpers import merge_nested_dicts, dict_depth
+from hypernetx.classes.factory import (
+    dataframe_factory_method,
+    dict_factory_method,
+    list_factory_method,
+    ndarray_factory_method,
+)
+from hypernetx.classes.incidence_store import IncidenceStore
+from hypernetx.classes.property_store import PropertyStore
+from hypernetx.classes.hyp_view import HypergraphView
+
+warnings.filterwarnings("default", category=DeprecationWarning)
 
 __all__ = ["Hypergraph"]
 
 T = TypeVar("T", bound=Union[str, int])
 
 
 class Hypergraph:
     """
     Parameters
     ----------
 
-    setsystem : (optional) dict of iterables, dict of dicts,iterable of iterables,
-        pandas.DataFrame, numpy.ndarray, default = None
-        See SetSystem above for additional setsystem requirements.
-
-    edge_col : (optional) str | int, default = 0
-        column index (or name) in pandas.dataframe or numpy.ndarray,
-        used for (hyper)edge ids. Will be used to reference edgeids for
-        all set systems.
-
-    node_col : (optional) str | int, default = 1
-        column index (or name) in pandas.dataframe or numpy.ndarray,
-        used for node ids. Will be used to reference nodeids for all set systems.
-
-    cell_weight_col : (optional) str | int, default = None
-        column index (or name) in pandas.dataframe or numpy.ndarray used for
-        referencing cell weights. For a dict of dicts references key in cell
-        property dicts.
-
-    cell_weights : (optional) Sequence[float,int] | int |  float , default = 1.0
-        User specified cell_weights or default cell weight.
-        Sequential values are only used if setsystem is a
-        dataframe or ndarray in which case the sequence must
-        have the same length and order as these objects.
-        Sequential values are ignored for dataframes if cell_weight_col is already
-        a column in the data frame.
-        If cell_weights is assigned a single value
-        then it will be used as default for missing values or when no cell_weight_col
-        is given.
-
-    cell_properties : (optional) Sequence[int | str] | Mapping[T,Mapping[T,Mapping[str,Any]]],
-        default = None
-        Column names from pd.DataFrame to use as cell properties
-        or a dict assigning cell_property to incidence pairs of edges and
-        nodes. Will generate a misc_cell_properties, which may have variable lengths per cell.
-
-    misc_cell_properties : (optional) str | int, default = None
-        Column name of dataframe corresponding to a column of variable
-        length property dictionaries for the cell. Ignored for other setsystem
-        types.
-
-    aggregateby : (optional) str, dict, default = 'first'
-        By default duplicate edge,node incidences will be dropped unless
-        specified with `aggregateby`.
-        See pandas.DataFrame.agg() methods for additional syntax and usage
-        information.
+    setsystem : pandas.DataFrame, dict of iterables, dict of dicts, list of iterables, numpy.ndarray, optional, default=None
+        See SetSystem below for additional setsystem requirements.
+
+    edge_col : str | int, optional, default=0
+        column index (or name) in pandas.DataFrame,
+        used for (hyper)edge ids. Only used when setsystem is a
+        pandas.DataFrame
+
+    node_col : str | int, optional, default=1
+        column index (or name) in pandas.dataframe,
+        used for node ids. Only used when setsystem is a
+        pandas.DataFrame
+
+    cell_weight_col : str | int, optional, default="weight"
+        column index (or name) in pandas.DataFrame used for
+        referencing cell weights. For a dict of dicts, it will be
+        used as a key in the nested dictionary of properties.
+        These are the same as edge dependent node weights and
+        will populate the incidence matrix when `weights=True`.
+
+    default_cell_weight : int | float, optional, default=1
+        All incidence pairs in the Hypergraph are assigned a
+        default weight if weight is not specified in the setsystem.
+
+    misc_cell_properties_col : str | int, optional, default=None
+        Used for Pandas Dataframe with one column containing dictionaries of
+        properties. Useful if objects have diverse property sets.
+        Ignored for other setsystem types.
+
+    properties : pd.DataFrame | dict, optional, default=None
+        Concatenation/union of edge_properties and node_properties.
+        By default, the object id is used and should be the first column of the dataframe, or key in the dict.
+        If there are nodes and edges with the same ids but distinct properties then separate them and use the
+        edge_properties and node_properties keywords.
+
+    weight_prop_col : str, optional, default=None
+        Name of property in properties to use for weight
 
-    edge_properties : (optional) pd.DataFrame | dict, default = None
+    default_weight : int | float, optional, default=1
+        Used when weight property is missing or undefined
+
+    edge_properties : pd.DataFrame | dict, optional, default=None
         Properties associated with edge ids.
+        If a dataframe, the first column must be the names of the edges.
         First column of dataframe or keys of dict link to edge ids in
         setsystem.
 
-    node_properties : (optional) pd.DataFrame | dict, default = None
-        Properties associated with node ids.
-        First column of dataframe or keys of dict link to node ids in
-        setsystem.
-
-    properties : (optional) pd.DataFrame | dict, default = None
-        Concatenation/union of edge_properties and node_properties.
-        By default, the object id is used and should be the first column of
-        the dataframe, or key in the dict. If there are nodes and edges
-        with the same ids and different properties then use the edge_properties
-        and node_properties keywords.
-
-    misc_properties : (optional) int | str, default = None
-        Column of property dataframes with dtype=dict. Intended for variable
-        length property dictionaries for the objects.
-
-    edge_weight_prop : (optional) str, default = None,
+    edge_weight_prop_col : str, optional, default=None
         Name of property in edge_properties to use for weight.
 
-    node_weight_prop : (optional) str, default = None,
-        Name of property in node_properties to use for weight.
+    default_edge_weight : int | float, optional, default=1
+        Used when edge weight property is missing or undefined.
 
-    weight_prop : (optional) str, default = None
-        Name of property in properties to use for 'weight'
+    node_properties : pd.DataFrame | dict, optional, default=None
+        Properties associated with node ids. If a dataframe, the first column must be the names of the nodes.
+        First column of dataframe or keys of dict link to nodes ids in setsystem.
 
-    default_edge_weight : (optional) int | float, default = 1
-        Used when edge weight property is missing or undefined.
+    node_weight_prop_col : str, optional, default=None
+        Name of property in node_properties to use for weight.
 
-    default_node_weight : (optional) int | float, default = 1
+    default_node_weight : int | float, optional, default=1
         Used when node weight property is missing or undefined
 
-    name : (optional) str, default = None
+    misc_properties_col : str | int, optional, default=None
+        Used for properties, edge_properties, and node_properties
+        Pandas Dataframes with one column containing dictionaries of
+        properties. Useful if objects have diverse property sets.
+        Ignored for other setsystem types.
+
+    name : str, optional, default=None
         Name assigned to hypergraph
 
 
     ======================
-    Hypergraphs in HNX 2.0
+    Hypergraphs in HNX 2.3
     ======================
 
     An hnx.Hypergraph H = (V,E) references a pair of disjoint sets:
     V = nodes (vertices) and E = (hyper)edges.
 
     HNX allows for multi-edges by distinguishing edges by
-    their identifiers instead of their contents. For example, if
+    their unique identifiers instead of their contents. For example, if
     V = {1,2,3} and E = {e1,e2,e3},
     where e1 = {1,2}, e2 = {1,2}, and e3 = {1,2,3},
     the edges e1 and e2 contain the same set of nodes and yet
     are distinct and are distinguishable within H = (V,E).
 
-    New as of version 2.0, HNX provides methods to easily store and
+    New as of version 2.3, HNX provides methods to easily store and
     access additional metadata such as cell, edge, and node weights.
-    Metadata associated with (edge,node) incidences
-    are referenced as **cell_properties**.
-    Metadata associated with a single edge or node is referenced
-    as its **properties**.
+    Metadata associated with all edges, nodes, and (edge,node) incidence
+    pairs stored in the hypergraph are viewable using: ::
+
+        >>> H.edges.to_dataframe
+        >>> H.nodes.to_dataframe
+        >>> H.incidences.to_dataframe
 
     The fundamental object needed to create a hypergraph is a **setsystem**. The
     setsystem defines the many-to-many relationships between edges and nodes in
-    the hypergraph. Cell properties for the incidence pairs can be defined within
-    the setsystem or in a separate pandas.Dataframe or dict.
-    Edge and node properties are defined with a pandas.DataFrame or dict.
+    the hypergraph. Properties for the incidence pairs are defined within
+    the setsystem. Properties for the edges and nodes are defined with separate
+    Pandas DataFrames or dictionaries.
+
+    A hypergraph is defined by its relationships. While the
+    nodes and edges are distinct objects with their own properties, it is only
+    when they are in a relationship (i.e. incidence pair) that nodes and egdges are viewable
+    within the hypergraph structure. Consequently, hypergraph metrics and combinatorics do not
+    use "isolated" nodes or "empty" edges. For example, while `node_properties` could
+    contain any number of node identifiers, only nodes belonging to an edge
+    in the hypergraph are counted when computing the size and shape of the
+    hypergraph.
 
     SetSystems
     ----------
     There are five types of setsystems currently accepted by the library.
 
-    1.  **iterable of iterables** : Barebones hypergraph uses Pandas default
+    1.  **iterable of iterables** : Barebones hypergraph, which uses Pandas default
         indexing to generate hyperedge ids. Elements must be hashable.: ::
 
-        >>> H = Hypergraph([{1,2},{1,2},{1,2,3}])
+        >>> list_of_lists = [['book','candle','cat'],['book','coffee cup'],['coffee cup','radio']]
+        >>> H = Hypergraph(list_of_lists)
 
-    2.  **dictionary of iterables** : the most basic way to express many-to-many
+    2.  **dictionary of iterables** : The most basic way to express many-to-many
         relationships providing edge ids. The elements of the iterables must be
         hashable): ::
 
-        >>> H = Hypergraph({'e1':[1,2],'e2':[1,2],'e3':[1,2,3]})
+        >>> scenes_dictionary = {
+        >>> 	0: ('FN', 'TH'),
+        >>> 	1: ('TH', 'JV'),
+        >>> 	2: ('BM', 'FN', 'JA'),
+        >>> 	3: ('JV', 'JU', 'CH', 'BM'),
+        >>> 	4: ('JU', 'CH', 'BR', 'CN', 'CC', 'JV', 'BM'),
+        >>> 	5: ('TH', 'GP'),
+        >>> 	6: ('GP', 'MP'),
+        >>> 	7: ('MA', 'GP'),
+        >>> 	8: ('FN', 'TH')}
+        >>> H = hnx.Hypergraph(scenes_dictionary)
 
     3.  **dictionary of dictionaries**  : allows cell properties to be assigned
         to a specific (edge, node) incidence. This is particularly useful when
         there are variable length dictionaries assigned to each pair: ::
 
-        >>> d = {'e1':{ 1: {'w':0.5, 'name': 'related_to'},
-        >>>             2: {'w':0.1, 'name': 'related_to',
-        >>>                 'startdate': '05.13.2020'}},
-        >>>      'e2':{ 1: {'w':0.52, 'name': 'owned_by'},
-        >>>             2: {'w':0.2}},
-        >>>      'e3':{ 1: {'w':0.5, 'name': 'related_to'},
-        >>>             2: {'w':0.2, 'name': 'owner_of'},
-        >>>             3: {'w':1, 'type': 'relationship'}}
-
-        >>> H = Hypergraph(d, cell_weight_col='w')
+        >>> nested_dictionary =  {
+        >>> 	0: {'FN':{'time':'early', 'weight': 7}, 'TH':{'time':'late'}},
+        >>> 	1: {'TH':{'subject':'war'}, 'JV':{'observed_by':'someone'}},
+        >>> 	2: {'BM':{}, 'FN':{}, 'JA':{'role':'policeman'}},
+        >>> 	3: {'JV':{'was_carrying':'stick'}, 'JU':{}, 'CH':{}, 'BM':{'state':'intoxicated', 'color':'pinkish'}},
+        >>> 	4: {'JU':{'weight':15}, 'CH':{}, 'BR':{'state':'worried'}, 'CN':{}, 'CC':{}, 'JV':{}, 'BM':{}},
+        >>> 	5: {'TH':{}, 'GP':{}},
+        >>> 	6: {'GP':{}, 'MP':{}},
+        >>> 	7: {'MA':{}, 'GP':{'accompanied_by':'dog', 'weight':15, 'was_singing': 'Frère Jacques'}}}
+        >>> H = hnx.Hypergraph(nested_dictionary)
 
     4.  **pandas.DataFrame** For large datasets and for datasets with cell
         properties it is most efficient to construct a hypergraph directly from
         a pandas.DataFrame. Incidence pairs are in the first two columns.
         Cell properties shared by all incidence pairs can be placed in their own
         column of the dataframe. Variable length dictionaries of cell properties
         particular to only some of the incidence pairs may be placed in a single
@@ -189,504 +201,362 @@
         |   e1      |   1       |   0.5     | {'name':'related_to'}             |
         +-----------+-----------+-----------+-----------------------------------+
         |   e1      |   2       |   0.1     | {"name":"related_to",             |
         |           |           |           |  "startdate":"05.13.2020"}        |
         +-----------+-----------+-----------+-----------------------------------+
         |   e2      |   1       |   0.52    | {"name":"owned_by"}               |
         +-----------+-----------+-----------+-----------------------------------+
-        |   e2      |   2       |   0.2     |                                   |
-        +-----------+-----------+-----------+-----------------------------------+
-        |   ...     |   ...     |   ...     | {...}                             |
-        +-----------+-----------+-----------+-----------------------------------+
 
         The first row of the dataframe is used to reference each column. ::
 
-        >>> H = Hypergraph(df,edge_col="col1",node_col="col2",
-        >>>                 cell_weight_col="w",misc_cell_properties="col3")
-
-    5.  **numpy.ndarray** For homogeneous datasets given in an ndarray a
-        pandas dataframe is generated and column names are added from the
-        edge_col and node_col arguments. Cell properties containing multiple data
-        types are added with a separate dataframe or dict and passed through the
-        cell_properties keyword. ::
-
-        >>> arr = np.array([['e1','1'],['e1','2'],
-        >>>                 ['e2','1'],['e2','2'],
-        >>>                 ['e3','1'],['e3','2'],['e3','3']])
-        >>> H = hnx.Hypergraph(arr, column_names=['col1','col2'])
-
+        >>> import pandas as pd
+        >>> d = {'col1': ['e1', 'e1', 'e2'],
+        >>>      'col2': [1, 2, 1],
+        >>>      'w': [0.5, 0.1, 0.52],
+        >>>      'col3':[{'name': 'related_to'}, {'name': 'related_to', 'startdate':'05.13.2020'}, {'name': 'owned_by'}]}
+        >>> df = pd.DataFrame(d)
+        >>> H = hnx.Hypergraph(df, edge_col="col1", node_col="col2",
+        >>>                    cell_weight_col="w", misc_cell_properties_col="col3")
+
+    5.  **numpy.ndarray** For homogeneous datasets given in a *n x 2* ndarray a
+        pandas dataframe is generated. In this case, the constructor will
+        only accept properties for the edges and nodes using the
+        edge and node uids listed in the array, although incidence properties can
+        be added after construction::
+
+        >>> import numpy as np
+        >>> np_array = np.array([['A','a'],['A','b'],['A','c'],['B','a'],['B','d'],['C','c'],['C','d']])
+        >>> H = hnx.Hypergraph(np_array)
+        >>> H.incidences[('A','a')].color = 'red'
+        >>> H.dataframe
 
     Edge and Node Properties
     ------------------------
     Properties specific to a single edge or node are passed through the
-    keywords: **edge_properties, node_properties, properties**.
-    Properties may be passed as dataframes or dicts.
-    The first column or index of the dataframe or keys of the dict keys
+    keywords: **edge_properties, node_properties, or properties**.
+    Properties may be passed as dataframes or dictionaries.
+    The first column or index of the dataframe or the keys of the dictionary
     correspond to the edge and/or node identifiers.
     If identifiers are shared among edges and nodes, or are distinct
     for edges and nodes, properties may be combined into a single
     object and passed to the **properties** keyword. For example:
 
-    +-----------+-----------+---------------------------------------+
-    |   id      |   weight  |   properties                          |
-    +-----------+-----------+---------------------------------------+
-    |   e1      |   5.0     |   {'type':'event'}                    |
-    +-----------+-----------+---------------------------------------+
-    |   e2      |   0.52    |   {"name":"owned_by"}                 |
-    +-----------+-----------+---------------------------------------+
-    |   ...     |   ...     |   {...}                               |
-    +-----------+-----------+---------------------------------------+
-    |   1       |   1.2     |   {'color':'red'}                     |
-    +-----------+-----------+---------------------------------------+
-    |   2       |   .003    |   {'name':'Fido','color':'brown'}     |
-    +-----------+-----------+---------------------------------------+
-    |   3       |   1.0     |    {}                                 |
-    +-----------+-----------+---------------------------------------+
+        +-----------+-----------+---------------------------------------+
+        |   uid     |   weight  |   properties                          |
+        +-----------+-----------+---------------------------------------+
+        |   e1      |   5.0     |   {'type':'event'}                    |
+        +-----------+-----------+---------------------------------------+
+        |   e2      |   0.52    |   {"name":"owned_by"}                 |
+        +-----------+-----------+---------------------------------------+
+        |   ...     |   ...     |   {...}                               |
+        +-----------+-----------+---------------------------------------+
+        |   1       |   1.2     |   {'color':'red'}                     |
+        +-----------+-----------+---------------------------------------+
+        |   2       |   .003    |   {'name':'Fido','color':'brown'}     |
+        +-----------+-----------+---------------------------------------+
+        |   3       |   1.0     |    {}                                 |
+        +-----------+-----------+---------------------------------------+
 
     A properties dictionary should have the format: ::
 
-        dp = {id1 : {prop1:val1, prop2,val2,...}, id2 : ... }
-
-    A properties dataframe may be used for nodes and edges sharing ids
-    but differing in cell properties by adding a level index using 0
-    for edges and 1 for nodes:
-
-    +-----------+-----------+-----------+---------------------------+
-    |  level    |   id      |   weight  |       properties          |
-    +-----------+-----------+-----------+---------------------------+
-    |   0       |   e1      |   5.0     |   {'type':'event'}        |
-    +-----------+-----------+-----------+---------------------------+
-    |   0       |   e2      |    0.52   |   {"name":"owned_by"}     |
-    +-----------+-----------+-----------+---------------------------+
-    |   ...     |   ...     |    ...    |          {...}            |
-    +-----------+-----------+-----------+---------------------------+
-    |   1       |   1.2     |   {'color':'red'}                     |
-    +-----------+-----------+-----------+---------------------------+
-    |   2       |   .003    |   {'name':'Fido','color':'brown'}     |
-    +-----------+-----------+-----------+---------------------------+
-    |   ...     |   ...     |    ...    |          {...}            |
-    +-----------+-----------+-----------+---------------------------+
-
+        dp = {uid1 : {prop1:val1, prop2:val2, ...},
+              uid2 : {...},
+              ...}
 
 
     Weights
     -------
     The default key for cell and object weights is "weight". The default value
-    is 1. Weights may be assigned and/or a new default prescribed in the
-    constructor using **cell_weight_col** and **cell_weights** for incidence pairs,
-    and using **edge_weight_prop, node_weight_prop, weight_prop,
-    default_edge_weight,** and **default_node_weight** for node and edge weights.
-
+    is 1. Weights may be assigned from a column in the dataframe by specifying the
+    column and/or a new default in the
+    constructor using **cell_weight_col** and **default_cell_weight** for incidence pairs,
+    and using **edge_weight_prop_col, default_edge_weight** for edges,
+    **node_weight_prop_col, default_node_weight** for nodes,
+    and **weight_prop_col, default_weight** for a shared property dataframe.
     """
 
-    @warn_nwhy
     def __init__(
         self,
-        setsystem: Optional[
-            pd.DataFrame
-            | np.ndarray
-            | Mapping[T, Iterable[T]]
-            | Iterable[Iterable[T]]
-            | Mapping[T, Mapping[T, Mapping[str, Any]]]
-        ] = None,
-        edge_col: str | int = 0,
-        node_col: str | int = 1,
-        cell_weight_col: Optional[str | int] = "cell_weights",
-        cell_weights: Sequence[float] | float = 1.0,
-        cell_properties: Optional[
-            Sequence[str | int] | Mapping[T, Mapping[T, Mapping[str, Any]]]
-        ] = None,
-        misc_cell_properties_col: Optional[str | int] = None,
-        aggregateby: str | dict[str, str] = "first",
-        edge_properties: Optional[pd.DataFrame | dict[T, dict[Any, Any]]] = None,
-        node_properties: Optional[pd.DataFrame | dict[T, dict[Any, Any]]] = None,
-        properties: Optional[
-            pd.DataFrame | dict[T, dict[Any, Any]] | dict[T, dict[T, dict[Any, Any]]]
-        ] = None,
-        misc_properties_col: Optional[str | int] = None,
-        edge_weight_prop_col: str | int = "weight",
-        node_weight_prop_col: str | int = "weight",
-        weight_prop_col: str | int = "weight",
-        default_edge_weight: Optional[float | None] = None,
-        default_node_weight: Optional[float | None] = None,
-        default_weight: float = 1.0,
-        name: Optional[str] = None,
-        **kwargs,
+        ### these are for the incidence pairs and their properties
+        ### format for properties must follow from incidence pairs
+        ### so that properties are provided either in the dataframe
+        ### or as part of a nested dictionary.
+        setsystem=None,
+        default_cell_weight=1,  ### we will no longer support a sequence
+        edge_col=0,
+        node_col=1,
+        cell_weight_col="weight",
+        misc_cell_properties_col=None,
+        aggregate_by="first",
+        ### Format for properties can be either a dataframe indexed on uid
+        ### or with first column equal to uid or a dictionary
+        ### use these for a single properties list
+        properties=None,
+        ### How do we know which column to use for uid? Always the first column.
+        misc_properties_col=None,
+        weight_prop_col="weight",
+        default_weight: float | int = 1,
+        ### these are just for properties on the edges - ignored if properties exists
+        edge_properties=None,
+        misc_edge_properties_col=None,
+        edge_weight_prop_col="weight",
+        default_edge_weight=1,
+        ### these are just for properties on the nodes - ignored if properties exists
+        node_properties=None,
+        misc_node_properties_col=None,
+        node_weight_prop_col="weight",
+        default_node_weight=1,
+        name=None,
+        **kwargs,  ## these are ignored but allow for some backwards compatibility
     ):
-        self.name = name or ""
-        self.misc_cell_properties_col = misc_cell_properties = (
-            misc_cell_properties_col or "cell_properties"
-        )
-        self.misc_properties_col = misc_properties_col = (
-            misc_properties_col or "properties"
-        )
-        self.default_edge_weight = default_edge_weight = (
-            default_edge_weight or default_weight
-        )
-        self.default_node_weight = default_node_weight = (
-            default_node_weight or default_weight
-        )
-        ### cell properties
-
-        #### Empty Case
-        if setsystem is None or (len(setsystem) == 0):
-            df = pd.DataFrame(columns=['edges','nodes'])
-            self.E = EntitySet(df)
-            self._edges = self.E ##Edges(self.E) ##
-            self._nodes = self.E.restrict_to_levels([1]) ##Nodes(self.E) ##
-            self._data_cols = data_cols = self.E._data_cols
-
-            self._dataframe = self.E._dataframe
-            self._set_default_state(empty=True)
-            if self._dataframe is not None:
-                self._dataframe[self._data_cols] = self._dataframe[self._data_cols].astype(
-                    "category"
-                )
-
-            self.__dict__.update(locals())
-
-        else:  #### DataFrame case
-            if isinstance(setsystem, pd.DataFrame):
-                if isinstance(edge_col, int):
-                    self._edge_col = edge_col = setsystem.columns[edge_col]
-                    if isinstance(edge_col, int):
-                        setsystem = setsystem.rename(columns={edge_col: "edges"})
-                        self._edge_col = edge_col = "edges"
-                else:
-                    self._edge_col = edge_col
-
-                if isinstance(node_col, int):
-                    self._node_col = node_col = setsystem.columns[node_col]
-                    if isinstance(node_col, int):
-                        setsystem = setsystem.rename(columns={node_col: "nodes"})
-                        self._node_col = node_col = "nodes"
-                else:
-                    self._node_col = node_col
 
-                entity = setsystem.copy()
-
-                if isinstance(cell_weight_col, int):
-                    self._cell_weight_col = setsystem.columns[cell_weight_col]
-                else:
-                    self._cell_weight_col = cell_weight_col
-
-                if cell_weight_col in entity:
-                    entity = entity.fillna({cell_weight_col: cell_weights})
-                else:
-                    entity[cell_weight_col] = cell_weights
+        type_dict = {
+            "DataFrame": dataframe_factory_method,
+            "dict": dict_factory_method,
+            "OrderedDict": dict_factory_method,
+            "defaultdict": dict_factory_method,
+            "list": list_factory_method,
+            "ndarray": ndarray_factory_method,
+        }
+
+        if setsystem is None:
+            setsystem = pd.DataFrame(
+                columns=["edges", "nodes", "weight", "misc_properties"]
+            )
+        setsystem_type = type(setsystem).__name__
+        if setsystem_type in type_dict:
+            df = type_dict[setsystem_type](
+                setsystem,
+                2,
+                uid_cols=[edge_col, node_col],
+                weight_col=cell_weight_col,
+                default_weight=default_cell_weight,
+                misc_properties_col=misc_cell_properties_col,
+                aggregate_by=aggregate_by,
+            )
+            ## dataframe_factory_method(edf,uid_cols=[uid_col],weight_col,default_weight,misc_properties)
+            ## multi index set by uid_cols = [edge_col,node_col]
+            incidence_store = IncidenceStore(
+                pd.DataFrame(list(df.index), columns=["edges", "nodes"])
+            )
+            incidence_propertystore = PropertyStore(
+                data=df, default_weight=default_cell_weight
+            )
+            self._E = HypergraphView(incidence_store, 2, incidence_propertystore)
+            ## if no properties PropertyStore should store in the most efficient way
+        else:
+            raise HyperNetXError("setsystem data type not supported")
 
-                if isinstance(cell_properties, Sequence):
-                    cell_properties = [
-                        c
-                        for c in cell_properties
-                        if not c in [edge_col, node_col, cell_weight_col]
-                    ]
-                    cols = [edge_col, node_col, cell_weight_col] + cell_properties
-                    entity = entity[cols]
-                elif isinstance(cell_properties, dict):
-                    cp = []
-                    for idx in entity.index:
-                        edge, node = entity.iloc[idx][[edge_col, node_col]].values
-                        cp.append(cell_properties[edge][node])
-                    entity["cell_properties"] = cp
-
-            else:  ### Cases Other than DataFrame
-                self._edge_col = edge_col = edge_col or "edges"
-                if node_col == 1:
-                    self._node_col = node_col = "nodes"
+        if properties is not None:
+            property_type = type(properties).__name__
+            if property_type in type_dict:
+                dfp = type_dict[property_type](
+                    properties,
+                    0,
+                    weight_col=weight_prop_col,
+                    default_weight=default_weight,
+                    misc_properties_col=misc_properties_col,
+                )
+                all_propertystore = PropertyStore(
+                    data=dfp, default_weight=default_weight
+                )
+                self._edges = HypergraphView(incidence_store, 0, all_propertystore)
+                self._nodes = HypergraphView(incidence_store, 1, all_propertystore)
+        else:
+            if edge_properties is not None:
+                edge_property_type = type(edge_properties).__name__
+                if edge_property_type in type_dict:
+                    edfp = type_dict[edge_property_type](
+                        edge_properties,
+                        0,
+                        weight_col=edge_weight_prop_col,
+                        default_weight=default_edge_weight,
+                        misc_properties_col=misc_edge_properties_col,
+                    )
+                    edge_propertystore = PropertyStore(
+                        edfp, default_weight=default_edge_weight
+                    )
                 else:
-                    self._node_col = node_col
-                self._cell_weight_col = cell_weight_col
+                    edge_properties = PropertyStore(default_weight=default_edge_weight)
+            else:
+                edge_propertystore = PropertyStore(default_weight=default_edge_weight)
+            self._edges = HypergraphView(incidence_store, 0, edge_propertystore)
 
-                if isinstance(setsystem, np.ndarray):
-                    if setsystem.shape[1] != 2:
-                        raise HyperNetXError("Numpy array must have exactly 2 columns.")
-                    entity = pd.DataFrame(setsystem, columns=[edge_col, node_col])
-                    entity[cell_weight_col] = cell_weights
-
-                elif isinstance(setsystem, dict):
-                    ## check if it is a dict of iterables or a nested dict. if the latter then pull
-                    ## out the nested dicts as cell properties.
-                    ## cell properties must be of the same type as setsystem
-
-                    entity = pd.Series(setsystem).explode()
-                    entity = pd.DataFrame(
-                        {edge_col: entity.index.to_list(), node_col: entity.values}
+            if node_properties is not None:
+                node_property_type = type(node_properties).__name__
+                if node_property_type in type_dict:
+                    ndfp = type_dict[node_property_type](
+                        node_properties,
+                        1,
+                        weight_col=node_weight_prop_col,
+                        default_weight=default_node_weight,
+                        misc_properties_col=misc_node_properties_col,
                     )
-
-                    if dict_depth(setsystem) > 2:
-                        cell_props = dict(setsystem)
-                        if isinstance(cell_properties, dict):
-                            ## if setsystem is a dict then cell properties must be a dict
-                            cell_properties = merge_nested_dicts(
-                                cell_props, cell_properties
-                            )
-                        else:
-                            cell_properties = cell_props
-
-                        df = setsystem
-                        cp = []
-                        wt = []
-                        for idx in entity.index:
-                            edge, node = entity.values[idx][[0, 1]]
-                            wt.append(df[edge][node].get(cell_weight_col, cell_weights))
-                            cp.append(df[edge][node])
-                        entity[self._cell_weight_col] = wt
-                        entity["cell_properties"] = cp
-
-                    else:
-                        entity[self._cell_weight_col] = cell_weights
-
-                elif isinstance(setsystem, Iterable):
-                    entity = pd.Series(setsystem).explode()
-                    entity = pd.DataFrame(
-                        {edge_col: entity.index.to_list(), node_col: entity.values}
+                    node_propertystore = PropertyStore(
+                        ndfp, default_weight=default_node_weight
                     )
-                    entity["cell_weights"] = cell_weights
-
                 else:
-                    raise HyperNetXError(
-                        "setsystem is not supported or is in the wrong format."
+                    node_propertystore = PropertyStore(
+                        default_weight=default_node_weight
                     )
-
-            def props2dict(df=None):
-                if df is None:
-                    return {}
-                elif isinstance(df, pd.DataFrame):
-                    return df.set_index(df.columns[0]).to_dict(orient="index")
-                else:
-                    return dict(df)
-
-            if properties is None:
-                if edge_properties is not None or node_properties is not None:
-                    if edge_properties is not None:
-                        edge_properties = props2dict(edge_properties)
-                        for e in entity[edge_col].unique():
-                            if not e in edge_properties:
-                                edge_properties[e] = {}
-                        for v in edge_properties.values():
-                            v.setdefault(edge_weight_prop_col, default_edge_weight)
-                    else:
-                        edge_properties = {}
-                    if node_properties is not None:
-                        node_properties = props2dict(node_properties)
-                        for nd in entity[node_col].unique():
-                            if not nd in node_properties:
-                                node_properties[nd] = {}
-                        for v in node_properties.values():
-                            v.setdefault(node_weight_prop_col, default_node_weight)
-                    else:
-                        node_properties = {}
-                    properties = {0: edge_properties, 1: node_properties}
             else:
-                if isinstance(properties, pd.DataFrame):
-                    if weight_prop_col in properties.columns:
-                        properties = properties.fillna(
-                            {weight_prop_col: default_weight}
-                        )
-                    elif misc_properties_col in properties.columns:
-                        for idx in properties.index:
-                            if not isinstance(
-                                properties[misc_properties_col][idx], dict
-                            ):
-                                properties[misc_properties_col][idx] = {
-                                    weight_prop_col: default_weight
-                                }
-                            else:
-                                properties[misc_properties_col][idx].setdefault(
-                                    weight_prop_col, default_weight
-                                )
-                    else:
-                        properties[weight_prop_col] = default_weight
-                if isinstance(properties, dict):
-                    if dict_depth(properties) <= 2:
-                        properties = pd.DataFrame(
-                            [
-                                {"id": k, misc_properties_col: v}
-                                for k, v in properties.items()
-                            ]
-                        )
-                        for idx in properties.index:
-                            if isinstance(properties[misc_properties_col][idx], dict):
-                                properties[misc_properties_col][idx].setdefault(
-                                    weight_prop_col, default_weight
-                                )
-                            else:
-                                properties[misc_properties_col][idx] = {
-                                    weight_prop_col: default_weight
-                                }
-                    elif set(properties.keys()) == {0, 1}:
-                        edge_properties = properties[0]
-                        for e in entity[edge_col].unique():
-                            if not e in edge_properties:
-                                edge_properties[e] = {
-                                    edge_weight_prop_col: default_edge_weight
-                                }
-                            else:
-                                edge_properties[e].setdefault(
-                                    edge_weight_prop_col, default_edge_weight
-                                )
-                        node_properties = properties[1]
-                        for nd in entity[node_col].unique():
-                            if not nd in node_properties:
-                                node_properties[nd] = {
-                                    node_weight_prop_col: default_node_weight
-                                }
-                            else:
-                                node_properties[nd].setdefault(
-                                    node_weight_prop_col, default_node_weight
-                                )
-                        for idx in properties.index:
-                            if not isinstance(
-                                properties[misc_properties_col][idx], dict
-                            ):
-                                properties[misc_properties_col][idx] = {
-                                    weight_prop_col: default_weight
-                                }
-                            else:
-                                properties[misc_properties_col][idx].setdefault(
-                                    weight_prop_col, default_weight
-                                )
-
-            self.E = EntitySet(
-                entity=entity,
-                data_cols=(edge_col, node_col),
-                weight_col=cell_weight_col,
-                weights=cell_weights,
-                cell_properties=cell_properties,
-                misc_cell_props_col=misc_cell_properties_col or "cell_properties",
-                aggregateby=aggregateby or "sum",
-                properties=properties,
-                misc_props_col=misc_properties_col,
-            )
-
-            self._edges = self.E
-            self._nodes = self.E.restrict_to_levels([1])
-            self._data_cols = data_cols = [self._edge_col, self._node_col]
-
-            self._dataframe = self.E.cell_properties
-            if self._dataframe is not None:
-                self._dataframe = self._dataframe.reset_index()
-                self._dataframe[data_cols] = self._dataframe[data_cols].astype(
-                    "category"
-                )
-                self._set_default_state()
+                node_propertystore = PropertyStore(default_weight=default_node_weight)
+            self._nodes = HypergraphView(incidence_store, 1, node_propertystore)
 
-            self.__dict__.update(locals())
+        self._dataframe = self.dataframe
+        self._set_default_state()
+        self.name = name
+        self.__dict__.update(locals())
 
     @property
     def edges(self):
         """
-        Object associated with self._edges.
+        Object associated with edges.
 
         Returns
         -------
-        EntitySet
+        : HypergraphView
         """
         return self._edges
 
     @property
     def nodes(self):
         """
-        Object associated with self._nodes.
+        Object associated with nodes.
 
         Returns
         -------
-        EntitySet
+        : HypergraphView
         """
         return self._nodes
 
     @property
-    def dataframe(self):
-        """Returns dataframe of incidence pairs and their properties.
+    def incidences(self):
+        """
+        Object associated with incidence pairs
 
         Returns
         -------
-        pd.DataFrame
+        : HypergraphView
         """
-        return self._dataframe
+        return self._E
 
     @property
-    def properties(self):
-        """Returns dataframe of edge and node properties.
+    def dataframe(self):
+        """Returns dataframe of incidence properties
+        as dataframe with edges and nodes in columns.
 
         Returns
         -------
-        pd.DataFrame
+        pandas.DataFrame
         """
-        return self.E.properties
+        return self._E.properties.reset_index()
 
     @property
-    def edge_props(self):
-        """Dataframe of edge properties
-        indexed on edge ids
+    def properties(self):
+        """Returns incidence properties
 
         Returns
         -------
-        pd.DataFrame
+        pandas.DataFrame
         """
-        return self.E.properties.loc[0]
+        return self._E.properties
 
-    @property
-    def node_props(self):
-        """Dataframe of node properties
-        indexed on node ids
+    def incidence_matrix(self, index=False, weights=False):
+        """
+        A sparse matrix indicating the existence of an incidence pair
+        in the hypergraph. Each row corresponds to a node v and each column
+        corresponds to an edge e. The entry corresponding to (row v, col e)
+        is nonzero if v is an element of e. If weights = True then the value
+        equals the weight given in the hypergraph incidence properties for
+        the incidence pair (e,v). Otherwise, the value is 1.
+
+        Parameters
+        ----------
+        index : bool, optional, default = False
+            If index=True, returns a tuple containing the incidence matrix, an np.ndarray containing the row and column
+            index of node_uids, and an np.ndarray containing the row and column index of edge_uids.
+            Otherwise, returns the incidence matrix.
+        weights : bool, optional, default = False
+            If True, use the incidence weights corresponding to
+            the row and column of the entry.
 
         Returns
         -------
-        pd.DataFrame
+        incidence matrix: scipy.sparse.csr_matrix
+        node indexes: np.ndarray
+            an np.ndarray containing the row and column index of node_uids
+        edge indexes: np.ndarray
+            an np.ndarray containing the row and column index of edge_uids
         """
-        return self.E.properties.loc[1]
+        e, n = self._state_dict["data"].T
+
+        if weights:
+            data = self._E.dataframe["weight"]
+        else:
+            data = np.ones(len(e)).astype(int)
+        mat = csr_matrix((data, (n, e)))
+
+        if index:
+            return (
+                mat,
+                self._state_dict["labels"]["nodes"],
+                self._state_dict["labels"]["edges"],
+            )
+        return mat
+
+    def incidence_dataframe(self, weights=False):
+        mat, rindex, cindex = self.incidence_matrix(index=True, weights=weights)
+        return pd.DataFrame(mat.toarray(), columns=cindex, index=rindex)
 
     @property
     def incidence_dict(self):
         """
-        Dictionary keyed by edge uids with values the uids of nodes in each
-        edge
+        Dictionary keyed by edge uids with values as the uids of nodes of each edge
 
         Returns
         -------
         dict
 
         """
-        return self.E.incidence_dict
+        return self._E.elements
 
     @property
     def shape(self):
         """
-        (number of nodes, number of edges)
+        The number of nodes, number of edges
 
         Returns
         -------
-        tuple
+        number of nodes, number of edges : tuple
 
         """
-        return len(self._nodes.elements), len(self._edges.elements)
+        return len(self._nodes), len(self._edges)
 
     def __str__(self):
         """
         String representation of hypergraph
 
         Returns
         -------
         str
 
         """
-        return f"{self.name}, <class 'hypernetx.classes.hypergraph.Hypergraph'>"
+        return f"{self.name} <class 'hypernetx.classes.hypergraph.Hypergraph'>"
 
     def __repr__(self):
         """
         String representation of hypergraph
 
         Returns
         -------
         str
 
         """
-        return f"{self.name}, hypernetx.classes.hypergraph.Hypergraph"
+        return f"{self.name} hypernetx.classes.hypergraph.Hypergraph"
 
     def __len__(self):
         """
         Number of nodes
 
         Returns
         -------
@@ -700,102 +570,162 @@
         Iterate over the nodes of the hypergraph
 
         Returns
         -------
         dict_keyiterator
 
         """
-        return iter(self.nodes)
+        return iter(self._nodes)
 
     def __contains__(self, item):
         """
         Returns boolean indicating if item is in self.nodes
 
         Parameters
         ----------
-        item : hashable or EntitySet
+        item : hashable
 
         """
-        return item in self.nodes
+        return item in self._nodes
 
     def __getitem__(self, node):
         """
-        Returns the neighbors of node
+        Returns the neighbors of node in the Hypergraph. These
+        will be the nodes sharing some edge with the node.
 
         Parameters
         ----------
-        node : EntitySet or hashable
+        node : hashable
             If hashable, then must be uid of node in hypergraph
 
         Returns
         -------
         neighbors(node) : iterator
 
         """
         return self.neighbors(node)
 
-    def get_cell_properties(
-        self, edge: str, node: str, prop_name: Optional[str] = None
-    ) -> Any | dict[str, Any]:
+    def clone(self, name=None):
+        """
+        Create a deep copy of the hypergraph
+
+        Parameters
+        ----------
+        name : str, optional, default = None
+
+        Returns
+        -------
+        : Hypergraph
+        """
+        return self._construct_hyp_from_stores(
+            self.incidences.to_dataframe, name=f"{name}_clone"
+        )
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self.incidences.items == other.incidences.items
+        return False
+
+    def rename(self, edges=None, nodes=None, name=None, inplace=True):
+        """
+        Rename the edges and/or nodes of the hypergraph.
+
+        Parameters
+        ----------
+        edges : dict, optional, default = None
+            dictionary of replacement edge_uids
+        nodes : dict, optional, default = None
+            dictionary of replacement node_uids
+        name : str, optional, default=None
+        inplace : bool, optional, default=True
+
+        Returns
+        -------
+        Hypergraph
+        """
+        if edges is None and nodes is None:
+            return self
+        else:
+            edf = self.edges.to_dataframe
+            ndf = self.nodes.to_dataframe
+            df = self.incidences.to_dataframe
+        if edges is not None:
+            edf = edf.rename(index=edges)
+            df = df.rename(index=edges, level=0)
+        if nodes is not None:
+            ndf = ndf.rename(index=nodes)
+            df = df.rename(index=nodes, level=1)
+        eps = PropertyStore(edf)
+        nps = PropertyStore(ndf)
+        return self._construct_hyp_from_stores(
+            df, edge_ps=eps, node_ps=nps, name=name, inplace=inplace
+        )
+
+    def get_cell_properties(self, edge_uid, node_uid, prop_name=None):
         """Get cell properties on a specified edge and node
 
         Parameters
         ----------
-        edge : str
-            edgeid
-        node : str
-            nodeid
-        prop_name : str, optional
+        edge_uid : str | int
+            edge_uid
+        node_uid : str | int
+            node_uid
+        prop_name : str, optional, default=None
             name of a cell property; if None, all cell properties will be returned
 
         Returns
         -------
-        : int or str or dict of {str: any}
+        Any
             cell property value if `prop_name` is provided, otherwise ``dict`` of all
             cell properties and values
         """
         if prop_name is None:
-            return self.edges.get_cell_properties(edge, node)
-
-        return self.edges.get_cell_property(edge, node, prop_name)
+            return self.incidences.property_store.get_properties((edge_uid, node_uid))
+        return self.incidences.property_store.get_property(
+            (edge_uid, node_uid), prop_name
+        )
 
-    def get_properties(self, id, level=None, prop_name=None):
-        """Returns an object's specific property or all properties
+    def get_properties(self, uid, level=0, prop_name=None):
+        """
+        Returns an object's specific property or all properties
 
         Parameters
         ----------
-        id : hashable
+        uid : hashable
             edge or node id
-        level : int | None , optional, default = None
-            if separate edge and node properties then enter 0 for edges
-            and 1 for nodes.
-        prop_name : str | None, optional, default = None
-            if None then all properties associated with the object will  be
-            returned.
+        level : int | None , optional, default=0
+            Enter 0 for edges and 1 for nodes.
+        prop_name : str | None, optional, default=None
+            if None then all properties associated with the object will be returned.
 
         Returns
         -------
-        : str or dict
+        Any
             single property or dictionary of properties
         """
-        if prop_name is None:
-            return self.E.get_properties(id, level=level)
-        else:
-            return self.E.get_property(id, prop_name, level=level)
 
-    @warn_nwhy
+        if level == 0:
+            store = self._edges
+        elif level == 1:
+            store = self._nodes
+        elif level == 2:
+            store = self._E
+        if prop_name is None:  ## rewrite for edges and nodes.
+            return store.property_store.get_properties(uid)
+        return store.property_store.get_property(uid, prop_name)
+
     def get_linegraph(self, s=1, edges=True):
         """
-        Creates an ::term::s-linegraph for the Hypergraph.
-        If edges=True (default)then the edges will be the vertices of the line
+        Creates an :term:`s-linegraph` for the Hypergraph.
+        If edges=True, then the edges will be the vertices of the line
         graph. Two vertices are connected by an s-line-graph edge if the
-        corresponding hypergraph edges intersect in at least s hypergraph nodes.
+        corresponding hypergraph edges intersect in at least `s` hypergraph nodes.
         If edges=False, the hypergraph nodes will be the vertices of the line
         graph. Two vertices are connected if the nodes they correspond to share
-        at least s incident hyper edges.
+        at least `s` incident (hyper)edges.
 
         Parameters
         ----------
         s : int
             The width of the connections.
         edges : bool, optional, default = True
             Determine if edges or nodes will be the vertices in the linegraph.
@@ -806,838 +736,1264 @@
             A NetworkX graph.
         """
         d = self._state_dict
         key = "sedgelg" if edges else "snodelg"
         if s in d[key]:
             return d[key][s]
 
-        if edges:
+        if edges:  ### Amaplist needs a dictionary returned for properties.
             A, Amap = self.edge_adjacency_matrix(s=s, index=True)
-            Amaplst = [(k, self.edge_props.loc[k].to_dict()) for k in Amap]
+            Amaplst = [(k, self._edges[k].properties) for k in Amap]
         else:
             A, Amap = self.adjacency_matrix(s=s, index=True)
-            Amaplst = [(k, self.node_props.loc[k].to_dict()) for k in Amap]
+            Amaplst = [(k, self._nodes[k].properties) for k in Amap]
 
         ### TODO: add key function to compute weights lambda x,y : funcval
 
         A = np.array(np.nonzero(A))
         e1 = np.array([Amap[idx] for idx in A[0]])
         e2 = np.array([Amap[idx] for idx in A[1]])
         A = np.array([e1, e2]).T
         g = nx.Graph()
-        g.add_edges_from(A)
         g.add_nodes_from(Amaplst)
+        g.add_edges_from(A)
         d[key][s] = g
         return g
 
     def set_state(self, **kwargs):
         """
         Allow state_dict updates from outside of class. Use with caution.
 
         Parameters
         ----------
-        **kwargs
-            key=value pairs to save in state dictionary
+        **kwargs : dict, optional
+            key-value pairs to save in state dictionary
         """
         self._state_dict.update(kwargs)
 
-    def _set_default_state(self,empty=False):
-        """Populate state_dict with default values"""
+    def _set_default_state(self, empty=False):
+        """
+        Populate state_dict with default values
+        """
         self._state_dict = {}
-
-        self._state_dict["dataframe"] = df = self.dataframe
+        df = self._E.incidence_store.data
+        self._state_dict["dataframe"] = df
 
         if empty:
-            self._state_dict["labels"] = {
-                "edges": np.array([]),
-                "nodes": np.array([])
-                }
-            self._state_dict["data"] = np.array([[],[]])
-
+            self._state_dict["labels"] = {"edges": np.array([]), "nodes": np.array([])}
+            self._state_dict["data"] = np.array([[], []])
         else:
+            df.edges = df.edges.astype("category")
+            df.nodes = df.nodes.astype("category")
             self._state_dict["labels"] = {
-                "edges": np.array(df[self._edge_col].cat.categories),
-                "nodes": np.array(df[self._node_col].cat.categories),
+                "edges": np.array(df["edges"].cat.categories),
+                "nodes": np.array(df["nodes"].cat.categories),
             }
             self._state_dict["data"] = np.array(
-                [df[self._edge_col].cat.codes, df[self._node_col].cat.codes], dtype=int
+                [df["edges"].cat.codes, df["nodes"].cat.codes], dtype=int
             ).T
 
-
         self._state_dict["snodelg"] = dict()  ### s: nx.graph
         self._state_dict["sedgelg"] = dict()
         self._state_dict["neighbors"] = defaultdict(dict)  ### s: {node: neighbors}
-        self._state_dict["edge_neighbors"] = defaultdict(dict)  ### s: {edge: edge_neighbors}
+        self._state_dict["edge_neighbors"] = defaultdict(
+            dict
+        )  ### s: {edge: edge_neighbors}
         self._state_dict["adjacency_matrix"] = dict()  ### s: scipy.sparse.csr_matrix
         self._state_dict["edge_adjacency_matrix"] = dict()
 
-
     def edge_size_dist(self):
         """
-        Returns the size for each edge
+        Returns the size for each edge.
 
         Returns
         -------
-        np.array
-
+        list
+            a list of sizes of each edge.
         """
-
         if "edge_size_dist" not in self._state_dict:
             dist = np.array(np.sum(self.incidence_matrix(), axis=0))[0].tolist()
             self.set_state(edge_size_dist=dist)
-            return dist
-        else:
-            return self._state_dict["edge_size_dist"]
+        return self._state_dict["edge_size_dist"]
 
-    def degree(self, node, s=1, max_size=None):
+    def degree(self, node_uid, s=1, max_size=None):
         """
-        The number of edges of size s that contain node.
+        The number of edges of size at least s and at most
+        max_size that contain the node.
 
         Parameters
         ----------
-        node : hashable
-            identifier for the node.
-        s : positive integer, optional, default 1
-            smallest size of edge to consider in degree
-        max_size : positive integer or None, optional, default = None
-            largest size of edge to consider in degree
+        node_uid : hashable
+            Identifier for the node.
+        s : int, optional, default=1
+            The smallest size (must be positive) of an edge to consider in degree.
+        max_size : int, optional, default=None
+            The largest size (must be positive) of edge to consider in degree.
 
         Returns
         -------
-         : int
-
+        int
+            The number of edges of size at least s and at most
+            max_size that contain the node.
         """
-        if s == 1 and max_size == None:
-            return len(self.E.memberships[node])
-        else:
-            memberships = set()
-            for edge in self.E.memberships[node]:
-                size = len(self.edges[edge])
-                if size >= s and (max_size is None or size <= max_size):
-                    memberships.add(edge)
+        if s == 1 and max_size is None:
+            return len(self._nodes.memberships[node_uid])
 
-            return len(memberships)
+        ### This could possibly be done more efficiently on the dataframe.
+        memberships = set()
+        for edge in self._nodes.memberships[node_uid]:
+            size = len(self.edges[edge])
+            if size >= s and (max_size is None or size <= max_size):
+                memberships.add(edge)
+        return len(memberships)
 
     def size(self, edge, nodeset=None):
         """
         The number of nodes in nodeset that belong to edge.
         If nodeset is None then returns the size of edge
 
         Parameters
         ----------
         edge : hashable
             The uid of an edge in the hypergraph
 
         Returns
         -------
         size : int
-
         """
         if nodeset is not None:
             return len(set(nodeset).intersection(set(self.edges[edge])))
 
         return len(self.edges[edge])
 
-    def number_of_nodes(self, nodeset=None):
+    def order(self):
         """
-        The number of nodes in nodeset belonging to hypergraph.
-
-        Parameters
-        ----------
-        nodeset : an interable of Entities, optional, default = None
-            If None, then return the number of nodes in hypergraph.
+        The number of nodes in hypergraph.
 
         Returns
         -------
-        number_of_nodes : int
-
+        order : int
         """
-        if nodeset is not None:
-            return len([n for n in self.nodes if n in nodeset])
-
         return len(self.nodes)
 
-    def number_of_edges(self, edgeset=None):
+    def dim(self, edge):
         """
-        The number of edges in edgeset belonging to hypergraph.
+        Same as :meth:`size(edge) - 1`
 
         Parameters
         ----------
-        edgeset : an iterable of Entities, optional, default = None
-            If None, then return the number of edges in hypergraph.
-
-        Returns
-        -------
-        number_of_edges : int
-        """
-        if edgeset:
-            return len([e for e in self.edges if e in edgeset])
-
-        return len(self.edges)
-
-    def order(self):
-        """
-        The number of nodes in hypergraph.
+        edge : hashable
+            The uid of an edge in the hypergraph
 
         Returns
         -------
-        order : int
-        """
-        return len(self.nodes)
-
-    def dim(self, edge):
-        """
-        Same as size(edge)-1.
+        int
         """
         return self.size(edge) - 1
 
     def neighbors(self, node, s=1):
         """
-        The nodes in hypergraph which share s edge(s) with node.
+        The nodes in hypergraph which share `s` edge(s) with node.
 
         Parameters
         ----------
-        node : hashable or EntitySet
-            uid for a node in hypergraph or the node Entity
+        node : hashable
+            uid for a node in hypergraph
 
-        s : int, list, optional, default = 1
+        s : int, optional, default=1
             Minimum number of edges shared by neighbors with node.
 
         Returns
         -------
         neighbors : list
             s-neighbors share at least s edges in the hypergraph
 
         """
         if node not in self.nodes:
-            print(f"{node} is not in hypergraph {self.name}.")
-            return None
+            warnings.warn(f"{node} is not in hypergraph {self.name}.")
+            return []
         if node in self._state_dict["neighbors"][s]:
             return self._state_dict["neighbors"][s][node]
+
+        inc_matrix = self.incidence_matrix()
+        rdx = self._state_dict["labels"]["nodes"]
+        jdx = np.where(rdx == node)
+        idx = (inc_matrix[jdx].dot(inc_matrix.T) >= s) * 1
+        idx = np.nonzero(idx)[1]
+        neighbors = list(rdx[idx])
+        if len(neighbors) > 0:
+            neighbors.remove(node)
+            self._state_dict["neighbors"][s][node] = neighbors
         else:
-            M = self.incidence_matrix()
-            rdx = self._state_dict["labels"]["nodes"]
-            jdx = np.where(rdx == node)
-            idx = (M[jdx].dot(M.T) >= s) * 1
-            idx = np.nonzero(idx)[1]
-            neighbors = list(rdx[idx])
-            if len(neighbors) > 0:
-                neighbors.remove(node)
-                self._state_dict["neighbors"][s][node] = neighbors
-            else:
-                self._state_dict["neighbors"][s][node] = []
-        return neighbors
+            self._state_dict["neighbors"][s][node] = []
+        return self._state_dict["neighbors"][s][node]
 
     def edge_neighbors(self, edge, s=1):
         """
-        The edges in hypergraph which share s nodes(s) with edge.
+        The edges in hypergraph which share `s` nodes(s) with edge.
 
         Parameters
         ----------
-        edge : hashable or EntitySet
-            uid for a edge in hypergraph or the edge Entity
+        edge : hashable
+            uid for an edge in hypergraph
 
-        s : int, list, optional, default = 1
+        s : int, optional, default=1
             Minimum number of nodes shared by neighbors edge node.
 
         Returns
         -------
-         : list
-            List of edge neighbors
+        list
+            a list of edge neighbors
 
         """
 
         if edge not in self.edges:
-            print(f"Edge is not in hypergraph {self.name}.")
-            return None
+            warnings.warn(f"Edge is not in hypergraph {self.name}.")
+            return []
         if edge in self._state_dict["edge_neighbors"][s]:
             return self._state_dict["edge_neighbors"][s][edge]
+
+        inc_matrix = self.incidence_matrix()
+        cdx = self._state_dict["labels"]["edges"]
+        jdx = np.where(cdx == edge)
+        idx = (inc_matrix.T[jdx].dot(inc_matrix) >= s) * 1
+        idx = np.nonzero(idx)[1]
+        edge_neighbors = list(cdx[idx])
+        if len(edge_neighbors) > 0:
+            edge_neighbors.remove(edge)
+            self._state_dict["edge_neighbors"][s][edge] = edge_neighbors
         else:
-            M = self.incidence_matrix()
-            cdx = self._state_dict["labels"]["edges"]
-            jdx = np.where(cdx == edge)
-            idx = (M.T[jdx].dot(M) >= s) * 1
-            idx = np.nonzero(idx)[1]
-            edge_neighbors = list(cdx[idx])
-            if len(edge_neighbors) > 0:
-                edge_neighbors.remove(edge)
-                self._state_dict["edge_neighbors"][s][edge] = edge_neighbors
-            else:
-                self._state_dict["edge_neighbors"][s][edge] = []
-            return edge_neighbors
+            self._state_dict["edge_neighbors"][s][edge] = []
+        return self._state_dict["edge_neighbors"][s][edge]
 
-    def incidence_matrix(self, weights=False, index=False):
+    def adjacency_matrix(self, s=1, index=False):
         """
-        An incidence matrix for the hypergraph indexed by nodes x edges.
+        Returns the :term:`s-adjacency matrix` for the hypergraph.
 
         Parameters
         ----------
-        weights : bool, default =False
-            If False all nonzero entries are 1.
-            If True and self.static all nonzero entries are filled by
-            self.edges.cell_weights dictionary values.
+        s : int, optional, default=1
 
-        index : boolean, optional, default = False
-            If True return will include a dictionary of node uid : row number
-            and edge uid : column number
+        index: boolean, optional, default=False
+            If True, returns both the adjacency matrix and an array containing the row and column index of node_uids
 
         Returns
         -------
-        incidence_matrix : scipy.sparse.csr.csr_matrix or np.ndarray
+        adjacency matrix: scipy.sparse.csr_matrix
 
-        row_index : list
-            index of node ids for rows
+        node indexes: np.ndarray
+            an np.ndarray containing the row and column index of node_uids.
+        """
+        # if the adjacency_matrix for size s is not in the state_dict, create the adjacency matrix
+        # and add it to the state_dict
+        if (
+            "adjacency_matrix" not in self._state_dict
+            or s not in self._state_dict["adjacency_matrix"]
+        ):
+            incidence_matrix = self.incidence_matrix()
 
-        col_index : list
-            index of edge ids for columns
+            # calculates the square of the incidence matrix by multiplying it with its transpose.
+            s_adj_matrix = incidence_matrix @ incidence_matrix.T
 
-        """
-        sdkey = "incidence_matrix"
-        if weights:
-            sdkey = "weighted_" + sdkey
+            # sets the diagonal elements of s_adj_matrix to zero to remove self-loops.
+            s_adj_matrix.setdiag(0)
 
-        if sdkey in self._state_dict:
-            M = self._state_dict[sdkey]
-        else:
-            df = self.dataframe
-            data_cols = [self._node_col, self._edge_col]
-            if weights == True:
-                data = df[self._cell_weight_col].values
-                M = csr_matrix(
-                    (data, tuple(np.array(df[col].cat.codes) for col in data_cols))
-                )
-            else:
-                M = csr_matrix(
-                    (
-                        [1] * len(df),
-                        tuple(np.array(df[col].cat.codes) for col in data_cols),
-                    )
-                )
-            self._state_dict[sdkey] = M
+            # sets all values in s_adj_matrix that are greater than or equal to a
+            # threshold 's' to 1, and all other values to 0.
 
-        if index == True:
-            rdx = self.dataframe[self._node_col].cat.categories
-            cdx = self.dataframe[self._edge_col].cat.categories
+            s_adj_matrix = (s_adj_matrix >= s) * 1
 
-            return M, rdx, cdx
-        else:
-            return M
+            self._state_dict["adjacency_matrix"][s] = s_adj_matrix
+
+        if index:
+            return (
+                self._state_dict["adjacency_matrix"][s],
+                self._state_dict["labels"]["nodes"],
+            )
+        return self._state_dict["adjacency_matrix"][s]
 
-    def adjacency_matrix(self, s=1, index=False, remove_empty_rows=False):
+    def edge_adjacency_matrix(self, s=1, index=False):
         """
-        The :term:`s-adjacency matrix` for the hypergraph.
+        Returns the :term:`s-adjacency matrix` for the dual hypergraph.
 
         Parameters
         ----------
-        s : int, optional, default = 1
-
-        index: boolean, optional, default = False
-            if True, will return the index of ids for rows and columns
+        s : int, optional, default=1
 
-        remove_empty_rows: boolean, optional, default = False
+        index: boolean, optional, default=False
+            If True, returns both the adjacency matrix and an array containing the row and column index of edge_uids
 
         Returns
         -------
-        adjacency_matrix : scipy.sparse.csr.csr_matrix
+        edge adjacency matrix : scipy.sparse.csr_matrix
 
-        node_index : list
-            index of ids for rows and columns
+        edge indexes : np.ndarray
+            an np.ndarray containing the row and column index of edge_uids.
 
+        Notes
+        -----
+        This is also the adjacency matrix for the line graph.
+        Two edges are s-adjacent if they share at least `s` nodes.
         """
-        try:
-            A = self._state_dict["adjacency_matrix"][s]
-        except:
-            M = self.incidence_matrix()
-            A = M @ (M.T)
-            A.setdiag(0)
-            A = (A >= s) * 1
-            self._state_dict["adjacency_matrix"][s] = A
-        if index == True:
-            return A, self._state_dict["labels"]["nodes"]
-        else:
-            return A
+        if (
+            "edge_adjacency_matrix" not in self._state_dict
+            or s not in self._state_dict["edge_adjacency_matrix"]
+        ):
+            incidence_matrix = self.incidence_matrix()
+            s_adj_matrix = incidence_matrix.T @ incidence_matrix
+            s_adj_matrix.setdiag(0)
+            s_adj_matrix = (s_adj_matrix >= s) * 1
+            self._state_dict["edge_adjacency_matrix"][s] = s_adj_matrix
 
-    def edge_adjacency_matrix(self, s=1, index=False):
+        if index:
+            return (
+                self._state_dict["edge_adjacency_matrix"][s],
+                self._state_dict["labels"]["edges"],
+            )
+        return self._state_dict["edge_adjacency_matrix"][s]
+
+    def auxiliary_matrix(self, s=1, node=True, index=False):
         """
-        The :term:`s-adjacency matrix` for the dual hypergraph.
+        The unweighted :term:`s-auxiliary matrix` for hypergraph
 
         Parameters
         ----------
-        s : int, optional, default 1
+        s : int, optional, default=1
+
+        node : bool, optional, default=True
+            whether to return based on node or edge adjacencies
 
-        index: boolean, optional, default = False
-            if True, will return the index of ids for rows and columns
+        index : bool, optional, default=False
+            If True, returns both the auxiliary matrix and an array containing
+            the row and column index of node or edge_uids
 
         Returns
         -------
-        edge_adjacency_matrix : scipy.sparse.csr.csr_matrix
+        auxiliary matrix : scipy.sparse.csr_matrix
+            Node/Edge adjacency matrix with empty rows and columns removed
 
-        edge_index : list
-            index of ids for rows and columns
+        index : np.ndarray
+            row and column index of node or edge uids
+        """
+        if node:
+            adj_matrix, indexes = self.adjacency_matrix(s, index=True)
+        else:
+            adj_matrix, indexes = self.edge_adjacency_matrix(s, index=True)
 
-        Notes
-        -----
-        This is also the adjacency matrix for the line graph.
-        Two edges are s-adjacent if they share at least s nodes.
-        If remove_zeros is True will return the auxillary matrix
+        # sum up the values in each row of the matrix, resulting in a 1D array
+        # where each element corresponds to the sum of a row.
 
-        """
-        try:
-            A = self._state_dict["edge_adjacency_matrix"][s]
-        except:
-            M = self.incidence_matrix()
-            A = (M.T) @ (M)
-            A.setdiag(0)
-            A = (A >= s) * 1
-            self._state_dict["edge_adjacency_matrix"][s] = A
-        if index == True:
-            return A, self._state_dict["labels"]["edges"]
+        adj_matrix_sum = np.sum(adj_matrix, axis=1)
+        # returns a tuple of arrays with the first tuple being an array of the indices of rows whose sum is non-zero.
+        indices = np.nonzero(np.sum(adj_matrix_sum, axis=1))
+        non_zero_indices = indices[0]
+        if len(non_zero_indices) < adj_matrix.shape[0]:
+            adj_matrix_res = adj_matrix[non_zero_indices][:, non_zero_indices]
         else:
-            return A
+            adj_matrix_res = adj_matrix
 
-    def auxiliary_matrix(self, s=1, node=True, index=False):
+        if index:
+            return adj_matrix_res, indexes[non_zero_indices]
+        return adj_matrix_res
+
+    def bipartite(self, keep_data=False, directed=False):
         """
-        The unweighted :term:`s-edge or node auxiliary matrix` for hypergraph
+        Creates a bipartite NetworkX graph from hypergraph.
+        The nodes and (hyper)edges of hypergraph become the nodes of bipartite
+        graph. For every (hyper)edge e in the hypergraph and node v in e there
+        is an edge (e,v) in the graph.
 
         Parameters
         ----------
-        s : int, optional, default = 1
-        node : bool, optional, default = True
-            whether to return based on node or edge adjacencies
+        keep_data : bool, optional, default = False
+            If True the node and edge data from the hypergraph will be added to
+            the NetworkX graph
+        directed : bool, optional, default = False
+            If True the graph edges will be directed so that the hypergraph
+            edges are the sources and the hypergraph nodes are the targets
 
         Returns
         -------
-        auxiliary_matrix : scipy.sparse.csr.csr_matrix
-            Node/Edge adjacency matrix with empty rows and columns
-            removed
-        index : np.array
-            row and column index of userids
-
+        networkx.Graph or DiGraph
         """
-        if node == True:
-            A, Amap = self.adjacency_matrix(s, index=True)
+        if directed is True:
+            B = nx.DiGraph()
         else:
-            A, Amap = self.edge_adjacency_matrix(s, index=True)
-
-        idx = np.nonzero(np.sum(A, axis=1))[0]
-        if len(idx) < A.shape[0]:
-            B = A[idx][:, idx]
-        else:
-            B = A
-        if index:
-            return B, Amap[idx]
+            B = nx.Graph()
+        if keep_data is False:
+            B.add_nodes_from(self.edges, bipartite=0)
+            B.add_nodes_from(self.nodes, bipartite=1)
+            B.add_edges_from(
+                [
+                    (e, v)
+                    for v in self._nodes.memberships
+                    for e in self._nodes.memberships[v]
+                ]
+            )
         else:
-            return B
+            for nd in self.nodes:
+                B.add_node(nd, bipartite=1, **self.nodes[nd].properties)
+            for ed in self.edges:
+                B.add_node(ed, bipartite=0, **self.edges[ed].properties)
+            B.add_edges_from([(*d, self._E[d].properties) for d in self._E])
+        return B
 
-    def bipartite(self):
+    def _construct_hyp_from_stores(
+        self, incidence_df, edge_ps=None, node_ps=None, name=None, inplace=False
+    ):
         """
-        Constructs the networkX bipartite graph associated to hypergraph.
+
+        Parameters
+        ----------
+        incidence_df : pd.DataFrame
+        edge_ps : PropertyStore, default=None
+        node_ps: PropertyStore, default=None
+        name : str, optional, default=None
+        inplace : bool, optional, default=False
+            If True, changes the existing Hypergraph. Otherwise, creates a new Hypergraph with the requested changes.
 
         Returns
         -------
-        bipartite : nx.Graph()
+        Hypergraph
+        """
+        if inplace:
+            h = self
+        else:
+            h = Hypergraph()
 
-        Notes
-        -----
-        Creates a bipartite networkx graph from hypergraph.
-        The nodes and (hyper)edges of hypergraph become the nodes of bipartite
-        graph. For every (hyper)edge e in the hypergraph and node n in e there
-        is an edge (n,e) in the graph.
+        incidence_store = IncidenceStore(
+            pd.DataFrame(incidence_df.index.tolist(), columns=["edges", "nodes"])
+        )
+        incidence_ps = PropertyStore(
+            incidence_df, default_weight=self.incidences.default_weight
+        )
+        h._E = HypergraphView(incidence_store, 2, incidence_ps)
 
-        """
-        B = nx.Graph()
-        nodes = self._state_dict["labels"]["nodes"]
-        edges = self._state_dict["labels"]["edges"]
-        B.add_nodes_from(self.edges, bipartite=0)
-        B.add_nodes_from(self.nodes, bipartite=1)
-        B.add_edges_from([(v, e) for e in self.edges for v in self.edges[e]])
-        return B
+        if edge_ps is None:
+            edge_ps = PropertyStore(
+                self.edges.to_dataframe, default_weight=self.edges.default_weight
+            )
+        h._edges = HypergraphView(incidence_store, 0, edge_ps)
+
+        if node_ps is None:
+            node_ps = PropertyStore(
+                self.nodes.to_dataframe, default_weight=self.nodes.default_weight
+            )
+        h._nodes = HypergraphView(incidence_store, 1, node_ps)
 
-    def dual(self, name=None, switch_names=True):
+        h._set_default_state()
+        h._dataframe = h.dataframe
+        if not inplace:
+            h.name = name
+        return h
+
+    def dual(self, name=None, share_properties=True):
         """
         Constructs a new hypergraph with roles of edges and nodes of hypergraph
         reversed.
 
         Parameters
         ----------
-        name : hashable, optional
+        name : hashable, optional, default=None
 
-        switch_names : bool, optional, default = True
-            reverses edge_col and node_col names
-            unless edge_col = 'edges' and node_col = 'nodes'
+        share_properties : bool, optional, default=True
+            Whether to tie the edge and node properties of
+            objects in the dual to objects in the hypergraph.
+            If True, a change to edge and node properties in one will
+            be reflected in the other.
 
         Returns
         -------
-        : hypergraph
-
+        Hypergraph
         """
-        dfp = deepcopy(self.edges.properties)
-        dfp = dfp.reset_index()
-        dfp.level = dfp.level.apply(lambda x: 1 * (x == 0))
-        dfp = dfp.set_index(["level", "id"])
 
-        edge, node, wt = self._edge_col, self._node_col, self._cell_weight_col
-        df = deepcopy(self.dataframe)
-        cprops = [col for col in df.columns if not col in [edge, node, wt]]
+        C = self.dataframe.columns.tolist()
 
-        df[[edge, node]] = df[[node, edge]]
-        if switch_names == True and not (
-            self._edge_col == "edges" and self._node_col == "nodes"
-        ):
-            # if switch_names == False or (self._edge_col == 'edges' and self._node_col == 'nodes'):
-            df = df.rename(columns={edge: self._node_col, node: self._edge_col})
-            node = self._edge_col
-            edge = self._node_col
-
-        return Hypergraph(
-            df,
-            edge_col=edge,
-            node_col=node,
-            cell_weight_col=wt,
-            cell_properties=cprops,
-            properties=dfp,
-            name=name,
+        dsetsystem = (
+            self.dataframe[[C[1], C[0]] + C[2:]]
+            .rename(columns={"edges": "nodes", "nodes": "edges"})
+            .set_index(["edges", "nodes"])
         )
 
+        if share_properties:
+            edge_ps = self._nodes.property_store
+            node_ps = self._edges.property_store
+        else:
+            edge_ps = PropertyStore(self.nodes.to_dataframe)
+            node_ps = PropertyStore(self.edges.to_dataframe)
+
+        hdual = self._construct_hyp_from_stores(
+            dsetsystem,
+            edge_ps=edge_ps,
+            node_ps=node_ps,
+            name=name or str(self.name) + "_dual",
+        )
+        return hdual
+
+    def equivalence_classes(self, edges=True):
+        """
+        Returns the equivalence classes created by collapsing edges or nodes.
+
+        Parameters
+        ----------
+        edges : bool, optional, default=True
+            If True collapses edges, otherwise collapses nodes.
+
+        Returns
+        -------
+        list
+            A list of sets of edges or nodes
+
+        See Also
+        --------
+        collapse_edges
+        collapse_nodes
+        collapse_nodes_and_edges
+        """
+        level = 0 if edges else 1
+        return self._E.incidence_store.equivalence_classes(level=level)
+
     def collapse_edges(
         self,
         name=None,
+        use_uids=None,
+        use_counts=False,
+        return_counts=True,
         return_equivalence_classes=False,
-        use_reps=None,
-        return_counts=None,
+        aggregate_edges_by=None,
+        aggregate_cells_by=None,
     ):
         """
-        Constructs a new hypergraph gotten by identifying edges containing the
-        same nodes
+        Returns a new hypergraph by collapsing edges.
 
         Parameters
         ----------
-        name : hashable, optional, default = None
+
+        name: str, optional, default = None
+
+        use_uids: list, optional, default = None
+            Specify the edge identifiers to use as representatives
+            for a single equivalence class. If two identifiers occur in the
+            same equivalence class, the first one found will be used.
+
+        use_counts: boolean, optional, default = False
+            Rename the equivalence class representatives as `<uid>:<size of class>`
+
+        return_counts: bool, optional, default = True
+            Add the size of the equivalence class to the properties
+            associated to the representative in the collapsed hypergraph using
+            keyword: `eclass_size`
 
         return_equivalence_classes: boolean, optional, default = False
-            Returns a dictionary of edge equivalence classes keyed by frozen
-            sets of nodes
+            Returns a dictionary of edge equivalence classes keyed by a
+            representative from each class
+
+        aggregate_edges_by, aggregate_cells_by : dict, optional, default = {'weight':'sum'}
+            dictionary of aggregation methods keyed by column names
+            in the properties dataframes, does not apply to misc_properties.
+            Defaults to 'first' on unlisted columns.
+            See pandas.core.groupby.DataFrameGroupBy.agg for usage examples with
+            dictionaries
 
         Returns
         -------
-        new hypergraph : Hypergraph
-            Equivalent edges are collapsed to a single edge named by a
-            representative of the equivalent edges followed by a colon and the
-            number of edges it represents.
-
-        equivalence_classes : dict
-            A dictionary keyed by representative edge names with values equal
-            to the edges in its equivalence class
+        Hypergraph
 
         Notes
         -----
-        Two edges are identified if their respective elements are the same.
-        Using this as an equivalence relation, the uids of the edges are
-        partitioned into equivalence classes.
-
-        A single edge from the collapsed edges followed by a colon and the
-        number of elements in its equivalence class as uid for the new edge
+        Collapses the edges of Hypergraph. Two edges are
+        duplicates if their respective elements are the same.
+        Using this as an equivalence relation, the uids of the edges
+        are partitioned into equivalence classes. A single member of the
+        equivalence class is chosen to represent the class.
 
+        Example
+        -------
 
+            >>> data = {'E1': ('a', 'b'), 'E2': ('a', 'b')}
+            >>> h = Hypergraph(data)
+            >>> h.incidence_dict
+            {'E1': ['a', 'b'], 'E2': ['a', 'b']}
+            >>> h.collapse_edges().incidence_dict
+            {'E1': ['a', 'b']}
+            >>> h.collapse_edges(use_counts=True).incidence_dict
+            {'E1:2': ['a', 'b']}
+            >>> h.collapse_edges().properties.to_dict(orient='records')
+            [{'weight': 2.0, 'misc_properties': {}}, {'weight': 2.0, 'misc_properties': {}}]
         """
-        if use_reps is not None or return_counts is not None:
-            msg = """
-            use_reps ane return_counts are no longer supported keyword
-            arguments and will throw an error in the next release.
-            collapsed hypergraph automatically names collapsed objects by a
-            string "rep:count"
-            """
-            warnings.warn(msg, DeprecationWarning)
+        _, eclasses = self._E.incidence_store.collapse_identical_elements(
+            0, use_keys=use_uids
+        )
+
+        aggregate_edges_by = aggregate_edges_by or {"weight": "sum"}
+        aggregate_cells_by = aggregate_cells_by or {"weight": "sum"}
 
-        temp = self.edges.collapse_identical_elements(
-            return_equivalence_classes=return_equivalence_classes
+        ndf = self.edges.to_dataframe
+        df = self.incidences.to_dataframe
+
+        if use_uids is not None:  ## then eclasses will reorder the dataframes
+            ## so the first occurence of the class is one of these uids.
+            newindex = []
+            for v in eclasses.values():
+                newindex += v
+            ndf = ndf.loc[newindex]
+            df = df.loc[newindex, :]
+
+        if use_counts:
+            mapper = {vv: f"{k}:{len(v)}" for k, v in eclasses.items() for vv in v}
+        else:
+            mapper = {vv: k for k, v in eclasses.items() for vv in v}
+
+        ndf = ndf.rename(index=mapper)
+        ndf = _agg_rows(ndf, ndf.index, aggregate_edges_by)
+        edge_ps = PropertyStore(ndf)
+
+        df = df.rename(index=mapper, level=0)
+        df = _agg_rows(df, ["edges", "nodes"], aggregate_cells_by)
+
+        node_ps = PropertyStore(self.nodes.to_dataframe)
+        H = self._construct_hyp_from_stores(
+            df, edge_ps=edge_ps, node_ps=node_ps, name=name
         )
 
-        if return_equivalence_classes:
-            return Hypergraph(temp[0].incidence_dict, name), temp[1]
+        if return_counts:
+            if use_counts:
+                for nd in H.edges:
+                    H.edges[nd].equivalence_class_size = int(nd.split(":")[1])
+            else:
+                for nd in H.edges:
+                    H.edges[nd].equivalence_class_size = len(eclasses[nd])
 
-        return Hypergraph(temp.incidence_dict, name)
+        if return_equivalence_classes:
+            return H, {mapper[k]: eclasses[k] for k in eclasses}
+        else:
+            return H
 
     def collapse_nodes(
         self,
         name=None,
+        use_uids=None,
+        use_counts=False,
+        return_counts=True,
         return_equivalence_classes=False,
-        use_reps=None,
-        return_counts=None,
-    ) -> Hypergraph:
+        aggregate_nodes_by=None,
+        aggregate_cells_by=None,
+    ):
         """
-        Constructs a new hypergraph gotten by identifying nodes contained by
-        the same edges
+        Returns a new hypergraph by collapsing nodes.
 
         Parameters
         ----------
+
         name: str, optional, default = None
 
-        return_equivalence_classes: boolean, optional, default = False
-            Returns a dictionary of node equivalence classes keyed by frozen
-            sets of edges
+        use_uids: list, optional, default = None
+            Specify the node identifiers to use as representatives
+            for a single equivalence class. If two identifiers occur in the
+            same equivalence class, the first one found will be used.
+
+        use_counts: boolean, optional, default = False
+            Rename the equivalence class representatives as `<uid>:<size of class>`
+
+        return_counts: bool, optional, default = True
+            Add the size of the equivalence class to the properties
+            associated to the representative in the collapsed hypergraph using
+            keyword: `eclass_size`
 
-        use_reps : boolean, optional, default = None
-            [DEPRECATED; WILL BE REMOVED IN NEXT RELEASE] Choose a single element from the
-            collapsed nodes as uid for the new node, otherwise uses a frozen
-            set of the uids of nodes in the equivalence class. If use_reps is True the new nodes have uids given by a
-            tuple of the rep and the count
+        return_equivalence_classes: boolean, optional, default = False
+            Returns a dictionary of edge equivalence classes keyed by a
+            representative from each class
 
-        return_counts: boolean, optional, default = None
-            [DEPRECATED; WILL BE REMOVED IN NEXT RELEASE]
+        aggregate_nodes_by, aggregate_cells_by : dict, optional, default = {'weight':'sum'}
+            dictionary of aggregation methods keyed by column names
+            in the properties dataframes, does not apply to misc_properties.
+            Defaults to 'first' on unlisted columns.
+            See pandas.core.groupby.DataFrameGroupBy.agg for usage examples with
+            dictionaries
 
         Returns
         -------
-        new hypergraph : Hypergraph
+        Hypergraph
 
         Notes
         -----
-        Two nodes are identified if their respective memberships are the same.
-        Using this as an equivalence relation, the uids of the nodes are
-        partitioned into equivalence classes. A single member of the
-        equivalence class is chosen to represent the class followed by the
-        number of members of the class.
+        Collapses the nodes of Hypergraph. Two nodes are
+        duplicates if their respective memberships are the same.
+        Using this as an equivalence relation, the uids of the nodes
+        are partitioned into equivalence classes. A single member of the
+        equivalence class is chosen to represent the class.
 
         Example
         -------
 
-            >>> data = {'E1': ('a', 'b'), 'E2': ('a', 'b')}))
+            >>> data = {'E1': ('a', 'b'), 'E2': ('a', 'b')}
             >>> h = Hypergraph(data)
+            >>> h.incidence_dict
+            {'E1': ['a', 'b'], 'E2': ['a', 'b']}
             >>> h.collapse_nodes().incidence_dict
-            {'E1': ['a: 2'], 'E2': ['a: 2']}
+            {'E1': ['a'], 'E2': ['a']}
+            >>> h.collapse_nodes(use_counts=True).incidence_dict
+            {'E1: ['a:2'], 'E2': ['a:2']}
+            >>> h.collapse_nodes().properties.to_dict(orient='records')
+            [{'weight': 2.0, 'misc_properties': {}}, {'weight': 2.0, 'misc_properties': {}}]
         """
-        if use_reps is not None or return_counts is not None:
-            msg = """
-            use_reps and return_counts are no longer supported keyword arguments and will throw
-            an error in the next release.
-            collapsed hypergraph automatically names collapsed objects by a string "rep:count"
-            """
-            warnings.warn(msg, DeprecationWarning)
+        _, eclasses = self._E.incidence_store.collapse_identical_elements(
+            1, use_keys=use_uids
+        )
+
+        aggregate_nodes_by = aggregate_nodes_by or {"weight": "sum"}
+        aggregate_cells_by = aggregate_cells_by or {"weight": "sum"}
+
+        ndf = self.nodes.to_dataframe
+        df = self.incidences.to_dataframe
 
-        temp = self.dual().edges.collapse_identical_elements(
-            return_equivalence_classes=return_equivalence_classes
+        if use_uids is not None:  ## then eclasses will reorder the dataframes
+            ## so the first occurence of the class is one of these uids.
+            newindex = []
+            for v in eclasses.values():
+                newindex += v
+            ndf = ndf.loc[newindex]
+            df = df.swaplevel().loc[newindex, :].swaplevel()
+
+        if use_counts:
+            mapper = {vv: f"{k}:{len(v)}" for k, v in eclasses.items() for vv in v}
+        else:
+            mapper = {vv: k for k, v in eclasses.items() for vv in v}
+
+        ndf = ndf.rename(index=mapper)
+        ndf = _agg_rows(ndf, ndf.index, aggregate_nodes_by)
+        node_ps = PropertyStore(ndf)
+
+        df = df.rename(index=mapper, level=1)
+        df = _agg_rows(df, ["edges", "nodes"], aggregate_cells_by)
+
+        edge_ps = PropertyStore(self.edges.to_dataframe)
+        H = self._construct_hyp_from_stores(
+            df, edge_ps=edge_ps, node_ps=node_ps, name=name
         )
 
-        if return_equivalence_classes:
-            return Hypergraph(temp[0].incidence_dict).dual(), temp[1]
+        if return_counts:
+            if use_counts:
+                for nd in H.nodes:
+                    H.nodes[nd].equivalence_class_size = int(nd.split(":")[1])
+            else:
+                for nd in H.nodes:
+                    H.nodes[nd].equivalence_class_size = len(eclasses[nd])
 
-        return Hypergraph(temp.incidence_dict, name).dual()
+        if return_equivalence_classes:
+            return H, {mapper[k]: eclasses[k] for k in eclasses}
+        else:
+            return H
 
     def collapse_nodes_and_edges(
         self,
         name=None,
+        use_edge_uids=None,
+        use_node_uids=None,
+        use_counts=False,
+        return_counts=True,
         return_equivalence_classes=False,
-        use_reps=None,
-        return_counts=None,
+        aggregate_nodes_by=None,
+        aggregate_edges_by=None,
+        aggregate_cells_by=None,
     ):
         """
         Returns a new hypergraph by collapsing nodes and edges.
 
         Parameters
         ----------
 
         name: str, optional, default = None
 
         return_equivalence_classes: boolean, optional, default = False
-            Returns a dictionary of edge equivalence classes keyed by frozen
-            sets of nodes
+            Returns a dictionary of edge equivalence classes keyed by a
+            representative from each class
 
-        use_reps: boolean, optional, default = None
-            [DEPRECATED; WILL BE REMOVED IN NEXT RELEASE] Choose a single element from the collapsed elements as a
-            representative. If use_reps is True, the new elements are keyed by a tuple of the
-            rep and the count.
+        use_edge_uids, use_node_uids: list, optional, default = None
+            Specify the edge and node identifiers to use as representatives
+            for a single equivalence class. If two identifiers occur in the
+            same equivalence class, the first one found will be used.
+
+        use_counts: boolean, optional, default = False
+            Rename the equivalence class representatives as `<uid>:<size of class>`
+
+        return_counts: bool, optional, default = True
+            Add the size of the equivalence class to the properties
+            associated to the representative in the collapsed hypergraph using
+            keyword: `eclass_size`
+
+        aggregate_nodes_by, aggregate_edges_by, aggregate_cells_by: optional
+            default = {'weight' = 'sum'}, all
+            Method to combine duplicate rows of data for the same uids
 
-        return_counts: boolean, optional, default = None
-            [DEPRECATED; WILL BE REMOVED IN NEXT RELEASE]
 
         Returns
         -------
         new hypergraph : Hypergraph
+        node equivalence classes : dict
+        edge equivalence classes : dict
 
         Notes
         -----
-        Collapses the Nodes and Edges of EntitySets. Two nodes(edges) are
+        Collapses the Nodes and Edges of Hypergraph. Two nodes(edges) are
         duplicates if their respective memberships(elements) are the same.
         Using this as an equivalence relation, the uids of the nodes(edges)
         are partitioned into equivalence classes. A single member of the
-        equivalence class is chosen to represent the class followed by the
-        number of members of the class.
+        equivalence class is chosen to represent the class.
 
         Example
         -------
 
             >>> data = {'E1': ('a', 'b'), 'E2': ('a', 'b')}
             >>> h = Hypergraph(data)
             >>> h.incidence_dict
             {'E1': ['a', 'b'], 'E2': ['a', 'b']}
             >>> h.collapse_nodes_and_edges().incidence_dict
-            {'E1: 2': ['a: 2']}
-
+            {'E1': ['a']}
+            >>> h.collapse_nodes_and_edges(use_counts=True).incidence_dict
+            {'E1:2': ['a:2']}
         """
-        if use_reps is not None or return_counts is not None:
-            msg = """
-            use_reps and return_counts are no longer supported keyword
-            arguments and will throw an error in the next release.
-            collapsed hypergraph automatically names collapsed objects by a
-            string "rep:count"
-            """
-            warnings.warn(msg, DeprecationWarning)
+
+        aggregate_nodes_by = aggregate_nodes_by or {"weight": "sum"}
+        aggregate_cells_by = aggregate_cells_by or {"weight": "sum"}
+        aggregate_edges_by = aggregate_edges_by or {"weight": "sum"}
 
         if return_equivalence_classes:
             temp, neq = self.collapse_nodes(
-                name="temp", return_equivalence_classes=True
+                return_equivalence_classes=True,
+                use_uids=use_node_uids,
+                use_counts=use_counts,
+                return_counts=return_counts,
+                aggregate_nodes_by=aggregate_nodes_by,
+                aggregate_cells_by=aggregate_cells_by,
+            )
+            ntemp, eeq = temp.collapse_edges(
+                name=name,
+                return_equivalence_classes=True,
+                use_uids=use_edge_uids,
+                use_counts=use_counts,
+                return_counts=return_counts,
+                aggregate_edges_by=aggregate_edges_by,
+                aggregate_cells_by=aggregate_cells_by,
             )
-            ntemp, eeq = temp.collapse_edges(name=name, return_equivalence_classes=True)
             return ntemp, neq, eeq
-
-        temp = self.collapse_nodes(name="temp")
-        return temp.collapse_edges(name=name)
+        else:
+            temp = self.collapse_nodes(
+                use_uids=use_node_uids,
+                use_counts=use_counts,
+                return_counts=return_counts,
+                aggregate_nodes_by=aggregate_nodes_by,
+                aggregate_cells_by=aggregate_cells_by,
+            )
+            return temp.collapse_edges(
+                name=name,
+                use_uids=use_edge_uids,
+                use_counts=use_counts,
+                return_counts=return_counts,
+                aggregate_edges_by=aggregate_edges_by,
+                aggregate_cells_by=aggregate_cells_by,
+            )
 
     def restrict_to_nodes(self, nodes, name=None):
-        """New hypergraph gotten by restricting to nodes
+        """
+        New hypergraph gotten by restricting to nodes
 
         Parameters
         ----------
         nodes : Iterable
-            nodeids to restrict to
+            node identifiers to restrict to
+        name : str | int, optional, default=None
+            node identifier
 
         Returns
         -------
-        : hnx. Hypergraph
-
+        Hypergraph
         """
-        keys = set(self._state_dict["labels"]["nodes"]).difference(nodes)
-        return self.remove(keys, level=1)
+
+        keys = list(set(self._state_dict["labels"]["nodes"]).difference(nodes))
+        return self._remove(keys, level=1, name=name, inplace=False)
 
     def restrict_to_edges(self, edges, name=None):
         """New hypergraph gotten by restricting to edges
 
         Parameters
         ----------
         edges : Iterable
-            edgeids to restrict to
+            edge identifiers to restrict to
+        name : str | int, optional, default=None
+            edge identifier
 
         Returns
         -------
-        hnx.Hypergraph
+        Hypergraph
+        """
+        keys = list(set(self._state_dict["labels"]["edges"]).difference(edges))
+        return self._remove(keys, level=0, name=name, inplace=False)
 
+    def add_edge(self, edge_uid, inplace=True, **attr):
         """
-        keys = set(self._state_dict["labels"]["edges"]).difference(edges)
-        return self.remove(keys, level=0)
+        Add a single edge with attributes to edge properties.
+        Does not add an incidence to the hypergraph.
+
+        Parameters
+        ----------
 
-    def remove_edges(self, keys, name=None):
-        return self.remove(keys, level=0, name=name)
+        edge_uid : int | str
+            edge_uid
+        inplace : bool, default=True
+            If True, changes the existing Hypergraph. Otherwise, creates a new Hypergraph with the requested changes.
+        **attr : dict, optional
+            Properties to add to edges as key=value pairs.
 
-    def remove_nodes(self, keys, name=None):
-        return self.remove(keys, level=1, name=name)
+        Returns
+        -------
+        Hypergraph
+        """
+        return self._add_items_from([(edge_uid, attr)], 0, inplace=inplace)
 
-    def remove(self, keys, level=None, name=None):
-        """Creates a new hypergraph with nodes and/or edges indexed by keys
-        removed. More efficient for creating a restricted hypergraph if the
-        restricted set is greater than what is being removed.
+    def add_edges_from(self, edge_uids, inplace=True):
+        """
+        Add a collection of edges with attributes to edge properties.
+        Does not add an incidence to the hypergraph.
 
         Parameters
         ----------
-        keys : list | tuple | set | Hashable
-            node and/or edge id(s) to restrict to
-        level : None, optional
-            Enter 0 to remove edges with ids in keys.
-            Enter 1 to remove nodes with ids in keys.
-            If None then all objects in nodes and edges with the id will
-            be removed.
-        name : str, optional
-            Name of new hypergraph
+        edge_uids : list[int | str] | list[tuple[int | str, dict]], list[int | str | tuple[int | str, dict]]
+            edge_uids must be a list of uids and/or tuples of the form (uid,data) where data is dictionary
+        inplace : bool, default=True
+            If True, changes the existing Hypergraph. Otherwise, creates a new Hypergraph with the requested changes.
 
         Returns
         -------
-        : hnx.Hypergraph
-
-        """
-        rdfprop = self.properties.copy()
-        rdf = self.dataframe.copy()
-        if isinstance(keys, (list, tuple, set)):
-            nkeys = keys
-        elif isinstance(keys, Hashable):
-            nkeys = list()
-            nkeys.append(keys)
-        else:
-            raise TypeError("`keys` parameter must be list | tuple | set | Hashable")
-        if level == 0:
-            kdx = set(nkeys).intersection(set(self._state_dict["labels"]["edges"]))
-            for k in kdx:
-                rdfprop = rdfprop.drop((0, k))
-            rdf = rdf.loc[~(rdf[self._edge_col].isin(kdx))]
-        elif level == 1:
-            kdx = set(nkeys).intersection(set(self._state_dict["labels"]["nodes"]))
-            for k in kdx:
-                rdfprop = rdfprop.drop((1, k))
-            rdf = rdf.loc[~(rdf[self._node_col].isin(kdx))]
-        else:
-            rdfprop = rdfprop.reset_index()
-            kdx = set(nkeys).intersection(rdfprop.id.unique())
-            rdfprop = rdfprop.set_index("id")
-            rdfprop = rdfprop.drop(index=kdx)
-            rdf = rdf.loc[~(rdf[self._edge_col].isin(kdx))]
-            rdf = rdf.loc[~(rdf[self._node_col].isin(kdx))]
-
-        return Hypergraph(
-            setsystem=rdf,
-            edge_col=self._edge_col,
-            node_col=self._node_col,
-            cell_weight_col=self._cell_weight_col,
-            misc_cell_properties_col=self.edges._misc_cell_props_col,
-            properties=rdfprop,
-            misc_properties_col=self.edges._misc_props_col,
-            name=name,
+        Hypergraph
+        """
+        edge_uids = self._process_uids(edge_uids)
+        return self._add_items_from(edge_uids, 0, inplace=inplace)
+
+    def add_node(self, node_uid, inplace=True, **attr):
+        """
+        Add a single node with attributes to node properties.
+        Does not add an incidence to the hypergraph.
+
+        Parameters
+        ----------
+        node_uid : int | str
+            node_uid
+        inplace : bool, default=True
+            If True, changes the existing Hypergraph. Otherwise, creates a new Hypergraph with the requested changes.
+        **attr : dict, optional
+            Properties to add to edges as key=value pairs.
+
+        Returns
+        -------
+        Hypergraph
+        """
+        return self._add_items_from([(node_uid, attr)], 1, inplace=inplace)
+
+    def add_nodes_from(self, node_uids, inplace=True):
+        """
+        Add a collection of nodes with attributes to nodes properties.
+        Does not add an incidence to the hypergraph.
+
+        Parameters
+        ----------
+        node_uids : list[int | str] | list[tuple[int | str, dict]], list[int | str | tuple[int | str, dict]]
+            node_uids must be a list of uids and/or tuples of the form (uid,data) where data is dictionary
+        inplace : bool, default=True
+            If True, changes the existing Hypergraph. Otherwise, creates a new Hypergraph with the requested changes.
+
+        Returns
+        -------
+        Hypergraph
+        """
+        node_uids = self._process_uids(node_uids)
+        return self._add_items_from(node_uids, 1, inplace=inplace)
+
+    def _process_uids(self, uids):
+        """Returns a list of items in the form of list[tuple[int | str, dict]"""
+        new_items = list()
+        for item in uids:
+            if not isinstance(item, tuple):
+                new_items.append((item, {}))
+            else:
+                new_items.append(item)
+        return new_items
+
+    def add_nodes_to_edges(self, edge_dict, inplace=True):
+        """
+        Adds a collection of incidences to Hypergraph
+
+        Parameters
+        ----------
+        edge_dict: dict[str, list[str | int] | dict[str, dict]]
+            The edge dictionary must be a dictionary of edges as the keys and a list of nodes or a dictionary
+            of nodes to properties as the values.
+        inplace : bool, default=True
+            If True, changes the existing. Otherwise, creates a new Hypergraph with the requested changes.
+
+        Returns
+        -------
+        Hypergraph
+            Hypergraph with the updated edges and their newly added nodes
+        """
+        items = list()
+        for ed, nodes in edge_dict.items():
+            if isinstance(nodes, dict):
+                for nd, data in nodes.items():
+                    items.append(((ed, nd), data))
+            else:
+                for nd in nodes:
+                    items.append(((ed, nd), {}))
+        return self._add_items_from(items, 2, inplace=inplace)
+
+    def add_incidence(self, edge_uid, node_uid, inplace=True, **attr):
+        """
+        Add a single incidence with attributes to Hypergraph.
+
+        Parameters
+        ----------
+        edge_uid : int | str
+            edge_uid
+        node_uid : int | str
+            node_uid
+        inplace : bool, optional, default=True
+            If True, changes the existing Hypergraph. Otherwise, creates a new Hypergraph with the requested changes.
+        **attr : dict, optional
+            Properties to add to incidences as key=value pairs.
+
+        Returns
+        -------
+        Hypergraph
+            Hypergraph with incidences added.
+        """
+        return self._add_items_from([((edge_uid, node_uid), attr)], 2, inplace=inplace)
+
+    def add_incidences_from(self, incidences, inplace=True):
+        """
+        Adds a collection of incidences to Hypergraph
+
+        Parameters
+        ----------
+        incidences: list[str | int, str | int], list[tuple[str | int, str | int, dict[str, Any]]
+            Incidence pairs must be a list of uids of the form (edge_uid,node_uid)
+            and/or tuples of the form (edge_uid, node_uid,data) where data is a
+            dictionary.
+        inplace : bool, optional, default=True
+            If True, changes the existing Hypergraph. Otherwise, creates a new Hypergraph with the requested changes.
+
+        Returns
+        -------
+        Hypergraph
+            Hypergraph with incidences added.
+        """
+        newincidences = list()
+        for pr in incidences:
+            if len(pr) == 2:
+                newincidences.append((pr, {}))
+            else:
+                newincidences.append(((pr[0], pr[1]), pr[2]))
+        return self._add_items_from(newincidences, 2, inplace=inplace)
+
+    def _add_items_from(self, items, level, inplace=True):
+        """
+        Helper method to add items to Hypergraph
+
+        Parameters
+        ----------
+        items : list[tuple[str | int, dict[str, Any]]]
+            Items must be a list of tuples of the form (uid,data) where data is dictionary
+        level : int
+            the level to add the items to; 0=edges, 1=nodes, 2=incidences
+        inplace : bool, optional, default=True
+            If True, changes the existing Hypergraph. Otherwise, creates a new Hypergraph with the requested changes.
+
+        Returns
+        -------
+        Hypergraph
+        """
+        df = self.incidences._property_store
+        ep = self.edges._property_store
+        ndp = self.nodes._property_store
+        hv = [ep, ndp, df][level]
+        for item in items:
+            uid = item[0]
+            data = item[1]
+            hv.set_properties(uid, data)
+        return self._construct_hyp_from_stores(
+            df.properties, edge_ps=ep, node_ps=ndp, name=self.name, inplace=inplace
         )
 
-    def toplexes(self, name=None):
+    #### This should follow behavior of restrictions
+    def remove_edges(self, edge_uids, name=None, inplace=True):
+        """
+        Removes the edges from the Hypergraph.
+        If inplace=True, changes the existing Hypergraph. Otherwise,
+        creates a new Hypergraph with the requested changes.
+
+        Parameters
+        ----------
+        edge_uids : str | int | list[str | int]
+            edge_uids
+        name : str, optional, default=None
+            The name of the new Hypergraph. Used only when inplace=False;
+            ignored if inplace=True.
+        inplace : bool, optional, default=True
+            Whether to replace the current hypergraph with a new one.
+
+        Returns
+        -------
+        Hypergraph
+        """
+        if not isinstance(edge_uids, list):
+            edge_uids = [edge_uids]
+        return self._remove(edge_uids, level=0, name=name, inplace=inplace)
+
+    def remove_nodes(self, node_uids, name=None, inplace=True):
         """
-        Returns a :term:`simple hypergraph` corresponding to self.
+        Removes the nodes from the Hypergraph.
+        If inplace=True, changes the existing Hypergraph. Otherwise, creates a new Hypergraph with the requested changes.
 
-        Warning
+        Parameters
+        ----------
+        node_uids : str | int | list[str | int]
+            node_uids
+        name : str, optional, default=None
+            The name of the new Hypergraph. Used only when inplace=False; ignored if inplace=True.
+        inplace : bool, optional, default=True
+            Whether to replace the current hypergraph with a new one.
+
+        Returns
         -------
-        Collapsing is no longer supported inside the toplexes method. Instead
-        generate a new collapsed hypergraph and compute the toplexes of the
-        new hypergraph.
+        Hypergraph
+        """
+        if not isinstance(node_uids, list):
+            node_uids = [node_uids]
+        return self._remove(node_uids, level=1, name=name, inplace=inplace)
+
+    def remove_incidences(self, incidence_uids, name=None, inplace=True):
+        """
+        Removes the incidences from the Hypergraph.
+        If inplace=True, changes the existing Hypergraph. Otherwise,
+        creates a new Hypergraph with the requested changes.
 
         Parameters
         ----------
-        name: str, optional, default = None
+        incidence_uids : tuple[str | int] | list[tuple[str | int]]
+            incidence_uids
+        name : str, optional, default=None
+            The name of the new Hypergraph. Used only when inplace=False;
+            ignored if inplace=True.
+        inplace : bool, optional, default=True
+            Whether to replace the current hypergraph with a new one.
+
+        Returns
+        -------
+        Hypergraph
         """
+        if not isinstance(incidence_uids, list):
+            incidence_uids = [incidence_uids]
+        return self._remove(incidence_uids, name=name, inplace=inplace)
 
-        thdict = {}
-        for e in self.edges:
-            thdict[e] = self.edges[e]
-
-        tops = []
-        for e in self.edges:
-            flag = True
-            old_tops = list(tops)
-            for top in old_tops:
-                if set(thdict[e]).issubset(thdict[top]):
-                    flag = False
-                    break
-
-                if set(thdict[top]).issubset(thdict[e]):
-                    tops.remove(top)
-            if flag:
-                tops += [e]
-        return self.restrict_to_edges(tops, name=name)
+    def _remove(self, uids, level=2, name=None, inplace=False):
+        """
+        Creates a hypergraph with nodes and/or edges indexed by keys removed.
+        More efficient for creating a restricted hypergraph if the
+        restricted set is greater than what is being removed.
+        If inplace=True, changes the existing Hypergraph.
+        Otherwise, creates a new Hypergraph with the requested changes.
+
+        Parameters
+        ----------
+        uids : list
+            list of uids from edges, nodes, or incidence pairs(listed as tuples)
+        level : int, optional, default=2
+            Enter 0 to remove edges.
+            Enter 1 to remove nodes.
+            Enter 2 to remove incidence pairs as tuples
+        name : str, optional, default=None
+            The name of the new Hypergraph. Used only when inplace=False;
+            ignored if inplace=True.
+        inplace : bool, default=False
+            Whether to replace the current hypergraph with the new one.
+
+        Returns
+        -------
+        Hypergraph
+
+        Notes
+        -----
+        Removal of a node or edge from the hypergraph will remove all
+        instances of these objects from incidence pairs and from the data.
+        Removal of an incidence pair, only removes that pair but does not
+        affect the user data attached to the edge and node in the pair.
+        """
+        if inplace:
+            df = self.incidences.properties
+            ep = self.edges.property_store
+            ndp = self.nodes.property_store
+        else:
+            df = self.incidences.to_dataframe
+            ep = self.edges.property_store.copy(deep=True)
+            ndp = self.nodes.property_store.copy(deep=True)
+        if level in [0, 1]:
+            hv = [ep, ndp][level]
+            df = df.drop(labels=uids, level=level, errors="ignore")
+            hv._data = hv._data.drop(labels=uids, errors="ignore")
+        else:
+            df = df.drop(labels=uids, errors="ignore")
+        return self._construct_hyp_from_stores(
+            df, edge_ps=ep, node_ps=ndp, name=name, inplace=inplace
+        )
+
+    def toplexes(self, return_hyp=False):
+        """
+        Computes a maximal collection of toplexes for the hypergraph.
+        A :term:`toplex` is a hyperedge, which is not contained in any other
+        hyperedge. If return_hyp=True, then returns the :term:`simple hypergraph` created by restricting
+        to the toplexes.
+
+        Parameters
+        ----------
+        return_hyp: bool, optional, default=False
 
+        Returns
+        -------
+        Hypergraph | list
+        """
+
+        def operate(a, b):
+            return np.mod(np.mod(a * b, 2) + b, 2)
+
+        df = self.incidence_dataframe().T
+        toplexes = []
+        while True:
+            edge_sizes = dict(df.sum(axis=1))
+            edges = np.array(
+                sorted(df.index, key=lambda x: edge_sizes[x], reverse=True)
+            )
+            toplexes.append(edges[0])
+            df = df.loc[edges]
+            mat = df.values
+            df = df.loc[edges[operate(mat[0], mat).sum(axis=1).nonzero()]]
+            if len(df.index) == 0:
+                break
+        if return_hyp:
+            return self.restrict_to_edges(toplexes)
+        return toplexes
+
+    #### hypergraph method using linegraph gotten from incidence store
     def is_connected(self, s=1, edges=False):
         """
-        Determines if hypergraph is :term:`s-connected <s-connected,
-        s-node-connected>`.
+        Determines if hypergraph is :term:`s-connected`.
 
         Parameters
         ----------
-        s: int, optional, default 1
+        s: int, optional, default=1
 
-        edges: boolean, optional, default = False
+        edges: boolean, optional, default=False
             If True, will determine if s-edge-connected.
             For s=1 s-edge-connected is the same as s-connected.
 
         Returns
         -------
         is_connected : boolean
 
@@ -1705,41 +2061,42 @@
                     singles.append(cdict[r])
         return singles
 
     def remove_singletons(self, name=None):
         """
         Constructs clone of hypergraph with singleton edges removed.
 
+        Parameters
+        ----------
+        name : str, optional, default=None
+
         Returns
         -------
-        new hypergraph : Hypergraph
-
+        Hypergraph
         """
         singletons = self.singletons()
         if len(singletons) > len(self.edges):
-            E = [e for e in self.edges if e not in singletons]
-            return self.restrict_to_edges(E, name=name)
-        else:
-            return self.remove(singletons, level=0, name=name)
+            edges = [e for e in self.edges if e not in singletons]
+            return self.restrict_to_edges(edges, name=name)
+        return self.remove_edges(singletons, name=name, inplace=False)
 
     def s_connected_components(self, s=1, edges=True, return_singletons=False):
         """
-        Returns a generator for the :term:`s-edge-connected components
-        <s-edge-connected component>`
-        or the :term:`s-node-connected components <s-connected component,
-        s-node-connected component>` of the hypergraph.
+        Returns a generator for the :term:`s-edge-connected component`
+        or the :term:`s-node-connected component` of the hypergraph.
 
         Parameters
         ----------
-        s : int, optional, default 1
+        s : int, optional, default=1
 
-        edges : boolean, optional, default = True
-            If True will return edge components, if False will return node
-            components
-        return_singletons : bool, optional, default = False
+        edges : boolean, optional, default=True
+            If True, return edge components; otherwise, return node components
+
+        return_singletons : bool, optional, default=False
+            If True, keep singletons. Otherwise, remove singletons
 
         Notes
         -----
         If edges=True, this method returns the s-edge-connected components as
         lists of lists of edge uids.
         An s-edge-component has the property that for any two edges e1 and e2
         there is a sequence of edges starting with e1 and ending with e2
@@ -1754,17 +2111,17 @@
         are the path components of the hypergraph.
 
         Example
         -------
             >>> S = {'A':{1,2,3},'B':{2,3,4},'C':{5,6},'D':{6}}
             >>> H = Hypergraph(S)
 
-            >>> list(H.s_components(edges=True))
+            >>> list(H.s_connected_components(edges=True))
             [{'C', 'D'}, {'A', 'B'}]
-            >>> list(H.s_components(edges=False))
+            >>> list(H.s_connected_components(edges=False))
             [{1, 2, 3, 4}, {5, 6}]
 
         Yields
         ------
         s_connected_components : iterator
             Iterator returns sets of uids of the edges (or nodes) in the
             s-edge(node) components of hypergraph.
@@ -1776,31 +2133,31 @@
                 continue
             yield c
 
     def s_component_subgraphs(
         self, s=1, edges=True, return_singletons=False, name=None
     ):
         """
-
         Returns a generator for the induced subgraphs of s_connected
         components. Removes singletons unless return_singletons is set to True.
         Computed using s-linegraph generated either by the hypergraph
         (edges=True) or its dual (edges = False)
 
         Parameters
         ----------
-        s : int, optional, default 1
+        s : int, optional, default=1
 
-        edges : boolean, optional, edges=False
+        edges : boolean, optional, default=False
             Determines if edge or node components are desired. Returns
             subgraphs equal to the hypergraph restricted to each set of
             nodes(edges) in the s-connected components or s-edge-connected
             components
-        return_singletons : bool, optional
-
+        return_singletons : bool, optional, default=False
+            If True, keep singletons in subgraph. Otherwise, remove singletons.
+        name : str, optional, default=None
         Yields
         ------
         s_component_subgraphs : iterator
             Iterator returns subgraphs generated by the edges (or nodes) in the
             s-edge(node) components of hypergraph.
 
         """
@@ -1810,15 +2167,15 @@
             if edges:
                 yield self.restrict_to_edges(c, name=f"{name or self.name}:{idx}")
             else:
                 yield self.restrict_to_nodes(c, name=f"{name or self.name}:{idx}")
 
     def s_components(self, s=1, edges=True, return_singletons=True):
         """
-        Same as s_connected_components
+        Same as :meth:`s_connected_components`
 
         See Also
         --------
         s_connected_components
         """
         return self.s_connected_components(
             s=s, edges=edges, return_singletons=return_singletons
@@ -1852,15 +2209,15 @@
         Same as :meth:`s_connected_components` with s=1, but nodes are returned
         by default. Return iterator.
 
         See Also
         --------
         s_connected_components
         """
-        return self.s_connected_components(s=1, edges=edges)
+        return self.s_connected_components(s=1, edges=edges, return_singletons=True)
 
     def component_subgraphs(self, return_singletons=False, name=None):
         """
         Same as :meth:`s_components_subgraphs` with s=1. Returns iterator.
 
         See Also
         --------
@@ -1868,57 +2225,56 @@
         """
         return self.s_component_subgraphs(
             return_singletons=return_singletons, name=name
         )
 
     def node_diameters(self, s=1):
         """
-        Returns the node diameters of the connected components in hypergraph.
+        Returns the node diameters of the connected components in the hypergraph.
 
         Parameters
         ----------
-        list of the diameters of the s-components and
-        list of the s-component nodes
+        s : int, optional, default=1
+
+        Returns
+        -------
+        maximum diameter, list of diameters, list of component : tuple[int, list, list]
+            maximum diameter, list of diameters (List of node_diameters for s-node component subgraphs in hypergraph),
+            list of component (List of the node uids in the s-node component subgraphs)
         """
         A, coldict = self.adjacency_matrix(s=s, index=True)
-        G = nx.from_scipy_sparse_matrix(A)
+        G = nx.from_scipy_sparse_array(A)
         diams = []
         comps = []
         for c in nx.connected_components(G):
             diamc = nx.diameter(G.subgraph(c))
             temp = set()
             for e in c:
                 temp.add(coldict[e])
             comps.append(temp)
             diams.append(diamc)
         loc = np.argmax(diams).tolist()
         return diams[loc], diams, comps
 
     def edge_diameters(self, s=1):
         """
-        Returns the edge diameters of the s_edge_connected component subgraphs
-        in hypergraph.
+        Returns the edge diameters of the s_edge_connected component subgraphs in the hypergraph.
 
         Parameters
         ----------
-        s : int, optional, default 1
+        s : int, optional, default=1
 
         Returns
         -------
-        maximum diameter : int
-
-        list of diameters : list
-            List of edge_diameters for s-edge component subgraphs in hypergraph
-
-        list of component : list
-            List of the edge uids in the s-edge component subgraphs.
-
+        maximum diameter, list of diameters, list of component : tuple[int, list, list]
+            maximum diameter, list of diameters (List of edge_diameters for s-edge component subgraphs in hypergraph),
+            list of component (List of the edge uids in the s-edge component subgraphs)
         """
         A, coldict = self.edge_adjacency_matrix(s=s, index=True)
-        G = nx.from_scipy_sparse_matrix(A)
+        G = nx.from_scipy_sparse_array(A)
         diams = []
         comps = []
         for c in nx.connected_components(G):
             diamc = nx.diameter(G.subgraph(c))
             temp = set()
             for e in c:
                 temp.add(coldict[e])
@@ -1930,15 +2286,15 @@
     def diameter(self, s=1):
         """
         Returns the length of the longest shortest s-walk between nodes in
         hypergraph
 
         Parameters
         ----------
-        s : int, optional, default 1
+        s : int, optional, default=1
 
         Returns
         -------
         diameter : int
 
         Raises
         ------
@@ -1948,31 +2304,29 @@
         Notes
         -----
         Two nodes are s-adjacent if they share s edges.
         Two nodes v_start and v_end are s-walk connected if there is a
         sequence of nodes v_start, v_1, v_2, ... v_n-1, v_end such that
         consecutive nodes are s-adjacent. If the graph is not connected,
         an error will be raised.
-
         """
-        A = self.adjacency_matrix(s=s)
-        G = nx.from_scipy_sparse_matrix(A)
-        if nx.is_connected(G):
-            return nx.diameter(G)
+        adj_matrix = self.adjacency_matrix(s=s)
+        graph = nx.from_scipy_sparse_array(adj_matrix)
+        if nx.is_connected(graph):
+            return nx.diameter(graph)
 
         raise HyperNetXError(f"Hypergraph is not s-connected. s={s}")
 
     def edge_diameter(self, s=1):
         """
-        Returns the length of the longest shortest s-walk between edges in
-        hypergraph
+        Returns the length of the longest shortest :term:`s-walk` between edges in the hypergraph
 
         Parameters
         ----------
-        s : int, optional, default 1
+        s : int, optional, default=1
 
         Return
         ------
         edge_diameter : int
 
         Raises
         ------
@@ -1985,34 +2339,33 @@
         Two nodes e_start and e_end are s-walk connected if there is a
         sequence of edges e_start, e_1, e_2, ... e_n-1, e_end such that
         consecutive edges are s-adjacent. If the graph is not connected, an
         error will be raised.
 
         """
         A = self.edge_adjacency_matrix(s=s)
-        G = nx.from_scipy_sparse_matrix(A)
+        G = nx.from_scipy_sparse_array(A)
         if nx.is_connected(G):
             return nx.diameter(G)
 
         raise HyperNetXError(f"Hypergraph is not s-connected. s={s}")
 
     def distance(self, source, target, s=1):
         """
-        Returns the shortest s-walk distance between two nodes in the
-        hypergraph.
+        Returns the shortest :term:`s-walk` distance between two nodes in the hypergraph.
 
         Parameters
         ----------
-        source : node.uid or node
+        source : str | int
             a node in the hypergraph
 
-        target : node.uid or node
+        target : str | int
             a node in the hypergraph
 
-        s : positive integer
+        s : positive int, optional, default=1
             the number of edges
 
         Returns
         -------
         s-walk distance : int
 
         See Also
@@ -2036,39 +2389,33 @@
         except (nx.NetworkXNoPath, nx.NodeNotFound):
             warnings.warn(f"No {s}-path between {source} and {target}")
             dist = np.inf
 
         return dist
 
     def edge_distance(self, source, target, s=1):
-        """XX TODO: still need to return path and translate into user defined
-        nodes and edges Returns the shortest s-walk distance between two edges
-        in the hypergraph.
+        """
+        Returns the shortest :term:`s-walk` distance between two edges in the hypergraph.
 
         Parameters
         ----------
-        source : edge.uid or edge
+        source : str | int
             an edge in the hypergraph
 
-        target : edge.uid or edge
+        target : str | int
             an edge in the hypergraph
 
-        s : positive integer
+        s : positive int, optional, default=1
             the number of intersections between pairwise consecutive edges
 
-        TODO: add edge weights
-        weight : None or string, optional, default = None
-            if None then all edges have weight 1. If string then edge attribute
-            string is used if available.
-
 
         Returns
         -------
-        s- walk distance : the shortest s-walk edge distance
-            A shortest s-walk is computed as a sequence of edges,
+        s-walk distance : int | float
+            The shortest s-walk edge distance. A shortest s-walk is computed as a sequence of edges;
             the s-walk distance is the number of edges in the sequence
             minus 1. If no such path exists returns np.inf.
 
         See Also
         --------
         distance
 
@@ -2078,103 +2425,69 @@
             An s-walk between edges is a sequence of edges such that
             consecutive pairwise edges intersect in at least s nodes. The
             length of the shortest s-walk is 1 less than the number of edges
             in the path sequence.
 
             Uses the networkx shortest_path_length method on the graph
             generated by the s-edge_adjacency matrix.
-
         """
         g = self.get_linegraph(s=s, edges=True)
         try:
             edge_dist = nx.shortest_path_length(g, source, target)
         except (nx.NetworkXNoPath, nx.NodeNotFound):
             warnings.warn(f"No {s}-path between {source} and {target}")
             edge_dist = np.inf
 
         return edge_dist
 
-    def incidence_dataframe(
-        self, sort_rows=False, sort_columns=False, cell_weights=True
-    ):
-        """
-        Returns a pandas dataframe for hypergraph indexed by the nodes and
-        with column headers given by the edge names.
-
-        Parameters
-        ----------
-        sort_rows : bool, optional, default =True
-            sort rows based on hashable node names
-        sort_columns : bool, optional, default =True
-            sort columns based on hashable edge names
-        cell_weights : bool, optional, default =True
-
-        """
-
-        ## An entity dataframe is already an incidence dataframe.
-        df = self.E.dataframe.pivot(
-            index=self.E._data_cols[1],
-            columns=self.E._data_cols[0],
-            values=self.E._cell_weight_col,
-        ).fillna(0)
-
-        if sort_rows:
-            df = df.sort_index("index")
-        if sort_columns:
-            df = df.sort_index("columns")
-        if not cell_weights:
-            df[df > 0] = 1
-
-        return df
-
+    #### Needs to create stores then hypergraph.
     @classmethod
-    @warn_nwhy
-    def from_bipartite(cls, B, set_names=("edges", "nodes"), name=None, **kwargs):
+    #### Need to preserve graph properties in data
+    def from_bipartite(cls, B, node_id=1, name=None, **kwargs):
         """
-        Static method creates a Hypergraph from a bipartite graph.
+        Static method creates a Hypergraph from a NetworkX bipartite graph.
+        Still to come: capturing edge and node properties from the graph for use
+        in the hypergraph.
 
         Parameters
         ----------
 
         B: nx.Graph()
             A networkx bipartite graph. Each node in the graph has a property
             'bipartite' taking the value of 0 or 1 indicating a 2-coloring of
             the graph.
 
-        set_names: iterable of length 2, optional, default = ['edges','nodes']
-            Category names assigned to the graph nodes associated to each
-            bipartite set
+        node_id : int
+            bipartite value assigned to graph nodes that will be hypergraph
+            edges
 
         name: hashable, optional
 
         Returns
         -------
-         : Hypergraph
+        Hypergraph
 
         Notes
         -----
         A partition for the nodes in a bipartite graph generates a hypergraph.
 
             >>> import networkx as nx
             >>> B = nx.Graph()
             >>> B.add_nodes_from([1, 2, 3, 4], bipartite=0)
             >>> B.add_nodes_from(['a', 'b', 'c'], bipartite=1)
-            >>> B.add_edges_from([(1, 'a'), (1, 'b'), (2, 'b'), (2, 'c'), /
-                (3, 'c'), (4, 'a')])
-            >>> H = Hypergraph.from_bipartite(B)
-            >>> H.nodes, H.edges
-            # output: (EntitySet(_:Nodes,[1, 2, 3, 4],{}), /
-            # EntitySet(_:Edges,['b', 'c', 'a'],{}))
-
+            >>> B.add_edges_from([(1, 'a'), (1, 'b'), (2, 'b'), (2, 'c'), (3, 'c'), (4, 'a')])
+            >>> H = Hypergraph.from_bipartite(B, nodes=1)
+            >>> list(H.nodes), list(H.edges)
+            (['a', 'b', 'c'], [1, 2, 3, 4])
         """
 
         edges = []
         nodes = []
         for n, d in B.nodes(data=True):
-            if d["bipartite"] == 1:
+            if d["bipartite"] == node_id:
                 nodes.append(n)
             else:
                 edges.append(n)
 
         if not bipartite.is_bipartite_node_set(B, nodes):
             raise HyperNetXError(
                 "Error: Method requires a 2-coloring of a bipartite graph."
@@ -2182,57 +2495,46 @@
 
         elist = []
         for e in list(B.edges):
             if e[0] in edges:
                 elist.append([e[0], e[1]])
             else:
                 elist.append([e[1], e[0]])
-        df = pd.DataFrame(elist, columns=set_names)
+        df = pd.DataFrame(elist)
         return Hypergraph(df, name=name, **kwargs)
 
     @classmethod
     def from_incidence_matrix(
         cls,
         M,
-        node_names=None,
-        edge_names=None,
-        node_label="nodes",
-        edge_label="edges",
         name=None,
-        key=None,
         **kwargs,
     ):
         """
-        Same as from_numpy_array.
+        Accepts numpy.matrix or scipy.sparse matrix
         """
-        return Hypergraph.from_numpy_array(
-            M,
-            node_names=node_names,
-            edge_names=edge_names,
-            node_label=node_label,
-            edge_label=edge_label,
-            name=name,
-            key=key,
-        )
+        mat = coo_matrix(M)
+        edges = mat.col
+        nodes = mat.row
+        weights = mat.data
+        df = pd.DataFrame({"edges": edges, "nodes": nodes, "weights": weights})
+        return Hypergraph(df, cell_weight_col="weights", name=name, **kwargs)
 
     @classmethod
-    @warn_nwhy
     def from_numpy_array(
         cls,
         M,
         node_names=None,
         edge_names=None,
-        node_label="nodes",
-        edge_label="edges",
         name=None,
         key=None,
         **kwargs,
     ):
         """
-        Create a hypergraph from a real valued matrix represented as a 2 dimensionsl numpy array.
+        Create a hypergraph from a real valued matrix represented as a 2 dimensional numpy array.
         The matrix is converted to a matrix of 0's and 1's so that any truthy cells are converted to 1's and
         all others to 0's.
 
         Parameters
         ----------
         M : real valued array-like object, 2 dimensions
             representing a real valued matrix with rows corresponding to nodes and columns to edges
@@ -2291,65 +2593,39 @@
         else:
             edgenames = np.array([f"e{jdx}" for jdx in range(M.shape[1])])
 
         df = pd.DataFrame(M, columns=edgenames, index=nodenames)
         return Hypergraph.from_incidence_dataframe(df, name=name)
 
     @classmethod
-    @warn_nwhy
     def from_incidence_dataframe(
         cls,
         df,
-        columns=None,
-        rows=None,
-        edge_col: str = "edges",
-        node_col: str = "nodes",
         name=None,
         fillna=0,
-        transpose=False,
-        transforms=[],
         key=None,
         return_only_dataframe=False,
         **kwargs,
     ):
         """
         Create a hypergraph from a Pandas Dataframe object, which has values equal
         to the incidence matrix of a hypergraph. Its index will identify the nodes
         and its columns will identify its edges.
 
         Parameters
         ----------
         df : Pandas.Dataframe
             a real valued dataframe with a single index
 
-        columns : (optional) list, default = None
-            restricts df to the columns with headers in this list.
-
-        rows : (optional) list, default = None
-            restricts df to the rows indexed by the elements in this list.
-
         name : (optional) string, default = None
 
         fillna : float, default = 0
             a real value to place in empty cell, all-zero columns will not
             generate an edge.
 
-        transpose : (optional) bool, default = False
-            option to transpose the dataframe, in this case df.Index will
-            identify the edges and df.columns will identify the nodes, transpose is
-            applied before transforms and key
-
-        transforms : (optional) list, default = []
-            optional list of transformations to apply to each column,
-            of the dataframe using pd.DataFrame.apply().
-            Transformations are applied in the order they are
-            given (ex. abs). To apply transforms to rows or for additional
-            functionality, consider transforming df using pandas.DataFrame
-            methods prior to generating the hypergraph.
-
         key : (optional) function, default = None
             boolean function to be applied to dataframe. will be applied to
             entire dataframe.
 
         return_only_dataframe : (optional) bool, default = False
             to use the incidence_dataframe with cell_properties or properties, set this
             to true and use it as the setsystem in the Hypergraph constructor.
@@ -2357,50 +2633,178 @@
         See also
         --------
         from_numpy_array
 
 
         Returns
         -------
-        : Hypergraph
-
+        Hypergraph | pd.DataFrame
         """
 
         if not isinstance(df, pd.DataFrame):
             raise HyperNetXError("Error: Input object must be a pandas dataframe.")
 
-        if columns:
-            df = df[columns]
-        if rows:
-            df = df.loc[rows]
-
         df = df.fillna(fillna)
-        if transpose:
-            df = df.transpose()
 
-        for t in transforms:
-            df = df.apply(t)
         if key:
             mat = key(df.values) * 1
         else:
             mat = df.values * 1
 
         cols = df.columns
         rows = df.index
         CM = coo_matrix(mat)
         c1 = CM.row
         c1 = [rows[c1[idx]] for idx in range(len(c1))]
         c2 = CM.col
         c2 = [cols[c2[idx]] for idx in range(len(c2))]
         c3 = CM.data
 
-        dfnew = pd.DataFrame({edge_col: c2, node_col: c1, "cell_weights": c3})
-        if return_only_dataframe == True:
+        dfnew = pd.DataFrame({"edges": c2, "nodes": c1, "weight": c3})
+        if return_only_dataframe is True:
             return dfnew
         else:
-            return Hypergraph(
-                dfnew,
-                edge_col=edge_col,
-                node_col=node_col,
-                weights="cell_weights",
-                name=None,
-            )
+            return Hypergraph(dfnew, cell_weight_col="weight", name=name, **kwargs)
+
+    def __add__(self, other):
+        """
+        Concatenate incidences from two hypergraphs, removing duplicates and
+        dropping duplicate property data in the order of addition.
+
+        Parameters
+        ----------
+        other : Hypergraph
+
+        Returns
+        -------
+        Hypergraph
+
+        """
+        return self.sum(other)
+
+    def __sub__(self, other):
+        """
+        Concatenate incidences from two hypergraphs, removing duplicates and
+        dropping duplicate property data in the order of addition.
+
+        Parameters
+        ----------
+        other : Hypergraph
+
+        Returns
+        -------
+        Hypergraph
+
+        """
+        return self.difference(other)
+
+    def sum(self, other, name=None):
+        """
+        Hypergraph obtained by joining incidences from self and other.
+        Removes duplicates and uses properties of self.
+
+        Parameters
+        ----------
+        other : Hypergraph
+
+        Returns
+        -------
+        Hypergraph
+
+        """
+        incidence_df = self._combine_properties_dataframes(
+            self.incidences.to_dataframe, other.incidences.to_dataframe
+        )
+        edges_data = self._combine_properties_dataframes(
+            self.edges.to_dataframe, other.edges.to_dataframe
+        )
+        nodes_data = self._combine_properties_dataframes(
+            self.nodes.to_dataframe, other.nodes.to_dataframe
+        )
+
+        return self._construct_hyp_from_stores(
+            incidence_df,
+            edge_ps=PropertyStore(edges_data),
+            node_ps=PropertyStore(nodes_data),
+            name=name,
+        )
+
+    def _combine_properties_dataframes(self, df1, df2):
+        df = pd.concat([df1, df2])
+        return df[~df.index.duplicated(keep="first")]
+
+    def difference(self, other, name=None):
+        """
+        Hypergraph obtained by restricting to incidences in self but not in other.
+
+        Parameters
+        ----------
+        other : Hypergraph
+        name : str, optional, default = None
+
+        Returns
+        -------
+        Hypergraph
+        """
+        ndx = list(self.incidences.items.difference(other.incidences.items))
+        ndf = self.incidences.to_dataframe.loc[ndx]
+        return self._construct_hyp_from_stores(ndf, name=name)
+
+    def intersection(self, other, name=None):
+        """
+        Returns a hypergraph created by restricting to incidence pairs contained in both self and other.
+        Properties inherited from self.
+
+        Parameters
+        ----------
+        other : Hypergraph
+        name : str, optional, default=None
+
+        Returns
+        -------
+        Hypergraph
+        """
+        nodes_intersection = list(
+            self.incidences.items.intersection(other.incidences.items)
+        )
+        incidence_df = self.incidences.to_dataframe.loc[nodes_intersection]
+        return self._construct_hyp_from_stores(incidence_df, name=name)
+
+    def union(self, other, name=None):
+        """
+        The hypergraph gotten by joining incidence pairs contained in
+        self and other. Duplicates removed. Properties inherited from self.
+        Same as :meth:`sum`
+
+        Parameters
+        ----------
+        other : Hypergraph
+        name : str, optional, default=None
+
+        Returns
+        -------
+        Hypergraph
+        """
+        return self.sum(other, name=name)
+
+
+def _agg_rows(df, groupby, rule_dict=None):
+    """
+    Helper method for collapsing nodes and edges in hypergraph
+
+    Parameters
+    ----------
+    df : pandas.DataFrame
+    groupby : index or columns aggregating on
+    rule_dict : dict, optional, defaults as 'first' for all keys
+        dictionary keyed by df columns where values are the
+        aggregation rules e.g. 'first', 'sum', 'last'
+
+    Returns
+    -------
+    pandas.DataFrame
+    """
+    default_agg = {col: "first" for col in df.columns}
+    for k, v in rule_dict.items():
+        if k in default_agg:
+            default_agg[k] = v
+    return df.reset_index().groupby(groupby).agg(default_agg)
```

### Comparing `hypernetx-2.2.0/hypernetx/drawing/rubber_band.py` & `hypernetx-2.3.0/hypernetx/drawing/rubber_band.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     Helper function to use a NetwrokX-like graph layout algorithm on a Hypergraph
 
     The hypergraph is converted to a bipartite graph, allowing the usual graph layout
     techniques to be applied.
 
     Parameters
     ----------
-    H: Hypergraph
+    H: hnx.Hypergraph
         the entity to be drawn
     G: Graph
         an additional set of links to consider during the layout process
     layout: function
         the layout algorithm which accepts a NetworkX graph and keyword arguments
     kwargs: dict
         Keyword arguments are passed through to the layout algorithm
@@ -68,15 +68,15 @@
 
     This function iterates over the hyper edges and finds the most distant
     pair of points given the positions provided. Then, the node radius is a fraction
     of the median of this distance take across all hyper-edges.
 
     Parameters
     ----------
-    H: Hypergraph
+    H: hnx.Hypergraph
         the entity to be drawn
     pos: dict
         mapping of node and edge positions to R^2
 
     Returns
     -------
     float
@@ -100,15 +100,15 @@
     the return value of draw_hyper_edges.
 
     The label will be draw on the least curvy part of the polygon, and will be
     aligned parallel to the orientation of the polygon where it is drawn.
 
     Parameters
     ----------
-    H: Hypergraph
+    H: hnx.Hypergraph
         the entity to be drawn
     polys: PolyCollection
         collection of polygons returned by draw_hyper_edges
     labels: dict
         mapping of node id to string label
     ax: Axis
         matplotlib axis on which the plot is rendered
@@ -120,15 +120,15 @@
 
     params = transpose_inflated_kwargs(inflate_kwargs(H.edges, kwargs))
 
     for edge, path, params in zip(H.edges, polys.get_paths(), params):
         s = labels.get(edge, edge)
 
         theta = 0
-        xy = pos[edge]
+        xy = None
 
         if edge_labels_on_edge:
             # calculate the xy location of the annotation
             # this is the midpoint of the pair of adjacent points the most distant
             d = ((path.vertices[:-1] - path.vertices[1:]) ** 2).sum(axis=1)
             i = d.argmax()
 
@@ -137,31 +137,33 @@
             theta = 360 * np.arctan2(y, x) / (2 * np.pi)
             theta = (theta + 360) % 360
 
             while theta > 90:
                 theta -= 180
 
             xy = (x1 + x2) / 2
+        else:
+            xy = pos[edge]
 
         # the string is a comma separated list of the edge uid
         ax.annotate(s, xy, rotation=theta, ha="center", va="center", **params)
 
 
-def layout_hyper_edges(H, pos, node_radius={}, dr=None):
+def layout_hyper_edges(H, pos, node_radius={}, dr=None, contain_hyper_edges=False):
     """
     Draws a convex hull for each edge in H.
 
     Position of the nodes in the graph is specified by the position dictionary,
     pos. Convex hulls are spaced out such that if one set contains another, the
     convex hull will surround the contained set. The amount of spacing added
     between hulls is specified by the parameter, dr.
 
     Parameters
     ----------
-    H: Hypergraph
+    H: hnx.Hypergraph
         the entity to be drawn
     pos: dict
         mapping of node and edge positions to R^2
     node_radius: dict
         mapping of node to R^1 (radius of each node)
     dr: float
         the spacing between concentric rings
@@ -181,44 +183,50 @@
 
     dr = dr or r0
 
     levels = get_set_layering(H)
 
     radii = {
         v: {v: i for i, v in enumerate(sorted(e, key=levels.get))}
-        for v, e in H.dual().edges.elements.items()
+        for v, e in H.nodes.memberships.items()
     }
 
     def get_padded_hull(uid, edge):
         # make sure the edge contains at least one node
         if len(edge):
-            points = np.vstack(
-                [
-                    cp * (node_radius.get(v, r0) + dr * (2 + radii[v][uid])) + pos[v]
-                    for v in edge
-                ]
-            )
+            points = [
+                cp * (node_radius.get(v, r0) + dr * (2 + radii[v][uid])) + pos[v]
+                for v in edge
+            ]
+
+            if contain_hyper_edges:
+                points.append(cp * r0 + pos[uid])
+
+            points = np.vstack(points)
+
         # if not, draw an empty edge centered around the location of the edge node (in the bipartite graph)
         else:
             points = 4 * r0 * cp + pos[uid]
 
         hull = ConvexHull(points)
 
         return hull.points[hull.vertices]
 
     return [get_padded_hull(uid, list(H.edges[uid])) for uid in H.edges]
 
 
-def draw_hyper_edges(H, pos, ax=None, node_radius={}, dr=None, **kwargs):
+def draw_hyper_edges(
+    H, pos, ax=None, node_radius={}, contain_hyper_edges=False, dr=None, **kwargs
+):
     """
     Draws a convex hull around the nodes contained within each edge in H
 
     Parameters
     ----------
-    H: Hypergraph
+    H: hnx.Hypergraph
         the entity to be drawn
     pos: dict
         mapping of node and edge positions to R^2
     node_radius: dict
         mapping of node to R^1 (radius of each node)
     dr: float
         the spacing between concentric rings
@@ -228,15 +236,17 @@
         keyword arguments, e.g., linewidth, facecolors, are passed through to the PolyCollection constructor
 
     Returns
     -------
     PolyCollection
         a Matplotlib PolyCollection that can be further styled
     """
-    points = layout_hyper_edges(H, pos, node_radius=node_radius, dr=dr)
+    points = layout_hyper_edges(
+        H, pos, node_radius=node_radius, dr=dr, contain_hyper_edges=contain_hyper_edges
+    )
 
     polys = PolyCollection(points, **inflate_kwargs(H.edges, kwargs))
 
     (ax or plt.gca()).add_collection(polys)
 
     return polys
 
@@ -250,15 +260,15 @@
     can be specified as a dictionary where node_radius[v] is the radius. If a
     node is missing from this dictionary, or the node_radius is not specified at
     all, a sensible default radius is chosen based on distances between nodes
     given by pos.
 
     Parameters
     ----------
-    H: Hypergraph
+    H: hnx.Hypergraph
         the entity to be drawn
     pos: dict
         mapping of node and edge positions to R^2
     node_radius: dict
         mapping of node to R^1 (radius of each node)
     r0: float
         minimum distance that concentric rings start from the node position
@@ -300,15 +310,15 @@
     a node to its custom label. By default, the label is the string
     representation of the node.
 
     Keyword arguments are passed through to Matplotlib's annotate function.
 
     Parameters
     ----------
-    H: Hypergraph
+    H: hnx.Hypergraph
         the entity to be drawn
     pos: dict
         mapping of node and edge positions to R^2
     node_radius: dict
         mapping of node to R^1 (radius of each node)
     ax: Axis
         matplotlib axis on which the plot is rendered
@@ -356,14 +366,15 @@
     node_labels={},
     node_labels_kwargs={},
     with_edge_labels=True,
     with_node_labels=True,
     node_label_alpha=0.35,
     edge_label_alpha=0.35,
     with_additional_edges=None,
+    contain_hyper_edges=False,
     additional_edges_kwargs={},
     return_pos=False,
 ):
     """
     Draw a hypergraph as a Matplotlib figure
 
     By default this will draw a colorful "rubber band" like hypergraph, where
@@ -402,15 +413,15 @@
     implies that the sets intersect, but sometimes sets overlap if there is no
     intersection. It is not possible, in general, to draw a "correct" hypergraph
     this way for an arbitrary hypergraph, in the same way that not all graphs
     have planar drawings.
 
     Parameters
     ----------
-    H: Hypergraph
+    H: hnx.Hypergraph
         the entity to be drawn
     pos: dict
         mapping of node and edge positions to R^2
     with_color: bool
         set to False to disable color cycling of edges
     with_node_counts: bool
         set to True to replace the label for collapsed nodes with the number of elements
@@ -438,14 +449,19 @@
         set to False to make edge labels invisible
     with_node_labels: bool
         set to False to make node labels invisible
     node_label_alpha: float
         the transparency (alpha) of the box behind text drawn in the figure for node labels
     edge_label_alpha: float
         the transparency (alpha) of the box behind text drawn in the figure for edge labels
+    with_additional_edges: networkx.Graph
+        ...
+    contain_hyper_edges: bool
+        whether the rubber band shoudl be drawn around the location of the edge in the bipartite graph. This may be invisibile unless "with_additional_edges" contains this information.
+
     """
 
     ax = ax or plt.gca()
 
     if pos is None:
         pos = layout_node_link(H, with_additional_edges, layout=layout, **layout_kwargs)
 
@@ -464,15 +480,22 @@
 
     # for convenience, we are using setdefault to mutate the argument
     # however, we need to copy this to prevent side-effects
     edges_kwargs = edges_kwargs.copy()
     edges_kwargs.setdefault("edgecolors", plt.cm.tab10(np.arange(len(H.edges)) % 10))
     edges_kwargs.setdefault("facecolors", "none")
 
-    polys = draw_hyper_edges(H, pos, node_radius=node_radius, ax=ax, **edges_kwargs)
+    polys = draw_hyper_edges(
+        H,
+        pos,
+        node_radius=node_radius,
+        ax=ax,
+        contain_hyper_edges=contain_hyper_edges,
+        **edges_kwargs
+    )
 
     if with_additional_edges:
         nx.draw_networkx_edges(
             with_additional_edges,
             pos=pos,
             ax=ax,
             **inflate_kwargs(with_additional_edges.edges(), additional_edges_kwargs)
```

### Comparing `hypernetx-2.2.0/hypernetx/drawing/two_column.py` & `hypernetx-2.3.0/hypernetx/drawing/two_column.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     Within a connected component, the spectral ordering of the bipartite graph
     provides a quick and dirty ordering that minimizes edge crossings in the
     diagram.
 
     Parameters
     ----------
-    H: Hypergraph
+    H: hnx.Hypergraph
         the entity to be drawn
     spacing: float
         amount of whitespace between disconnected components
     """
     offset = 0
     pos = {}
 
@@ -59,15 +59,15 @@
     Renders hyper edges for the two column layout.
 
     Each node-hyper edge membership is rendered as a line connecting the node
     in the left column to the edge in the right column.
 
     Parameters
     ----------
-    H: Hypergraph
+    H: hnx.Hypergraph
         the entity to be drawn
     pos: dict
         mapping of node and edge positions to R^2
     ax: Axis
         matplotlib axis on which the plot is rendered
     kwargs: dict
         keyword arguments passed to matplotlib.LineCollection
@@ -97,15 +97,15 @@
     H, pos, labels={}, with_node_labels=True, with_edge_labels=True, ax=None
 ):
     """
     Renders hyper labels (nodes and edges) for the two column layout.
 
     Parameters
     ----------
-    H: Hypergraph
+    H: hnx.Hypergraph
         the entity to be drawn
     pos: dict
         mapping of node and edge positions to R^2
     labels: dict
         custom labels for nodes and edges can be supplied
     with_node_labels: bool
         False to disable node labels
@@ -153,15 +153,15 @@
 
     The order of nodes and edges is optimized to reduce line crossings between
     the two columns. Spacing between disconnected components is adjusted to make
     the diagram easier to read, by reducing the angle of the lines.
 
     Parameters
     ----------
-    H: Hypergraph
+    H: hnx.Hypergraph
         the entity to be drawn
     with_node_labels: bool
         False to disable node labels
     with_edge_labels: bool
         False to disable edge labels
     with_node_counts: bool
         set to True to label collapsed nodes with number of elements
```

### Comparing `hypernetx-2.2.0/hypernetx/drawing/util.py` & `hypernetx-2.3.0/hypernetx/drawing/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 def get_line_graph(H, collapse=True):
     """
     Computes the line graph, a directed graph, where a directed edge (u, v)
     exists if the edge u is a subset of the edge v in the hypergraph.
 
     Parameters
     ----------
-    H: Hypergraph
+    H: hnx.Hypergraph
         the entity to be drawn
     collapse: bool
         True if edges should be added if hyper edges are identical
 
     Returns
     -------
     networkx.DiGraph
@@ -119,15 +119,15 @@
     Computes a layering of the edges in the hyper graph.
 
     In this layering, each edge is assigned a level. An edge u will be above
     (e.g., have a smaller level value) another edge v if v is a subset of u.
 
     Parameters
     ----------
-    H: Hypergraph
+    H: hnx.Hypergraph
         the entity to be drawn
     collapse: bool
         True if edges should be added if hyper edges are identical
 
     Returns
     -------
     dict
```

### Comparing `hypernetx-2.2.0/hypernetx/reports/descriptive_stats.py` & `hypernetx-2.3.0/hypernetx/reports/descriptive_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     * Node degree distribution
     * Component size distribution
     * Toplex size distribution
     * Diameter
 
 Also computes general hypergraph information: number of nodes, edges, cells, aspect ratio, incidence matrix density
 """
+
 from collections import Counter
 import numpy as np
 from hypernetx.utils.decorators import not_implemented_for
 
 
 def centrality_stats(X):
     """
@@ -38,15 +39,15 @@
 
 def edge_size_dist(H, aggregated=False):
     """
     Computes edge sizes of a hypergraph.
 
     Parameters
     ----------
-    H : Hypergraph
+    H: hnx.Hypergraph
     aggregated :
         If aggregated is True, returns a dictionary of
         edge sizes and counts. If aggregated is False, returns a
         list of edge sizes in H.
 
     Returns
     -------
@@ -62,15 +63,15 @@
 
 def degree_dist(H, aggregated=False):
     """
     Computes degrees of nodes of a hypergraph.
 
     Parameters
     ----------
-    H : Hypergraph
+    H: hnx.Hypergraph
     aggregated :
         If aggregated is True, returns a dictionary of
         degrees and counts. If aggregated is False, returns a
         list of degrees in H.
 
     Returns
     -------
@@ -86,15 +87,15 @@
 
 def comp_dist(H, aggregated=False):
     """
     Computes component sizes, number of nodes.
 
     Parameters
     ----------
-    H : Hypergraph
+    H: hnx.Hypergraph
     aggregated :
         If aggregated is True, returns a dictionary of
         component sizes (number of nodes) and counts. If aggregated
         is False, returns a list of components sizes in H.
 
     Returns
     -------
@@ -116,15 +117,15 @@
 
 def s_comp_dist(H, s=1, aggregated=False, edges=True, return_singletons=True):
     """
     Computes s-component sizes, counting nodes or edges.
 
     Parameters
     ----------
-    H : Hypergraph
+    H: hnx.Hypergraph
     s : positive integer, default is 1
     aggregated :
         If aggregated is True, returns a dictionary of
         s-component sizes and counts in H. If aggregated is
         False, returns a list of s-component sizes in H.
     edges :
         If edges is True, the component size is number of edges.
@@ -158,15 +159,15 @@
 def toplex_dist(H, aggregated=False):
     """
 
     Computes toplex sizes for hypergraph H.
 
     Parameters
     ----------
-    H : Hypergraph
+    H: hnx.Hypergraph
     aggregated :
         If aggregated is True, returns a dictionary of
         toplex sizes and counts in H. If aggregated
         is False, returns a list of toplex sizes in H.
 
     Returns
     -------
@@ -180,15 +181,15 @@
         return distr
 
 
 def s_node_diameter_dist(H):
     """
     Parameters
     ----------
-    H : Hypergraph
+    H: hnx.Hypergraph
 
     Returns
     -------
      s_node_diameter_dist : list
         List of s-node-diameters for hypergraph H starting with s=1
         and going up as long as the hypergraph is s-node-connected
     """
@@ -200,15 +201,15 @@
     return diams
 
 
 def s_edge_diameter_dist(H):
     """
     Parameters
     ----------
-    H : Hypergraph
+    H: hnx.Hypergraph
 
     Returns
     -------
      s_edge_diameter_dist : list
         List of s-edge-diameters for hypergraph H starting with s=1
         and going up as long as the hypergraph is s-edge-connected
     """
@@ -222,15 +223,15 @@
 
 def info(H, node=None, edge=None):
     """
     Print a summary of simple statistics for H
 
     Parameters
     ----------
-    H : Hypergraph
+    H: hnx.Hypergraph
     obj : optional
         either a node or edge uid from the hypergraph
     dictionary : optional
         If True then returns the info as a dictionary rather
         than a string
         If False (default) returns the info as a string
 
@@ -266,15 +267,15 @@
 
 def info_dict(H, node=None, edge=None):
     """
     Create a summary of simple statistics for H
 
     Parameters
     ----------
-    H : Hypergraph
+    H: hnx.Hypergraph
     obj : optional
         either a node or edge uid from the hypergraph
 
     Returns
     -------
      info_dict : dict
         Returns a dictionary of statistics of the size,
@@ -330,15 +331,15 @@
         * comp edges list = s_comp_dist(H, s=1, edges=True)
         * comp edges dist = centrality_stats(s_comp_dist(H, s=1, edges=True))
         * comp edges hist = Counter(s_comp_dist(H, s=1, edges=True))
         * num comps = len(s_comp_dist(H))
 
     Parameters
     ----------
-    H : Hypergraph
+    H: hnx.Hypergraph
 
     Returns
     -------
      dist_stats : dict
         Dictionary which keeps track of each of the above items (e.g., basic['nrows'] = the number of nodes in H)
     """
     stats = H._state_dict.get("dist_stats", None)
```

### Comparing `hypernetx-2.2.0/hypernetx/utils/__init__.py` & `hypernetx-2.3.0/hypernetx/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from hypernetx.utils.extras import (
     HNXCount,
     DefaultOrderedDict,
     remove_row_duplicates,
-    create_labels,
     reverse_dictionary,
 )
 from hypernetx.utils.decorators import not_implemented_for
 from hypernetx.utils.toys.harrypotter import HarryPotter
 from hypernetx.utils.toys.gene_data import GeneData
 from hypernetx.utils.toys.lesmis import LesMis, lesmis_hypergraph_from_df, book_tour
 from hypernetx.utils.toys.transmission_problem import TransmissionProblem
 
 __all__ = [
     "HNXCount",
     "DefaultOrderedDict",
     "remove_row_duplicates",
-    "create_labels",
     "reverse_dictionary",
     "not_implemented_for",
     "HarryPotter",
     "GeneData",
     "LesMis",
     "lesmis_hypergraph_from_df",
     "book_tour",
```

### Comparing `hypernetx-2.2.0/hypernetx/utils/decorators.py` & `hypernetx-2.3.0/hypernetx/utils/decorators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import warnings
 from functools import wraps
 
 from decorator import decorator
 
 import hypernetx as hnx
-from hypernetx.exception import NWHY_WARNING
 
-__all__ = ["not_implemented_for", "warn_nwhy", "warn_to_be_deprecated"]
+
+__all__ = ["not_implemented_for", "warn_to_be_deprecated"]
 
 
 def not_implemented_for(*object_types):
     """Decorator to hypergraph methods to mark algorithms as not implemented
     Ruthlessly copied from NetworkX.
 
     Parameters
@@ -58,40 +58,14 @@
             raise hnx.HyperNetXNotImplementedError(msg)
         else:
             return not_implemented_for_func(*args, **kwargs)
 
     return _not_implemented_for
 
 
-def warn_nwhy(func):
-    """Decorator for methods that allow the deprecated `use_nwhy` kwarg
-
-    As of HyperNetX v2.0.0, NWHy C++ backend is no longer supported.
-    Public references to the deprecated NWHy add-on will be removed from the Hypergraph
-    API in a future release.
-
-    Warns
-    -----
-    FutureWarning
-        If kwargs contain ``use_nwhy=True``
-    """
-
-    @wraps(func)
-    def wrapper(*args, **kwargs):
-        if kwargs.get("use_nwhy"):
-            kwargs.update(use_nwhy=False)
-            warnings.simplefilter("always", FutureWarning)
-            warnings.warn(NWHY_WARNING, FutureWarning, stacklevel=2)
-            warnings.simplefilter("default", FutureWarning)
-
-        return func(*args, **kwargs)
-
-    return wrapper
-
-
 def warn_to_be_deprecated(func):
     """Decorator for methods that are to be deprecated
 
     Public references to deprecated methods or functions will be removed from the Hypergraph API in a future release.
 
     Warns
     -----
```

### Comparing `hypernetx-2.2.0/hypernetx/utils/extras.py` & `hypernetx-2.3.0/hypernetx/utils/extras.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from collections import OrderedDict, defaultdict
+from collections import OrderedDict
 from collections.abc import Callable
 import numpy as np
 import pandas as pd
 from hypernetx import HyperNetXError
 
 __all__ = [
     "HNXCount",
     "DefaultOrderedDict",
     "remove_row_duplicates",
-    "create_labels",
     "reverse_dictionary",
 ]
 
 
 class HNXCount:
     def __init__(self, init=0):
         self.init = init
@@ -149,50 +148,14 @@
         data = np.reshape(data, (len(data), 1))
     else:
         data = np.array(list(G.keys()))
 
     return data, G
 
 
-def create_labels(
-    num_edges,
-    num_nodes,
-    edgeprefix="e",
-    nodeprefix="v",
-    edgelabel="Edges",
-    nodelabel="Nodes",
-):
-    """
-    Creates default labels for static entity sets derived without labels
-
-    Parameters
-    ----------
-    num_edges : int
-
-    num_nodes : int
-
-    edgeprefix : str, optional, default : 'e'
-
-    nodeprefix : str, optional, default : 'v'
-
-    edgelabel : str, optional, default : 'Edges'
-
-    nodelabel : str, optional, default : 'Nodes'
-
-
-    Returns
-    -------
-    OrderedDict
-        used for labels in constructing a EntitySet
-    """
-    enames = np.array([f"{edgeprefix}{idx}" for idx in range(num_edges)])
-    nnames = np.array([f"{nodeprefix}{jdx}" for jdx in range(num_nodes)])
-    return OrderedDict([(edgelabel, enames), (nodelabel, nnames)])
-
-
 def reverse_dictionary(d):
     new_d = DefaultOrderedDict(list)
     for key, values in d.items():
         for val in values:
             new_d[val].append(key)
 
     return new_d
```

### Comparing `hypernetx-2.2.0/hypernetx/utils/log.py` & `hypernetx-2.3.0/hypernetx/utils/log.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.2.0/hypernetx/utils/toys/HarryPotter_Characters.csv` & `hypernetx-2.3.0/hypernetx/utils/toys/HarryPotter_Characters.csv`

 * *Files identical despite different names*

### Comparing `hypernetx-2.2.0/hypernetx/utils/toys/harrypotter.py` & `hypernetx-2.3.0/hypernetx/utils/toys/harrypotter.py`

 * *Files 23% similar despite different names*

```diff
@@ -71,7 +71,39 @@
             imat[tuple(d)] = self.counts[tuple(d)]
         self.arr = imat
 
         slabels = OrderedDict()
         for col_idx, col in enumerate(list(ldict.keys())):
             slabels.update({col_idx: np.array(list(ldict[col].keys()))})
         self.labels = slabels
+        self.cell_weight_col = "wandweight"
+
+    def set_random_wandweights(self) -> None:
+        self.dataframe[self.cell_weight_col] = [
+            np.random.rand() for _ in self.dataframe.index
+        ]
+
+    def get_edge_properties(self):
+        if self.cell_weight_col not in self.dataframe:
+            return
+
+        edgeprops = (
+            self.dataframe.groupby(["House"])
+            .agg({self.cell_weight_col: "sum"})
+            .reset_index()
+            .rename(columns={"House": "id"})
+        )
+        edgeprops["level"] = 0
+        return edgeprops
+
+    def get_node_properties(self):
+        if self.cell_weight_col not in self.dataframe:
+            return
+
+        nodeprops = (
+            self.dataframe.groupby(["Blood status"])
+            .agg({self.cell_weight_col: "sum"})
+            .reset_index()
+            .rename(columns={"Blood status": "id"})
+        )
+        nodeprops["level"] = 1
+        return nodeprops
```

### Comparing `hypernetx-2.2.0/hypernetx/utils/toys/lesmis.py` & `hypernetx-2.3.0/hypernetx/utils/toys/lesmis.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.2.0/hypernetx/utils/toys/transmission_problem.py` & `hypernetx-2.3.0/hypernetx/utils/toys/transmission_problem.py`

 * *Files identical despite different names*

