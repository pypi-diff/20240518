# Comparing `tmp/CNAsim-1.3.2.tar.gz` & `tmp/cnasim-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CNAsim-1.3.2.tar", last modified: Fri May 17 20:07:36 2024, max compression
+gzip compressed data, was "cnasim-1.3.3.tar", last modified: Fri May 17 23:48:21 2024, max compression
```

## Comparing `CNAsim-1.3.2.tar` & `cnasim-1.3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sweiner  (30000) nabavilab (10062)        0 2024-05-17 20:07:36.455220 CNAsim-1.3.2/
-drwxr-xr-x   0 sweiner  (30000) nabavilab (10062)        0 2024-05-17 20:07:36.401339 CNAsim-1.3.2/CNAsim/
--rw-r--r--   0 sweiner  (30000) nabavilab (10062)       21 2024-05-17 19:47:49.000000 CNAsim-1.3.2/CNAsim/__init__.py
--rw-r--r--   0 sweiner  (30000) nabavilab (10062)     3950 2024-05-16 19:36:20.000000 CNAsim-1.3.2/CNAsim/format_profiles.py
--rw-r--r--   0 sweiner  (30000) nabavilab (10062)    15734 2024-05-17 20:05:32.000000 CNAsim-1.3.2/CNAsim/main.py
--rw-r--r--   0 sweiner  (30000) nabavilab (10062)     6253 2024-05-16 19:36:20.000000 CNAsim-1.3.2/CNAsim/noise.py
--rw-r--r--   0 sweiner  (30000) nabavilab (10062)    12946 2024-05-16 19:36:20.000000 CNAsim-1.3.2/CNAsim/reads.py
--rw-r--r--   0 sweiner  (30000) nabavilab (10062)     1602 2024-05-16 19:36:20.000000 CNAsim-1.3.2/CNAsim/sequence.py
--rw-r--r--   0 sweiner  (30000) nabavilab (10062)    14866 2024-05-16 19:36:20.000000 CNAsim-1.3.2/CNAsim/sim_genomes.py
--rw-r--r--   0 sweiner  (30000) nabavilab (10062)    17424 2024-05-16 19:36:20.000000 CNAsim-1.3.2/CNAsim/tree.py
--rw-r--r--   0 sweiner  (30000) nabavilab (10062)     7649 2024-05-17 19:41:42.000000 CNAsim-1.3.2/CNAsim/utilities.py
-drwxr-xr-x   0 sweiner  (30000) nabavilab (10062)        0 2024-05-17 20:07:36.444103 CNAsim-1.3.2/CNAsim.egg-info/
--rw-r--r--   0 sweiner  (30000) nabavilab (10062)    25623 2024-05-17 20:07:36.000000 CNAsim-1.3.2/CNAsim.egg-info/PKG-INFO
--rw-r--r--   0 sweiner  (30000) nabavilab (10062)      380 2024-05-17 20:07:36.000000 CNAsim-1.3.2/CNAsim.egg-info/SOURCES.txt
--rw-r--r--   0 sweiner  (30000) nabavilab (10062)        1 2024-05-17 20:07:36.000000 CNAsim-1.3.2/CNAsim.egg-info/dependency_links.txt
--rw-r--r--   0 sweiner  (30000) nabavilab (10062)       44 2024-05-17 20:07:36.000000 CNAsim-1.3.2/CNAsim.egg-info/entry_points.txt
--rw-r--r--   0 sweiner  (30000) nabavilab (10062)       76 2024-05-17 20:07:36.000000 CNAsim-1.3.2/CNAsim.egg-info/requires.txt
--rw-r--r--   0 sweiner  (30000) nabavilab (10062)        7 2024-05-17 20:07:36.000000 CNAsim-1.3.2/CNAsim.egg-info/top_level.txt
--rw-r--r--   0 sweiner  (30000) nabavilab (10062)    32452 2024-05-16 19:36:20.000000 CNAsim-1.3.2/LICENSE.txt
--rw-r--r--   0 sweiner  (30000) nabavilab (10062)    25623 2024-05-17 20:07:36.451905 CNAsim-1.3.2/PKG-INFO
--rw-r--r--   0 sweiner  (30000) nabavilab (10062)    25137 2024-05-16 19:41:01.000000 CNAsim-1.3.2/README.md
--rw-r--r--   0 sweiner  (30000) nabavilab (10062)       38 2024-05-17 20:07:36.456794 CNAsim-1.3.2/setup.cfg
--rw-r--r--   0 sweiner  (30000) nabavilab (10062)      903 2024-05-17 20:03:50.000000 CNAsim-1.3.2/setup.py
+drwxr-xr-x   0 sweiner  (30000) nabavilab (10062)        0 2024-05-17 23:48:21.586908 cnasim-1.3.3/
+drwxr-xr-x   0 sweiner  (30000) nabavilab (10062)        0 2024-05-17 23:48:21.511706 cnasim-1.3.3/CNAsim/
+-rw-r--r--   0 sweiner  (30000) nabavilab (10062)       21 2024-05-17 23:44:28.000000 cnasim-1.3.3/CNAsim/__init__.py
+-rw-r--r--   0 sweiner  (30000) nabavilab (10062)     3950 2024-05-16 19:36:20.000000 cnasim-1.3.3/CNAsim/format_profiles.py
+-rw-r--r--   0 sweiner  (30000) nabavilab (10062)    15741 2024-05-17 23:16:32.000000 cnasim-1.3.3/CNAsim/main.py
+-rw-r--r--   0 sweiner  (30000) nabavilab (10062)     6253 2024-05-16 19:36:20.000000 cnasim-1.3.3/CNAsim/noise.py
+-rw-r--r--   0 sweiner  (30000) nabavilab (10062)    12947 2024-05-17 23:16:30.000000 cnasim-1.3.3/CNAsim/reads.py
+-rw-r--r--   0 sweiner  (30000) nabavilab (10062)     1602 2024-05-16 19:36:20.000000 cnasim-1.3.3/CNAsim/sequence.py
+-rw-r--r--   0 sweiner  (30000) nabavilab (10062)    14867 2024-05-17 23:16:28.000000 cnasim-1.3.3/CNAsim/sim_genomes.py
+-rw-r--r--   0 sweiner  (30000) nabavilab (10062)    17424 2024-05-16 19:36:20.000000 cnasim-1.3.3/CNAsim/tree.py
+-rw-r--r--   0 sweiner  (30000) nabavilab (10062)     7649 2024-05-17 19:41:42.000000 cnasim-1.3.3/CNAsim/utilities.py
+drwxr-xr-x   0 sweiner  (30000) nabavilab (10062)        0 2024-05-17 23:48:21.569934 cnasim-1.3.3/CNAsim.egg-info/
+-rw-r--r--   0 sweiner  (30000) nabavilab (10062)    25774 2024-05-17 23:48:21.000000 cnasim-1.3.3/CNAsim.egg-info/PKG-INFO
+-rw-r--r--   0 sweiner  (30000) nabavilab (10062)      380 2024-05-17 23:48:21.000000 cnasim-1.3.3/CNAsim.egg-info/SOURCES.txt
+-rw-r--r--   0 sweiner  (30000) nabavilab (10062)        1 2024-05-17 23:48:21.000000 cnasim-1.3.3/CNAsim.egg-info/dependency_links.txt
+-rw-r--r--   0 sweiner  (30000) nabavilab (10062)       44 2024-05-17 23:48:21.000000 cnasim-1.3.3/CNAsim.egg-info/entry_points.txt
+-rw-r--r--   0 sweiner  (30000) nabavilab (10062)       76 2024-05-17 23:48:21.000000 cnasim-1.3.3/CNAsim.egg-info/requires.txt
+-rw-r--r--   0 sweiner  (30000) nabavilab (10062)        7 2024-05-17 23:48:21.000000 cnasim-1.3.3/CNAsim.egg-info/top_level.txt
+-rw-r--r--   0 sweiner  (30000) nabavilab (10062)    32452 2024-05-16 19:36:20.000000 cnasim-1.3.3/LICENSE.txt
+-rw-r--r--   0 sweiner  (30000) nabavilab (10062)    25774 2024-05-17 23:48:21.579748 cnasim-1.3.3/PKG-INFO
+-rw-r--r--   0 sweiner  (30000) nabavilab (10062)    25137 2024-05-17 23:44:22.000000 cnasim-1.3.3/README.md
+-rw-r--r--   0 sweiner  (30000) nabavilab (10062)       38 2024-05-17 23:48:21.588744 cnasim-1.3.3/setup.cfg
+-rw-r--r--   0 sweiner  (30000) nabavilab (10062)      903 2024-05-17 23:44:22.000000 cnasim-1.3.3/setup.py
```

### Comparing `CNAsim-1.3.2/CNAsim/format_profiles.py` & `cnasim-1.3.3/CNAsim/format_profiles.py`

 * *Files identical despite different names*

### Comparing `CNAsim-1.3.2/CNAsim/main.py` & `cnasim-1.3.3/CNAsim/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 # along with this program.  If not, see http://www.gnu.org/licenses/.
 
 
 import argparse
 import os
 import time
 
