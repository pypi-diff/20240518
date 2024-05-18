# Comparing `tmp/quad_iou-0.0.0.tar.gz` & `tmp/quad_iou-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quad_iou-0.0.0.tar", last modified: Sat May 18 21:35:46 2024, max compression
+gzip compressed data, was "quad_iou-0.16.0.tar", last modified: Sat May 18 21:19:14 2024, max compression
```

## Comparing `quad_iou-0.0.0.tar` & `quad_iou-0.16.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 isalia    (1000) isalia    (1000)        0 2024-05-18 21:35:46.649158 quad_iou-0.0.0/
--rw-r--r--   0 isalia    (1000) isalia    (1000)      544 2024-05-18 20:51:33.000000 quad_iou-0.0.0/LICENSE
--rw-r--r--   0 isalia    (1000) isalia    (1000)       91 2024-05-18 19:47:42.000000 quad_iou-0.0.0/MANIFEST.in
--rw-r--r--   0 isalia    (1000) isalia    (1000)     1763 2024-05-18 21:35:46.649158 quad_iou-0.0.0/PKG-INFO
--rw-r--r--   0 isalia    (1000) isalia    (1000)     1354 2024-05-18 21:29:00.000000 quad_iou-0.0.0/README.md
--rw-r--r--   0 isalia    (1000) isalia    (1000)       38 2024-05-18 21:35:46.649158 quad_iou-0.0.0/setup.cfg
--rw-rw-r--   0 isalia    (1000) isalia    (1000)     1000 2024-05-18 21:27:58.000000 quad_iou-0.0.0/setup.py
-drwxr-xr-x   0 isalia    (1000) isalia    (1000)        0 2024-05-18 21:35:46.645158 quad_iou-0.0.0/src/
-drwxr-xr-x   0 isalia    (1000) isalia    (1000)        0 2024-05-18 21:35:46.649158 quad_iou-0.0.0/src/cuda/
--rw-r--r--   0 isalia    (1000) isalia    (1000)      579 2024-05-18 16:19:02.000000 quad_iou-0.0.0/src/cuda/allPoints.cuh
--rw-r--r--   0 isalia    (1000) isalia    (1000)      799 2024-05-15 17:20:33.000000 quad_iou-0.0.0/src/cuda/checks.cuh
--rw-r--r--   0 isalia    (1000) isalia    (1000)     3285 2024-05-18 17:29:58.000000 quad_iou-0.0.0/src/cuda/insidePoints.cuh
--rw-r--r--   0 isalia    (1000) isalia    (1000)     3794 2024-05-18 17:29:59.000000 quad_iou-0.0.0/src/cuda/intersectionPoints.cuh
--rw-rw-r--   0 isalia    (1000) isalia    (1000)     2007 2024-05-18 17:30:01.000000 quad_iou-0.0.0/src/cuda/polygonArea.cuh
--rw-r--r--   0 isalia    (1000) isalia    (1000)     8187 2024-05-18 20:22:00.000000 quad_iou-0.0.0/src/cuda/quad_iou_tensors.cu
--rw-r--r--   0 isalia    (1000) isalia    (1000)      289 2024-05-18 19:44:34.000000 quad_iou-0.0.0/src/cuda/quad_iou_tensors_cuda.cpp
--rw-rw-r--   0 isalia    (1000) isalia    (1000)     1925 2024-05-16 07:28:12.000000 quad_iou-0.0.0/src/cuda/simpleIntersectCheck.cuh
--rw-r--r--   0 isalia    (1000) isalia    (1000)     5028 2024-05-18 17:30:12.000000 quad_iou-0.0.0/src/cuda/sortPoints.cuh
--rw-r--r--   0 isalia    (1000) isalia    (1000)      147 2024-05-18 17:30:14.000000 quad_iou-0.0.0/src/cuda/utils.cuh
-drwxr-xr-x   0 isalia    (1000) isalia    (1000)        0 2024-05-18 21:35:46.649158 quad_iou-0.0.0/src/quad_iou/
--rw-r--r--   0 isalia    (1000) isalia    (1000)       73 2024-05-18 20:36:15.000000 quad_iou-0.0.0/src/quad_iou/__init__.py
--rw-r--r--   0 isalia    (1000) isalia    (1000)     1237 2024-05-18 20:27:56.000000 quad_iou-0.0.0/src/quad_iou/wrap.py
-drwxr-xr-x   0 isalia    (1000) isalia    (1000)        0 2024-05-18 21:35:46.649158 quad_iou-0.0.0/src/quad_iou.egg-info/
--rw-r--r--   0 isalia    (1000) isalia    (1000)     1763 2024-05-18 21:35:46.000000 quad_iou-0.0.0/src/quad_iou.egg-info/PKG-INFO
--rw-r--r--   0 isalia    (1000) isalia    (1000)      495 2024-05-18 21:35:46.000000 quad_iou-0.0.0/src/quad_iou.egg-info/SOURCES.txt
--rw-r--r--   0 isalia    (1000) isalia    (1000)        1 2024-05-18 21:35:46.000000 quad_iou-0.0.0/src/quad_iou.egg-info/dependency_links.txt
--rw-r--r--   0 isalia    (1000) isalia    (1000)       25 2024-05-18 21:35:46.000000 quad_iou-0.0.0/src/quad_iou.egg-info/top_level.txt
+drwxr-xr-x   0 isalia    (1000) isalia    (1000)        0 2024-05-18 21:19:14.903554 quad_iou-0.16.0/
+-rw-r--r--   0 isalia    (1000) isalia    (1000)      544 2024-05-18 20:51:33.000000 quad_iou-0.16.0/LICENSE
+-rw-r--r--   0 isalia    (1000) isalia    (1000)       91 2024-05-18 19:47:42.000000 quad_iou-0.16.0/MANIFEST.in
+-rw-r--r--   0 isalia    (1000) isalia    (1000)     2758 2024-05-18 21:19:14.903554 quad_iou-0.16.0/PKG-INFO
+-rw-r--r--   0 isalia    (1000) isalia    (1000)     2429 2024-05-18 16:21:01.000000 quad_iou-0.16.0/README.md
+-rw-r--r--   0 isalia    (1000) isalia    (1000)       38 2024-05-18 21:19:14.903554 quad_iou-0.16.0/setup.cfg
+-rw-rw-r--   0 isalia    (1000) isalia    (1000)      920 2024-05-18 21:19:09.000000 quad_iou-0.16.0/setup.py
+drwxr-xr-x   0 isalia    (1000) isalia    (1000)        0 2024-05-18 21:19:14.899554 quad_iou-0.16.0/src/
+drwxr-xr-x   0 isalia    (1000) isalia    (1000)        0 2024-05-18 21:19:14.899554 quad_iou-0.16.0/src/cuda/
+-rw-r--r--   0 isalia    (1000) isalia    (1000)      579 2024-05-18 16:19:02.000000 quad_iou-0.16.0/src/cuda/allPoints.cuh
+-rw-r--r--   0 isalia    (1000) isalia    (1000)      799 2024-05-15 17:20:33.000000 quad_iou-0.16.0/src/cuda/checks.cuh
+-rw-r--r--   0 isalia    (1000) isalia    (1000)     3285 2024-05-18 17:29:58.000000 quad_iou-0.16.0/src/cuda/insidePoints.cuh
+-rw-r--r--   0 isalia    (1000) isalia    (1000)     3794 2024-05-18 17:29:59.000000 quad_iou-0.16.0/src/cuda/intersectionPoints.cuh
+-rw-rw-r--   0 isalia    (1000) isalia    (1000)     2007 2024-05-18 17:30:01.000000 quad_iou-0.16.0/src/cuda/polygonArea.cuh
+-rw-r--r--   0 isalia    (1000) isalia    (1000)     8187 2024-05-18 20:22:00.000000 quad_iou-0.16.0/src/cuda/quad_iou_tensors.cu
+-rw-r--r--   0 isalia    (1000) isalia    (1000)      289 2024-05-18 19:44:34.000000 quad_iou-0.16.0/src/cuda/quad_iou_tensors_cuda.cpp
+-rw-rw-r--   0 isalia    (1000) isalia    (1000)     1925 2024-05-16 07:28:12.000000 quad_iou-0.16.0/src/cuda/simpleIntersectCheck.cuh
+-rw-r--r--   0 isalia    (1000) isalia    (1000)     5028 2024-05-18 17:30:12.000000 quad_iou-0.16.0/src/cuda/sortPoints.cuh
+-rw-r--r--   0 isalia    (1000) isalia    (1000)      147 2024-05-18 17:30:14.000000 quad_iou-0.16.0/src/cuda/utils.cuh
+drwxr-xr-x   0 isalia    (1000) isalia    (1000)        0 2024-05-18 21:19:14.899554 quad_iou-0.16.0/src/quad_iou/
+-rw-r--r--   0 isalia    (1000) isalia    (1000)       73 2024-05-18 20:36:15.000000 quad_iou-0.16.0/src/quad_iou/__init__.py
+-rw-r--r--   0 isalia    (1000) isalia    (1000)     1237 2024-05-18 20:27:56.000000 quad_iou-0.16.0/src/quad_iou/wrap.py
+drwxr-xr-x   0 isalia    (1000) isalia    (1000)        0 2024-05-18 21:19:14.899554 quad_iou-0.16.0/src/quad_iou.egg-info/
+-rw-r--r--   0 isalia    (1000) isalia    (1000)     2758 2024-05-18 21:19:14.000000 quad_iou-0.16.0/src/quad_iou.egg-info/PKG-INFO
+-rw-r--r--   0 isalia    (1000) isalia    (1000)      495 2024-05-18 21:19:14.000000 quad_iou-0.16.0/src/quad_iou.egg-info/SOURCES.txt
+-rw-r--r--   0 isalia    (1000) isalia    (1000)        1 2024-05-18 21:19:14.000000 quad_iou-0.16.0/src/quad_iou.egg-info/dependency_links.txt
+-rw-r--r--   0 isalia    (1000) isalia    (1000)       25 2024-05-18 21:19:14.000000 quad_iou-0.16.0/src/quad_iou.egg-info/top_level.txt
```

### Comparing `quad_iou-0.0.0/LICENSE` & `quad_iou-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quad_iou-0.0.0/PKG-INFO` & `quad_iou-0.16.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,55 @@
-Metadata-Version: 2.1
-Name: quad_iou
-Version: 0.0.0
-Summary: A CUDA extension for calculating IoU(Intersection over Union) for quadrilaterals(MxN) bound to PyTorch(usable with torch tensors).
-Home-page: https://github.com/Isalia20/quadrilaterals_iou_cuda_kernel
-Author: Irakli Salia
-Author-email: irakli.salia854@gmail.com
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # IoU(Intersection over Union) Calculation for Quadrilaterals(CUDA Kernel)
 
