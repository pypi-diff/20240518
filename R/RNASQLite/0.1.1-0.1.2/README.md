# Comparing `tmp/rnasqlite-0.1.1.tar.gz` & `tmp/rnasqlite-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnasqlite-0.1.1.tar", last modified: Sat May 18 13:54:02 2024, max compression
+gzip compressed data, was "rnasqlite-0.1.2.tar", last modified: Sat May 18 13:59:46 2024, max compression
```

## Comparing `rnasqlite-0.1.1.tar` & `rnasqlite-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 13:54:02.748168 rnasqlite-0.1.1/
--rw-rw-rw-   0        0        0      418 2024-05-18 13:54:02.747168 rnasqlite-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1899 2024-05-18 13:46:45.000000 rnasqlite-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 13:54:02.722643 rnasqlite-0.1.1/RNASQLite/
--rw-rw-rw-   0        0        0       23 2024-05-18 13:34:52.000000 rnasqlite-0.1.1/RNASQLite/__init__.py
--rw-rw-rw-   0        0        0     1526 2024-05-18 13:51:07.000000 rnasqlite-0.1.1/RNASQLite/cli.py
--rw-rw-rw-   0        0        0     2097 2024-05-18 13:46:51.000000 rnasqlite-0.1.1/RNASQLite/db_utils.py
--rw-rw-rw-   0        0        0     3676 2024-05-18 13:46:48.000000 rnasqlite-0.1.1/RNASQLite/process_file.py
-drwxrwxrwx   0        0        0        0 2024-05-18 13:54:02.746168 rnasqlite-0.1.1/RNASQLite.egg-info/
--rw-rw-rw-   0        0        0      418 2024-05-18 13:54:02.000000 rnasqlite-0.1.1/RNASQLite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-18 13:54:02.000000 rnasqlite-0.1.1/RNASQLite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 13:54:02.000000 rnasqlite-0.1.1/RNASQLite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-18 13:54:02.000000 rnasqlite-0.1.1/RNASQLite.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2024-05-18 13:54:02.000000 rnasqlite-0.1.1/RNASQLite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 13:54:02.000000 rnasqlite-0.1.1/RNASQLite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 13:54:02.748168 rnasqlite-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      727 2024-05-18 13:52:44.000000 rnasqlite-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 13:59:46.692927 rnasqlite-0.1.2/
+-rw-rw-rw-   0        0        0      418 2024-05-18 13:59:46.690924 rnasqlite-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1899 2024-05-18 13:46:45.000000 rnasqlite-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 13:59:46.665906 rnasqlite-0.1.2/RNASQLite/
+-rw-rw-rw-   0        0        0       23 2024-05-18 13:34:52.000000 rnasqlite-0.1.2/RNASQLite/__init__.py
+-rw-rw-rw-   0        0        0     1628 2024-05-18 13:59:18.000000 rnasqlite-0.1.2/RNASQLite/cli.py
+-rw-rw-rw-   0        0        0     2097 2024-05-18 13:46:51.000000 rnasqlite-0.1.2/RNASQLite/db_utils.py
+-rw-rw-rw-   0        0        0     3676 2024-05-18 13:46:48.000000 rnasqlite-0.1.2/RNASQLite/process_file.py
+drwxrwxrwx   0        0        0        0 2024-05-18 13:59:46.689927 rnasqlite-0.1.2/RNASQLite.egg-info/
+-rw-rw-rw-   0        0        0      418 2024-05-18 13:59:46.000000 rnasqlite-0.1.2/RNASQLite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-18 13:59:46.000000 rnasqlite-0.1.2/RNASQLite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 13:59:46.000000 rnasqlite-0.1.2/RNASQLite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-18 13:59:46.000000 rnasqlite-0.1.2/RNASQLite.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2024-05-18 13:59:46.000000 rnasqlite-0.1.2/RNASQLite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-18 13:59:46.000000 rnasqlite-0.1.2/RNASQLite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 13:59:46.692927 rnasqlite-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      727 2024-05-18 13:59:16.000000 rnasqlite-0.1.2/setup.py
```

### Comparing `rnasqlite-0.1.1/README.md` & `rnasqlite-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.1/RNASQLite/cli.py` & `rnasqlite-0.1.2/RNASQLite/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import argparse
-import os  # os 모듈을 임포트합니다.
+import os
 from RNASQLite.db_utils import setup_database, insert_counts_into_db, get_count_files, fetch_all_samples
 from RNASQLite.process_file import process_file
 
 def main():
     parser = argparse.ArgumentParser(description='RNASQLite command line tool')
     parser.add_argument('-create', action='store_true', help='Create the SQLite database')
     parser.add_argument('-split', type=str, help='Process RNAseq counts file and split into count files')
@@ -14,15 +14,18 @@
     db_path = 'geo_rna_seq.db'  # SQLite 데이터베이스 파일 경로
     counts_dir = 'counts'  # Counts 파일이 저장될 디렉토리
 
     if args.create:
         setup_database(db_path)
     elif args.split:
         rna_seq_counts_path = args.split
-        gene_info_path = os.path.join(os.path.dirname(__file__), '..', 'gene_info.csv')  # gene_info 파일 경로를 고정
+        gene_info_path = 'gene_info.csv'  # 실행 디렉토리에서 gene_info.csv 파일을 찾습니다
+        if not os.path.isfile(gene_info_path):
+            print(f"Error: {gene_info_path} file not found in the current directory.")
+            return
         process_file(gene_info_path, rna_seq_counts_path, counts_dir)
     elif args.load:
         count_files = get_count_files(counts_dir)
         insert_counts_into_db(db_path, count_files)
     elif args.fetch:
         fetch_all_samples(db_path)
     else:
```

### Comparing `rnasqlite-0.1.1/RNASQLite/db_utils.py` & `rnasqlite-0.1.2/RNASQLite/db_utils.py`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.1/RNASQLite/process_file.py` & `rnasqlite-0.1.2/RNASQLite/process_file.py`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.1/setup.py` & `rnasqlite-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RNASQLite',
-    version='0.1.1',  # 버전을 업데이트합니다.
+    version='0.1.2',  # 버전을 업데이트합니다.
     packages=find_packages(),
     install_requires=[
         'pandas',
     ],
     entry_points={
         'console_scripts': [
             'RNASQLite=RNASQLite.cli:main',
```