-from tree import *
-from sim_genomes import init_diploid_genome, evolve_tree, prepare_ancestral_profiles
-from sequence import read_fasta
-from reads import gen_reads, gen_readcounts
-from noise import add_noise_mixed
-from format_profiles import save_CN_profiles_leaves, save_CN_profiles_ancestors
-from utilities import *
+from .tree import *
+from .sim_genomes import init_diploid_genome, evolve_tree, prepare_ancestral_profiles
+from .sequence import read_fasta
+from .reads import gen_reads, gen_readcounts
+from .noise import add_noise_mixed
+from .format_profiles import save_CN_profiles_leaves, save_CN_profiles_ancestors
+from .utilities import *
 
 
 def parse_args():
     #Arguments
     parser = argparse.ArgumentParser()
     parser.add_argument('-m', '--mode', type=int, default=None, help='Main simulator mode for generating data. 0: CNPs only, 1: readcounts & CNPs, 2: sequencing reads & CNPs')
     parser.add_argument('-o', '--out-path', type=str, default='CNAsim_output/', help='Path to output directory.')
```

### Comparing `CNAsim-1.3.2/CNAsim/noise.py` & `cnasim-1.3.3/CNAsim/noise.py`

 * *Files identical despite different names*

### Comparing `CNAsim-1.3.2/CNAsim/reads.py` & `cnasim-1.3.3/CNAsim/reads.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from Bio import SeqIO
 
 import numpy as np
 from scipy.stats import beta, poisson
 from scipy.optimize import newton_krylov
 from scipy.optimize.nonlin import NoConvergence
 
