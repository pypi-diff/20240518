# Comparing `tmp/mnist_separator-1.0.4.tar.gz` & `tmp/mnist_separator-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnist_separator-1.0.4.tar", max compression
+gzip compressed data, was "mnist_separator-1.0.5.tar", max compression
```

## Comparing `mnist_separator-1.0.4.tar` & `mnist_separator-1.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      227 2024-04-12 10:18:12.545299 mnist_separator-1.0.4/README.md
--rw-r--r--   0        0        0     6148 2024-05-02 19:58:07.877980 mnist_separator-1.0.4/mnist_separator/.DS_Store
--rw-r--r--   0        0        0      177 2024-05-02 14:31:44.020164 mnist_separator-1.0.4/mnist_separator/__init__.py
--rw-r--r--   0        0        0     6148 2024-05-02 19:58:42.600397 mnist_separator-1.0.4/mnist_separator/src/.DS_Store
--rw-r--r--   0        0        0     2116 2024-05-02 19:35:03.542924 mnist_separator-1.0.4/mnist_separator/src/calc_similarity.py
--rw-r--r--   0        0        0     2188 2024-05-02 19:35:03.550554 mnist_separator-1.0.4/mnist_separator/src/calc_similarity_2pnts.py
--rw-r--r--   0        0        0     4139 2024-05-02 19:35:03.540241 mnist_separator-1.0.4/mnist_separator/src/calc_similarity_3pnts.py
--rw-r--r--   0        0        0      763 2024-05-02 19:35:03.476310 mnist_separator-1.0.4/mnist_separator/src/calc_similarity_next.py
--rw-r--r--   0        0        0      671 2024-05-02 03:22:36.869786 mnist_separator-1.0.4/mnist_separator/src/cfg.py
--rw-r--r--   0        0        0      553 2024-05-02 03:22:36.857384 mnist_separator-1.0.4/mnist_separator/src/clean_all.py
--rw-r--r--   0        0        0     2820 2024-05-02 03:22:36.842248 mnist_separator-1.0.4/mnist_separator/src/convert_data.py
--rw-r--r--   0        0        0     2076 2024-05-02 03:22:36.911146 mnist_separator-1.0.4/mnist_separator/src/create_dirs.py
--rw-r--r--   0        0        0     3373 2024-05-02 19:35:03.527654 mnist_separator-1.0.4/mnist_separator/src/get_angle.py
--rw-r--r--   0        0        0     2813 2024-05-02 19:35:03.555673 mnist_separator-1.0.4/mnist_separator/src/get_peaks.py
--rw-r--r--   0        0        0      741 2024-05-02 19:35:03.546320 mnist_separator-1.0.4/mnist_separator/src/get_similarity.py
--rw-r--r--   0        0        0     1262 2024-05-02 19:04:07.351629 mnist_separator-1.0.4/mnist_separator/src/get_similarity_group.py
--rw-r--r--   0        0        0      690 2024-05-02 03:22:36.899832 mnist_separator-1.0.4/mnist_separator/src/glbl.py
--rw-r--r--   0        0        0     3103 2024-05-02 03:22:36.887208 mnist_separator-1.0.4/mnist_separator/src/go.py
--rw-r--r--   0        0        0      181 2024-05-02 03:22:36.821442 mnist_separator-1.0.4/mnist_separator/src/init.py
--rw-r--r--   0        0        0      970 2024-05-02 14:35:43.534234 mnist_separator-1.0.4/mnist_separator/src/load_data.py
--rw-r--r--   0        0        0     1012 2024-05-02 03:22:36.836421 mnist_separator-1.0.4/mnist_separator/src/load_samples.py
--rw-r--r--   0        0        0     1495 2024-05-02 19:35:03.535140 mnist_separator-1.0.4/mnist_separator/src/magnitude.py
--rw-r--r--   0        0        0     1386 2024-05-02 03:22:36.848610 mnist_separator-1.0.4/mnist_separator/src/save_result.py
--rw-r--r--   0        0        0     1015 2024-05-02 03:22:36.890181 mnist_separator-1.0.4/mnist_separator/src/shell_sort.py
--rw-r--r--   0        0        0      740 2024-05-02 19:35:03.531322 mnist_separator-1.0.4/mnist_separator/src/sort_peaks.py
--rw-r--r--   0        0        0      825 2024-05-02 03:22:36.833593 mnist_separator-1.0.4/mnist_separator/src/timer.py
--rw-r--r--   0        0        0     4104 2024-05-02 03:22:36.896651 mnist_separator-1.0.4/mnist_separator/src/to_canonical.py
--rw-r--r--   0        0        0      663 2024-05-02 14:27:33.572174 mnist_separator-1.0.4/mnist_separator/src/utils_directory.py
--rw-r--r--   0        0        0      600 2024-05-02 03:22:36.907332 mnist_separator-1.0.4/mnist_separator/src/utils_list.py
--rw-r--r--   0        0        0     1297 2024-05-02 19:35:03.521738 mnist_separator-1.0.4/mnist_separator/src/utils_list_of_peaks.py
--rw-r--r--   0        0        0      400 2024-05-02 03:22:36.876539 mnist_separator-1.0.4/mnist_separator/src/utils_table.py
--rw-r--r--   0        0        0      497 2024-05-02 20:08:28.959139 mnist_separator-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 mnist_separator-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      314 2024-05-18 15:07:46.328377 mnist_separator-1.0.5/README.md
+-rw-r--r--   0        0        0     6148 2024-05-02 19:58:07.877980 mnist_separator-1.0.5/mnist_separator/.DS_Store
+-rw-r--r--   0        0        0      177 2024-05-02 14:31:44.020164 mnist_separator-1.0.5/mnist_separator/__init__.py
+-rw-r--r--   0        0        0     6148 2024-05-02 19:58:42.600397 mnist_separator-1.0.5/mnist_separator/src/.DS_Store
+-rw-r--r--   0        0        0     2116 2024-05-03 09:39:47.028643 mnist_separator-1.0.5/mnist_separator/src/calc_similarity.py
+-rw-r--r--   0        0        0     2188 2024-05-03 09:39:47.016841 mnist_separator-1.0.5/mnist_separator/src/calc_similarity_2pnts.py
+-rw-r--r--   0        0        0     4139 2024-05-03 09:39:46.955786 mnist_separator-1.0.5/mnist_separator/src/calc_similarity_3pnts.py
+-rw-r--r--   0        0        0      763 2024-05-03 09:39:47.058658 mnist_separator-1.0.5/mnist_separator/src/calc_similarity_next.py
+-rw-r--r--   0        0        0      671 2024-05-03 09:39:46.993920 mnist_separator-1.0.5/mnist_separator/src/cfg.py
+-rw-r--r--   0        0        0      553 2024-05-03 09:39:46.984846 mnist_separator-1.0.5/mnist_separator/src/clean_all.py
+-rw-r--r--   0        0        0     2820 2024-05-03 09:39:46.903771 mnist_separator-1.0.5/mnist_separator/src/convert_data.py
+-rw-r--r--   0        0        0     2076 2024-05-03 09:39:46.884798 mnist_separator-1.0.5/mnist_separator/src/create_dirs.py
+-rw-r--r--   0        0        0     3373 2024-05-03 09:39:46.895449 mnist_separator-1.0.5/mnist_separator/src/get_angle.py
+-rw-r--r--   0        0        0     2813 2024-05-03 09:39:47.019747 mnist_separator-1.0.5/mnist_separator/src/get_peaks.py
+-rw-r--r--   0        0        0      741 2024-05-03 09:39:46.959191 mnist_separator-1.0.5/mnist_separator/src/get_similarity.py
+-rw-r--r--   0        0        0     1262 2024-05-03 09:39:46.962916 mnist_separator-1.0.5/mnist_separator/src/get_similarity_group.py
+-rw-r--r--   0        0        0      690 2024-05-03 09:39:47.202508 mnist_separator-1.0.5/mnist_separator/src/glbl.py
+-rw-r--r--   0        0        0     3103 2024-05-03 09:39:46.950594 mnist_separator-1.0.5/mnist_separator/src/go.py
+-rw-r--r--   0        0        0      181 2024-05-03 09:39:46.933995 mnist_separator-1.0.5/mnist_separator/src/init.py
+-rw-r--r--   0        0        0      970 2024-05-03 09:39:46.906774 mnist_separator-1.0.5/mnist_separator/src/load_data.py
+-rw-r--r--   0        0        0     1012 2024-05-03 09:39:47.037835 mnist_separator-1.0.5/mnist_separator/src/load_samples.py
+-rw-r--r--   0        0        0     1495 2024-05-03 09:39:47.010217 mnist_separator-1.0.5/mnist_separator/src/magnitude.py
+-rw-r--r--   0        0        0     1386 2024-05-03 09:39:47.228656 mnist_separator-1.0.5/mnist_separator/src/save_result.py
+-rw-r--r--   0        0        0     1015 2024-05-03 09:39:46.919389 mnist_separator-1.0.5/mnist_separator/src/shell_sort.py
+-rw-r--r--   0        0        0      740 2024-05-03 09:39:46.972400 mnist_separator-1.0.5/mnist_separator/src/sort_peaks.py
+-rw-r--r--   0        0        0      825 2024-05-03 09:39:46.978156 mnist_separator-1.0.5/mnist_separator/src/timer.py
+-rw-r--r--   0        0        0     4104 2024-05-03 09:39:46.898193 mnist_separator-1.0.5/mnist_separator/src/to_canonical.py
+-rw-r--r--   0        0        0      663 2024-05-03 09:39:46.887299 mnist_separator-1.0.5/mnist_separator/src/utils_directory.py
+-rw-r--r--   0        0        0      600 2024-05-03 09:39:46.870174 mnist_separator-1.0.5/mnist_separator/src/utils_list.py
+-rw-r--r--   0        0        0     1297 2024-05-03 09:39:47.000938 mnist_separator-1.0.5/mnist_separator/src/utils_list_of_peaks.py
+-rw-r--r--   0        0        0      400 2024-05-03 09:39:46.853948 mnist_separator-1.0.5/mnist_separator/src/utils_table.py
+-rw-r--r--   0        0        0      497 2024-05-18 15:19:32.313058 mnist_separator-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 mnist_separator-1.0.5/PKG-INFO
```

### Comparing `mnist_separator-1.0.4/mnist_separator/.DS_Store` & `mnist_separator-1.0.5/mnist_separator/.DS_Store`

 * *Files identical despite different names*

### Comparing `mnist_separator-1.0.4/mnist_separator/src/.DS_Store` & `mnist_separator-1.0.5/mnist_separator/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `mnist_separator-1.0.4/mnist_separator/src/calc_similarity.py` & `mnist_separator-1.0.5/mnist_separator/src/calc_similarity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # calc_similarity.py
 
 import numpy as np
 
 from mnist_separator.src.magnitude import get_magn_roi, get_magn_half
 from mnist_separator.src.get_peaks import get_peaks
 from mnist_separator.src.sort_peaks import sort_peaks
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/calc_similarity_2pnts.py` & `mnist_separator-1.0.5/mnist_separator/src/calc_similarity_2pnts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # calc_similarity_2pnts.py
 
 import cv2 as cv
 import numpy as np
 import math
 
 from mnist_separator.src import cfg
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/calc_similarity_3pnts.py` & `mnist_separator-1.0.5/mnist_separator/src/calc_similarity_3pnts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # calc_similarity_3pnts.py
 
 import cv2 as cv
 import numpy as np
 
 from mnist_separator.src import cfg
 from mnist_separator.src.calc_similarity_next import calc_similarity_next
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/calc_similarity_next.py` & `mnist_separator-1.0.5/mnist_separator/src/calc_similarity_next.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # calc_similarity_next.py
 
 import numpy as np
 
 from mnist_separator.src import cfg
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/cfg.py` & `mnist_separator-1.0.5/mnist_separator/src/cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # cfg.py
 
 path_image: str = ''
 path_templ: str = ''
 
 # Число локальных максимумов в
 # верхней полуплоскости.
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/clean_all.py` & `mnist_separator-1.0.5/mnist_separator/src/clean_all.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # clean_all.py
 
 from pathlib import Path
 
 from mnist_separator.src import glbl
 from mnist_separator.src.utils_directory import init_directory
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/convert_data.py` & `mnist_separator-1.0.5/mnist_separator/src/convert_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # convert_data.py
 
 import cv2 as cv
 import os
 from pathlib import Path
 
 from mnist_separator.src import glbl
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/create_dirs.py` & `mnist_separator-1.0.5/mnist_separator/src/create_dirs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # create_dirs.py
 
 from pathlib import Path
 import os
 
 
 def create_dirs():
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/get_angle.py` & `mnist_separator-1.0.5/mnist_separator/src/get_angle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # get_angle.py
 
 """
 Система координат изображения в OpenCV (opencv-coordinates)
 
 The coordinate origin is assumed to be the top-left corner. Rotation angle in degrees.
 Positive values mean counter-clockwise rotation (против часовой стрелки).
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/get_peaks.py` & `mnist_separator-1.0.5/mnist_separator/src/get_peaks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # get_peaks.py
 
 import numpy as np
 from numpy import ndarray
 
 from mnist_separator.src import cfg
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/get_similarity.py` & `mnist_separator-1.0.5/mnist_separator/src/get_similarity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # get_similarity.py
 
 import sys
 import cv2 as cv
 
 from mnist_separator.src.to_canonical import to_canonical
 from mnist_separator.src.calc_similarity import calc_similarity
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/get_similarity_group.py` & `mnist_separator-1.0.5/mnist_separator/src/get_similarity_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # get_similarity_group.py
 
 import os
 import cv2 as cv
 import numpy as np
 
 from mnist_separator.src.calc_similarity import calc_similarity
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/glbl.py` & `mnist_separator-1.0.5/mnist_separator/src/glbl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # glbl.py
 
 
 result_name: str = '_RESULT_'
 
 path_test_mnist: str = ''
 path_train_0_mnist: str = ''
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/go.py` & `mnist_separator-1.0.5/mnist_separator/src/go.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # go.py
 
 import sys
 import os
 import numpy as np
 import random
 from tqdm import tqdm
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/load_data.py` & `mnist_separator-1.0.5/mnist_separator/src/load_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # load_data.py
 
 import sys
 import os
 import shutil
 from pathlib import Path
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/load_samples.py` & `mnist_separator-1.0.5/mnist_separator/src/load_samples.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # load_samples.py
 
 import sys
 import os
 import shutil
 from pathlib import Path
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/magnitude.py` & `mnist_separator-1.0.5/mnist_separator/src/magnitude.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # magnitude.py
 
 import cv2 as cv
 import numpy as np
 
 from mnist_separator.src import cfg
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/save_result.py` & `mnist_separator-1.0.5/mnist_separator/src/save_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # save_result.py
 
 from mnist_separator.src import glbl
 from mnist_separator.src.utils_list import save_list
 
 
 def save_result(list_result_0, list_result_1,
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/shell_sort.py` & `mnist_separator-1.0.5/mnist_separator/src/shell_sort.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # shell_sort.py
 
 
 # vect1: 1, 2, 3, ...
 def shell_sort_increase(vect1, vect2, n):
 
     gap = n // 2
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/sort_peaks.py` & `mnist_separator-1.0.5/mnist_separator/src/sort_peaks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # sort_peaks.py
 
 import numpy as np
 
 from mnist_separator.src.shell_sort import shell_sort_decrease
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/timer.py` & `mnist_separator-1.0.5/mnist_separator/src/timer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # timer.py
 
 import time
 from pathlib import Path
 from datetime import date, datetime
 
 global timer_start
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/to_canonical.py` & `mnist_separator-1.0.5/mnist_separator/src/to_canonical.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # to_canonical.py
 
 import cv2 as cv
 import numpy as np
 
 
 def to_canonical(image_in):
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/utils_directory.py` & `mnist_separator-1.0.5/mnist_separator/src/utils_directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # utils_directory.py
 
 from pathlib import Path
 
 
 def init_directory(dir_name):
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/utils_list.py` & `mnist_separator-1.0.5/mnist_separator/src/utils_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # utils_list.py
 
 import os
 from pathlib import Path
 
 
 def save_list(list_name, dir_name, any_list):
```

