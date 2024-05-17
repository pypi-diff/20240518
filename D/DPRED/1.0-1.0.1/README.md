# Comparing `tmp/DPRED-1.0.tar.gz` & `tmp/DPRED-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DPRED-1.0.tar", last modified: Fri May 17 22:06:30 2024, max compression
+gzip compressed data, was "DPRED-1.0.1.tar", last modified: Fri May 17 22:51:06 2024, max compression
```

## Comparing `DPRED-1.0.tar` & `DPRED-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 22:06:30.610154 DPRED-1.0/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 22:06:29.248110 DPRED-1.0/DPRED/
--rwxrwxrwx   0 root         (0) root         (0)       52 2024-05-17 21:45:14.000000 DPRED-1.0/DPRED/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1166 2024-05-17 21:45:16.000000 DPRED-1.0/DPRED/blast.py
--rwxrwxrwx   0 root         (0) root         (0)     5852 2024-05-17 21:45:18.000000 DPRED-1.0/DPRED/get_pdb_data.py
--rwxrwxrwx   0 root         (0) root         (0)     2657 2024-05-17 22:04:48.000000 DPRED-1.0/DPRED/get_pdb_files.py
--rwxrwxrwx   0 root         (0) root         (0)     1257 2024-05-17 21:45:22.000000 DPRED-1.0/DPRED/get_uniprot_data.py
--rwxrwxrwx   0 root         (0) root         (0)      751 2024-05-17 21:45:24.000000 DPRED-1.0/DPRED/hmm.py
--rwxrwxrwx   0 root         (0) root         (0)     2993 2024-05-17 21:45:27.000000 DPRED-1.0/DPRED/main.py
--rwxrwxrwx   0 root         (0) root         (0)     3483 2024-05-17 22:05:30.000000 DPRED-1.0/DPRED/msa.py
--rwxrwxrwx   0 root         (0) root         (0)     1572 2024-05-17 21:45:30.000000 DPRED-1.0/DPRED/performance.py
--rwxrwxrwx   0 root         (0) root         (0)      271 2024-05-17 21:45:32.000000 DPRED-1.0/DPRED/remove.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 22:06:30.417718 DPRED-1.0/DPRED/src/
--rwxrwxrwx   0 root         (0) root         (0)    11686 2018-07-26 08:18:18.000000 DPRED-1.0/DPRED/src/Kabsch.h
--rwxrwxrwx   0 root         (0) root         (0)      109 2022-01-04 04:17:11.000000 DPRED-1.0/DPRED/src/Makefile
--rwxrwxrwx   0 root         (0) root         (0)     6006 2018-07-26 08:18:17.000000 DPRED-1.0/DPRED/src/NW.h
--rwxrwxrwx   0 root         (0) root         (0)    72079 2022-01-05 10:38:25.000000 DPRED-1.0/DPRED/src/TMM.cpp
--rwxrwxrwx   0 root         (0) root         (0)     3657 2022-01-04 06:07:35.000000 DPRED-1.0/DPRED/src/TMM.h
--rwxrwxrwx   0 root         (0) root         (0)    36346 2018-07-26 08:18:17.000000 DPRED-1.0/DPRED/src/TMalign.h
--rwxrwxrwx   0 root         (0) root         (0)    14228 2018-07-26 08:18:17.000000 DPRED-1.0/DPRED/src/TMalign_main.h
--rwxrwxrwx   0 root         (0) root         (0)    14694 2018-07-26 08:18:17.000000 DPRED-1.0/DPRED/src/UPGMA.cpp
--rwxrwxrwx   0 root         (0) root         (0)     1973 2018-07-26 08:18:17.000000 DPRED-1.0/DPRED/src/UPGMA.h
--rwxrwxrwx   0 root         (0) root         (0)    14990 2018-09-13 06:40:53.000000 DPRED-1.0/DPRED/src/basic_fun.h
--rwxrwxrwx   0 root         (0) root         (0)   347960 2024-04-30 10:42:08.000000 DPRED-1.0/DPRED/src/mTM-align
--rwxrwxrwx   0 root         (0) root         (0)     4179 2022-01-05 10:48:54.000000 DPRED-1.0/DPRED/src/main.cpp
--rwxrwxrwx   0 root         (0) root         (0)     7687 2024-05-17 21:45:34.000000 DPRED-1.0/DPRED/validation.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 22:06:29.547791 DPRED-1.0/DPRED.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 22:06:27.000000 DPRED-1.0/DPRED.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      683 2024-05-17 22:06:28.000000 DPRED-1.0/DPRED.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-17 22:06:27.000000 DPRED-1.0/DPRED.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       42 2024-05-17 22:06:27.000000 DPRED-1.0/DPRED.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       25 2024-05-17 22:06:27.000000 DPRED-1.0/DPRED.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        6 2024-05-17 22:06:27.000000 DPRED-1.0/DPRED.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:08.000000 DPRED-1.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       19 2024-05-17 21:26:51.000000 DPRED-1.0/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 22:06:30.587010 DPRED-1.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:02.000000 DPRED-1.0/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-17 22:06:30.611406 DPRED-1.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      961 2024-05-17 22:05:36.000000 DPRED-1.0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 22:06:30.532796 DPRED-1.0/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:27.000000 DPRED-1.0/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:35.000000 DPRED-1.0/tests/test_main.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 22:51:06.563751 DPRED-1.0.1/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 22:51:05.097180 DPRED-1.0.1/DPRED/
+-rwxrwxrwx   0 root         (0) root         (0)       52 2024-05-17 21:45:14.000000 DPRED-1.0.1/DPRED/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1166 2024-05-17 21:45:16.000000 DPRED-1.0.1/DPRED/blast.py
+-rwxrwxrwx   0 root         (0) root         (0)     5852 2024-05-17 22:44:12.000000 DPRED-1.0.1/DPRED/get_pdb_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     2556 2024-05-17 22:48:46.000000 DPRED-1.0.1/DPRED/get_pdb_files.py
+-rwxrwxrwx   0 root         (0) root         (0)     1257 2024-05-17 22:48:43.000000 DPRED-1.0.1/DPRED/get_uniprot_data.py
+-rwxrwxrwx   0 root         (0) root         (0)      751 2024-05-17 22:48:50.000000 DPRED-1.0.1/DPRED/hmm.py
+-rwxrwxrwx   0 root         (0) root         (0)     2993 2024-05-17 22:48:54.000000 DPRED-1.0.1/DPRED/main.py
+-rwxrwxrwx   0 root         (0) root         (0)     3403 2024-05-17 22:49:26.000000 DPRED-1.0.1/DPRED/msa.py
+-rwxrwxrwx   0 root         (0) root         (0)     1572 2024-05-17 22:49:31.000000 DPRED-1.0.1/DPRED/performance.py
+-rwxrwxrwx   0 root         (0) root         (0)      271 2024-05-17 21:45:32.000000 DPRED-1.0.1/DPRED/remove.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 22:51:06.359473 DPRED-1.0.1/DPRED/src/
+-rwxrwxrwx   0 root         (0) root         (0)    11686 2018-07-26 08:18:18.000000 DPRED-1.0.1/DPRED/src/Kabsch.h
+-rwxrwxrwx   0 root         (0) root         (0)      109 2022-01-04 04:17:11.000000 DPRED-1.0.1/DPRED/src/Makefile
+-rwxrwxrwx   0 root         (0) root         (0)     6006 2018-07-26 08:18:17.000000 DPRED-1.0.1/DPRED/src/NW.h
+-rwxrwxrwx   0 root         (0) root         (0)    72079 2022-01-05 10:38:25.000000 DPRED-1.0.1/DPRED/src/TMM.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     3657 2022-01-04 06:07:35.000000 DPRED-1.0.1/DPRED/src/TMM.h
+-rwxrwxrwx   0 root         (0) root         (0)    36346 2018-07-26 08:18:17.000000 DPRED-1.0.1/DPRED/src/TMalign.h
+-rwxrwxrwx   0 root         (0) root         (0)    14228 2018-07-26 08:18:17.000000 DPRED-1.0.1/DPRED/src/TMalign_main.h
+-rwxrwxrwx   0 root         (0) root         (0)    14694 2018-07-26 08:18:17.000000 DPRED-1.0.1/DPRED/src/UPGMA.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     1973 2018-07-26 08:18:17.000000 DPRED-1.0.1/DPRED/src/UPGMA.h
+-rwxrwxrwx   0 root         (0) root         (0)    14990 2018-09-13 06:40:53.000000 DPRED-1.0.1/DPRED/src/basic_fun.h
+-rwxrwxrwx   0 root         (0) root         (0)   347960 2024-04-30 10:42:08.000000 DPRED-1.0.1/DPRED/src/mTM-align
+-rwxrwxrwx   0 root         (0) root         (0)     4179 2022-01-05 10:48:54.000000 DPRED-1.0.1/DPRED/src/main.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     7687 2024-05-17 21:45:34.000000 DPRED-1.0.1/DPRED/validation.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 22:51:05.403920 DPRED-1.0.1/DPRED.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      538 2024-05-17 22:51:03.000000 DPRED-1.0.1/DPRED.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      683 2024-05-17 22:51:04.000000 DPRED-1.0.1/DPRED.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-17 22:51:03.000000 DPRED-1.0.1/DPRED.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       42 2024-05-17 22:51:03.000000 DPRED-1.0.1/DPRED.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       25 2024-05-17 22:51:03.000000 DPRED-1.0.1/DPRED.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        6 2024-05-17 22:51:03.000000 DPRED-1.0.1/DPRED.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:08.000000 DPRED-1.0.1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       19 2024-05-17 21:26:51.000000 DPRED-1.0.1/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      538 2024-05-17 22:51:06.535146 DPRED-1.0.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:02.000000 DPRED-1.0.1/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-17 22:51:06.563751 DPRED-1.0.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      963 2024-05-17 22:50:21.000000 DPRED-1.0.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 22:51:06.479346 DPRED-1.0.1/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:27.000000 DPRED-1.0.1/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:35.000000 DPRED-1.0.1/tests/test_main.py
```

### Comparing `DPRED-1.0/DPRED/blast.py` & `DPRED-1.0.1/DPRED/blast.py`

 * *Files identical despite different names*

### Comparing `DPRED-1.0/DPRED/get_pdb_data.py` & `DPRED-1.0.1/DPRED/get_pdb_data.py`

 * *Files identical despite different names*

### Comparing `DPRED-1.0/DPRED/get_pdb_files.py` & `DPRED-1.0.1/DPRED/get_pdb_files.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,12 +54,8 @@
                 self._filter_atoms_by_chain(pdbfile, pdbid[:4], chain)
                 i += 1
             remove.Remove('obsolete').remove()
         except Exception as e:
             remove.Remove('msa').remove()
             remove.Remove('input_pdb').remove()
             remove.Remove('obsolete').remove()