-from sequence import *
+from .sequence import *
 
 def iter_by_chunk(iterable, chunksize):
     return itertools.zip_longest(*[iter(iterable)] * chunksize)
 
 def init_pool_processes():
     np.random.seed()
```

### Comparing `CNAsim-1.3.2/CNAsim/sequence.py` & `cnasim-1.3.3/CNAsim/sequence.py`

 * *Files identical despite different names*

### Comparing `CNAsim-1.3.2/CNAsim/sim_genomes.py` & `cnasim-1.3.3/CNAsim/sim_genomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from tree import Tree
+from .tree import Tree
 from collections import Counter
 import os
 import pickle
 
 
 # Categories --> 0: focal, 1: whole-chromosomal, 2: chromosome-arm
 class CNV():
```

### Comparing `CNAsim-1.3.2/CNAsim/tree.py` & `cnasim-1.3.3/CNAsim/tree.py`

 * *Files identical despite different names*

### Comparing `CNAsim-1.3.2/CNAsim/utilities.py` & `cnasim-1.3.3/CNAsim/utilities.py`

 * *Files identical despite different names*

### Comparing `CNAsim-1.3.2/CNAsim.egg-info/PKG-INFO` & `cnasim-1.3.3/CNAsim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: CNAsim
-Version: 1.3.2
+Version: 1.3.3
 Summary: CNAsim is a software package for simulation of single-cell CNA data from tumors.
 Home-page: https://github.com/samsonweiner/CNAsim
 Author: Samson Weiner
 Author-email: samson.weiner@uconn.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: numpy>=1.24.3
