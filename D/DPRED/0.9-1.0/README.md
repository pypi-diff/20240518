# Comparing `tmp/DPRED-0.9.tar.gz` & `tmp/DPRED-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DPRED-0.9.tar", last modified: Fri May 17 21:46:43 2024, max compression
+gzip compressed data, was "DPRED-1.0.tar", last modified: Fri May 17 22:06:30 2024, max compression
```

## Comparing `DPRED-0.9.tar` & `DPRED-1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:46:43.181473 DPRED-0.9/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:46:41.547348 DPRED-0.9/DPRED/
--rwxrwxrwx   0 root         (0) root         (0)       52 2024-05-17 21:45:14.000000 DPRED-0.9/DPRED/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1166 2024-05-17 21:45:16.000000 DPRED-0.9/DPRED/blast.py
--rwxrwxrwx   0 root         (0) root         (0)     5852 2024-05-17 21:45:18.000000 DPRED-0.9/DPRED/get_pdb_data.py
--rwxrwxrwx   0 root         (0) root         (0)     2383 2024-05-17 21:45:20.000000 DPRED-0.9/DPRED/get_pdb_files.py
--rwxrwxrwx   0 root         (0) root         (0)     1257 2024-05-17 21:45:22.000000 DPRED-0.9/DPRED/get_uniprot_data.py
--rwxrwxrwx   0 root         (0) root         (0)      751 2024-05-17 21:45:24.000000 DPRED-0.9/DPRED/hmm.py
--rwxrwxrwx   0 root         (0) root         (0)     2993 2024-05-17 21:45:27.000000 DPRED-0.9/DPRED/main.py
--rwxrwxrwx   0 root         (0) root         (0)     3472 2024-05-17 21:45:29.000000 DPRED-0.9/DPRED/msa.py
--rwxrwxrwx   0 root         (0) root         (0)     1572 2024-05-17 21:45:30.000000 DPRED-0.9/DPRED/performance.py
--rwxrwxrwx   0 root         (0) root         (0)      271 2024-05-17 21:45:32.000000 DPRED-0.9/DPRED/remove.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:46:43.001540 DPRED-0.9/DPRED/src/
--rwxrwxrwx   0 root         (0) root         (0)    11686 2018-07-26 08:18:18.000000 DPRED-0.9/DPRED/src/Kabsch.h
--rwxrwxrwx   0 root         (0) root         (0)      109 2022-01-04 04:17:11.000000 DPRED-0.9/DPRED/src/Makefile
--rwxrwxrwx   0 root         (0) root         (0)     6006 2018-07-26 08:18:17.000000 DPRED-0.9/DPRED/src/NW.h
--rwxrwxrwx   0 root         (0) root         (0)    72079 2022-01-05 10:38:25.000000 DPRED-0.9/DPRED/src/TMM.cpp
--rwxrwxrwx   0 root         (0) root         (0)     3657 2022-01-04 06:07:35.000000 DPRED-0.9/DPRED/src/TMM.h
--rwxrwxrwx   0 root         (0) root         (0)    36346 2018-07-26 08:18:17.000000 DPRED-0.9/DPRED/src/TMalign.h
--rwxrwxrwx   0 root         (0) root         (0)    14228 2018-07-26 08:18:17.000000 DPRED-0.9/DPRED/src/TMalign_main.h
--rwxrwxrwx   0 root         (0) root         (0)    14694 2018-07-26 08:18:17.000000 DPRED-0.9/DPRED/src/UPGMA.cpp
--rwxrwxrwx   0 root         (0) root         (0)     1973 2018-07-26 08:18:17.000000 DPRED-0.9/DPRED/src/UPGMA.h
--rwxrwxrwx   0 root         (0) root         (0)    14990 2018-09-13 06:40:53.000000 DPRED-0.9/DPRED/src/basic_fun.h
--rwxrwxrwx   0 root         (0) root         (0)   347960 2024-04-30 10:42:08.000000 DPRED-0.9/DPRED/src/mTM-align
--rwxrwxrwx   0 root         (0) root         (0)     4179 2022-01-05 10:48:54.000000 DPRED-0.9/DPRED/src/main.cpp
--rwxrwxrwx   0 root         (0) root         (0)     7687 2024-05-17 21:45:34.000000 DPRED-0.9/DPRED/validation.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:46:41.817075 DPRED-0.9/DPRED.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 21:46:40.000000 DPRED-0.9/DPRED.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      683 2024-05-17 21:46:40.000000 DPRED-0.9/DPRED.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-17 21:46:40.000000 DPRED-0.9/DPRED.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       42 2024-05-17 21:46:40.000000 DPRED-0.9/DPRED.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       25 2024-05-17 21:46:40.000000 DPRED-0.9/DPRED.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        6 2024-05-17 21:46:40.000000 DPRED-0.9/DPRED.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:08.000000 DPRED-0.9/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       19 2024-05-17 21:26:51.000000 DPRED-0.9/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 21:46:43.158176 DPRED-0.9/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:02.000000 DPRED-0.9/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-17 21:46:43.181473 DPRED-0.9/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      961 2024-05-17 21:45:40.000000 DPRED-0.9/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:46:43.096194 DPRED-0.9/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:27.000000 DPRED-0.9/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:35.000000 DPRED-0.9/tests/test_main.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 22:06:30.610154 DPRED-1.0/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 22:06:29.248110 DPRED-1.0/DPRED/
+-rwxrwxrwx   0 root         (0) root         (0)       52 2024-05-17 21:45:14.000000 DPRED-1.0/DPRED/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1166 2024-05-17 21:45:16.000000 DPRED-1.0/DPRED/blast.py
+-rwxrwxrwx   0 root         (0) root         (0)     5852 2024-05-17 21:45:18.000000 DPRED-1.0/DPRED/get_pdb_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     2657 2024-05-17 22:04:48.000000 DPRED-1.0/DPRED/get_pdb_files.py
+-rwxrwxrwx   0 root         (0) root         (0)     1257 2024-05-17 21:45:22.000000 DPRED-1.0/DPRED/get_uniprot_data.py
+-rwxrwxrwx   0 root         (0) root         (0)      751 2024-05-17 21:45:24.000000 DPRED-1.0/DPRED/hmm.py
+-rwxrwxrwx   0 root         (0) root         (0)     2993 2024-05-17 21:45:27.000000 DPRED-1.0/DPRED/main.py
+-rwxrwxrwx   0 root         (0) root         (0)     3483 2024-05-17 22:05:30.000000 DPRED-1.0/DPRED/msa.py
+-rwxrwxrwx   0 root         (0) root         (0)     1572 2024-05-17 21:45:30.000000 DPRED-1.0/DPRED/performance.py
+-rwxrwxrwx   0 root         (0) root         (0)      271 2024-05-17 21:45:32.000000 DPRED-1.0/DPRED/remove.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 22:06:30.417718 DPRED-1.0/DPRED/src/
+-rwxrwxrwx   0 root         (0) root         (0)    11686 2018-07-26 08:18:18.000000 DPRED-1.0/DPRED/src/Kabsch.h
+-rwxrwxrwx   0 root         (0) root         (0)      109 2022-01-04 04:17:11.000000 DPRED-1.0/DPRED/src/Makefile
+-rwxrwxrwx   0 root         (0) root         (0)     6006 2018-07-26 08:18:17.000000 DPRED-1.0/DPRED/src/NW.h
+-rwxrwxrwx   0 root         (0) root         (0)    72079 2022-01-05 10:38:25.000000 DPRED-1.0/DPRED/src/TMM.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     3657 2022-01-04 06:07:35.000000 DPRED-1.0/DPRED/src/TMM.h
+-rwxrwxrwx   0 root         (0) root         (0)    36346 2018-07-26 08:18:17.000000 DPRED-1.0/DPRED/src/TMalign.h
+-rwxrwxrwx   0 root         (0) root         (0)    14228 2018-07-26 08:18:17.000000 DPRED-1.0/DPRED/src/TMalign_main.h
+-rwxrwxrwx   0 root         (0) root         (0)    14694 2018-07-26 08:18:17.000000 DPRED-1.0/DPRED/src/UPGMA.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     1973 2018-07-26 08:18:17.000000 DPRED-1.0/DPRED/src/UPGMA.h
+-rwxrwxrwx   0 root         (0) root         (0)    14990 2018-09-13 06:40:53.000000 DPRED-1.0/DPRED/src/basic_fun.h
+-rwxrwxrwx   0 root         (0) root         (0)   347960 2024-04-30 10:42:08.000000 DPRED-1.0/DPRED/src/mTM-align
+-rwxrwxrwx   0 root         (0) root         (0)     4179 2022-01-05 10:48:54.000000 DPRED-1.0/DPRED/src/main.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     7687 2024-05-17 21:45:34.000000 DPRED-1.0/DPRED/validation.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 22:06:29.547791 DPRED-1.0/DPRED.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 22:06:27.000000 DPRED-1.0/DPRED.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      683 2024-05-17 22:06:28.000000 DPRED-1.0/DPRED.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-17 22:06:27.000000 DPRED-1.0/DPRED.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       42 2024-05-17 22:06:27.000000 DPRED-1.0/DPRED.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       25 2024-05-17 22:06:27.000000 DPRED-1.0/DPRED.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        6 2024-05-17 22:06:27.000000 DPRED-1.0/DPRED.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:08.000000 DPRED-1.0/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       19 2024-05-17 21:26:51.000000 DPRED-1.0/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 22:06:30.587010 DPRED-1.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:02.000000 DPRED-1.0/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-17 22:06:30.611406 DPRED-1.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      961 2024-05-17 22:05:36.000000 DPRED-1.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 22:06:30.532796 DPRED-1.0/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:27.000000 DPRED-1.0/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:35.000000 DPRED-1.0/tests/test_main.py
```

### Comparing `DPRED-0.9/DPRED/blast.py` & `DPRED-1.0/DPRED/blast.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.9/DPRED/get_pdb_data.py` & `DPRED-1.0/DPRED/get_pdb_data.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.9/DPRED/get_pdb_files.py` & `DPRED-1.0/DPRED/get_pdb_files.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from Bio.PDB import PDBList, PDBParser, PDBIO, Select
 import logging
 import os