### Comparing `mnist_separator-1.0.4/mnist_separator/src/utils_list_of_peaks.py` & `mnist_separator-1.0.5/mnist_separator/src/utils_list_of_peaks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# May-02-2024
+# May-03-2024
 # utils_list_of_peaks.py
 
 from mnist_separator.src import cfg
 
 
 def cut_list_of_peaks(list_of_peaks) -> list:
```

### Comparing `mnist_separator-1.0.4/PKG-INFO` & `mnist_separator-1.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: mnist-separator
-Version: 1.0.4
+Version: 1.0.5
 Summary: mnist-separator is a new technology for recognizing handwritten numbers from the MNIST dataset
 License: MIT
 Author: Boris Kravtsov
 Author-email: boriskravtsov.contacts@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: opencv-python-headless (>=4.9.0.80,<5.0.0.0)
-Requires-Dist: tqdm (>=4.66.2,<5.0.0)
+Requires-Dist: tqdm (>=4.66.4,<5.0.0)
 Description-Content-Type: text/markdown
 
 ## MNIST SEPARATOR
 **mnist-separator** is a new technology for recognizing handwritten numbers of the MNIST dataset
 
 ### Installation
 ```
 pip install mnist-separator
 ```
-[Here](https://boriskravtsov.com) we show how to use it 
+[Here](https://kravtsov-development.medium.com/new-method-for-recognizing-handwritten-digits-mnist-dataset-c6f83e5291ee) we show how to use it
```