+Requires-Dist: scipy>=1.10.1
+Requires-Dist: msprime>=1.2.0
+Requires-Dist: biopython>=1.81
+Requires-Dist: pyfaidx>=0.7.2.1
 
 # CNAsim
 
 CNAsim is a software package for improved simulation of single-cell copy number alteration (CNA) data from tumors. CNAsim can be used to generate copy number profiles with noise patterns that mimic those of single-cell CNA detection algorithms, readcount data with ground truth CNPs, and DNA sequencing reads for sampled cells with ground truth CNPs. It offers significantly improved scalability, a high degree of customizability, and improved biological realism of simulated data.
 
 CNAsim can be cited as follows:
 
 <a href="https://doi.org/10.1093/bioinformatics/btad434">CNAsim: Improved simulation of single-cell copy number profiles and DNA-seq data from tumors</a><br>
 Samson Weiner and Mukul S. Bansal<br>
 Bioinformatics, Volume 39, Issue 7, July 2023, btad434.
 
-Current Version: 1.3.1
+Current Version: 1.3.3
 
 ### New Features
 
 * Sequencing reads can be sampled from two distinct haploid reference genomes, enabling the analysis of allelic frequency. To make sure of this feature, run CNAsim in mode **2** and specify the paths to the reference sequences using the `-r1` and `-r2` parameters.
 * CNAsim can now be used to simulate readcounts directly without having to generate synthetic sequencing reads. This can be achieved by using mode **1**. Passing a reference genome is optional.
 
 <!--
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 2.1 Name: CNAsim Version: 1.3.2 Summary: CNAsim is a software
+Metadata-Version: 2.1 Name: CNAsim Version: 1.3.3 Summary: CNAsim is a software
 package for simulation of single-cell CNA data from tumors. Home-page: https://
 github.com/samsonweiner/CNAsim Author: Samson Weiner Author-email:
 samson.weiner@uconn.edu Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
-markdown License-File: LICENSE.txt # CNAsim CNAsim is a software package for
+markdown License-File: LICENSE.txt Requires-Dist: numpy>=1.24.3 Requires-Dist:
+scipy>=1.10.1 Requires-Dist: msprime>=1.2.0 Requires-Dist: biopython>=1.81
+Requires-Dist: pyfaidx>=0.7.2.1 # CNAsim CNAsim is a software package for
 improved simulation of single-cell copy number alteration (CNA) data from
 tumors. CNAsim can be used to generate copy number profiles with noise patterns
 that mimic those of single-cell CNA detection algorithms, readcount data with
 ground truth CNPs, and DNA sequencing reads for sampled cells with ground truth
 CNPs. It offers significantly improved scalability, a high degree of
 customizability, and improved biological realism of simulated data. CNAsim can
 be cited as follows: _C_N_A_s_i_m_:_ _I_m_p_r_o_v_e_d_ _s_i_m_u_l_a_t_i_o_n_ _o_f_ _s_i_n_g_l_e_-_c_e_l_l_ _c_o_p_y_ _n_u_m_b_e_r
 _p_r_o_f_i_l_e_s_ _a_n_d_ _D_N_A_-_s_e_q_ _d_a_t_a_ _f_r_o_m_ _t_u_m_o_r_s
 Samson Weiner and Mukul S. Bansal