+import warnings
 
 from . import remove
 
 logging.getLogger("Bio").setLevel(logging.ERROR)
 
 class ChainSelector(Select):
     '''A chain selector for Bio.PDB'''
@@ -39,16 +40,21 @@
         '''Downloads the chain-filtered PDB files'''
         try:
             pdblist = PDBList(verbose=False)
             i = 0
             for pdbid in self.pdbids:
                 chain = pdbid[4]
                 pdblist.retrieve_pdb_file(pdbid[:4], pdir=self.outdir, file_format='pdb', overwrite=True) 
-                self._rename_file(chain, i)    
+                self._rename_file(chain, i)
                 pdbfile = os.path.join(self.outdir, f"pdb{pdbid[:4]}_{chain}.pdb")
+                # if a .ent file is still kept, continue
+                if os.path.splitext(pdbfile)[1] == ".ent":
+                    os.remove(pdbfile)
+                    warnings.warn(f"It was not possible to download {pdbid}")
+                    continue
                 self._filter_atoms_by_chain(pdbfile, pdbid[:4], chain)
                 i += 1
             remove.Remove('obsolete').remove()
         except Exception as e:
             remove.Remove('msa').remove()
             remove.Remove('input_pdb').remove()
             remove.Remove('obsolete').remove()
```

### Comparing `DPRED-0.9/DPRED/get_uniprot_data.py` & `DPRED-1.0/DPRED/get_uniprot_data.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.9/DPRED/hmm.py` & `DPRED-1.0/DPRED/hmm.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.9/DPRED/main.py` & `DPRED-1.0/DPRED/main.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.9/DPRED/msa.py` & `DPRED-1.0/DPRED/msa.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         print(f'Done. Time = {int(round(h))}:{int(round(m))}:{int(round(s))}')
     
     def _msa(self) -> None:
         if not os.path.exists(self.pdbdir): self._download_pdb()    
         with open('pdblst', 'w') as f: f.write(self.pdbobj.get_lst())
         start = time.time()
         print('Performing multiple structural alignment...')