-Cuda kernel for calculating IoU(intersection over union) for quadrilaterals. It can calculate IoU either for 1->1 match or N->M match, returning an iou matrix with N rows and M columns. Torch CUDA extensions are used for running the compiled kernels. 
+Cuda kernel for calculating IoU for quadrilaterals. It can calculate IoU either for 1->1 match or N->M match, returning an iou matrix with N rows and M columns. Torch CUDA extensions are used for running the compiled kernels. 
+
+
+## Installation
+
+**NOTE:** Installation and usage of this module requires NVIDIA GPU, gcc, nvcc and torch installed. Tested with following setups:
+
+|OS| GPU Card | gcc version| nvcc version | torch_version |
+|--|--|--|--|--|
+| Ubuntu 22.04 | RTX 4060 Ti | 11.4 | 12.1 | Stable 2.1.2 CUDA 12.1 |
+| Debian 11 | L4 | 10.2.1 | 12.1 | Stable 2.1.2 CUDA 12.2 |
+| Windows 10 | RTX 4060 Ti | Microsoft Visual C++(Part of Visual Studio) | 12.1 | Stable 2.1.2 CUDA 12.1 |
+
+
+
+1. Clone the repo.
+2. Go into the folder.
+3. Install latest torch with the cuda version you have. Check with `nvcc --version`, upgrade if necessary.
+4. Run `python setup.py install`
+5. Run `python tryout_scripts/usage.py` to test it out. Expected output is `0.25`
+6. To run `comparison.py` you should install shapely as well with `pip install shapely`
 
 ## Example usage:
 ```
 import torch
 import quad_iou
 
 # NxM quadrilaterals
 a = torch.rand((200, 4, 2)).cuda()
 b = torch.rand((300, 4, 2)).cuda()
 
 # sort_input_quads indicate whether kernel should sort the quadrilateral corners
 # clockwise before calculating iou
-iou_matrix = quad_iou.calculate_iou(a, b, sort_input_quads=True) # returns tensor of shape [200, 300]
+iou_matrix = quad_iou.calculateIoU(a, b, sort_input_quads=True) # returns tensor of shape [200, 300]
 
 # 1x1 case
 a = torch.tensor([0.0, 0, 300, 0, 300, 300, 0, 300]).cuda()
 b = torch.tensor([0.0, 0, 150, 0, 150, 150, 0, 150]).cuda()
 # Module expects tensor of shape [N, 4, 2], so we reshape the tensors
 a = a.reshape(-1, 4, 2)
 b = b.reshape(-1, 4, 2)
-iou = quad_iou.calculate_iou(a, b, sort_input_quads=True)
+iou = quad_iou.calculateIoU(a, b, sort_input_quads=True)
 ```
 
