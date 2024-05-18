# Comparing `tmp/spyndex-0.5.0.tar.gz` & `tmp/spyndex-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyndex-0.5.0.tar", last modified: Tue Jul 11 08:03:21 2023, max compression
+gzip compressed data, was "spyndex-0.6.0.tar", last modified: Sat May 18 09:16:14 2024, max compression
```

## Comparing `spyndex-0.5.0.tar` & `spyndex-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-11 08:03:21.220546 spyndex-0.5.0/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1077 2021-09-03 21:24:15.000000 spyndex-0.5.0/LICENSE
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)    18042 2023-07-11 08:03:21.220546 spyndex-0.5.0/PKG-INFO
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)    17386 2023-07-10 11:17:33.000000 spyndex-0.5.0/README.md
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)       38 2023-07-11 08:03:21.220546 spyndex-0.5.0/setup.cfg
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1366 2023-07-11 07:51:15.000000 spyndex-0.5.0/setup.py
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-11 08:03:21.207213 spyndex-0.5.0/spyndex/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      243 2023-07-11 07:51:20.000000 spyndex-0.5.0/spyndex/__init__.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)    14436 2023-03-13 09:17:05.000000 spyndex-0.5.0/spyndex/axioms.py
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-11 08:03:21.220546 spyndex-0.5.0/spyndex/data/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)  6284146 2021-09-06 18:53:31.000000 spyndex-0.5.0/spyndex/data/S2_10m.json
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)    23999 2023-03-13 09:17:05.000000 spyndex-0.5.0/spyndex/data/bands.json
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     2954 2023-07-10 11:17:33.000000 spyndex-0.5.0/spyndex/data/constants.json
--rwxr-xr-x   0 dmontero  (1001) dmontero  (1001)   156701 2023-07-10 11:17:33.000000 spyndex-0.5.0/spyndex/data/spectral-indices-dict.json
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)    16684 2021-09-11 12:19:14.000000 spyndex-0.5.0/spyndex/data/spectral.json
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1743 2021-10-07 15:49:12.000000 spyndex-0.5.0/spyndex/datasets.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     2040 2023-07-10 13:58:03.000000 spyndex-0.5.0/spyndex/plot.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)    13418 2022-01-17 22:12:10.000000 spyndex-0.5.0/spyndex/spyndex.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1721 2022-06-02 13:19:12.000000 spyndex-0.5.0/spyndex/utils.py
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-11 08:03:21.207213 spyndex-0.5.0/spyndex.egg-info/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)    18042 2023-07-11 08:03:21.000000 spyndex-0.5.0/spyndex.egg-info/PKG-INFO
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      434 2023-07-11 08:03:21.000000 spyndex-0.5.0/spyndex.egg-info/SOURCES.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)        1 2023-07-11 08:03:21.000000 spyndex-0.5.0/spyndex.egg-info/dependency_links.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      104 2023-07-11 08:03:21.000000 spyndex-0.5.0/spyndex.egg-info/requires.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)        8 2023-07-11 08:03:21.000000 spyndex-0.5.0/spyndex.egg-info/top_level.txt
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2024-05-18 09:16:14.128705 spyndex-0.6.0/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1077 2021-09-03 21:24:15.000000 spyndex-0.6.0/LICENSE
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)    18599 2024-05-18 09:16:14.128705 spyndex-0.6.0/PKG-INFO
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)    17943 2024-05-18 09:14:10.000000 spyndex-0.6.0/README.md
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)       38 2024-05-18 09:16:14.128705 spyndex-0.6.0/setup.cfg
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1366 2024-05-18 09:14:10.000000 spyndex-0.6.0/setup.py
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2024-05-18 09:16:14.095371 spyndex-0.6.0/spyndex/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      243 2024-05-18 09:14:10.000000 spyndex-0.6.0/spyndex/__init__.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)    14436 2023-03-13 09:17:05.000000 spyndex-0.6.0/spyndex/axioms.py
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2024-05-18 09:16:14.128705 spyndex-0.6.0/spyndex/data/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)  6284146 2021-09-06 18:53:31.000000 spyndex-0.6.0/spyndex/data/S2_10m.json
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)    23999 2023-03-13 09:17:05.000000 spyndex-0.6.0/spyndex/data/bands.json
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     3053 2024-05-18 09:14:10.000000 spyndex-0.6.0/spyndex/data/constants.json
+-rwxr-xr-x   0 dmontero  (1001) dmontero  (1001)   165610 2024-05-18 09:14:10.000000 spyndex-0.6.0/spyndex/data/spectral-indices-dict.json
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)    16684 2021-09-11 12:19:14.000000 spyndex-0.6.0/spyndex/data/spectral.json
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1743 2021-10-07 15:49:12.000000 spyndex-0.6.0/spyndex/datasets.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     2040 2023-07-10 13:58:03.000000 spyndex-0.6.0/spyndex/plot.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)    13418 2022-01-17 22:12:10.000000 spyndex-0.6.0/spyndex/spyndex.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1721 2022-06-02 13:19:12.000000 spyndex-0.6.0/spyndex/utils.py
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2024-05-18 09:16:14.095371 spyndex-0.6.0/spyndex.egg-info/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)    18599 2024-05-18 09:16:13.000000 spyndex-0.6.0/spyndex.egg-info/PKG-INFO
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      434 2024-05-18 09:16:13.000000 spyndex-0.6.0/spyndex.egg-info/SOURCES.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)        1 2024-05-18 09:16:13.000000 spyndex-0.6.0/spyndex.egg-info/dependency_links.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      104 2024-05-18 09:16:13.000000 spyndex-0.6.0/spyndex.egg-info/requires.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)        8 2024-05-18 09:16:13.000000 spyndex-0.6.0/spyndex.egg-info/top_level.txt
```

### Comparing `spyndex-0.5.0/LICENSE` & `spyndex-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spyndex-0.5.0/PKG-INFO` & `spyndex-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyndex
-Version: 0.5.0
+Version: 0.6.0
 Summary: Awesome Spectral Indices in Python
 Home-page: https://github.com/awesome-spectral-indices/spyndex
 Author: David Montero Loaiza
 Author-email: dml.mont@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -85,14 +85,31 @@
 
 **Conda-forge**: [https://anaconda.org/conda-forge/spyndex](https://anaconda.org/conda-forge/spyndex)
 
 **Tutorials**: [https://spyndex.readthedocs.io/en/latest/tutorials.html](https://spyndex.readthedocs.io/en/latest/tutorials.html)
 
 ---
 
+## Citation
+
+If you use this work, please consider citing the following paper:
+
+```bibtex
+@article{montero2023standardized,
+  title={A standardized catalogue of spectral indices to advance the use of remote sensing in Earth system research},
+  author={Montero, David and Aybar, C{\'e}sar and Mahecha, Miguel D and Martinuzzi, Francesco and S{\"o}chting, Maximilian and Wieneke, Sebastian},
+  journal={Scientific Data},
+  volume={10},
+  number={1},
+  pages={197},
+  year={2023},
+  publisher={Nature Publishing Group UK London}
+}
+```
+
 ## Overview
 
 The [Awesome Spectral Indices](https://github.com/davemlz/awesome-spectral-indices) is a standardized ready-to-use curated list of spectral indices
 that can be used as expressions for computing spectral indices in remote sensing applications. The list was born initially to supply spectral 
 indices for [Google Earth Engine](https://earthengine.google.com/) through [eemont](https://github.com/davemlz/eemont) and 
 [spectral](https://github.com/davemlz/spectral), but given the necessity to compute spectral indices for other object classes outside the Earth 
 Engine ecosystem, a new package was required.
@@ -152,15 +169,14 @@
 ```python
 idx = spyndex.indices.NDVI.compute(
     N = da.sel(band = "NIR"),
     R = da.sel(band = "Red"),
 )
 ```
 
-
 ## How does it work?
 
 Any python object class that supports overloaded operators can be used with spyndex methods.
 
 ---
 
 *"Hey... what do you mean by 'overloaded operators'?"*
@@ -334,17 +350,17 @@
         "L": 0.5
     }
 )
 
 # Plot the indices (and the RGB image for comparison)
 fig, ax = plt.subplots(2,2,figsize = (10,10))
 plot.show(snt.sel(band = ["B04","B03","B02"]).data / 0.3,ax = ax[0,0],title = "RGB")
-plot.show(idx.sel(index = "NDVI"),ax = ax[0,1],title = "NDVI")
-plot.show(idx.sel(index = "GNDVI"),ax = ax[1,0],title = "GNDVI")
-plot.show(idx.sel(index = "SAVI"),ax = ax[1,1],title = "SAVI")
+plot.show(idx.sel(index = "NDVI").data,ax = ax[0,1],title = "NDVI")
+plot.show(idx.sel(index = "GNDVI").data,ax = ax[1,0],title = "GNDVI")
+plot.show(idx.sel(index = "SAVI").data,ax = ax[1,1],title = "SAVI")
 ```
 
 <p align="center">
   <a href="https://github.com/davemlz/spyndex"><img src="https://raw.githubusercontent.com/davemlz/spyndex/main/docs/_static/sentinel.png" alt="sentinel spectral indices"></a>
 </p>
 
 ### Kernel Indices Computation
@@ -385,16 +401,16 @@
             }),
     }
 )
 
 # Plot the indices (and the RGB image for comparison)
 fig, ax = plt.subplots(1,3,figsize = (15,15))
 plot.show(snt.sel(band = ["B04","B03","B02"]).data / 0.3,ax = ax[0],title = "RGB")
-plot.show(idx.sel(index = "NDVI"),ax = ax[1],title = "NDVI")
-plot.show(idx.sel(index = "kNDVI"),ax = ax[2],title = "kNDVI")
+plot.show(idx.sel(index = "NDVI").data,ax = ax[1],title = "NDVI")
+plot.show(idx.sel(index = "kNDVI").data,ax = ax[2],title = "kNDVI")
 ```
 
 <p align="center">
   <a href="https://github.com/davemlz/spyndex"><img src="https://raw.githubusercontent.com/davemlz/spyndex/main/docs/_static/kNDVI.png" alt="sentinel kNDVI"></a>
 </p>
 
 ### A `pandas.DataFrame`? Sure!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spyndex Version: 0.5.0 Summary: Awesome Spectral
+Metadata-Version: 2.1 Name: spyndex Version: 0.6.0 Summary: Awesome Spectral
 Indices in Python Home-page: https://github.com/awesome-spectral-indices/
 spyndex Author: David Montero Loaiza Author-email: dml.mont@gmail.com License:
 MIT Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Description-
@@ -15,15 +15,22 @@
 --- **GitHub**: [https://github.com/davemlz/spyndex](https://github.com/
 davemlz/spyndex) **Documentation**: [https://spyndex.readthedocs.io/](https://
 spyndex.readthedocs.io/) **Paper**: [https://doi.org/10.1038/s41597-023-02096-
 0](https://doi.org/10.1038/s41597-023-02096-0) **PyPI**: [https://pypi.org/
 project/spyndex/](https://pypi.org/project/spyndex/) **Conda-forge**: [https://
 anaconda.org/conda-forge/spyndex](https://anaconda.org/conda-forge/spyndex)
 **Tutorials**: [https://spyndex.readthedocs.io/en/latest/tutorials.html](https:
-//spyndex.readthedocs.io/en/latest/tutorials.html) --- ## Overview The [Awesome
+//spyndex.readthedocs.io/en/latest/tutorials.html) --- ## Citation If you use
+this work, please consider citing the following paper: ```bibtex @article
+{montero2023standardized, title={A standardized catalogue of spectral indices
+to advance the use of remote sensing in Earth system research}, author=
+{Montero, David and Aybar, C{\'e}sar and Mahecha, Miguel D and Martinuzzi,
+Francesco and S{\"o}chting, Maximilian and Wieneke, Sebastian}, journal=
+{Scientific Data}, volume={10}, number={1}, pages={197}, year={2023},
+publisher={Nature Publishing Group UK London} } ``` ## Overview The [Awesome
 Spectral Indices](https://github.com/davemlz/awesome-spectral-indices) is a
 standardized ready-to-use curated list of spectral indices that can be used as
 expressions for computing spectral indices in remote sensing applications. The
 list was born initially to supply spectral indices for [Google Earth Engine]
 (https://earthengine.google.com/) through [eemont](https://github.com/davemlz/
 eemont) and [spectral](https://github.com/davemlz/spectral), but given the
 necessity to compute spectral indices for other object classes outside the
@@ -121,17 +128,17 @@
 (in this case a xarray.DataArray) snt = spyndex.datasets.open("sentinel") #
 Scale the data (remember that the valid domain for reflectance is [0,1]) snt =
 snt / 10000 # Compute the desired spectral indices idx = spyndex.computeIndex
 ( index = ["NDVI","GNDVI","SAVI"], params = { "N": snt.sel(band = "B08"), "R":
 snt.sel(band = "B04"), "G": snt.sel(band = "B03"), "L": 0.5 } ) # Plot the
 indices (and the RGB image for comparison) fig, ax = plt.subplots(2,2,figsize =
 (10,10)) plot.show(snt.sel(band = ["B04","B03","B02"]).data / 0.3,ax = ax
-[0,0],title = "RGB") plot.show(idx.sel(index = "NDVI"),ax = ax[0,1],title =
-"NDVI") plot.show(idx.sel(index = "GNDVI"),ax = ax[1,0],title = "GNDVI")
-plot.show(idx.sel(index = "SAVI"),ax = ax[1,1],title = "SAVI") ```
+[0,0],title = "RGB") plot.show(idx.sel(index = "NDVI").data,ax = ax[0,1],title
+= "NDVI") plot.show(idx.sel(index = "GNDVI").data,ax = ax[1,0],title = "GNDVI")
+plot.show(idx.sel(index = "SAVI").data,ax = ax[1,1],title = "SAVI") ```
                           _[_s_e_n_t_i_n_e_l_ _s_p_e_c_t_r_a_l_ _i_n_d_i_c_e_s_]
 ### Kernel Indices Computation Use the `computeKernel()` method to compute the
 required kernel for kernel indices like the kNDVI! The `kernel` parameter
 receives the kernel to compute, while the `params` parameter receives a
 dictionary with the [required parameters](https://github.com/davemlz/awesome-
 ee-spectral-indices#expressions) for the kernel computation (e.g., `a`, `b` and
 `sigma` for the RBF kernel). ```python import spyndex import xarray as xr
@@ -142,16 +149,16 @@
 spyndex.computeIndex( index = ["NDVI","kNDVI"], params = { # Parameters
 required for NDVI "N": snt.sel(band = "B08"), "R": snt.sel(band = "B04"), #
 Parameters required for kNDVI "kNN" : 1.0, "kNR" : spyndex.computeKernel
 ( kernel = "RBF", params = { "a": snt.sel(band = "B08"), "b": snt.sel(band =
 "B04"), "sigma": snt.sel(band = ["B08","B04"]).mean("band") }), } ) # Plot the
 indices (and the RGB image for comparison) fig, ax = plt.subplots(1,3,figsize =
 (15,15)) plot.show(snt.sel(band = ["B04","B03","B02"]).data / 0.3,ax = ax
-[0],title = "RGB") plot.show(idx.sel(index = "NDVI"),ax = ax[1],title = "NDVI")
-plot.show(idx.sel(index = "kNDVI"),ax = ax[2],title = "kNDVI") ```
+[0],title = "RGB") plot.show(idx.sel(index = "NDVI").data,ax = ax[1],title =
+"NDVI") plot.show(idx.sel(index = "kNDVI").data,ax = ax[2],title = "kNDVI") ```
                                _[_s_e_n_t_i_n_e_l_ _k_N_D_V_I_]
 ### A `pandas.DataFrame`? Sure! No matter what kind of python object you're
 working with, it can be used with `spyndex` as long as it supports mathematical
 overloaded operators! ```python import spyndex import pandas as pd import
 seaborn as sns import matplotlib.pyplot as plt # Open a dataset (in this case a
 pandas.DataFrame) df = spyndex.datasets.open("spectral") # Compute the desired
 spectral indices idx = spyndex.computeIndex( index = ["NDVI","NDWI","NDBI"],
```

### Comparing `spyndex-0.5.0/README.md` & `spyndex-0.6.0/spyndex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: spyndex
+Version: 0.6.0
+Summary: Awesome Spectral Indices in Python
+Home-page: https://github.com/awesome-spectral-indices/spyndex
+Author: David Montero Loaiza
+Author-email: dml.mont@gmail.com
+License: MIT
+Platform: UNKNOWN
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
   <a href="https://github.com/davemlz/spyndex"><img src="https://raw.githubusercontent.com/davemlz/spyndex/main/docs/_static/spyndex.png" alt="spyndex"></a>
 </p>
 <p align="center">
     <em><a href="https://github.com/davemlz/awesome-ee-spectral-indices" target="_blank">
     Awesome Spectral Indices</a> in Python:</em>
 </p>
@@ -66,14 +85,31 @@
 
 **Conda-forge**: [https://anaconda.org/conda-forge/spyndex](https://anaconda.org/conda-forge/spyndex)
 
 **Tutorials**: [https://spyndex.readthedocs.io/en/latest/tutorials.html](https://spyndex.readthedocs.io/en/latest/tutorials.html)
 
 ---
 
+## Citation
+
+If you use this work, please consider citing the following paper:
+
+```bibtex
+@article{montero2023standardized,
+  title={A standardized catalogue of spectral indices to advance the use of remote sensing in Earth system research},
+  author={Montero, David and Aybar, C{\'e}sar and Mahecha, Miguel D and Martinuzzi, Francesco and S{\"o}chting, Maximilian and Wieneke, Sebastian},
+  journal={Scientific Data},
+  volume={10},
+  number={1},
+  pages={197},
+  year={2023},
+  publisher={Nature Publishing Group UK London}
+}
+```
+
 ## Overview
 
 The [Awesome Spectral Indices](https://github.com/davemlz/awesome-spectral-indices) is a standardized ready-to-use curated list of spectral indices
 that can be used as expressions for computing spectral indices in remote sensing applications. The list was born initially to supply spectral 
 indices for [Google Earth Engine](https://earthengine.google.com/) through [eemont](https://github.com/davemlz/eemont) and 
 [spectral](https://github.com/davemlz/spectral), but given the necessity to compute spectral indices for other object classes outside the Earth 
 Engine ecosystem, a new package was required.
@@ -133,15 +169,14 @@
 ```python
 idx = spyndex.indices.NDVI.compute(
     N = da.sel(band = "NIR"),
     R = da.sel(band = "Red"),
 )
 ```
 
-
 ## How does it work?
 
 Any python object class that supports overloaded operators can be used with spyndex methods.
 
 ---
 
 *"Hey... what do you mean by 'overloaded operators'?"*
@@ -315,17 +350,17 @@
         "L": 0.5
     }
 )
 
 # Plot the indices (and the RGB image for comparison)
 fig, ax = plt.subplots(2,2,figsize = (10,10))
 plot.show(snt.sel(band = ["B04","B03","B02"]).data / 0.3,ax = ax[0,0],title = "RGB")
-plot.show(idx.sel(index = "NDVI"),ax = ax[0,1],title = "NDVI")
-plot.show(idx.sel(index = "GNDVI"),ax = ax[1,0],title = "GNDVI")
-plot.show(idx.sel(index = "SAVI"),ax = ax[1,1],title = "SAVI")
+plot.show(idx.sel(index = "NDVI").data,ax = ax[0,1],title = "NDVI")
+plot.show(idx.sel(index = "GNDVI").data,ax = ax[1,0],title = "GNDVI")
+plot.show(idx.sel(index = "SAVI").data,ax = ax[1,1],title = "SAVI")
 ```
 
 <p align="center">
   <a href="https://github.com/davemlz/spyndex"><img src="https://raw.githubusercontent.com/davemlz/spyndex/main/docs/_static/sentinel.png" alt="sentinel spectral indices"></a>
 </p>
 
 ### Kernel Indices Computation
@@ -366,16 +401,16 @@
             }),
     }
 )
 
 # Plot the indices (and the RGB image for comparison)
 fig, ax = plt.subplots(1,3,figsize = (15,15))
 plot.show(snt.sel(band = ["B04","B03","B02"]).data / 0.3,ax = ax[0],title = "RGB")
-plot.show(idx.sel(index = "NDVI"),ax = ax[1],title = "NDVI")
-plot.show(idx.sel(index = "kNDVI"),ax = ax[2],title = "kNDVI")
+plot.show(idx.sel(index = "NDVI").data,ax = ax[1],title = "NDVI")
+plot.show(idx.sel(index = "kNDVI").data,ax = ax[2],title = "kNDVI")
 ```
 
 <p align="center">
   <a href="https://github.com/davemlz/spyndex"><img src="https://raw.githubusercontent.com/davemlz/spyndex/main/docs/_static/kNDVI.png" alt="sentinel kNDVI"></a>
 </p>
 
 ### A `pandas.DataFrame`? Sure!
@@ -489,8 +524,9 @@
 
 ## License
 
 The project is licensed under the MIT license.
 
 ## Contributing
 
-Check the [contributing page](https://spyndex.readthedocs.io/en/latest/contributing.html).
+Check the [contributing page](https://spyndex.readthedocs.io/en/latest/contributing.html).
+
```

#### html2text {}

```diff
@@ -1,20 +1,36 @@
+Metadata-Version: 2.1 Name: spyndex Version: 0.6.0 Summary: Awesome Spectral
+Indices in Python Home-page: https://github.com/awesome-spectral-indices/
+spyndex Author: David Montero Loaiza Author-email: dml.mont@gmail.com License:
+MIT Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Description-
+Content-Type: text/markdown License-File: LICENSE
                                    _[_s_p_y_n_d_e_x_]
                       _AA_ww_ee_ss_oo_mm_ee_ _SS_pp_ee_cc_tt_rr_aa_ll_ _II_nn_dd_ii_cc_ee_ss iinn PPyytthhoonn::
 _NN_uu_mm_pp_yy || _PP_aa_nn_dd_aa_ss || _GG_ee_oo_PP_aa_nn_dd_aa_ss || _XX_aa_rr_rr_aa_yy || _EE_aa_rr_tt_hh_ _EE_nn_gg_ii_nn_ee || _PP_ll_aa_nn_ee_tt_aa_rr_yy_ _CC_oo_mm_pp_uu_tt_ee_rr || _DD_aa_ss_kk
   _[_P_y_P_I_]_[_c_o_n_d_a_-_f_o_r_g_e_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_T_e_s_t_s_]_[_A_w_e_s_o_m_e_ _S_p_e_c_t_r_a_l_ _I_n_d_i_c_e_s_]
    _[_L_i_c_e_n_s_e_]_[_G_i_t_H_u_b_ _S_p_o_n_s_o_r_s_]_[_B_u_y_ _m_e_ _a_ _c_o_f_f_e_e_]_[_K_o_-_f_i_]_[_T_w_i_t_t_e_r_]_[_B_l_a_c_k_]_[_i_s_o_r_t_]
 --- **GitHub**: [https://github.com/davemlz/spyndex](https://github.com/
 davemlz/spyndex) **Documentation**: [https://spyndex.readthedocs.io/](https://
 spyndex.readthedocs.io/) **Paper**: [https://doi.org/10.1038/s41597-023-02096-
 0](https://doi.org/10.1038/s41597-023-02096-0) **PyPI**: [https://pypi.org/
 project/spyndex/](https://pypi.org/project/spyndex/) **Conda-forge**: [https://
 anaconda.org/conda-forge/spyndex](https://anaconda.org/conda-forge/spyndex)
 **Tutorials**: [https://spyndex.readthedocs.io/en/latest/tutorials.html](https:
-//spyndex.readthedocs.io/en/latest/tutorials.html) --- ## Overview The [Awesome
+//spyndex.readthedocs.io/en/latest/tutorials.html) --- ## Citation If you use
+this work, please consider citing the following paper: ```bibtex @article
+{montero2023standardized, title={A standardized catalogue of spectral indices
+to advance the use of remote sensing in Earth system research}, author=
+{Montero, David and Aybar, C{\'e}sar and Mahecha, Miguel D and Martinuzzi,
+Francesco and S{\"o}chting, Maximilian and Wieneke, Sebastian}, journal=
+{Scientific Data}, volume={10}, number={1}, pages={197}, year={2023},
+publisher={Nature Publishing Group UK London} } ``` ## Overview The [Awesome
 Spectral Indices](https://github.com/davemlz/awesome-spectral-indices) is a
 standardized ready-to-use curated list of spectral indices that can be used as
 expressions for computing spectral indices in remote sensing applications. The
 list was born initially to supply spectral indices for [Google Earth Engine]
 (https://earthengine.google.com/) through [eemont](https://github.com/davemlz/
 eemont) and [spectral](https://github.com/davemlz/spectral), but given the
 necessity to compute spectral indices for other object classes outside the
@@ -112,17 +128,17 @@
 (in this case a xarray.DataArray) snt = spyndex.datasets.open("sentinel") #
 Scale the data (remember that the valid domain for reflectance is [0,1]) snt =
 snt / 10000 # Compute the desired spectral indices idx = spyndex.computeIndex
 ( index = ["NDVI","GNDVI","SAVI"], params = { "N": snt.sel(band = "B08"), "R":
 snt.sel(band = "B04"), "G": snt.sel(band = "B03"), "L": 0.5 } ) # Plot the
 indices (and the RGB image for comparison) fig, ax = plt.subplots(2,2,figsize =
 (10,10)) plot.show(snt.sel(band = ["B04","B03","B02"]).data / 0.3,ax = ax
-[0,0],title = "RGB") plot.show(idx.sel(index = "NDVI"),ax = ax[0,1],title =
-"NDVI") plot.show(idx.sel(index = "GNDVI"),ax = ax[1,0],title = "GNDVI")
-plot.show(idx.sel(index = "SAVI"),ax = ax[1,1],title = "SAVI") ```
+[0,0],title = "RGB") plot.show(idx.sel(index = "NDVI").data,ax = ax[0,1],title
+= "NDVI") plot.show(idx.sel(index = "GNDVI").data,ax = ax[1,0],title = "GNDVI")
+plot.show(idx.sel(index = "SAVI").data,ax = ax[1,1],title = "SAVI") ```
                           _[_s_e_n_t_i_n_e_l_ _s_p_e_c_t_r_a_l_ _i_n_d_i_c_e_s_]
 ### Kernel Indices Computation Use the `computeKernel()` method to compute the
 required kernel for kernel indices like the kNDVI! The `kernel` parameter
 receives the kernel to compute, while the `params` parameter receives a
 dictionary with the [required parameters](https://github.com/davemlz/awesome-
 ee-spectral-indices#expressions) for the kernel computation (e.g., `a`, `b` and
 `sigma` for the RBF kernel). ```python import spyndex import xarray as xr
@@ -133,16 +149,16 @@
 spyndex.computeIndex( index = ["NDVI","kNDVI"], params = { # Parameters
 required for NDVI "N": snt.sel(band = "B08"), "R": snt.sel(band = "B04"), #
 Parameters required for kNDVI "kNN" : 1.0, "kNR" : spyndex.computeKernel
 ( kernel = "RBF", params = { "a": snt.sel(band = "B08"), "b": snt.sel(band =
 "B04"), "sigma": snt.sel(band = ["B08","B04"]).mean("band") }), } ) # Plot the
 indices (and the RGB image for comparison) fig, ax = plt.subplots(1,3,figsize =
 (15,15)) plot.show(snt.sel(band = ["B04","B03","B02"]).data / 0.3,ax = ax
-[0],title = "RGB") plot.show(idx.sel(index = "NDVI"),ax = ax[1],title = "NDVI")
-plot.show(idx.sel(index = "kNDVI"),ax = ax[2],title = "kNDVI") ```
+[0],title = "RGB") plot.show(idx.sel(index = "NDVI").data,ax = ax[1],title =
+"NDVI") plot.show(idx.sel(index = "kNDVI").data,ax = ax[2],title = "kNDVI") ```
                                _[_s_e_n_t_i_n_e_l_ _k_N_D_V_I_]
 ### A `pandas.DataFrame`? Sure! No matter what kind of python object you're
 working with, it can be used with `spyndex` as long as it supports mathematical
 overloaded operators! ```python import spyndex import pandas as pd import
 seaborn as sns import matplotlib.pyplot as plt # Open a dataset (in this case a
 pandas.DataFrame) df = spyndex.datasets.open("spectral") # Compute the desired
 spectral indices idx = spyndex.computeIndex( index = ["NDVI","NDWI","NDBI"],
```

### Comparing `spyndex-0.5.0/setup.py` & `spyndex-0.6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     text_type = type(u"")
     with io.open(filename, mode="r", encoding="utf-8") as fd:
         return re.sub(text_type(r":[a-z]+:`~?(.*?)`"), text_type(r"``\1``"), fd.read())
 
 
 setup(
     name="spyndex",
-    version="0.5.0",
+    version="0.6.0",
     url="https://github.com/awesome-spectral-indices/spyndex",
     license="MIT",
     author="David Montero Loaiza",
     author_email="dml.mont@gmail.com",
     description="Awesome Spectral Indices in Python",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
```

### Comparing `spyndex-0.5.0/spyndex/axioms.py` & `spyndex-0.6.0/spyndex/axioms.py`

 * *Files identical despite different names*

### Comparing `spyndex-0.5.0/spyndex/data/S2_10m.json` & `spyndex-0.6.0/spyndex/data/S2_10m.json`

 * *Files identical despite different names*

### Comparing `spyndex-0.5.0/spyndex/data/bands.json` & `spyndex-0.6.0/spyndex/data/bands.json`

 * *Files identical despite different names*

### Comparing `spyndex-0.5.0/spyndex/data/constants.json` & `spyndex-0.6.0/spyndex/data/constants.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9456521739130435%*

 * *Differences: {"'lambdaG'": "{'description': 'Green central wavelength (nm)'}",*

 * * "'lambdaN'": "{'description': 'NIR central wavelength (nm)'}",*

 * * "'lambdaR'": "{'description': 'Red central wavelength (nm)'}",*

 * * "'lambdaS1'": "OrderedDict([('default', None), ('description', 'SWIR1 central wavelength (nm)'), "*

 * *               "('short_name', 'lambdaS1')])"}*

```diff
@@ -62,27 +62,32 @@
     "k": {
         "default": 0.0,
         "description": "Slope parameter by soil used for NIRvH2",
         "short_name": "k"
     },
     "lambdaG": {
         "default": null,
-        "description": "Green wavelength (nm) used for NDGI",
+        "description": "Green central wavelength (nm)",
         "short_name": "lambdaG"
     },
     "lambdaN": {
         "default": null,
-        "description": "NIR wavelength (nm) used for NIRvH2 and NDGI",
+        "description": "NIR central wavelength (nm)",
         "short_name": "lambdaN"
     },
     "lambdaR": {
         "default": null,
-        "description": "Red wavelength (nm) used for NIRvH2 and NDGI",
+        "description": "Red central wavelength (nm)",
         "short_name": "lambdaR"
     },
+    "lambdaS1": {
+        "default": null,
+        "description": "SWIR1 central wavelength (nm)",
+        "short_name": "lambdaS1"
+    },
     "nexp": {
         "default": 2.0,
         "description": "Exponent used for GDVI",
         "short_name": "nexp"
     },
     "omega": {
         "default": 2.0,
```

### Comparing `spyndex-0.5.0/spyndex/data/spectral-indices-dict.json` & `spyndex-0.6.0/spyndex/data/spectral-indices-dict.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9753968253968255%*

 * *Differences: {"'SpectralIndices'": "{'NBAI': {'formula': '(S2 - S1/G)/(S2 + S1/G)'}, 'NDSoI': {'short_name': "*

 * *                      "'NDSoI'}, 'ENDVI': OrderedDict([('application_domain', 'vegetation'), "*

 * *                      "('bands', ['N', 'G', 'B']), ('contributor', 'https://github.com/gagev'), "*

 * *                      "('date_of_addition', '2024-04-08'), ('formula', '((N + G) - (2 * B)) / ((N "*

 * *                      "+ G) + (2 * B))'), ('long_name', 'Enhanced Normalized Difference Vegetation "*

 * *                     […]*

```diff
@@ -891,14 +891,36 @@
                 "Landsat-TM",
                 "Landsat-ETM+",
                 "MODIS"
             ],
             "reference": "https://doi.org/10.1016/j.jag.2022.102703",
             "short_name": "EMBI"
         },
+        "ENDVI": {
+            "application_domain": "vegetation",
+            "bands": [
+                "N",
+                "G",
+                "B"
+            ],
+            "contributor": "https://github.com/gagev",
+            "date_of_addition": "2024-04-08",
+            "formula": "((N + G) - (2 * B)) / ((N + G) + (2 * B))",
+            "long_name": "Enhanced Normalized Difference Vegetation Index",
+            "platforms": [
+                "Sentinel-2",
+                "Landsat-OLI",
+                "Landsat-TM",
+                "Landsat-ETM+",
+                "MODIS",
+                "Planet-Fusion"
+            ],
+            "reference": "https://doi.org/10.1371/journal.pone.0186193",
+            "short_name": "ENDVI"
+        },
         "EVI": {
             "application_domain": "vegetation",
             "bands": [
                 "g",
                 "N",
                 "R",
                 "C1",
@@ -940,14 +962,36 @@
                 "Landsat-ETM+",
                 "MODIS",
                 "Planet-Fusion"
             ],
             "reference": "https://doi.org/10.1016/j.rse.2008.06.006",
             "short_name": "EVI2"
         },
+        "EVIv": {
+            "application_domain": "vegetation",
+            "bands": [
+                "N",
+                "R",
+                "B"
+            ],
+            "contributor": "https://github.com/davemlz",
+            "date_of_addition": "2024-05-16",
+            "formula": "2.5 * ((N - R)/(N + 6 * R - 7.5 * B + 1.0)) * N",
+            "long_name": "Enhanced Vegetation Index of Vegetation",
+            "platforms": [
+                "Sentinel-2",
+                "Landsat-OLI",
+                "Landsat-TM",
+                "Landsat-ETM+",
+                "MODIS",
+                "Planet-Fusion"
+            ],
+            "reference": "https://doi.org/10.22541/essoar.171561872.22414664/v1",
+            "short_name": "EVIv"
+        },
         "ExG": {
             "application_domain": "vegetation",
             "bands": [
                 "G",
                 "R",
                 "B"
             ],
@@ -1005,14 +1049,38 @@
                 "Landsat-ETM+",
                 "MODIS",
                 "Planet-Fusion"
             ],
             "reference": "https://doi.org/10.1117/12.336896",
             "short_name": "ExR"
         },
+        "FAI": {
+            "application_domain": "water",
+            "bands": [
+                "N",
+                "R",
+                "S1",
+                "lambdaN",
+                "lambdaR",
+                "lambdaS1"
+            ],
+            "contributor": "https://github.com/emanuelcastanho",
+            "date_of_addition": "2024-05-03",
+            "formula": "N - (R + (S1 - R)*((lambdaN - lambdaR)/(lambdaS1 - lambdaR)))",
+            "long_name": "Floating Algae Index",
+            "platforms": [
+                "Sentinel-2",
+                "Landsat-OLI",
+                "Landsat-TM",
+                "Landsat-ETM+",
+                "MODIS"
+            ],
+            "reference": "https://doi.org/10.1016/j.rse.2009.05.012",
+            "short_name": "FAI"
+        },
         "FCVI": {
             "application_domain": "vegetation",
             "bands": [
                 "N",
                 "R",
                 "G",
                 "B"
@@ -1938,15 +2006,15 @@
             "bands": [
                 "S2",
                 "S1",
                 "G"
             ],
             "contributor": "https://github.com/davemlz",
             "date_of_addition": "2022-09-22",
-            "formula": "((S2 - S1)/G)/((S2 + S1)/G)",
+            "formula": "(S2 - S1/G)/(S2 + S1/G)",
             "long_name": "Normalized Built-up Area Index",
             "platforms": [
                 "Sentinel-2",
                 "Landsat-OLI",
                 "Landsat-TM",
                 "Landsat-ETM+",
                 "MODIS"
@@ -2640,15 +2708,15 @@
                 "Sentinel-2",
                 "Landsat-OLI",
                 "Landsat-TM",
                 "Landsat-ETM+",
                 "MODIS"
             ],
             "reference": "https://doi.org/10.1016/j.jag.2015.02.010",
-            "short_name": "NDSoiI"
+            "short_name": "NDSoI"
         },
         "NDTI": {
             "application_domain": "water",
             "bands": [
                 "R",
                 "G"
             ],
@@ -3238,14 +3306,57 @@
                 "Landsat-ETM+",
                 "MODIS",
                 "Planet-Fusion"
             ],
             "reference": "https://doi.org/10.1016/0034-4257(95)00186-7",
             "short_name": "OSAVI"
         },
+        "OSI": {
+            "application_domain": "water",
+            "bands": [
+                "G",
+                "R",
+                "B"
+            ],
+            "contributor": "https://github.com/emanuelcastanho",
+            "date_of_addition": "2024-05-03",
+            "formula": "(G + R)/B",
+            "long_name": "Oil Spill Index",
+            "platforms": [
+                "Sentinel-2",
+                "Landsat-OLI",
+                "Landsat-TM",
+                "Landsat-ETM+",
+                "MODIS",
+                "Planet-Fusion"
+            ],
+            "reference": "https://doi.org/10.1016/j.mex.2021.101327",
+            "short_name": "OSI"
+        },
+        "PI": {
+            "application_domain": "water",
+            "bands": [
+                "N",
+                "R"
+            ],
+            "contributor": "https://github.com/emanuelcastanho",
+            "date_of_addition": "2024-05-03",
+            "formula": "N/(N + R)",
+            "long_name": "Plastic Index",
+            "platforms": [
+                "Sentinel-2",
+                "Landsat-OLI",
+                "Landsat-TM",
+                "Landsat-ETM+",
+                "MODIS",
+                "Planet-Fusion"
+            ],
+            "reference": "https://doi.org/10.3390/rs12162648",
+            "short_name": "PI"
+        },
         "PISI": {
             "application_domain": "urban",
             "bands": [
                 "B",
                 "N"
             ],
             "contributor": "https://github.com/davemlz",
@@ -3468,14 +3579,35 @@
                 "Landsat-ETM+",
                 "MODIS",
                 "Planet-Fusion"
             ],
             "reference": "https://doi.org/10.1016/S0034-4257(98)00030-3",
             "short_name": "RI4XS"
         },
+        "RNDVI": {
+            "application_domain": "water",
+            "bands": [
+                "R",
+                "N"
+            ],
+            "contributor": "https://github.com/davemlz",
+            "date_of_addition": "2024-05-16",
+            "formula": "(R - N)/(R + N)",
+            "long_name": "Reversed Normalized Difference Vegetation Index",
+            "platforms": [
+                "Sentinel-2",
+                "Landsat-OLI",
+                "Landsat-TM",
+                "Landsat-ETM+",
+                "MODIS",
+                "Planet-Fusion"
+            ],
+            "reference": "https://doi.org/10.3390/rs12162648",
+            "short_name": "RNDVI"
+        },
         "RVI": {
             "application_domain": "vegetation",
             "bands": [
                 "RE2",
                 "R"
             ],
             "contributor": "https://github.com/davemlz",
@@ -4508,14 +4640,35 @@
                 "Landsat-TM",
                 "Landsat-ETM+",
                 "MODIS"
             ],
             "reference": "https://doi.org/10.1109/GEOINFORMATICS.2010.5567762",
             "short_name": "WRI"
         },
+        "bNIRv": {
+            "application_domain": "vegetation",
+            "bands": [
+                "N",
+                "B"
+            ],
+            "contributor": "https://github.com/davemlz",
+            "date_of_addition": "2024-05-16",
+            "formula": "((N - B)/(N + B)) * N",
+            "long_name": "Blue Near-Infrared Reflectance of Vegetation",
+            "platforms": [
+                "Sentinel-2",
+                "Landsat-OLI",
+                "Landsat-TM",
+                "Landsat-ETM+",
+                "MODIS",
+                "Planet-Fusion"
+            ],
+            "reference": "https://doi.org/10.22541/essoar.171561872.22414664/v1",
+            "short_name": "bNIRv"
+        },
         "kEVI": {
             "application_domain": "kernel",
             "bands": [
                 "g",
                 "kNN",
                 "kNR",
                 "C1",
@@ -4651,10 +4804,115 @@
             "formula": "(RE2 - A)/(RE2 + A)",
             "long_name": "Modified Simple Ratio (705 and 445 nm)",
             "platforms": [
                 "Sentinel-2"
             ],
             "reference": "https://doi.org/10.1016/S0034-4257(02)00010-X",
             "short_name": "mSR705"
+        },
+        "sNIRvLSWI": {
+            "application_domain": "vegetation",
+            "bands": [
+                "N",
+                "S2"
+            ],
+            "contributor": "https://github.com/davemlz",
+            "date_of_addition": "2024-05-16",
+            "formula": "((N - S2)/(N + S2)) * N",
+            "long_name": "SWIR-enhanced Near-Infrared Reflectance of Vegetation for LSWI",
+            "platforms": [
+                "Sentinel-2",
+                "Landsat-OLI",
+                "Landsat-TM",
+                "Landsat-ETM+",
+                "MODIS"
+            ],
+            "reference": "https://doi.org/10.22541/essoar.171561872.22414664/v1",
+            "short_name": "sNIRvLSWI"
+        },
+        "sNIRvNDPI": {
+            "application_domain": "vegetation",
+            "bands": [
+                "N",
+                "alpha",
+                "R",
+                "S2"
+            ],
+            "contributor": "https://github.com/davemlz",
+            "date_of_addition": "2024-05-16",
+            "formula": "(N - (alpha * R + (1.0 - alpha) * S2))/(N + (alpha * R + (1.0 - alpha) * S2)) * N",
+            "long_name": "SWIR-enhanced Near-Infrared Reflectance of Vegetation for NDPI",
+            "platforms": [
+                "Sentinel-2",
+                "Landsat-OLI",
+                "Landsat-TM",
+                "Landsat-ETM+",
+                "MODIS"
+            ],
+            "reference": "https://doi.org/10.22541/essoar.171561872.22414664/v1",
+            "short_name": "sNIRvNDPI"
+        },
+        "sNIRvNDVILSWIP": {
+            "application_domain": "vegetation",
+            "bands": [
+                "N",
+                "R",
+                "S2"
+            ],
+            "contributor": "https://github.com/davemlz",
+            "date_of_addition": "2024-05-16",
+            "formula": "((N - R)/(N + R)) * ((N - S2)/(N + S2)) * N",
+            "long_name": "SWIR-enhanced Near-Infrared Reflectance of Vegetation for the NDVI-LSWI Product",
+            "platforms": [
+                "Sentinel-2",
+                "Landsat-OLI",
+                "Landsat-TM",
+                "Landsat-ETM+",
+                "MODIS"
+            ],
+            "reference": "https://doi.org/10.22541/essoar.171561872.22414664/v1",
+            "short_name": "sNIRvNDVILSWIP"
+        },
+        "sNIRvNDVILSWIS": {
+            "application_domain": "vegetation",
+            "bands": [
+                "N",
+                "R",
+                "S2"
+            ],
+            "contributor": "https://github.com/davemlz",
+            "date_of_addition": "2024-05-16",
+            "formula": "(((N - R)/(N + R)) + ((N - S2)/(N + S2))) * N",
+            "long_name": "SWIR-enhanced Near-Infrared Reflectance of Vegetation for the NDVI-LSWI Sum",
+            "platforms": [
+                "Sentinel-2",
+                "Landsat-OLI",
+                "Landsat-TM",
+                "Landsat-ETM+",
+                "MODIS"
+            ],
+            "reference": "https://doi.org/10.22541/essoar.171561872.22414664/v1",
+            "short_name": "sNIRvNDVILSWIS"
+        },
+        "sNIRvSWIR": {
+            "application_domain": "vegetation",
+            "bands": [
+                "N",
+                "R",
+                "S2"
+            ],
+            "contributor": "https://github.com/MartinuzziFrancesco",
+            "date_of_addition": "2024-05-14",
+            "formula": "((N - R - S2 ** 2.0)/(N + R + S2 ** 2.0)) * N",
+            "long_name": "SWIR-enhanced Near-Infrared Reflectance of Vegetation",
+            "platforms": [
+                "Sentinel-2",
+                "Landsat-OLI",
+                "Landsat-TM",
+                "Landsat-ETM+",
+                "MODIS"
+            ],
+            "reference": "https://doi.org/10.22541/essoar.171561872.22414664/v1",
+            "short_name": "sNIRvSWIR"
         }
     }
 }
```

### Comparing `spyndex-0.5.0/spyndex/data/spectral.json` & `spyndex-0.6.0/spyndex/data/spectral.json`

 * *Files identical despite different names*

### Comparing `spyndex-0.5.0/spyndex/datasets.py` & `spyndex-0.6.0/spyndex/datasets.py`

 * *Files identical despite different names*

### Comparing `spyndex-0.5.0/spyndex/plot.py` & `spyndex-0.6.0/spyndex/plot.py`

 * *Files identical despite different names*

### Comparing `spyndex-0.5.0/spyndex/spyndex.py` & `spyndex-0.6.0/spyndex/spyndex.py`

 * *Files identical despite different names*

### Comparing `spyndex-0.5.0/spyndex/utils.py` & `spyndex-0.6.0/spyndex/utils.py`

 * *Files identical despite different names*

### Comparing `spyndex-0.5.0/spyndex.egg-info/PKG-INFO` & `spyndex-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: spyndex
-Version: 0.5.0
-Summary: Awesome Spectral Indices in Python
-Home-page: https://github.com/awesome-spectral-indices/spyndex
-Author: David Montero Loaiza
-Author-email: dml.mont@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <a href="https://github.com/davemlz/spyndex"><img src="https://raw.githubusercontent.com/davemlz/spyndex/main/docs/_static/spyndex.png" alt="spyndex"></a>
 </p>
 <p align="center">
     <em><a href="https://github.com/davemlz/awesome-ee-spectral-indices" target="_blank">
     Awesome Spectral Indices</a> in Python:</em>
 </p>
@@ -85,14 +66,31 @@
 
 **Conda-forge**: [https://anaconda.org/conda-forge/spyndex](https://anaconda.org/conda-forge/spyndex)
 
 **Tutorials**: [https://spyndex.readthedocs.io/en/latest/tutorials.html](https://spyndex.readthedocs.io/en/latest/tutorials.html)
 
 ---
 
+## Citation
+
+If you use this work, please consider citing the following paper:
+
+```bibtex
+@article{montero2023standardized,
+  title={A standardized catalogue of spectral indices to advance the use of remote sensing in Earth system research},
+  author={Montero, David and Aybar, C{\'e}sar and Mahecha, Miguel D and Martinuzzi, Francesco and S{\"o}chting, Maximilian and Wieneke, Sebastian},
+  journal={Scientific Data},
+  volume={10},
+  number={1},
+  pages={197},
+  year={2023},
+  publisher={Nature Publishing Group UK London}
+}
+```
+
 ## Overview
 
 The [Awesome Spectral Indices](https://github.com/davemlz/awesome-spectral-indices) is a standardized ready-to-use curated list of spectral indices
 that can be used as expressions for computing spectral indices in remote sensing applications. The list was born initially to supply spectral 
 indices for [Google Earth Engine](https://earthengine.google.com/) through [eemont](https://github.com/davemlz/eemont) and 
 [spectral](https://github.com/davemlz/spectral), but given the necessity to compute spectral indices for other object classes outside the Earth 
 Engine ecosystem, a new package was required.
@@ -152,15 +150,14 @@
 ```python
 idx = spyndex.indices.NDVI.compute(
     N = da.sel(band = "NIR"),
     R = da.sel(band = "Red"),
 )
 ```
 
-
 ## How does it work?
 
 Any python object class that supports overloaded operators can be used with spyndex methods.
 
 ---
 
 *"Hey... what do you mean by 'overloaded operators'?"*
@@ -334,17 +331,17 @@
         "L": 0.5
     }
 )
 
 # Plot the indices (and the RGB image for comparison)
 fig, ax = plt.subplots(2,2,figsize = (10,10))
 plot.show(snt.sel(band = ["B04","B03","B02"]).data / 0.3,ax = ax[0,0],title = "RGB")
-plot.show(idx.sel(index = "NDVI"),ax = ax[0,1],title = "NDVI")
-plot.show(idx.sel(index = "GNDVI"),ax = ax[1,0],title = "GNDVI")
-plot.show(idx.sel(index = "SAVI"),ax = ax[1,1],title = "SAVI")
+plot.show(idx.sel(index = "NDVI").data,ax = ax[0,1],title = "NDVI")
+plot.show(idx.sel(index = "GNDVI").data,ax = ax[1,0],title = "GNDVI")
+plot.show(idx.sel(index = "SAVI").data,ax = ax[1,1],title = "SAVI")
 ```
 
 <p align="center">
   <a href="https://github.com/davemlz/spyndex"><img src="https://raw.githubusercontent.com/davemlz/spyndex/main/docs/_static/sentinel.png" alt="sentinel spectral indices"></a>
 </p>
 
 ### Kernel Indices Computation
@@ -385,16 +382,16 @@
             }),
     }
 )
 
 # Plot the indices (and the RGB image for comparison)
 fig, ax = plt.subplots(1,3,figsize = (15,15))
 plot.show(snt.sel(band = ["B04","B03","B02"]).data / 0.3,ax = ax[0],title = "RGB")
-plot.show(idx.sel(index = "NDVI"),ax = ax[1],title = "NDVI")
-plot.show(idx.sel(index = "kNDVI"),ax = ax[2],title = "kNDVI")
+plot.show(idx.sel(index = "NDVI").data,ax = ax[1],title = "NDVI")
+plot.show(idx.sel(index = "kNDVI").data,ax = ax[2],title = "kNDVI")
 ```
 
 <p align="center">
   <a href="https://github.com/davemlz/spyndex"><img src="https://raw.githubusercontent.com/davemlz/spyndex/main/docs/_static/kNDVI.png" alt="sentinel kNDVI"></a>
 </p>
 
 ### A `pandas.DataFrame`? Sure!
@@ -508,9 +505,8 @@
 
 ## License
 
 The project is licensed under the MIT license.
 
 ## Contributing
 
-Check the [contributing page](https://spyndex.readthedocs.io/en/latest/contributing.html).
-
+Check the [contributing page](https://spyndex.readthedocs.io/en/latest/contributing.html).
```

#### html2text {}

```diff
@@ -1,29 +1,27 @@
-Metadata-Version: 2.1 Name: spyndex Version: 0.5.0 Summary: Awesome Spectral
-Indices in Python Home-page: https://github.com/awesome-spectral-indices/
-spyndex Author: David Montero Loaiza Author-email: dml.mont@gmail.com License:
-MIT Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Description-
-Content-Type: text/markdown License-File: LICENSE
                                    _[_s_p_y_n_d_e_x_]
                       _AA_ww_ee_ss_oo_mm_ee_ _SS_pp_ee_cc_tt_rr_aa_ll_ _II_nn_dd_ii_cc_ee_ss iinn PPyytthhoonn::
 _NN_uu_mm_pp_yy || _PP_aa_nn_dd_aa_ss || _GG_ee_oo_PP_aa_nn_dd_aa_ss || _XX_aa_rr_rr_aa_yy || _EE_aa_rr_tt_hh_ _EE_nn_gg_ii_nn_ee || _PP_ll_aa_nn_ee_tt_aa_rr_yy_ _CC_oo_mm_pp_uu_tt_ee_rr || _DD_aa_ss_kk
   _[_P_y_P_I_]_[_c_o_n_d_a_-_f_o_r_g_e_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_T_e_s_t_s_]_[_A_w_e_s_o_m_e_ _S_p_e_c_t_r_a_l_ _I_n_d_i_c_e_s_]
    _[_L_i_c_e_n_s_e_]_[_G_i_t_H_u_b_ _S_p_o_n_s_o_r_s_]_[_B_u_y_ _m_e_ _a_ _c_o_f_f_e_e_]_[_K_o_-_f_i_]_[_T_w_i_t_t_e_r_]_[_B_l_a_c_k_]_[_i_s_o_r_t_]
 --- **GitHub**: [https://github.com/davemlz/spyndex](https://github.com/
 davemlz/spyndex) **Documentation**: [https://spyndex.readthedocs.io/](https://
 spyndex.readthedocs.io/) **Paper**: [https://doi.org/10.1038/s41597-023-02096-
 0](https://doi.org/10.1038/s41597-023-02096-0) **PyPI**: [https://pypi.org/
 project/spyndex/](https://pypi.org/project/spyndex/) **Conda-forge**: [https://
 anaconda.org/conda-forge/spyndex](https://anaconda.org/conda-forge/spyndex)
 **Tutorials**: [https://spyndex.readthedocs.io/en/latest/tutorials.html](https:
-//spyndex.readthedocs.io/en/latest/tutorials.html) --- ## Overview The [Awesome
+//spyndex.readthedocs.io/en/latest/tutorials.html) --- ## Citation If you use
+this work, please consider citing the following paper: ```bibtex @article
+{montero2023standardized, title={A standardized catalogue of spectral indices
+to advance the use of remote sensing in Earth system research}, author=
+{Montero, David and Aybar, C{\'e}sar and Mahecha, Miguel D and Martinuzzi,
+Francesco and S{\"o}chting, Maximilian and Wieneke, Sebastian}, journal=
+{Scientific Data}, volume={10}, number={1}, pages={197}, year={2023},
+publisher={Nature Publishing Group UK London} } ``` ## Overview The [Awesome
 Spectral Indices](https://github.com/davemlz/awesome-spectral-indices) is a
 standardized ready-to-use curated list of spectral indices that can be used as
 expressions for computing spectral indices in remote sensing applications. The
 list was born initially to supply spectral indices for [Google Earth Engine]
 (https://earthengine.google.com/) through [eemont](https://github.com/davemlz/
 eemont) and [spectral](https://github.com/davemlz/spectral), but given the
 necessity to compute spectral indices for other object classes outside the
@@ -121,17 +119,17 @@
 (in this case a xarray.DataArray) snt = spyndex.datasets.open("sentinel") #
 Scale the data (remember that the valid domain for reflectance is [0,1]) snt =
 snt / 10000 # Compute the desired spectral indices idx = spyndex.computeIndex
 ( index = ["NDVI","GNDVI","SAVI"], params = { "N": snt.sel(band = "B08"), "R":
 snt.sel(band = "B04"), "G": snt.sel(band = "B03"), "L": 0.5 } ) # Plot the
 indices (and the RGB image for comparison) fig, ax = plt.subplots(2,2,figsize =
 (10,10)) plot.show(snt.sel(band = ["B04","B03","B02"]).data / 0.3,ax = ax
-[0,0],title = "RGB") plot.show(idx.sel(index = "NDVI"),ax = ax[0,1],title =
-"NDVI") plot.show(idx.sel(index = "GNDVI"),ax = ax[1,0],title = "GNDVI")
-plot.show(idx.sel(index = "SAVI"),ax = ax[1,1],title = "SAVI") ```
+[0,0],title = "RGB") plot.show(idx.sel(index = "NDVI").data,ax = ax[0,1],title
+= "NDVI") plot.show(idx.sel(index = "GNDVI").data,ax = ax[1,0],title = "GNDVI")
+plot.show(idx.sel(index = "SAVI").data,ax = ax[1,1],title = "SAVI") ```
                           _[_s_e_n_t_i_n_e_l_ _s_p_e_c_t_r_a_l_ _i_n_d_i_c_e_s_]
 ### Kernel Indices Computation Use the `computeKernel()` method to compute the
 required kernel for kernel indices like the kNDVI! The `kernel` parameter
 receives the kernel to compute, while the `params` parameter receives a
 dictionary with the [required parameters](https://github.com/davemlz/awesome-
 ee-spectral-indices#expressions) for the kernel computation (e.g., `a`, `b` and
 `sigma` for the RBF kernel). ```python import spyndex import xarray as xr
@@ -142,16 +140,16 @@
 spyndex.computeIndex( index = ["NDVI","kNDVI"], params = { # Parameters
 required for NDVI "N": snt.sel(band = "B08"), "R": snt.sel(band = "B04"), #
 Parameters required for kNDVI "kNN" : 1.0, "kNR" : spyndex.computeKernel
 ( kernel = "RBF", params = { "a": snt.sel(band = "B08"), "b": snt.sel(band =
 "B04"), "sigma": snt.sel(band = ["B08","B04"]).mean("band") }), } ) # Plot the
 indices (and the RGB image for comparison) fig, ax = plt.subplots(1,3,figsize =
 (15,15)) plot.show(snt.sel(band = ["B04","B03","B02"]).data / 0.3,ax = ax
-[0],title = "RGB") plot.show(idx.sel(index = "NDVI"),ax = ax[1],title = "NDVI")
-plot.show(idx.sel(index = "kNDVI"),ax = ax[2],title = "kNDVI") ```
+[0],title = "RGB") plot.show(idx.sel(index = "NDVI").data,ax = ax[1],title =
+"NDVI") plot.show(idx.sel(index = "kNDVI").data,ax = ax[2],title = "kNDVI") ```
                                _[_s_e_n_t_i_n_e_l_ _k_N_D_V_I_]
 ### A `pandas.DataFrame`? Sure! No matter what kind of python object you're
 working with, it can be used with `spyndex` as long as it supports mathematical
 overloaded operators! ```python import spyndex import pandas as pd import
 seaborn as sns import matplotlib.pyplot as plt # Open a dataset (in this case a
 pandas.DataFrame) df = spyndex.datasets.open("spectral") # Compute the desired
 spectral indices idx = spyndex.computeIndex( index = ["NDVI","NDWI","NDBI"],
```