-Bioinformatics, Volume 39, Issue 7, July 2023, btad434. Current Version: 1.3.1
+Bioinformatics, Volume 39, Issue 7, July 2023, btad434. Current Version: 1.3.3
 ### New Features * Sequencing reads can be sampled from two distinct haploid
 reference genomes, enabling the analysis of allelic frequency. To make sure of
 this feature, run CNAsim in mode **2** and specify the paths to the reference
 sequences using the `-r1` and `-r2` parameters. * CNAsim can now be used to
 simulate readcounts directly without having to generate synthetic sequencing
 reads. This can be achieved by using mode **1**. Passing a reference genome is
 optional. # Table of Contents [Installation](#Installation)       [Python
```

### Comparing `CNAsim-1.3.2/LICENSE.txt` & `cnasim-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CNAsim-1.3.2/PKG-INFO` & `cnasim-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: CNAsim
-Version: 1.3.2
+Version: 1.3.3
 Summary: CNAsim is a software package for simulation of single-cell CNA data from tumors.
 Home-page: https://github.com/samsonweiner/CNAsim
 Author: Samson Weiner
 Author-email: samson.weiner@uconn.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: numpy>=1.24.3
+Requires-Dist: scipy>=1.10.1
+Requires-Dist: msprime>=1.2.0
+Requires-Dist: biopython>=1.81
+Requires-Dist: pyfaidx>=0.7.2.1
 
 # CNAsim
 
 CNAsim is a software package for improved simulation of single-cell copy number alteration (CNA) data from tumors. CNAsim can be used to generate copy number profiles with noise patterns that mimic those of single-cell CNA detection algorithms, readcount data with ground truth CNPs, and DNA sequencing reads for sampled cells with ground truth CNPs. It offers significantly improved scalability, a high degree of customizability, and improved biological realism of simulated data.
 
 CNAsim can be cited as follows:
 
 <a href="https://doi.org/10.1093/bioinformatics/btad434">CNAsim: Improved simulation of single-cell copy number profiles and DNA-seq data from tumors</a><br>
 Samson Weiner and Mukul S. Bansal<br>
 Bioinformatics, Volume 39, Issue 7, July 2023, btad434.
 
-Current Version: 1.3.1
+Current Version: 1.3.3
 
 ### New Features
 
 * Sequencing reads can be sampled from two distinct haploid reference genomes, enabling the analysis of allelic frequency. To make sure of this feature, run CNAsim in mode **2** and specify the paths to the reference sequences using the `-r1` and `-r2` parameters.
 * CNAsim can now be used to simulate readcounts directly without having to generate synthetic sequencing reads. This can be achieved by using mode **1**. Passing a reference genome is optional.
 
 <!--
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 2.1 Name: CNAsim Version: 1.3.2 Summary: CNAsim is a software
+Metadata-Version: 2.1 Name: CNAsim Version: 1.3.3 Summary: CNAsim is a software
 package for simulation of single-cell CNA data from tumors. Home-page: https://
 github.com/samsonweiner/CNAsim Author: Samson Weiner Author-email:
 samson.weiner@uconn.edu Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
-markdown License-File: LICENSE.txt # CNAsim CNAsim is a software package for
+markdown License-File: LICENSE.txt Requires-Dist: numpy>=1.24.3 Requires-Dist:
+scipy>=1.10.1 Requires-Dist: msprime>=1.2.0 Requires-Dist: biopython>=1.81
+Requires-Dist: pyfaidx>=0.7.2.1 # CNAsim CNAsim is a software package for
 improved simulation of single-cell copy number alteration (CNA) data from
 tumors. CNAsim can be used to generate copy number profiles with noise patterns
 that mimic those of single-cell CNA detection algorithms, readcount data with
 ground truth CNPs, and DNA sequencing reads for sampled cells with ground truth
 CNPs. It offers significantly improved scalability, a high degree of
 customizability, and improved biological realism of simulated data. CNAsim can
 be cited as follows: _C_N_A_s_i_m_:_ _I_m_p_r_o_v_e_d_ _s_i_m_u_l_a_t_i_o_n_ _o_f_ _s_i_n_g_l_e_-_c_e_l_l_ _c_o_p_y_ _n_u_m_b_e_r
 _p_r_o_f_i_l_e_s_ _a_n_d_ _D_N_A_-_s_e_q_ _d_a_t_a_ _f_r_o_m_ _t_u_m_o_r_s
 Samson Weiner and Mukul S. Bansal