-            raise RuntimeError(e)
-
-if __name__ == '__main__':
-    pdb = PDBChainDownloader('PF00014')
-    pdb.download_filtered_pdbs()
+            raise RuntimeError(e)
```

### Comparing `DPRED-1.0/DPRED/get_uniprot_data.py` & `DPRED-1.0.1/DPRED/get_uniprot_data.py`

 * *Files identical despite different names*

### Comparing `DPRED-1.0/DPRED/hmm.py` & `DPRED-1.0.1/DPRED/hmm.py`

 * *Files identical despite different names*

### Comparing `DPRED-1.0/DPRED/main.py` & `DPRED-1.0.1/DPRED/main.py`

 * *Files identical despite different names*

### Comparing `DPRED-1.0/DPRED/msa.py` & `DPRED-1.0.1/DPRED/msa.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,12 +77,8 @@
         start = self._find_start(msa)
         end = self._find_end(msa)
         clean_msa = ''
         for i, line in enumerate(msa.splitlines()): clean_msa += self.ids[i] + line[int(start):int(end)] + '\n'
         return clean_msa
     
     def write_msa(self) -> None:
-        with open('msa', 'w') as f: f.write(self._clear_msa())
-        
-if __name__ == '__main__':
-    obj = MSA('PF00014')
-    obj._msa()
+        with open('msa', 'w') as f: f.write(self._clear_msa())
```

### Comparing `DPRED-1.0/DPRED/performance.py` & `DPRED-1.0.1/DPRED/performance.py`

 * *Files identical despite different names*

### Comparing `DPRED-1.0/DPRED/src/Kabsch.h` & `DPRED-1.0.1/DPRED/src/Kabsch.h`

 * *Files identical despite different names*

### Comparing `DPRED-1.0/DPRED/src/NW.h` & `DPRED-1.0.1/DPRED/src/NW.h`

 * *Files identical despite different names*

### Comparing `DPRED-1.0/DPRED/src/TMM.cpp` & `DPRED-1.0.1/DPRED/src/TMM.cpp`

 * *Files identical despite different names*

### Comparing `DPRED-1.0/DPRED/src/TMM.h` & `DPRED-1.0.1/DPRED/src/TMM.h`

 * *Files identical despite different names*

### Comparing `DPRED-1.0/DPRED/src/TMalign.h` & `DPRED-1.0.1/DPRED/src/TMalign.h`

 * *Files identical despite different names*

### Comparing `DPRED-1.0/DPRED/src/TMalign_main.h` & `DPRED-1.0.1/DPRED/src/TMalign_main.h`

 * *Files identical despite different names*

### Comparing `DPRED-1.0/DPRED/src/UPGMA.cpp` & `DPRED-1.0.1/DPRED/src/UPGMA.cpp`

 * *Files identical despite different names*

### Comparing `DPRED-1.0/DPRED/src/UPGMA.h` & `DPRED-1.0.1/DPRED/src/UPGMA.h`

 * *Files identical despite different names*

### Comparing `DPRED-1.0/DPRED/src/basic_fun.h` & `DPRED-1.0.1/DPRED/src/basic_fun.h`

 * *Files identical despite different names*

### Comparing `DPRED-1.0/DPRED/src/mTM-align` & `DPRED-1.0.1/DPRED/src/mTM-align`

 * *Files identical despite different names*

### Comparing `DPRED-1.0/DPRED/src/main.cpp` & `DPRED-1.0.1/DPRED/src/main.cpp`

 * *Files identical despite different names*

### Comparing `DPRED-1.0/DPRED/validation.py` & `DPRED-1.0.1/DPRED/validation.py`

 * *Files identical despite different names*

### Comparing `DPRED-1.0/DPRED.egg-info/PKG-INFO` & `DPRED-1.0.1/DPRED.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DPRED
-Version: 1.0
+Version: 1.0.1
 Summary: DPRED is a softwares package for HMM domain prediction and validation
 Home-page: https://github.com/dganci/DPRED
 Author: Daniele Ganci
 Author-email: daniele.ganci@studio.unibo.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DPRED-1.0/DPRED.egg-info/SOURCES.txt` & `DPRED-1.0.1/DPRED.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DPRED-1.0/PKG-INFO` & `DPRED-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DPRED
-Version: 1.0
+Version: 1.0.1
 Summary: DPRED is a softwares package for HMM domain prediction and validation
 Home-page: https://github.com/dganci/DPRED
 Author: Daniele Ganci
 Author-email: daniele.ganci@studio.unibo.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DPRED-1.0/setup.py` & `DPRED-1.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='DPRED',
-    version='1.0',
+    version='1.0.1',
     packages=find_packages(include=['DPRED', 'DPRED.*']),
     install_requires=[
         'biopython',
         'requests',
         'numpy',
     ],
     entry_points={
```

