# Comparing `tmp/rnasqlite-0.1.2.tar.gz` & `tmp/rnasqlite-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnasqlite-0.1.2.tar", last modified: Sat May 18 13:59:46 2024, max compression
+gzip compressed data, was "rnasqlite-0.1.3.tar", last modified: Sat May 18 14:19:56 2024, max compression
```

## Comparing `rnasqlite-0.1.2.tar` & `rnasqlite-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 13:59:46.692927 rnasqlite-0.1.2/
--rw-rw-rw-   0        0        0      418 2024-05-18 13:59:46.690924 rnasqlite-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1899 2024-05-18 13:46:45.000000 rnasqlite-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 13:59:46.665906 rnasqlite-0.1.2/RNASQLite/
--rw-rw-rw-   0        0        0       23 2024-05-18 13:34:52.000000 rnasqlite-0.1.2/RNASQLite/__init__.py
--rw-rw-rw-   0        0        0     1628 2024-05-18 13:59:18.000000 rnasqlite-0.1.2/RNASQLite/cli.py
--rw-rw-rw-   0        0        0     2097 2024-05-18 13:46:51.000000 rnasqlite-0.1.2/RNASQLite/db_utils.py
--rw-rw-rw-   0        0        0     3676 2024-05-18 13:46:48.000000 rnasqlite-0.1.2/RNASQLite/process_file.py
-drwxrwxrwx   0        0        0        0 2024-05-18 13:59:46.689927 rnasqlite-0.1.2/RNASQLite.egg-info/
--rw-rw-rw-   0        0        0      418 2024-05-18 13:59:46.000000 rnasqlite-0.1.2/RNASQLite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-18 13:59:46.000000 rnasqlite-0.1.2/RNASQLite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 13:59:46.000000 rnasqlite-0.1.2/RNASQLite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-18 13:59:46.000000 rnasqlite-0.1.2/RNASQLite.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2024-05-18 13:59:46.000000 rnasqlite-0.1.2/RNASQLite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 13:59:46.000000 rnasqlite-0.1.2/RNASQLite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 13:59:46.692927 rnasqlite-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      727 2024-05-18 13:59:16.000000 rnasqlite-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:19:56.554349 rnasqlite-0.1.3/
+-rw-rw-rw-   0        0        0      418 2024-05-18 14:19:56.553349 rnasqlite-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1452 2024-05-18 14:18:11.000000 rnasqlite-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 14:19:56.522825 rnasqlite-0.1.3/RNASQLite/
+-rw-rw-rw-   0        0        0       23 2024-05-18 13:34:52.000000 rnasqlite-0.1.3/RNASQLite/__init__.py
+-rw-rw-rw-   0        0        0     1628 2024-05-18 13:59:18.000000 rnasqlite-0.1.3/RNASQLite/cli.py
+-rw-rw-rw-   0        0        0     2097 2024-05-18 13:46:51.000000 rnasqlite-0.1.3/RNASQLite/db_utils.py
+-rw-rw-rw-   0        0        0     3676 2024-05-18 13:46:48.000000 rnasqlite-0.1.3/RNASQLite/process_file.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:19:56.552348 rnasqlite-0.1.3/RNASQLite.egg-info/
+-rw-rw-rw-   0        0        0      418 2024-05-18 14:19:56.000000 rnasqlite-0.1.3/RNASQLite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-18 14:19:56.000000 rnasqlite-0.1.3/RNASQLite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 14:19:56.000000 rnasqlite-0.1.3/RNASQLite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-18 14:19:56.000000 rnasqlite-0.1.3/RNASQLite.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2024-05-18 14:19:56.000000 rnasqlite-0.1.3/RNASQLite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-18 14:19:56.000000 rnasqlite-0.1.3/RNASQLite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 14:19:56.554349 rnasqlite-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      727 2024-05-18 14:19:40.000000 rnasqlite-0.1.3/setup.py
```

### Comparing `rnasqlite-0.1.2/README.md` & `rnasqlite-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,38 @@
-# RNASQLite
-
+RNASQLite
 RNASQLite is a tool for managing RNA-Seq data with SQLite. This package allows you to process RNA-Seq counts files, insert count files into a database, and retrieve sample information from the database.
 
-## Installation
-
+Installation
 First, navigate to the directory containing setup.py and install the package.
 
 pip install .
 
-## Usage
-
-1. Create Database
-
+Usage
+Create Database
 Create a new database. If a database file with the same name already exists, it will be deleted.
 
 RNASQLite -create
 
-2. Process and Split RNAseq Counts File
-
+Process and Split RNAseq Counts File
 Process the given RNAseq counts file and save the count files for each sample in the counts directory. This step uses the gene info file (gene_info.csv) to add gene information.
 
 RNASQLite -split path/to/your/rna_seq_counts_file.csv
 
-3. Insert Count Files into Database
-
+Insert Count Files into Database
 Read the count files from the counts directory and insert them into the database.
 
 RNASQLite -load
 
-4. Fetch All Samples from Database
-
+Fetch All Samples from Database
 Retrieve all sample information from the database.
 
 RNASQLite -fetch
 
-## File Structure
-
-RNASQLite/
-├── RNASQLite/
-│   ├── __init__.py
-│   ├── cli.py
-│   ├── db_utils.py
-│   └── process_file.py
-├── gene_info.csv
-├── setup.py
-└── README.md
-
-### Description
-
-- RNASQLite/cli.py: Handles the command line interface.
-- RNASQLite/db_utils.py: Contains utility functions related to the database.
-- RNASQLite/process_file.py: Processes the given gene_info.csv and RNAseq counts file to generate count files.
-- gene_info.csv: CSV file containing gene information.
-- setup.py: Contains package metadata and dependencies.
-- README.md: This file, which includes the description and usage of the RNASQLite package.
 
-### Note
 
-The gene_info.csv file should be placed in the root directory of the project. This ensures that all scripts can reference the gene_info.csv file.
+Description
+RNASQLite/cli.py: Handles the command line interface.
+RNASQLite/db_utils.py: Contains utility functions related to the database.
+RNASQLite/process_file.py: Processes the given gene_info.csv and RNAseq counts file to generate count files.
+gene_info.csv: CSV file containing gene information.
+setup.py: Contains package metadata and dependencies.
+README.md: This file, which includes the description and usage of the RNASQLite package.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rnasqlite-0.1.2/RNASQLite/cli.py` & `rnasqlite-0.1.3/RNASQLite/cli.py`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.2/RNASQLite/db_utils.py` & `rnasqlite-0.1.3/RNASQLite/db_utils.py`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.2/RNASQLite/process_file.py` & `rnasqlite-0.1.3/RNASQLite/process_file.py`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.2/setup.py` & `rnasqlite-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RNASQLite',
-    version='0.1.2',  # 버전을 업데이트합니다.
+    version='0.1.3',  # 버전을 업데이트합니다.
     packages=find_packages(),
     install_requires=[
         'pandas',
     ],
     entry_points={
         'console_scripts': [
             'RNASQLite=RNASQLite.cli:main',
```