+## TODO
+- [ ] Add more tests in `tests/test.py` for dealing with MxN quadrilaterals, now tests are only for 1->1 quadrilaterals
+- [ ] Add more tests in `tests/test.py` for dealing with 1x1 quadrilateral without sorting `sort_input_quads=False`
+- [ ] Make package available on pypi
+
+
 ## Comparison with Shapely library
 
 While CPUs and GPUs are not to be compared for speed, we provide a script to demonstrate the potential speedup when using a GPU. To compare the execution time of calculating the IoU for quadrilaterals using the `Shapely` library versus our GPU-accelerated implementation, run `python tryout_scripts/comparison.py`
```

### Comparing `quad_iou-0.0.0/setup.py` & `quad_iou-0.16.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from torch.utils.cpp_extension import BuildExtension, CUDAExtension
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="quad_iou",
-    version="0.0.0",
+    version="0.16.0",
     author="Irakli Salia",
     author_email="irakli.salia854@gmail.com",
-    description="A CUDA extension for calculating IoU(Intersection over Union) for quadrilaterals(MxN) bound to PyTorch(usable with torch tensors).",
+    description="A CUDA extension for Quad IoU binding to PyTorch.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/Isalia20/quadrilaterals_iou_cuda_kernel",  # Update with your repository URL
     package_dir={'': 'src'},
     packages=find_packages(where="src"),
     ext_modules=[
         CUDAExtension('quad_iou_kernel', [
```

### Comparing `quad_iou-0.0.0/src/cuda/allPoints.cuh` & `quad_iou-0.16.0/src/cuda/allPoints.cuh`

 * *Files identical despite different names*

### Comparing `quad_iou-0.0.0/src/cuda/checks.cuh` & `quad_iou-0.16.0/src/cuda/checks.cuh`

 * *Files identical despite different names*

### Comparing `quad_iou-0.0.0/src/cuda/insidePoints.cuh` & `quad_iou-0.16.0/src/cuda/insidePoints.cuh`

 * *Files identical despite different names*

### Comparing `quad_iou-0.0.0/src/cuda/intersectionPoints.cuh` & `quad_iou-0.16.0/src/cuda/intersectionPoints.cuh`

 * *Files identical despite different names*

### Comparing `quad_iou-0.0.0/src/cuda/polygonArea.cuh` & `quad_iou-0.16.0/src/cuda/polygonArea.cuh`

 * *Files identical despite different names*

### Comparing `quad_iou-0.0.0/src/cuda/quad_iou_tensors.cu` & `quad_iou-0.16.0/src/cuda/quad_iou_tensors.cu`

 * *Files identical despite different names*

### Comparing `quad_iou-0.0.0/src/cuda/simpleIntersectCheck.cuh` & `quad_iou-0.16.0/src/cuda/simpleIntersectCheck.cuh`

 * *Files identical despite different names*

### Comparing `quad_iou-0.0.0/src/cuda/sortPoints.cuh` & `quad_iou-0.16.0/src/cuda/sortPoints.cuh`

 * *Files identical despite different names*

### Comparing `quad_iou-0.0.0/src/quad_iou/wrap.py` & `quad_iou-0.16.0/src/quad_iou/wrap.py`

 * *Files identical despite different names*