-        subprocess.run([os.path.join(os.path.dirname(DPRED.__file__), 'src', 'mTM-align'), "-i", "pdblst"], stdout=subprocess.DEVNULL)
+        subprocess.run([os.path.join(os.path.abspath(os.path.dirname(__file__)), 'src', 'mTM-align'), "-i", "pdblst"], stdout=subprocess.DEVNULL)
         lap = time.time()-start
         h, rem = divmod(lap, 3600)
         m, s = divmod(rem, 60)
         print(f'Done. Time = {int(round(h))}:{int(round(m))}:{int(round(s))}')
         if self.pdb is False: remove.Remove(self.pdbdir).remove() # remove input_pdb
         if self.mtm is False: remove.Remove('pdblst').remove() # remove pdblst
```

### Comparing `DPRED-0.9/DPRED/performance.py` & `DPRED-1.0/DPRED/performance.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.9/DPRED/src/Kabsch.h` & `DPRED-1.0/DPRED/src/Kabsch.h`

 * *Files identical despite different names*

### Comparing `DPRED-0.9/DPRED/src/NW.h` & `DPRED-1.0/DPRED/src/NW.h`

 * *Files identical despite different names*

### Comparing `DPRED-0.9/DPRED/src/TMM.cpp` & `DPRED-1.0/DPRED/src/TMM.cpp`

 * *Files identical despite different names*

### Comparing `DPRED-0.9/DPRED/src/TMM.h` & `DPRED-1.0/DPRED/src/TMM.h`

 * *Files identical despite different names*

### Comparing `DPRED-0.9/DPRED/src/TMalign.h` & `DPRED-1.0/DPRED/src/TMalign.h`

 * *Files identical despite different names*

### Comparing `DPRED-0.9/DPRED/src/TMalign_main.h` & `DPRED-1.0/DPRED/src/TMalign_main.h`

 * *Files identical despite different names*

### Comparing `DPRED-0.9/DPRED/src/UPGMA.cpp` & `DPRED-1.0/DPRED/src/UPGMA.cpp`

 * *Files identical despite different names*

### Comparing `DPRED-0.9/DPRED/src/UPGMA.h` & `DPRED-1.0/DPRED/src/UPGMA.h`

 * *Files identical despite different names*

### Comparing `DPRED-0.9/DPRED/src/basic_fun.h` & `DPRED-1.0/DPRED/src/basic_fun.h`

 * *Files identical despite different names*

### Comparing `DPRED-0.9/DPRED/src/mTM-align` & `DPRED-1.0/DPRED/src/mTM-align`

 * *Files identical despite different names*

### Comparing `DPRED-0.9/DPRED/src/main.cpp` & `DPRED-1.0/DPRED/src/main.cpp`

 * *Files identical despite different names*

### Comparing `DPRED-0.9/DPRED/validation.py` & `DPRED-1.0/DPRED/validation.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.9/DPRED.egg-info/PKG-INFO` & `DPRED-1.0/DPRED.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DPRED
-Version: 0.9
+Version: 1.0
 Summary: DPRED is a softwares package for HMM domain prediction and validation
 Home-page: https://github.com/dganci/DPRED
 Author: Daniele Ganci
 Author-email: daniele.ganci@studio.unibo.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DPRED-0.9/DPRED.egg-info/SOURCES.txt` & `DPRED-1.0/DPRED.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DPRED-0.9/PKG-INFO` & `DPRED-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DPRED
-Version: 0.9
+Version: 1.0
 Summary: DPRED is a softwares package for HMM domain prediction and validation
 Home-page: https://github.com/dganci/DPRED
 Author: Daniele Ganci
 Author-email: daniele.ganci@studio.unibo.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DPRED-0.9/setup.py` & `DPRED-1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='DPRED',
-    version='0.9',
+    version='1.0',
     packages=find_packages(include=['DPRED', 'DPRED.*']),
     install_requires=[
         'biopython',
         'requests',
         'numpy',
     ],
     entry_points={
```