-Bioinformatics, Volume 39, Issue 7, July 2023, btad434. Current Version: 1.3.1
+Bioinformatics, Volume 39, Issue 7, July 2023, btad434. Current Version: 1.3.3
 ### New Features * Sequencing reads can be sampled from two distinct haploid
 reference genomes, enabling the analysis of allelic frequency. To make sure of
 this feature, run CNAsim in mode **2** and specify the paths to the reference
 sequences using the `-r1` and `-r2` parameters. * CNAsim can now be used to
 simulate readcounts directly without having to generate synthetic sequencing
 reads. This can be achieved by using mode **1**. Passing a reference genome is
 optional. # Table of Contents [Installation](#Installation)       [Python
```

### Comparing `CNAsim-1.3.2/README.md` & `cnasim-1.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 CNAsim can be cited as follows:
 
 <a href="https://doi.org/10.1093/bioinformatics/btad434">CNAsim: Improved simulation of single-cell copy number profiles and DNA-seq data from tumors</a><br>
 Samson Weiner and Mukul S. Bansal<br>
 Bioinformatics, Volume 39, Issue 7, July 2023, btad434.
 
-Current Version: 1.3.1
+Current Version: 1.3.3
 
 ### New Features
 
 * Sequencing reads can be sampled from two distinct haploid reference genomes, enabling the analysis of allelic frequency. To make sure of this feature, run CNAsim in mode **2** and specify the paths to the reference sequences using the `-r1` and `-r2` parameters.
 * CNAsim can now be used to simulate readcounts directly without having to generate synthetic sequencing reads. This can be achieved by using mode **1**. Passing a reference genome is optional.
 
 <!--
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 copy number profiles with noise patterns that mimic those of single-cell CNA
 detection algorithms, readcount data with ground truth CNPs, and DNA sequencing
 reads for sampled cells with ground truth CNPs. It offers significantly
 improved scalability, a high degree of customizability, and improved biological
 realism of simulated data. CNAsim can be cited as follows: _C_N_A_s_i_m_:_ _I_m_p_r_o_v_e_d
 _s_i_m_u_l_a_t_i_o_n_ _o_f_ _s_i_n_g_l_e_-_c_e_l_l_ _c_o_p_y_ _n_u_m_b_e_r_ _p_r_o_f_i_l_e_s_ _a_n_d_ _D_N_A_-_s_e_q_ _d_a_t_a_ _f_r_o_m_ _t_u_m_o_r_s
 Samson Weiner and Mukul S. Bansal
-Bioinformatics, Volume 39, Issue 7, July 2023, btad434. Current Version: 1.3.1
+Bioinformatics, Volume 39, Issue 7, July 2023, btad434. Current Version: 1.3.3
 ### New Features * Sequencing reads can be sampled from two distinct haploid
 reference genomes, enabling the analysis of allelic frequency. To make sure of
 this feature, run CNAsim in mode **2** and specify the paths to the reference
 sequences using the `-r1` and `-r2` parameters. * CNAsim can now be used to
 simulate readcounts directly without having to generate synthetic sequencing
 reads. This can be achieved by using mode **1**. Passing a reference genome is
 optional. # Table of Contents [Installation](#Installation)       [Python
```

### Comparing `CNAsim-1.3.2/setup.py` & `cnasim-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CNAsim',
-    version='1.3.2',
+    version='1.3.3',
     author='Samson Weiner',
     author_email='samson.weiner@uconn.edu',
     description='CNAsim is a software package for simulation of single-cell CNA data from tumors.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/samsonweiner/CNAsim',
     classifiers=[
```

