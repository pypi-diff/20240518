# Comparing `tmp/taffy-0.0.2.tar.gz` & `tmp/taffy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taffy-0.0.2.tar", last modified: Wed Feb  7 05:27:41 2024, max compression
+gzip compressed data, was "taffy-0.0.3.tar", last modified: Fri May 17 21:58:19 2024, max compression
```

## Comparing `taffy-0.0.2.tar` & `taffy-0.0.3.tar`

### file list

```diff
@@ -1,129 +1,136 @@
-drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-02-07 05:27:41.414598 taffy-0.0.2/
--rw-r--r--   0 benedictpaten   (501) staff       (20)     1071 2022-11-30 22:52:38.000000 taffy-0.0.2/LICENSE
--rw-r--r--   0 benedictpaten   (501) staff       (20)    26231 2024-02-07 05:27:41.414353 taffy-0.0.2/PKG-INFO
--rw-r--r--   0 benedictpaten   (501) staff       (20)    25579 2024-02-07 05:07:31.000000 taffy-0.0.2/README.md
--rw-r--r--   0 benedictpaten   (501) staff       (20)      746 2024-02-07 05:23:17.000000 taffy-0.0.2/pyproject.toml
--rw-r--r--   0 benedictpaten   (501) staff       (20)       38 2024-02-07 05:27:41.414640 taffy-0.0.2/setup.cfg
--rw-r--r--   0 benedictpaten   (501) staff       (20)      662 2022-12-30 18:28:33.000000 taffy-0.0.2/setup.py
-drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-02-07 05:27:41.392838 taffy-0.0.2/taffy/
--rw-r--r--   0 benedictpaten   (501) staff       (20)        0 2022-11-30 22:52:38.000000 taffy-0.0.2/taffy/__init__.py
--rw-r--r--   0 benedictpaten   (501) staff       (20)    10526 2024-02-03 17:34:31.000000 taffy-0.0.2/taffy/_taffy_build.py
-drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-02-07 05:27:41.396295 taffy-0.0.2/taffy/impl/
--rw-r--r--   0 benedictpaten   (501) staff       (20)    12164 2024-02-07 05:07:31.000000 taffy-0.0.2/taffy/impl/alignment_block.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     3431 2023-12-29 12:34:58.000000 taffy-0.0.2/taffy/impl/line_iterator.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     4014 2024-02-03 17:34:31.000000 taffy-0.0.2/taffy/impl/maf.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    13035 2024-02-07 05:07:31.000000 taffy-0.0.2/taffy/impl/merge_adjacent_alignments.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    11715 2022-11-30 22:52:38.000000 taffy-0.0.2/taffy/impl/ond.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     7203 2024-02-03 17:34:31.000000 taffy-0.0.2/taffy/impl/paf.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     7187 2024-02-07 05:07:31.000000 taffy-0.0.2/taffy/impl/prefix_sort.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    22430 2024-02-07 05:07:31.000000 taffy-0.0.2/taffy/impl/taf.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    25689 2024-02-03 17:34:31.000000 taffy-0.0.2/taffy/impl/tai.c
-drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-02-07 05:27:41.397135 taffy-0.0.2/taffy/inc/
--rw-r--r--   0 benedictpaten   (501) staff       (20)     1698 2023-12-29 12:34:58.000000 taffy-0.0.2/taffy/inc/line_iterator.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)      535 2022-11-30 22:52:38.000000 taffy-0.0.2/taffy/inc/ond.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)    12101 2024-02-07 05:07:31.000000 taffy-0.0.2/taffy/inc/taf.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     2020 2023-12-29 12:34:58.000000 taffy-0.0.2/taffy/inc/tai.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)    16413 2024-02-03 17:34:31.000000 taffy-0.0.2/taffy/lib.py
--rw-r--r--   0 benedictpaten   (501) staff       (20)     1720 2023-12-29 12:34:58.000000 taffy-0.0.2/taffy/ml.py
-drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-02-07 05:27:41.390831 taffy-0.0.2/taffy/submodules/
-drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-02-07 05:27:41.391077 taffy-0.0.2/taffy/submodules/sonLib/
-drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-02-07 05:27:41.391007 taffy-0.0.2/taffy/submodules/sonLib/C/
-drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-02-07 05:27:41.406487 taffy-0.0.2/taffy/submodules/sonLib/C/impl/
--rw-r--r--   0 benedictpaten   (501) staff       (20)    28457 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/avl.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    18523 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/bioioC.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    24787 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/commonC.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     4989 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/fastCMaths.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    10345 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/hashTableC.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     5553 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/hashTableC_itr.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     8916 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/jsmn.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    30948 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/lz4.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     5600 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/lz4.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)    23496 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/lz4hc.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     2295 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/lz4hc.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     7536 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/pairwiseAlignment.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    14185 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibCache.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     5720 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibCommon.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     9206 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibCompression.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    28217 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibConnectivity.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    22979 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibEulerTour.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     3189 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibExcept.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     4279 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibFile.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)      681 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibGlobalsInternal.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     7474 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibHash.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    20270 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibKVDatabase.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    13238 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibKVDatabaseConf.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     2862 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibKVDatabasePrivate.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     9492 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibKVDatabase_BigRecordFile.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    18106 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibKVDatabase_MySql.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    11772 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibKVDatabase_Redis.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    12698 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibKVDatabase_TokyoCabinet.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    11441 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibList.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)      357 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibListPrivate.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     1431 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibMath.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    11498 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibNaiveConnectivity.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     2127 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibRandom.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     7186 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibSet.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    11218 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibSortedSet.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     6721 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibString.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    11707 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibTreap.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    13505 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibTree.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     5704 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibTuples.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     3102 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/stGraph.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     2372 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/stJson.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     4226 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/stMatrix.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    87278 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/stPhylogeny.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)    10359 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/stPosetAlignment.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     3764 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/stSafeC.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     8525 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/stThreadPool.c
--rw-r--r--   0 benedictpaten   (501) staff       (20)     3223 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/impl/stUnionFind.c
-drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-02-07 05:27:41.413563 taffy-0.0.2/taffy/submodules/sonLib/C/inc/
--rw-r--r--   0 benedictpaten   (501) staff       (20)     5078 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/avl.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     5046 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/bioioC.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     7990 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/commonC.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     3236 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/fastCMaths.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     7615 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/hashTableC.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     4149 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/hashTableC_itr.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     3094 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/hashTablePrivateC.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     2697 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/jsmn.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     1566 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/pairwiseAlignment.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     1306 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/safesort.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     1027 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLib.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     2493 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibCache.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     2753 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibCommon.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     1443 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibCompression.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     4049 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibConnectivity.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     2813 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibEulerTour.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     6403 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibExcept.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     2342 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibFile.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     3676 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibHash.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     7022 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibKVDatabase.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     4385 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibKVDatabaseConf.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     7308 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibList.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)      598 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibMath.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     1479 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibNaiveConnectivity.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     1565 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibRandom.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     3312 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibSet.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     5412 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibSortedSet.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     3517 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibString.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     1716 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibTreap.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     3126 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibTree.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     2670 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibTuples.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     2791 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibTypes.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)      984 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/stGraph.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     1134 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/stJson.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     2000 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/stMatrix.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)    10503 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/stPhylogeny.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     1260 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/stPosetAlignment.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     2619 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/stSafeC.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)      875 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/stSpimapLayer.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     2128 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/stThreadPool.h
--rw-r--r--   0 benedictpaten   (501) staff       (20)     1106 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/C/inc/stUnionFind.h
-drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-02-07 05:27:41.391128 taffy-0.0.2/taffy/submodules/sonLib/externalTools/
-drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-02-07 05:27:41.413711 taffy-0.0.2/taffy/submodules/sonLib/externalTools/cutest/
--rw-r--r--   0 benedictpaten   (501) staff       (20)     4097 2022-11-30 22:52:40.000000 taffy-0.0.2/taffy/submodules/sonLib/externalTools/cutest/CuTest.h
-drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-02-07 05:27:41.414062 taffy-0.0.2/taffy.egg-info/
--rw-r--r--   0 benedictpaten   (501) staff       (20)    26231 2024-02-07 05:27:41.000000 taffy-0.0.2/taffy.egg-info/PKG-INFO
--rw-r--r--   0 benedictpaten   (501) staff       (20)     4597 2024-02-07 05:27:41.000000 taffy-0.0.2/taffy.egg-info/SOURCES.txt
--rw-r--r--   0 benedictpaten   (501) staff       (20)        1 2024-02-07 05:27:41.000000 taffy-0.0.2/taffy.egg-info/dependency_links.txt
--rw-r--r--   0 benedictpaten   (501) staff       (20)       24 2024-02-07 05:27:41.000000 taffy-0.0.2/taffy.egg-info/requires.txt
--rw-r--r--   0 benedictpaten   (501) staff       (20)        6 2024-02-07 05:27:41.000000 taffy-0.0.2/taffy.egg-info/top_level.txt
+drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-05-17 21:58:19.319404 taffy-0.0.3/
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     1071 2022-11-30 22:52:38.000000 taffy-0.0.3/LICENSE
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     3829 2024-05-17 21:58:19.319144 taffy-0.0.3/PKG-INFO
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     3177 2024-05-17 21:52:41.000000 taffy-0.0.3/README.md
+-rw-r--r--   0 benedictpaten   (501) staff       (20)      746 2024-05-17 21:53:18.000000 taffy-0.0.3/pyproject.toml
+-rw-r--r--   0 benedictpaten   (501) staff       (20)       38 2024-05-17 21:58:19.319472 taffy-0.0.3/setup.cfg
+-rw-r--r--   0 benedictpaten   (501) staff       (20)      662 2024-02-19 04:20:00.000000 taffy-0.0.3/setup.py
+drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-05-17 21:58:19.287358 taffy-0.0.3/taffy/
+-rw-r--r--   0 benedictpaten   (501) staff       (20)        0 2022-11-30 22:52:38.000000 taffy-0.0.3/taffy/__init__.py
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    10338 2024-05-17 21:52:41.000000 taffy-0.0.3/taffy/_taffy_build.py
+drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-05-17 21:58:19.291993 taffy-0.0.3/taffy/impl/
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    13224 2024-05-17 21:52:41.000000 taffy-0.0.3/taffy/impl/alignment_block.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     3431 2023-12-29 12:34:58.000000 taffy-0.0.3/taffy/impl/line_iterator.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     4014 2024-02-03 17:34:31.000000 taffy-0.0.3/taffy/impl/maf.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    21884 2024-04-09 23:22:29.000000 taffy-0.0.3/taffy/impl/merge_adjacent_alignments.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    11715 2022-11-30 22:52:38.000000 taffy-0.0.3/taffy/impl/ond.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     7174 2024-04-16 19:30:32.000000 taffy-0.0.3/taffy/impl/paf.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    12853 2024-05-17 21:52:41.000000 taffy-0.0.3/taffy/impl/prefix_sort.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    21906 2024-05-17 21:52:41.000000 taffy-0.0.3/taffy/impl/taf.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    25917 2024-05-17 21:52:41.000000 taffy-0.0.3/taffy/impl/tai.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     6738 2024-05-17 21:52:41.000000 taffy-0.0.3/taffy/impl/wiggle.c
+drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-05-17 21:58:19.293083 taffy-0.0.3/taffy/inc/
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     1698 2023-12-29 12:34:58.000000 taffy-0.0.3/taffy/inc/line_iterator.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)      535 2022-11-30 22:52:38.000000 taffy-0.0.3/taffy/inc/ond.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    13601 2024-05-17 21:52:41.000000 taffy-0.0.3/taffy/inc/taf.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     2913 2024-05-17 21:52:41.000000 taffy-0.0.3/taffy/inc/tai.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    28106 2024-05-17 21:52:41.000000 taffy-0.0.3/taffy/lib.py
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     7567 2024-05-17 21:52:41.000000 taffy-0.0.3/taffy/ml.py
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     5742 2024-05-17 21:52:41.000000 taffy-0.0.3/taffy/newick.py
+drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-05-17 21:58:19.283935 taffy-0.0.3/taffy/submodules/
+drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-05-17 21:58:19.283852 taffy-0.0.3/taffy/submodules/abPOA/
+drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-05-17 21:58:19.293690 taffy-0.0.3/taffy/submodules/abPOA/include/
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     8686 2024-02-17 04:27:15.000000 taffy-0.0.3/taffy/submodules/abPOA/include/abpoa.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    32048 2024-02-17 04:27:15.000000 taffy-0.0.3/taffy/submodules/abPOA/include/simd_instruction.h
+drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-05-17 21:58:19.284196 taffy-0.0.3/taffy/submodules/sonLib/
+drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-05-17 21:58:19.284122 taffy-0.0.3/taffy/submodules/sonLib/C/
+drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-05-17 21:58:19.310259 taffy-0.0.3/taffy/submodules/sonLib/C/impl/
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    28457 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/avl.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    18523 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/bioioC.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    24787 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/commonC.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     4989 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/fastCMaths.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    10345 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/hashTableC.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     5553 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/hashTableC_itr.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     8916 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/jsmn.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    30948 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/lz4.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     5600 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/lz4.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    23496 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/lz4hc.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     2295 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/lz4hc.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     7536 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/pairwiseAlignment.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    14185 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibCache.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     5720 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibCommon.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     9206 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibCompression.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    28217 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibConnectivity.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    22979 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibEulerTour.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     3189 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibExcept.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     4279 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibFile.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)      681 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibGlobalsInternal.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     7474 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibHash.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    20270 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibKVDatabase.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    13238 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibKVDatabaseConf.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     2862 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibKVDatabasePrivate.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     9492 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibKVDatabase_BigRecordFile.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    18106 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibKVDatabase_MySql.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    11772 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibKVDatabase_Redis.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    12698 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibKVDatabase_TokyoCabinet.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    11441 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibList.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)      357 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibListPrivate.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     1431 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibMath.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    11498 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibNaiveConnectivity.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     2127 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibRandom.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     7186 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibSet.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    11218 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibSortedSet.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     6721 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibString.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    11707 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibTreap.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    13505 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibTree.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     5704 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibTuples.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     3102 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/stGraph.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     2372 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/stJson.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     4226 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/stMatrix.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    87278 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/stPhylogeny.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    10359 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/stPosetAlignment.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     3764 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/stSafeC.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     8525 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/stThreadPool.c
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     3223 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/impl/stUnionFind.c
+drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-05-17 21:58:19.318251 taffy-0.0.3/taffy/submodules/sonLib/C/inc/
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     5078 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/avl.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     5046 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/bioioC.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     7990 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/commonC.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     3236 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/fastCMaths.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     7615 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/hashTableC.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     4149 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/hashTableC_itr.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     3094 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/hashTablePrivateC.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     2697 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/jsmn.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     1566 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/pairwiseAlignment.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     1306 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/safesort.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     1027 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLib.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     2493 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibCache.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     2753 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibCommon.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     1443 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibCompression.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     4049 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibConnectivity.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     2813 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibEulerTour.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     6403 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibExcept.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     2342 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibFile.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     3676 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibHash.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     7022 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibKVDatabase.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     4385 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibKVDatabaseConf.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     7308 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibList.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)      598 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibMath.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     1479 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibNaiveConnectivity.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     1565 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibRandom.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     3312 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibSet.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     5412 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibSortedSet.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     3517 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibString.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     1716 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibTreap.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     3126 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibTree.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     2670 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibTuples.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     2791 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibTypes.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)      984 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/stGraph.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     1134 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/stJson.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     2000 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/stMatrix.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)    10503 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/stPhylogeny.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     1260 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/stPosetAlignment.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     2619 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/stSafeC.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)      875 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/stSpimapLayer.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     2128 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/stThreadPool.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     1106 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/C/inc/stUnionFind.h
+drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-05-17 21:58:19.284255 taffy-0.0.3/taffy/submodules/sonLib/externalTools/
+drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-05-17 21:58:19.318407 taffy-0.0.3/taffy/submodules/sonLib/externalTools/cutest/
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     4097 2022-11-30 22:52:40.000000 taffy-0.0.3/taffy/submodules/sonLib/externalTools/cutest/CuTest.h
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     2310 2024-05-17 21:52:41.000000 taffy-0.0.3/taffy/wiggle.py
+drwxr-xr-x   0 benedictpaten   (501) staff       (20)        0 2024-05-17 21:58:19.318792 taffy-0.0.3/taffy.egg-info/
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     3829 2024-05-17 21:58:19.000000 taffy-0.0.3/taffy.egg-info/PKG-INFO
+-rw-r--r--   0 benedictpaten   (501) staff       (20)     4738 2024-05-17 21:58:19.000000 taffy-0.0.3/taffy.egg-info/SOURCES.txt
+-rw-r--r--   0 benedictpaten   (501) staff       (20)        1 2024-05-17 21:58:19.000000 taffy-0.0.3/taffy.egg-info/dependency_links.txt
+-rw-r--r--   0 benedictpaten   (501) staff       (20)       24 2024-05-17 21:58:19.000000 taffy-0.0.3/taffy.egg-info/requires.txt
+-rw-r--r--   0 benedictpaten   (501) staff       (20)        6 2024-05-17 21:58:19.000000 taffy-0.0.3/taffy.egg-info/top_level.txt
```

### Comparing `taffy-0.0.2/LICENSE` & `taffy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/pyproject.toml` & `taffy-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "cffi>=1.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "taffy"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Benedict Paten", email="bpaten@ucsc.edu" },
   { name="Glenn Hickey", email="glenn.hickey@gmail.com" },
 ]
 description = "For manipulating taf and maf format alignments"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `taffy-0.0.2/setup.py` & `taffy-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/_taffy_build.py` & `taffy-0.0.3/taffy/_taffy_build.py`

 * *Files 8% similar despite different names*

```diff
@@ -110,30 +110,22 @@
      * Gets the number of columns in the alignment
      */
     int64_t alignment_length(Alignment *alignment);
     
     /*
      * Gets the max length of an interstitial gap sequence between this block and the next one.
      */
-    int64_t alignment_total_gap_length(Alignment *left_alignment);
+    int64_t alignment_max_gap_length(Alignment *left_alignment);
     
     /*
      * Number of shared rows between two alignments
      */
     int64_t alignment_number_of_common_rows(Alignment *left_alignment, Alignment *right_alignment);
     
     /*
-     * Merge together adjacent blocks into one alignment. Requires that the alignment
-     * rows are linked together (e.g. with alignment_link_adjacent). Destroys the input
-     * alignments in the process and returns a merged alignment. If there are interstitial
-     * sequences between the blocks, aligns these sequences together.
-     */
-    Alignment *alignment_merge_adjacent(Alignment *left_alignment, Alignment *right_alignment);
-    
-    /*
      * Cleanup a row
      */
     void alignment_row_destruct(Alignment_Row *row);
     
     /*
      * Returns non-zero if left_row represents a substring on the same contig and strand as right_row, but
      * immediately before
@@ -153,14 +145,19 @@
     
     /*
      * Read a column of the alignment and return as a string
      */
     char *alignment_get_column(Alignment *alignment, int64_t column_index);
 
     /*
+     * Read a column of the alignment as an integer array where A/a=0, C/c=1, G/g=2, T/t=3, -=4, everything else=5
+     */
+    int32_t *alignment_get_column_as_int_array(Alignment *alignment, int64_t column_index);
+
+    /*
      * Returns a pretty-printed string representing the alignment. Useful for debugging.
     */
     char *alignment_to_string(Alignment *alignment);
 
     /**
      * Sniff file format from header line.  returns:
      *  0: taf
@@ -281,15 +278,15 @@
                                "taffy/submodules/sonLib/C/impl/avl.c",
                                "taffy/submodules/sonLib/C/impl/sonLibSortedSet.c",
                                "taffy/submodules/sonLib/C/impl/sonLibSet.c",
                                "taffy/submodules/sonLib/C/impl/sonLibList.c",
                                "taffy/submodules/sonLib/C/impl/sonLibFile.c",
                                "taffy/impl/line_iterator.c",
                                "taffy/impl/alignment_block.c",
-                               "taffy/impl/merge_adjacent_alignments.c",
+                               # "taffy/impl/merge_adjacent_alignments.c" - this is excluded because it uses abPOA
                                "taffy/impl/maf.c",
                                "taffy/impl/ond.c",
                                "taffy/impl/taf.c",
                                "taffy/impl/tai.c",
                                ],
                       extra_compile_args=["-DUSE_HTSLIB"],
                       libraries=["hts"],
```

### Comparing `taffy-0.0.2/taffy/impl/alignment_block.c` & `taffy-0.0.3/taffy/impl/alignment_block.c`

 * *Files 8% similar despite different names*

```diff
@@ -227,15 +227,15 @@
     WFA_destruct(wfa);
 }
 
 int64_t alignment_length(Alignment *alignment) {
     return alignment->column_number;
 }
 
-int64_t alignment_total_gap_length(Alignment *left_alignment) {
+int64_t alignment_max_gap_length(Alignment *left_alignment) {
     Alignment_Row *l_row = left_alignment->row;
     int64_t total_interstitial_gap_length = 0;
     while(l_row != NULL) {
         if(l_row->r_row != NULL && alignment_row_is_predecessor(l_row, l_row->r_row)) {
             int64_t i = l_row->r_row->start - (l_row->start + l_row->length);
             if (i > total_interstitial_gap_length) {
                 total_interstitial_gap_length = i;
@@ -335,13 +335,52 @@
 char *alignment_get_column(Alignment *alignment, int64_t column_index) {
     char *column_string = st_malloc(sizeof(char) * (alignment->row_number+1));
     column_string[alignment->row_number] = '\0';
     assert(column_index >= 0);
     assert(column_index < alignment->column_number);
     Alignment_Row *row = alignment->row;
     for(int64_t i=0; i<alignment->row_number; i++) {
+        assert(row != NULL);
         column_string[i] = row->bases[column_index];
         row = row->n_row;
     }
     assert(row == NULL);
     return column_string;
 }
+
+int32_t *alignment_get_column_as_int_array(Alignment *alignment, int64_t column_index) {
+    int32_t *column_array = st_malloc(sizeof(int32_t) * alignment->row_number);
+    assert(column_index >= 0);
+    assert(column_index < alignment->column_number);
+    Alignment_Row *row = alignment->row;
+    for(int64_t i=0; i<alignment->row_number; i++) {
+        assert(row != NULL);
+        int32_t j;
+        switch(row->bases[column_index]) {
+            case '-':
+                j = 4;
+                break;
+            case 'a':
+            case 'A':
+                j = 0;
+                break;
+            case 'c':
+            case 'C':
+                j = 1;
+                break;
+            case 'g':
+            case 'G':
+                j = 2;
+                break;
+            case 't':
+            case 'T':
+                j = 3;
+                break;
+            default:
+                j = 5;
+        }
+        column_array[i] = j;
+        row = row->n_row;
+    }
+    assert(row == NULL);
+    return column_array;
+}
```

### Comparing `taffy-0.0.2/taffy/impl/line_iterator.c` & `taffy-0.0.3/taffy/impl/line_iterator.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/impl/maf.c` & `taffy-0.0.3/taffy/impl/maf.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/impl/merge_adjacent_alignments.c` & `taffy-0.0.3/taffy/impl/prefix_sort.c`

 * *Files 24% similar despite different names*

```diff
@@ -1,319 +1,312 @@
 #include "taf.h"
-#include "ond.h"
+#include "tai.h"
 #include "sonLib.h"
+#include <stdio.h>
+#include <ctype.h>
 
 /*
- * Method to merge together two adjacent alignments.
+ * Functions for sorting alignment rows by prefixes of their sequence name
  */
 
-static char *make_run(int64_t length, char c) {
-    char gap_alignment[length+1];
-    for(int64_t i=0; i<length; i++) {
-        gap_alignment[i] = c;
-    }
-    gap_alignment[length] = '\0';
-    return stString_copy(gap_alignment);
-}
-
-int64_t make_msa(int64_t string_no, int64_t column_no, int64_t max_alignment_length,
-                 int64_t **msa, char **strings, int64_t *string_lengths,
-                 char **msa_strings) {
-    /*
-     * Convert the list of aligned columns in msa into a 2D alignment of the strings.
-     */
-    // Build the MSA
-    int64_t offsets[string_no];
-    for (int64_t i=0; i<string_no; i++) { // Initialize the offsets
-        offsets[i] = -1;
-    }
-    int64_t alignment_offset=0;
-    for(int64_t j=0; j<column_no; j++) {
-        // Work out the max indel length before position j
-        int64_t max_indel=0;
-        for(int64_t i=0; i<string_no; i++) {
-            int64_t k=msa[i][j]; // Position in sequence i aligned to column j of longest sequence
-            if(k != -1) { // Is not a gap, work out length
-                max_indel = k - offsets[i] - 1 > max_indel ? k - offsets[i] - 1 : max_indel;
-            }
-        }
+void sequence_prefix_destruct(Sequence_Prefix *sequence_prefix) {
+    free(sequence_prefix->prefix);
+    free(sequence_prefix);
+}
 
-        // Now fill in the indels and column j
-        for(int64_t i=0; i<string_no; i++) {
-            int64_t k=msa[i][j]; // Position in sequence i aligned to column j of longest sequence
-            if(k != -1) { // Is not a gap
-                // Fill in the unaligned sequence in sequence i
-                int64_t l=0;
-                while(++offsets[i] < k) {
-                    msa_strings[i][alignment_offset+l++] = strings[i][offsets[i]];
-                }
+Sequence_Prefix *sequence_prefix_construct(char *prefix, int64_t index) {
+    Sequence_Prefix *sequence_prefix = st_calloc(1, sizeof(Sequence_Prefix));
+    sequence_prefix->prefix = prefix;
+    sequence_prefix->prefix_length = strlen(prefix);
+    if(sequence_prefix->prefix_length == 0) {
+        st_errAbort("Found an empty sequence prefix");
+    }
+    sequence_prefix->index = index;
+    return sequence_prefix;
+}
 
-                // Add trailing gaps
-                while(l<max_indel) {
-                    msa_strings[i][alignment_offset+l++] = '-';
-                }
+int sequence_prefix_cmp_fn(Sequence_Prefix *p1, Sequence_Prefix *p2) {
+    return strcmp(p1->prefix, p2->prefix);
+}
 
-                // Add aligned position
-                msa_strings[i][alignment_offset+max_indel] = strings[i][offsets[i]];
-            }
-            else { // Add gaps to alignment to account for max indel and column j
-                for(int64_t l=0; l<=max_indel; l++) {
-                    msa_strings[i][alignment_offset+l] = '-';
-                }
+stList *sequence_prefix_load(FILE *sort_fh) {
+    stList *prefixes_to_sort_by = stList_construct3(0, (void (*)(void *))sequence_prefix_destruct);
+    int64_t index = 0;
+    char *line;
+    while((line = stFile_getLineFromFile(sort_fh)) != NULL) {
+        stList *tokens = stString_split(line);
+        if(stList_length(tokens) != 1) {
+            st_errAbort("Expected exactly one string in sort file on line: %s", line);
+        }
+        Sequence_Prefix *sequence_prefix = sequence_prefix_construct(stList_pop(tokens), index++);
+        stList_append(prefixes_to_sort_by, sequence_prefix);
+        // Clean up
+        free(line);
+        stList_destruct(tokens);
+    }
+    stList_sort(prefixes_to_sort_by, (int (*)(const void *, const void *))sequence_prefix_cmp_fn);
+    return prefixes_to_sort_by;
+}
+
+static int get_closest_prefix_cmp_fn(char *sequence_name, Sequence_Prefix *sp) {
+    int64_t i = strcmp(sequence_name, sp->prefix);
+    if(i > 0) { // If sequence_name is lexicographically larger than sequence_prefix could
+        // be a prefix (can not be a prefix is i < 0)
+        for(int64_t j=0; j<sp->prefix_length; j++) {
+            if(sequence_name[j] != sp->prefix[j]) {
+                return 1;
             }
         }
-        // Update the length of the alignment built so far
-        alignment_offset += max_indel + 1; // indel length and the ref position
+        return 0;
     }
-    // Now add in any suffix gaps
-    int64_t max_indel=0;
-    for(int64_t i=0; i<string_no; i++) {
-        int64_t j = string_lengths[i] - offsets[i] - 1;
-        max_indel = j > max_indel ? j : max_indel;
-    }
-    for(int64_t i=0; i<string_no; i++) {
-        int64_t j=0;
-        while(++offsets[i] < string_lengths[i]) {
-            msa_strings[i][alignment_offset+j++] = strings[i][offsets[i]];
-        }
-        while(j < max_indel) {
-            msa_strings[i][alignment_offset+j++] = '-';
-        }
+    return i;
+}
+
+int64_t alignment_row_get_closest_sequence_prefix(Alignment_Row *row, stList *prefixes_to_sort_by) {
+    // Binary search the sequence name
+    Sequence_Prefix *sp = stList_binarySearch(prefixes_to_sort_by, row->sequence_name,
+                                              (int (*)(const void *a, const void *b))get_closest_prefix_cmp_fn);
+    if(sp == NULL) {
+        st_logDebug("Did not find a valid prefix to match: %s\n", row->sequence_name);
     }
-    alignment_offset += max_indel;
-    return alignment_offset;
+    return sp != NULL ? sp->index : -1; // Sequences that don't have a match will appear first in the sort
 }
 
-bool cmp_chars(void *a, void *b) {
-    return ((char *)a)[0] == ((char *)b)[0];
+int alignment_sequence_prefix_cmp_fn(Alignment_Row *a1, Alignment_Row *a2,
+                                     stList *prefixes_to_sort_by) {
+    int i = alignment_row_get_closest_sequence_prefix(a1, prefixes_to_sort_by);
+    int j = alignment_row_get_closest_sequence_prefix(a2, prefixes_to_sort_by);
+    return i < j ? -1 : (i > j ? 1 : strcmp(a1->sequence_name, a2->sequence_name));
 }
 
-int64_t align_interstitial_gaps(Alignment *alignment) {
-    /*
-     * Align the sequences that lie within the gaps between two adjacent blocks.
-     * Return the length of the interstitial alignment.
-     */
+void alignment_sort_the_rows(Alignment *p_alignment, Alignment *alignment, stList *prefixes_to_sort_by, bool ignore_first_row) {
+    // Get the rows
+    stList *rows = alignment_get_rows_in_a_list(ignore_first_row && alignment->row ? alignment->row->n_row : alignment->row);
+    assert(stList_length(rows) == (ignore_first_row ? alignment->row_number -1 : alignment->row_number)); // Quick sanity check
+
+    // Sort the rows by the prefix ordering
+    stList_sort2(rows, (int (*)(const void *, const void *, void *))alignment_sequence_prefix_cmp_fn, prefixes_to_sort_by);
+
+    // Add back the first row if ignored
+    if(ignore_first_row && alignment->row) {
+        // hack for now cos no insert method in stList!
+        stList_reverse(rows);
+        stList_append(rows, alignment->row);
+        stList_reverse(rows);
+        assert(stList_get(rows, 0) == alignment->row);
+    }
+    assert(stList_length(rows) == alignment->row_number); // One more sanity check
+
+    // Re-connect the rows
+    alignment_set_rows(alignment, rows);
+
+    // Reset the alignment of the rows with the prior row
+    if(p_alignment != NULL) {
+        alignment_link_adjacent(p_alignment, alignment, 1);
+    }
+}
 
-    // Add any missing gap strings in
-    Alignment_Row *row = alignment->row;
-    while (row != NULL) {
-        if(row->l_row != NULL && alignment_row_is_predecessor(row->l_row, row) && row->left_gap_sequence == NULL) {
-            row->left_gap_sequence = make_run(row->start - (row->l_row->start + row->l_row->length), 'N');
-        }
+static void remove_rows(Alignment *alignment, int (*delete_row)(Alignment_Row *, void *),
+                        void *extra_arg, bool ignore_first_row) {
+    Alignment_Row *row = alignment->row, **p_row = &(alignment->row);
+    if(ignore_first_row && row != NULL) {  // Keep the first row
+        p_row = &(row->n_row);  // Update pointers
         row = row->n_row;
     }
-
-    // Find the longest gap sequence and number of sequences to align
-    //TODO: Consider not allowing picking the longest sequence if it is all Ns
-    row = alignment->row;
-    char *longest_string = NULL;
-    int64_t string_no=0, longest_string_length=0, total_string_length=0;
-    while (row != NULL) {
-        if(row->left_gap_sequence != NULL) {
-            string_no++; // Increase the number of strings we are aligning
-            int64_t i=strlen(row->left_gap_sequence);
-            total_string_length += i;
-            if(i > longest_string_length) {
-                longest_string = row->left_gap_sequence;
-                longest_string_length = strlen(longest_string);
-            }
+    while(row != NULL) {
+        if(delete_row(row, extra_arg)) { //stSet_search(rows_to_delete, row) != -1) { // Filter the row
+            alignment->row_number--; // Reduce the number of row
+            assert(alignment->row_number >= 0);
+            *p_row = row->n_row; // Update the previous link to point at the row after the current row
+            alignment_row_destruct(row); // Clean up the row
+            row = (*p_row); // Set row to point at the next row
+        }
+        else { // Keep the row, do nothing
+            p_row = &(row->n_row);  // Update pointers
+            row = row->n_row;
         }
-        row = row->n_row;
     }
+}
 
-    // Align each sequence to the longest sequence
-    
-    // A longest sequence x sequence number sized integer matrix,
-    int64_t **msa = st_calloc(string_no, sizeof(int64_t*));
-    for (int64_t i = 0; i < string_no; ++i) {
-        msa[i] = st_calloc(longest_string_length, sizeof(int64_t));
-    }
-    // each entry is the index of the position aligned at that node (or -1 if unaligned)
-    char **row_strings = st_calloc(string_no, sizeof(char*)); // The gap strings
-    int64_t *row_string_lengths = st_calloc(string_no, sizeof(int64_t));
-    row = alignment->row;
-    int64_t i=0;
-    while (row != NULL) {
-        if(row->left_gap_sequence != NULL) {
-            row_strings[i] = row->left_gap_sequence;
-            row_string_lengths[i] = strlen(row_strings[i]);
-            // TODO: Consider making WFA have affine gaps
-            WFA *wfa = WFA_construct(longest_string, row_strings[i], longest_string_length, row_string_lengths[i],
-                                     sizeof(char), (bool (*)(void *, void *))cmp_chars, 1, 1);
-            WFA_get_alignment(wfa, msa[i]); i++;
-            WFA_destruct(wfa);
+static int alignment_filter_fn(Alignment_Row *row, stList *prefixes_to_filter_by) {
+    return alignment_row_get_closest_sequence_prefix(row, prefixes_to_filter_by) != -1;
+}
+
+void alignment_filter_the_rows(Alignment *alignment, stList *prefixes_to_filter_by, bool ignore_first_row) {
+    remove_rows(alignment, (int (*)(Alignment_Row *, void *))alignment_filter_fn,
+                       prefixes_to_filter_by, ignore_first_row);
+}
+
+void alignment_show_only_lineage_differences(Alignment *alignment, char mask_char, stList *sequence_prefixes, stList *tree_nodes) {
+    // First create map of tree nodes to bases
+    stHash *tree_nodes_to_bases = stHash_construct2(NULL, (void (*)(void *))stList_destruct);
+    Alignment_Row *row = alignment->row;
+    while(row != NULL) { // For each row
+        // Get corresponding tree node using sequence prefixes
+        int64_t i = alignment_row_get_closest_sequence_prefix(row, sequence_prefixes);
+        if(i != -1) { // We found it in the tree
+            // Add to the tree_nodes_to_bases map
+            stTree *node = stList_get(tree_nodes, i);
+            stList *ancestor_sequences = stHash_search(tree_nodes_to_bases, node);
+            if(ancestor_sequences == NULL) {
+                ancestor_sequences = stList_construct3(0, free);
+                stHash_insert(tree_nodes_to_bases, node, ancestor_sequences);
+            }
+            stList_append(ancestor_sequences, stString_copy(row->bases));
+        }
+        else {
+            st_logDebug("Alignment row sequence not found in tree: %s\n", row->sequence_name);
         }
         row = row->n_row;
     }
 
-    // Now convert to a traditional MSA
-    int64_t max_alignment_length = total_string_length < (longest_string_length+1)*longest_string_length ? total_string_length : (longest_string_length+1)*longest_string_length;
-    // can not be longer than the minimum of the total length of the strings (where all bases
-    char **msa_strings = st_calloc(string_no, sizeof(char*));
-    for (int64_t i = 0; i < string_no; ++i) {
-        msa_strings[i] = st_calloc(max_alignment_length, sizeof(char*));
-    }
-    // are unique gaps) and the square of the longest sequence length
-    int64_t msa_length = make_msa(string_no, longest_string_length, max_alignment_length, msa, row_strings,
-                                  row_string_lengths, msa_strings);
-    assert(msa_length <= max_alignment_length);
-
-    // Now copy the alignment strings back to the sequences
-    row = alignment->row; i=0;
-    while (row != NULL) {
-        if(row->left_gap_sequence != NULL) {
-            // Do a quick check that the sequence is as expected
-            int64_t j=0, l=0;
-            while(l < msa_length) {
-                assert(j <= row_string_lengths[i]);
-                if(msa_strings[i][l] != '-') {
-                    assert(row->left_gap_sequence[j] == msa_strings[i][l]);
-                    j++;
+    // Now identify mutations
+    row = alignment->row;
+    while(row != NULL) { // For each row
+        //  Identify node in tree using prefix search
+        int64_t i = alignment_row_get_closest_sequence_prefix(row, sequence_prefixes);
+        if(i != -1) { // We found it in the tree
+            stTree *node = stList_get(tree_nodes, i);
+            stTree *ancestor = stTree_getParent(node);
+            if(ancestor != NULL) { // If we're not at the root of the tree - otherwise we must report the base
+                stList *ancestor_sequences = stHash_search(tree_nodes_to_bases, ancestor);
+                for(int64_t j=0; j<alignment->column_number; j++) { // For each alignment column
+                    char base = row->bases[j];
+                    if(base != '-') { // If not a gap base
+                        for (int64_t k = 0; k < stList_length(ancestor_sequences); k++) { // For each ancestor base
+                            char *ancestor_sequence = stList_get(ancestor_sequences, k);
+                            if(toupper(base) == toupper(ancestor_sequence[j])) { // If identical to ancestor base
+                                row->bases[j] = mask_char; // Switch to a star character
+                                break;
+                            }
+                        }
+                    }
                 }
-                l++;
             }
-            assert(j == row_string_lengths[i]);
-            //
-            free(row->left_gap_sequence);
-            row->left_gap_sequence = stString_getSubString(msa_strings[i++], 0, msa_length);
-        }
+        } // If not found do nothing, as we log missing sequences in the loop above
         row = row->n_row;
     }
-    for (int64_t i = 0; i < string_no; ++i) {
-        free(msa[i]);
-    }
-    free(msa);    
-    free(row_strings);
-    free(row_string_lengths);
-    for (int64_t i = 0; i < string_no; ++i) {
-        free(msa_strings[i]);
-    }    
-    free(msa_strings);
-    return msa_length;
-}
-
-Alignment *alignment_merge_adjacent(Alignment *left_alignment, Alignment *right_alignment) {
-    // First un-link any rows that are substitutions as these can't be merged
-    Alignment_Row *r_row = right_alignment->row;
-    while(r_row != NULL) {
-        if(r_row->l_row != NULL && !alignment_row_is_predecessor(r_row->l_row, r_row)) {
-            assert(r_row->l_row->r_row == r_row);
-            r_row->l_row->r_row = NULL; // unlink 1
-            r_row->l_row = NULL; // unlink 2
-        }
-        r_row = r_row->n_row;
-    }
 
-    // Add the new rows in the right alignment to the left alignment
-    r_row = right_alignment->row; Alignment_Row **p_l_row = &(left_alignment->row);
-    while(r_row != NULL) {
-        if(r_row->l_row == NULL) { // Is an insertion
-            // Make a new l_row
-            Alignment_Row *l_row = st_calloc(1, sizeof(Alignment_Row));
-
-            // Set coordinates
-            l_row->sequence_name = stString_copy(r_row->sequence_name);
-            l_row->start = r_row->start;
-            l_row->length = 0; // is an empty alignment
-            l_row->sequence_length = r_row->sequence_length;
-            l_row->strand = r_row->strand;
-            l_row->bases = make_run(left_alignment->column_number, '-');
-
-            // Connect the left and right rows
-            l_row->r_row = r_row;
-            r_row->l_row = l_row;
-
-            // Now connect the left row into the left alignment at the correct place
-            l_row->n_row = *p_l_row;
-            *p_l_row = l_row;
+    // Clean up
+    stHash_destruct(tree_nodes_to_bases);
+}
 
-            // Update p_l_row to point at l_row's n_row pointer
-            p_l_row = &(l_row->n_row);
+/*
+ * Functions to pad an alignment block with an extra dummy row for each missing sequences - helpful for
+ * making normalized alignments
+ */
 
-            // Increase the row number
-            left_alignment->row_number++;
-        }
-        else {
-            // Update p_l_row to point at r_row->l_row's n_row pointer
-            p_l_row = &(r_row->l_row->n_row);
+static int get_closest_row_cmp_fn(Sequence_Prefix *p, Alignment_Row *r) {
+    int64_t i = strcmp(p->prefix, r->sequence_name);
+    if(i < 0) { // If prefix_name is lexicographically smaller than row's sequence could
+        // be a prefix (can not be a prefix is i > 0)
+        for(int64_t j=0; j<p->prefix_length; j++) {
+            if(r->sequence_name[j] != p->prefix[j]) {
+                return -1;
+            }
         }
-        r_row = r_row->n_row; // Move to the next right alignment row
+        return 0;
     }
+    return i;
+}
 
-    // Align the interstitial insert sequences, padding the left_gap_sequence strings with gaps to represent the alignment
-    int64_t interstitial_alignment_length = align_interstitial_gaps(right_alignment);
-
-    // Now finally extend the left alignment rows to include the right alignment rows
-    Alignment_Row *l_row = left_alignment->row;
-    char *right_gap = make_run(right_alignment->column_number + interstitial_alignment_length, '-'); // any trailing bases needed
-    while(l_row != NULL) {
-        if(l_row->r_row == NULL) {
-            // Is a deletion, so add in trailing gaps equal in length to the right alignment length plus any interstitial
-            // gap
-            char *bases = stString_print("%s%s", l_row->bases, right_gap);
-            free(l_row->bases);
-            l_row->bases = bases;
-        }
-        else {
-            Alignment_Row *r_row = l_row->r_row;
+static int alignment_row_cmp_fn(Alignment_Row *r1, Alignment_Row *r2) {
+    return strcmp(r1->sequence_name, r2->sequence_name);
+}
 
-            // Check the rows agree coordinate wise
-            assert(strcmp(l_row->sequence_name, r_row->sequence_name) == 0);
-            assert(l_row->strand == r_row->strand);
-            assert(l_row->start + l_row->length <= r_row->start);
-
-            // Is not a deletion, so merge together two adjacent rows
-            assert(r_row->left_gap_sequence != NULL);
-            assert(strlen(r_row->left_gap_sequence) == interstitial_alignment_length);
-            char *bases = stString_print("%s%s%s", l_row->bases, r_row->left_gap_sequence, r_row->bases);
-            free(l_row->bases); // clean up
-            l_row->bases = bases;
-
-            // Update the left row's length coordinate
-            int64_t interstitial_bases = r_row->start - (l_row->start + l_row->length);
-            l_row->length += interstitial_bases + r_row->length;
-            // Update the l_row's r_row pointer...
-            if(r_row->r_row != NULL) { // Check pointers are correct
-                assert(r_row->r_row->l_row == r_row);
-            }
-            l_row->r_row = r_row->r_row;
-            if(l_row->r_row != NULL) {
-                l_row->r_row->l_row = l_row;
+void alignment_pad_the_rows(Alignment *p_alignment, Alignment *alignment, stList *sequence_prefixes) {
+    // Get the rows in a list
+    stList *rows = alignment_get_rows_in_a_list(alignment->row);
+    assert(stList_length(rows) == (alignment->row_number)); // Quick sanity check
+
+    // Sort the rows by name
+    stList_sort(rows, (int (*)(const void *, const void *))alignment_row_cmp_fn);
+
+    // Get the pointer to the last row of the alignment so we can add rows
+    Alignment_Row **p_r = &(alignment->row);
+    while(*p_r != NULL) {
+        p_r = &((*p_r)->n_row);
+    }
+
+    // For each sequence prefix
+    for(int64_t i=0; i<stList_length(sequence_prefixes); i++) {
+        Sequence_Prefix *sp = stList_get(sequence_prefixes, i);
+
+        // Check if there is a corresponding sequence name using binary search
+        Alignment_Row *r = stList_binarySearch(rows, sp,(int (*)(const void *a, const void *b))get_closest_row_cmp_fn);
+
+        if(r == NULL) { // If there isn't a corresponding row, add one to the alignment at the end setting the coordinates to zero
+            r = st_calloc(1, sizeof(Alignment_Row));
+            alignment->row_number++; // Increment the row number
+            r->sequence_name = stString_copy(sp->prefix);
+            r->bases = st_calloc(alignment->column_number+1, sizeof(char));
+            for(int64_t j=0; j<alignment->column_number; j++) {
+                r->bases[j] = '-';
             }
-            // Null r_row's left and right pointers
-            r_row->l_row = NULL;
-            r_row->r_row = NULL;
+            r->bases[alignment->column_number] = '\0';
+            r->strand = 1;
+            *p_r = r;
+            p_r = &(r->n_row);
         }
+    }
+
+    // Clean up
+    stList_destruct(rows);
 
-        l_row = l_row->n_row; // Move to the next left alignment row
+    // Reset the alignment of the rows with the prior row
+    if(p_alignment != NULL) {
+        alignment_link_adjacent(p_alignment, alignment, 1);
     }
+}
 
-    // Calculate the number of columns in the merged alignment
-    int64_t total_column_number = left_alignment->column_number + right_alignment->column_number + interstitial_alignment_length;
+/*
+ * Functions to filter duplicate sequence rows
+ */
 
-    // Fix the tags
-    if(left_alignment->column_tags != NULL) {
-        assert(right_alignment->column_tags != NULL);
-        Tag **combined_column_tags = st_malloc(sizeof(Tag *) * total_column_number); // Allocate an expanded set of columns
-        int64_t j=0;
-        for(int64_t i=0; i<left_alignment->column_number; i++) { // Add the left alignment's column's tags
-            combined_column_tags[j++] = left_alignment->column_tags[i];
-        }
-        for(int64_t i=0; i<interstitial_alignment_length; i++) { // Add empty tag lists for new columns
-            combined_column_tags[j++] = NULL;
-        }
-        for(int64_t i=0; i<right_alignment->column_number; i++) { // Add the right alignment's column's tags
-            combined_column_tags[j++] = right_alignment->column_tags[i];
+int alignment_filter_rows_fn(Alignment_Row *row, stSet *rows_to_delete) {
+    return stSet_search(rows_to_delete, row) != NULL;
+}
+
+void alignment_filter_duplicate_rows(Alignment *alignment, stList *prefixes_to_match_on, bool ignore_first_row) {
+    // Create a map from prefixes to rows
+    stHash *prefixes_to_rows = stHash_construct2(NULL, (void (*)(void *))stList_destruct);
+    stSet *rows_to_delete = stSet_construct();
+    Alignment_Row *r = alignment->row;
+    while(r != NULL) {
+        Sequence_Prefix *sp = stList_binarySearch(prefixes_to_match_on, r->sequence_name,
+                                                  (int (*)(const void *a, const void *b))get_closest_prefix_cmp_fn);
+        if(sp != NULL) {
+            stList *l = stHash_search(prefixes_to_rows, sp);
+            if (!l) {
+                l = stList_construct();
+                stHash_insert(prefixes_to_rows, sp, l);
+            }
+            stList_append(l, r);
         }
-        free(left_alignment->column_tags); // Cleanup, but not the tag strings which we copied
-        left_alignment->column_tags = combined_column_tags;
+        r = r->n_row;
     }
 
-    // Fix column number
-    left_alignment->column_number = total_column_number;
+    // For each sequence prefix
+    for(int64_t i=0; i<stList_length(prefixes_to_match_on); i++) {
+        Sequence_Prefix *sp = stList_get(prefixes_to_match_on, i);
+        stList *l = stHash_search(prefixes_to_rows, sp);
 
-    // Clean up
-    alignment_destruct(right_alignment, 1);  // Delete the right alignment
-    free(right_gap);
+        // Where there is a sequence prefix with multiple rows
+        if(l != NULL && stList_length(l) > 1) {
+
+            // TODO: Add option to more intelligently rank rows....
+
+            // Add weakest rows to the set to delete
+            for(int64_t j=1; j<stList_length(l); j++) {
+                stSet_insert(rows_to_delete, stList_get(l, j));
+            }
+        }
+    }
 
-    return left_alignment;
+    // Now delete the rows
+    remove_rows(alignment, (int (*)(Alignment_Row *, void *))alignment_filter_rows_fn,
+                rows_to_delete, ignore_first_row);
+
+    // Cleanup
+    stSet_destruct(rows_to_delete);
+    stHash_destruct(prefixes_to_rows);
 }
```

### Comparing `taffy-0.0.2/taffy/impl/ond.c` & `taffy-0.0.3/taffy/impl/ond.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/impl/paf.c` & `taffy-0.0.3/taffy/impl/paf.c`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,14 @@
             }
         }
 
     }
 
     // finalize trailing event
     if (current_start < num_col && current_start >= 0 && current_event[0] != '.') {
-        int64_t i = num_col;
         // note, this code block is (must be) identical to above. todo: factor out
         if (cs_cigar) {
             query_buffer[query_buffer_length] = '\0';
             target_buffer[target_buffer_length] = '\0';
             if (current_event[0] == 'M') {
                 assert(current_length == query_buffer_length && current_length == target_buffer_length);
                 sprintf(buffer, "=%s", query_buffer);
```

### Comparing `taffy-0.0.2/taffy/impl/taf.c` & `taffy-0.0.3/taffy/impl/taf.c`

 * *Files 5% similar despite different names*

```diff
@@ -100,28 +100,31 @@
 }
 
 /*
  * Parse the base alignment for the column.
  */
 char *get_bases(int64_t column_length, stList *tokens, bool run_length_encode_bases) {
     if(run_length_encode_bases) { // Case the bases are encoded using run length encoding
-        char *column = st_calloc(column_length, sizeof(char));
+        char *column = st_calloc(column_length+1, sizeof(char));
+        column[column_length] = '\0'; // Make into a properly terminated string
         int64_t i=0, j=0;
         while(j < column_length) {
             assert(i < stList_length(tokens));
             char *base_token = stList_get(tokens, i++);
             assert(strlen(base_token) == 1); // The base must be a single character
             int64_t k = atol(stList_get(tokens, i++));
             assert(k > 0); // Each count must be greater than zero
             while(k-- > 0) {
                 column[j++] = base_token[0];
             }
             assert(j <= column_length);
         }
         assert(j == column_length);
+        assert(strlen(column) == column_length); // Final sanity check: Must be a contiguous run of bases equal
+        // in length to the number of rows
         return column;
     }
     // Otherwise column is just a string of bases without whitespace
     char *column = stString_copy(stList_get(tokens, 0));
     assert(strlen(column) == column_length); // Must be a contiguous run of bases equal in length to the number of rows
     return column;
 }
@@ -234,26 +237,26 @@
         block->column_tags[i] = stList_get(tag_lists, i);
     }
     stList_destruct(tag_lists);
 
     //Now parse the actual alignments into the rows
     Alignment_Row *row = block->row;
     int64_t j = 0, k = block->column_number;
-    char bases[k+1];
-    bases[k] = '\0';
     while(row != NULL) {
+        char *bases = st_malloc(sizeof(char) * (k+1));
+        bases[k] = '\0';
         int64_t length = 0;
         for(int64_t i=0; i<k; i++) {
             char *column = stList_get(alignment_columns, i);
             bases[i] = column[j];
             if(bases[i] != '-') {
                 length++;
             }
         }
-        row->bases = stString_copy(bases);
+        row->bases = bases;
         row->length = length;
         row = row->n_row; j++;
     }
     assert(j == block->row_number);
 
     // Clean up
     stList_destruct(alignment_columns);
@@ -305,47 +308,20 @@
     int64_t base_count = 0;
     while(row != NULL) {
         if(row->bases[column] == base) {
             base_count++;
         }
         else {
             write_base(base, base_count, lw, run_length_encode_bases, color_bases);
-            /*if(base != '\0') {
-                if(run_length_encode_bases) {
-                    LW_write(lw, "%c %" PRIi64 " ", base, base_count);
-                }
-                else {
-                    for (int64_t i = 0; i < base_count; i++) {
-                        if(color_bases) {
-                            char *colored_base_string = color_base_char(base);
-                            LW_write(lw, colored_base_string);
-                            free(colored_base_string);
-                        }
-                        else {
-                            LW_write(lw, "%c", base);
-                        }
-                    }
-                }
-            }*/
             base = row->bases[column];
             base_count = 1;
         }
         row = row->n_row;
     }
     write_base(base, base_count, lw, run_length_encode_bases, color_bases);
-    /*if(base != '\0') {
-        if(run_length_encode_bases) {
-            LW_write(lw, "%c %" PRIi64 " ", base, base_count);
-        }
-        else {
-            for (int64_t i = 0; i < base_count; i++) {
-                LW_write(lw, "%c", base);
-            }
-        }
-    }*/
 }
 
 void write_coordinates(Alignment_Row *p_row, Alignment_Row *row, int64_t repeat_coordinates_every_n_columns, LW *lw) {
     int64_t i = 0;
     LW_write(lw, " ;");
     while(p_row != NULL) { // Write any row deletions
         if(p_row->r_row == NULL) { // if the row is deleted
@@ -411,38 +387,43 @@
         row = row->n_row; i++;
     }
 }
 
 void write_header(Tag *tag, LW *lw, char *header_prefix, char *delimiter, char *end);
 
 void taf_write_block2(Alignment *p_alignment, Alignment *alignment, bool run_length_encode_bases,
-                     int64_t repeat_coordinates_every_n_columns, LW *lw, bool color_bases) {
+                     int64_t repeat_coordinates_every_n_columns, LW *lw, bool color_bases, bool omit_coordinates) {
     Alignment_Row *row = alignment->row;
     if(row != NULL) {
         int64_t column_no = strlen(row->bases);
         assert(column_no > 0);
         write_column(row, 0, lw, run_length_encode_bases, color_bases);
-        write_coordinates(p_alignment != NULL ? p_alignment->row : NULL, row, repeat_coordinates_every_n_columns, lw);
-        if(alignment->column_tags != NULL && alignment->column_tags[0] != NULL) {
-            write_header(alignment->column_tags[0], lw, " @", ":", "");
+        if(!omit_coordinates) {
+            write_coordinates(p_alignment != NULL ? p_alignment->row : NULL, row, repeat_coordinates_every_n_columns,
+                              lw);
+            if (alignment->column_tags != NULL && alignment->column_tags[0] != NULL) {
+                write_header(alignment->column_tags[0], lw, " @", ":", "");
+            }
+            LW_write(lw, "\n");
         }
-        LW_write(lw, "\n");
         for(int64_t i=1; i<column_no; i++) {
             write_column(row, i, lw, run_length_encode_bases, color_bases);
-            if(alignment->column_tags != NULL && alignment->column_tags[i] != NULL) {
-                write_header(alignment->column_tags[i], lw, " @", ":", "");
+            if(!omit_coordinates) {
+                if (alignment->column_tags != NULL && alignment->column_tags[i] != NULL) {
+                    write_header(alignment->column_tags[i], lw, " @", ":", "");
+                }
             }
             LW_write(lw, "\n");
         }
     }
 }
 
 void taf_write_block(Alignment *p_alignment, Alignment *alignment, bool run_length_encode_bases,
                        int64_t repeat_coordinates_every_n_columns, LW *lw) {
-    taf_write_block2(p_alignment, alignment, run_length_encode_bases, repeat_coordinates_every_n_columns, lw, 0);
+    taf_write_block2(p_alignment, alignment, run_length_encode_bases, repeat_coordinates_every_n_columns, lw, 0, 0);
 }
 
 void taf_write_header(Tag *tag, LW *lw) {
     write_header(tag, lw, "#taf", ":", "\n");
 }
 
 int check_input_format(const char *header_line) {
```

### Comparing `taffy-0.0.2/taffy/impl/tai.c` & `taffy-0.0.3/taffy/impl/tai.c`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                     contig_length = 0;
                 } else {
                     *length = end - *start;
                 }
             }
         }
     }
-    return contig_length > 0 ? stString_getSubString(region, 0, contig_length) : NULL;
+    return contig_length > 0 && *length > 0 && *start >=0 ? stString_getSubString(region, 0, contig_length) : NULL;
 }
 
 // gets the "reference" (first row) coordinate information
 // but only returns everything if there's a coordinate for every row in the column
 // this can happen when everything is an "i" like on the first line
 // or when everything is an "s" like on a repeat-coordinates-every-n-columns line
 static char *parse_coordinates_line(stList *tokens, int64_t *start, bool *strand,
@@ -83,15 +83,15 @@
     int64_t num_coordinates = 0;
     char *seq = NULL;
     int64_t sequence_length;
     bool dummy;
     int64_t n = stList_length(tokens);
 
     ++j;
-    while (j < n) {
+    while (j < n && strcmp(stList_get(tokens, j), "@") != 0) {
         // copied from taf.c
         char *op_type = stList_get(tokens, j++); // This is the operation
         assert(strlen(op_type) == 1); // Must be a single character in length
         int64_t row_index = atol(stList_get(tokens, j++)); // Get the index of the affected row
         if(op_type[0] == 'i' || op_type[0] == 's') { // We have coordinates!
             num_coordinates++;
             if (row_index == 0) {
@@ -133,15 +133,15 @@
     bool dummy_bool;
     bool found_s = false;
 
     if (hc) {
         int64_t n = stList_length(tokens);
         bool *mask = st_calloc(n, sizeof(bool));        
         ++j;
-        while (j < n) {
+        while (j < n && strcmp(stList_get(tokens, j), "@") != 0) {
             char *op_type = stList_get(tokens, j++); // This is the operation
             j++; // the row index;
             assert(strlen(op_type) == 1); // Must be a single character in length
             if(op_type[0] == 'i' || op_type[0] == 's') { // We have coordinates!
                 found_s = found_s || op_type[0] == 's';
                 op_type[0] = 'i';
                 // only parse to increment j (would rather use api than just add 4)
@@ -373,15 +373,15 @@
     return tai;
 }
 
 // dummy function to let us toggle between maf/taf reading at runtime (by providing a
 // maf reader with same interface as taf reader)
 static Alignment *maf_read_block_3(Alignment *p_block, bool run_length_encode_bases, LI *li) {
     Alignment *alignment = maf_read_block(li);
-    if(p_block != NULL) {
+    if(p_block != NULL && alignment != NULL) {
         alignment_link_adjacent(p_block, alignment, 1);
     }
     return alignment;
 }
 
 TaiIt *tai_iterator(Tai* tai, LI *li, bool run_length_encode_bases, const char *contig, int64_t start, int64_t length) {
     time_t start_time = time(NULL);
@@ -389,27 +389,38 @@
     tai_it->maf = tai->maf;
 
     // parse the region into the iterator
     tai_it->name = stString_copy(contig);
     tai_it->start = start;
     tai_it->end = length < 0 ? LONG_MAX : start + length;
     tai_it->run_length_encode_bases = run_length_encode_bases;
+    tai_it->alignment = NULL;
+    tai_it->p_alignment = NULL;
+
+    // no sense querying anything if length is empty
+    if (length <= 0) {
+        return tai_it;
+    }
 
     // look up the region in the taf index, which takes a dummy record
     TaiRec qr;
     qr.name = tai_it->name;
     qr.seq_pos = tai_it->start;
 
     TaiRec *tair_1 = stSortedSet_searchLessThanOrEqual(tai->idx, &qr);
     if (tair_1 == NULL) {
-        tai_iterator_destruct(tai_it);
-        // there's no chance of finding the region as its contig isn't
-        // in the index or its start position is too low
-        // up to caller to spit out an error
-        return NULL;
+        // This will be null even if the query overlaps the first record in the index
+        // so we explicitly double check below (ie query 0-10 but index starts at 5)
+        tair_1 = stSortedSet_getFirst(tai->idx);
+        if (strcmp(tair_1->name, tai_it->name) != 0 || tai_it->end < tair_1->seq_pos) {
+            // there's no chance of finding the region as its contig isn't
+            // in the index or its start position is too low
+            // up to caller to spit out an error
+            return tai_it;
+        }
     }
 
     // sorted set doesn't let us iterate, so we use a second lookup to get
     // the next record
     TaiRec qr2;
     qr2.name = tai_it->name;
     qr2.seq_pos = tai_it->end;
@@ -476,25 +487,14 @@
         file_pos = LI_tell(li);
     }
     if (p_alignment != NULL) {
         alignment_destruct(p_alignment, true);
         p_alignment = NULL;
     }
 
-    // we scanned past our region, which could happen if your taf doesn't contain the whole
-    // sequence -- jsut return nothing
-    if (tai_it->alignment == NULL) {
-        if (tai_it->p_alignment) {
-            alignment_destruct(tai_it->p_alignment, true);
-        }
-        tai_iterator_destruct(tai_it);
-        st_logInfo("Scanned %" PRIi64 " blocks to NOT find region start in %" PRIi64 " seconds\n", scan_block_count, time(NULL) - start_time);
-        return NULL;
-    }
-
     st_logInfo("Scanned %" PRIi64 " blocks to find region start in %" PRIi64 " seconds\n", scan_block_count, time(NULL) - start_time);
     
     return tai_it;
 }
 
 /** 
  * clip an alignment, assumes start/end overlap aln and would leave a non-empty remainder
@@ -534,22 +534,20 @@
             } else {
                 char *bases = row->bases;
                 row->bases = stString_getSubString(bases, cut_point, strlen(row->bases) - cut_point);
                 free(bases);
             }
             assert(strlen(row->bases) >= row->length);            
         }
-        aln->column_number -= left_trim;
     }
 
     //clip the right side
     int64_t right_trim = (aln->row->start + aln->row->length) - end;
     if (right_trim > 0) {
         ret = ret | 1;
-        assert(aln->column_number > right_trim);
 
         // we need to find the cut point by counting off right_trim non-gap bases from the end of the reference row
         int64_t cut_point = strlen(aln->row->bases) - 1;
         for (int64_t cut_count = 0; cut_count < right_trim && cut_point >= 0; --cut_point) {
             if (aln->row->bases[cut_point] != '-') {
                 ++cut_count;
             }
@@ -568,80 +566,83 @@
             } else {
                 char *bases = row->bases;
                 row->bases = stString_getSubString(bases, 0, cut_point + 1);
                 free(bases);
             }
             assert(strlen(row->bases) >= row->length);
         }
-        aln->column_number -= right_trim;                
     }
 
     // now we make sure any deleted rows are unlinked from prev alignment.
     if (p_aln) {
         for (Alignment_Row *row = p_aln->row; row != NULL; row = row->n_row) {
             if (row->r_row && row->r_row->length == 0) {
                 assert(strlen(row->r_row->bases) == 0);
+                row->r_row->l_row = NULL;
                 row->r_row = NULL;
             }
         }
     }
-    
-    // then get rid of empty rows as they api doesn't handle them
-    Alignment_Row *prev = NULL;
-    Alignment_Row *next = NULL;
-    for (Alignment_Row *row = aln->row; row != NULL; row = next) {
-        next = row->n_row;
+
+    aln->column_number = aln->row_number > 0 ? strlen(aln->row->bases) : 0;
+
+    // then fill empty rows with gaps
+    for (Alignment_Row *row = aln->row; row != NULL; row = row->n_row) {
         if (row->length == 0) {
             assert(strlen(row->bases) == 0);
-            assert(prev != NULL);
-            prev->n_row = next;
-            alignment_row_destruct(row);
-            --aln->row_number;
-        } else {
-            prev = row;
+            row->bases = (char*)st_calloc(aln->column_number + 1, sizeof(char));
+            for (int64_t i = 0; i < aln->column_number; ++i) {
+                row->bases[i] = '-';
+            }
+            row->bases[aln->column_number] = '\0';
         }
     }
-    assert(aln->column_number > 0);
-    
+
     return ret;
 }
 
 Alignment *tai_next(TaiIt *tai_it, LI *li) {    
     if (tai_it->alignment == NULL) {
         return NULL;
     }
 
     // start by clamping the alignment block to the region
     assert(strcmp(tai_it->alignment->row->sequence_name, tai_it->name) == 0);
-    unsigned int ret = clip_alignment(tai_it->alignment, tai_it->p_alignment, tai_it->start, tai_it->end);
-
+    
     // save this alignment, it's what we're gonna return
     tai_it->p_alignment = tai_it->alignment;
 
     Alignment* (*maftaf_read_block)(Alignment*, bool, LI*) = maf_read_block_3;
     if (!tai_it->maf) {
         maftaf_read_block = taf_read_block;
     }
     
     // scan forward
-    if (ret & 1) {
+    if (tai_it->alignment->row->start + tai_it->alignment->row->length > tai_it->end) {
         tai_it->alignment = NULL;
     } else {
         tai_it->alignment = maftaf_read_block(tai_it->p_alignment, tai_it->run_length_encode_bases, li);
         if (tai_it->alignment != NULL &&
             (strcmp(tai_it->alignment->row->sequence_name, tai_it->name) != 0 ||
              tai_it->alignment->row->start >= tai_it->end)) {
             alignment_destruct(tai_it->alignment, true);
             tai_it->alignment = NULL;
         }
     }
+
+    // clip the alignment (done after read_block, which needs unclipped prev blocks for coordinate transform)
+    clip_alignment(tai_it->p_alignment, NULL, tai_it->start, tai_it->end);
     
     return tai_it->p_alignment;
 }
 
+bool tai_has_next(TaiIt *tai_it) {
+    return tai_it->alignment != NULL;
+}
+
 void tai_iterator_destruct(TaiIt *tai_it) {
     free(tai_it->name);
     free(tai_it);
 }
 
 stHash *tai_sequence_lengths(Tai *tai, LI *li) {
     // read the header
```

### Comparing `taffy-0.0.2/taffy/inc/line_iterator.h` & `taffy-0.0.3/taffy/inc/line_iterator.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/inc/ond.h` & `taffy-0.0.3/taffy/inc/ond.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/inc/taf.h` & `taffy-0.0.3/taffy/inc/taf.h`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
  * Gets the number of columns in the alignment
  */
 int64_t alignment_length(Alignment *alignment);
 
 /*
  * Gets the max length of an interstitial gap sequence between this block and the next one.
  */
-int64_t alignment_total_gap_length(Alignment *left_alignment);
+int64_t alignment_max_gap_length(Alignment *left_alignment);
 
 /*
  * Number of shared rows between two alignments
  */
 int64_t alignment_number_of_common_rows(Alignment *left_alignment, Alignment *right_alignment);
 
 /*
@@ -132,14 +132,19 @@
 
 /*
  * Read a column of the alignment and return as a string
  */
 char *alignment_get_column(Alignment *alignment, int64_t column_index);
 
 /*
+ * Read a column of the alignment as an integer array where A/a=0, C/c=1, G/g=2, T/t=3, -=4, everything else=5
+ */
+int32_t *alignment_get_column_as_int_array(Alignment *alignment, int64_t column_index);
+
+/*
  * Cleanup a row
  */
 void alignment_row_destruct(Alignment_Row *row);
 
 /*
  * Returns non-zero if left_row represents a substring on the same contig and strand as right_row, but
  * immediately before
@@ -222,18 +227,18 @@
 /*
  * Write a taf block.
  */
 void taf_write_block(Alignment *p_alignment, Alignment *alignment, bool run_length_encode_bases,
                      int64_t repeat_coordinates_every_n_columns, LW *lw);
 
 /*
- * As taf write block, but with option to pretty print the output
+ * As taf write block, but with option to pretty print the output and/or omit coordinates for viewing
  */
 void taf_write_block2(Alignment *p_alignment, Alignment *alignment, bool run_length_encode_bases,
-                      int64_t repeat_coordinates_every_n_columns, LW *lw, bool color_bases);
+                      int64_t repeat_coordinates_every_n_columns, LW *lw, bool color_bases, bool omit_coordinates);
 
 
 // the following are low-level functions used in indexing.  they could
 // potentially be better put in an "internal" header
 
 /**
  * Check if a tokenized TAF line has coordinates (ie search for ;)
@@ -330,22 +335,32 @@
 /*
  * Gets the index in the list of the sequence prefix of the given row's sequence name.
  */
 int64_t alignment_row_get_closest_sequence_prefix(Alignment_Row *row, stList *prefixes_to_sort_by);
 
 /*
  * Sorts the rows of an alignment according to the given sequence prefixes. Reconnects the rows
- * with the previous alignment in the process.
+ * with the previous alignment in the process. Optionally ignore the first row so that it is not reordered
+ */
+void alignment_sort_the_rows(Alignment *p_alignment, Alignment *alignment, stList *prefixes_to_sort_by, bool ignore_first_row);
+
+/*
+ * Removes any rows from the alignment whose sequence name prefix matches a string in the prefixes_to_filter_by list
  */
-void alignment_sort_the_rows(Alignment *p_alignment, Alignment *alignment, stList *prefixes_to_sort_by);
+void alignment_filter_the_rows(Alignment *alignment, stList *prefixes_to_filter_by, bool ignore_first_row);
 
 /*
- * Removes any rows from the alignment whose sequence name prefix matches a string in the prefixes_to_filtet_by list
+ * Ensure there is at most one row per sequence prefix.
  */
-void alignment_filter_the_rows(Alignment *alignment, stList *prefixes_to_filter_by);
+void alignment_filter_duplicate_rows(Alignment *alignment, stList *prefixes_to_match_on, bool ignore_first_row);
+
+/*
+ * Adds additional padding rows to an alignment so that every sequence prefix in the list has a row in the alignment block
+ */
+void alignment_pad_the_rows(Alignment *p_alignment, Alignment *alignment, stList *sequence_prefixes);
 
 /*
  * Load sequences in fasta files into a hash from sequence names to sequences
  */
 stHash *load_sequences_from_fasta_files(char **seq_file_names, int64_t seq_file_number);
 
 /*
@@ -355,9 +370,28 @@
 
 /*
  * Add any gap strings between representing unaligned sequences between rows of alignment and p_alignment.
  */
 void alignment_add_gap_strings(Alignment *p_alignment, Alignment *alignment, stHash *fastas, int hal_handle, stSet *hal_species,
                                int64_t maximum_gap_string_length);
 
+
+/*
+ * Parse a wiggle file (which may be compressed) returning a hash table from sequence names to nested hashes,
+ * each nested hash being a map from sequence coordinates to floating point values.
+ *
+ * Make zero based flag will make coordinates 0 based rather than 1 based.
+ *
+ * Seq_prefix is prepended to each chromosome name to form the sequence name stored in the
+ * returned hash.
+ *
+ * Not very memory efficient, but used by taffy annotate.
+ */
+stHash *wig_parse(char *file, char *seq_prefix, bool make_zero_based);
+
+/*
+ * Get a value for a specific coordinate. Returns given default_value if coordinate doesn't exist.
+ */
+double wig_get_value(stHash *wig, char *seq, int64_t coordinate, double default_value);
+
 #endif /* STTAF_H_ */
```

### Comparing `taffy-0.0.2/taffy/lib.py` & `taffy-0.0.3/taffy/lib.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from taffy._taffy_cffi import ffi, lib
 import numpy as np
-
+import torch
+from collections import deque
 
 def _to_py_string(s):
     """ Convert a cffi string into a Python string in Python3 """
     return ffi.string(s).decode("utf-8")
 
 
 def _to_c_string(s):
@@ -81,18 +82,40 @@
         # requesting a column from the end of the alignment
         assert 0 <= column_index < self.column_number()
         column = lib.alignment_get_column(self._c_alignment, column_index)  # Get the column
         column_string = _to_py_string(column)  # Convert to Python string
         lib.free(column)  # Free C string
         return column_string
 
+    def get_column_as_np_array(self, column_index):
+        """ Get a column of the alignment as a numpy int32 array, where we map the bases to
+        consecutive integers, e.g. A/a=0, C/c=1, G/g=2, T/t=3, -=4, everything else=5.
+
+        Use negative coordinates to get columns from the end of the block """
+        column_index = column_index if column_index >= 0 else (self.column_number() + column_index)  # Correct if
+        # requesting a column from the end of the alignment
+        assert 0 <= column_index < self.column_number()
+        column = lib.alignment_get_column_as_int_array(self._c_alignment, column_index)  # Get the column
+        column_length = self.row_number()
+        # Convert the C array to a NumPy array, copying it in process
+        column_np = np.copy(np.frombuffer(ffi.buffer(column, ffi.sizeof("int32_t") * column_length), dtype=np.int32))
+        lib.free(column)  # Free C string
+        return column_np
+
+    def get_column_as_np_array_one_hot(self, column_index):
+        """ As get_column_as_np_array, but encoded one hot, using float32 """
+        column_np = self.get_column_as_np_array(column_index)
+        column_np_one_hot = np.zeros(shape=(len(column_np),6), dtype=np.float32)
+        column_np_one_hot[np.arange(len(column_np)), column_np] = 1.0
+        return column_np_one_hot
+
     def get_column_sequences(self):
-        """ Get the names of the sequences in the alignment in order as an array """
+        """ Get the names of the sequences in the alignment in order as a list """
         row = self.first_row()
-        sequence_names = np.empty(self.row_number(), dtype=object)
+        sequence_names = [None]*self.row_number()
         for i in range(self.row_number()):
             sequence_names[i] = row.sequence_name()
             row = row.next_row()
         return sequence_names
 
     def __del__(self):
         lib.alignment_destruct(self._c_alignment, 0)  # Cleans up the underlying C alignment structure
@@ -116,19 +139,18 @@
 
         return RowIter(self.first_row())
 
 
 class Row:
     """ Represents a row of an alignment block. See taf.h """
 
-    def __init__(self, c_row=None, l_row=None, r_row=None, n_row=None):
+    def __init__(self, c_row=None, n_row=None):
         self._c_row = c_row  # The underlying C row
-        self._l_row = l_row  # The prior (left) row in the previous alignment block
-        self._r_row = r_row  # The next (right) row in the next alignemnt clock
         self._n_row = n_row  # The next row in the sequence of rows
+        # Note by choice we do not store pointers to the left and right rows
 
     def sequence_name(self):
         """ The name of the sequence for the row """
         return _to_py_string(self._c_row.sequence_name)
 
     def start(self):
         """ The start coordinate of the base in the row (if strand is False then will be with respect to
@@ -156,22 +178,14 @@
         (left) alignment block """
         return "" if self._c_row.left_gap_sequence == ffi.NULL else _to_py_string(self._c_row.self.left_gap_sequence)
 
     def next_row(self):
         """ Get the next row in the alignment block or None if last row """
         return self._n_row
 
-    def left_row(self):
-        """ Get any left row in the prior alignment block """
-        return self._l_row
-
-    def right_row(self):
-        """ Get any right row in the next alignment block """
-        return self._r_row
-
     def __del__(self):
         lib.alignment_row_destruct(self._c_row)  # Cleans up the underlying C alignment structure
 
     def __str__(self):
         return _to_py_string(lib.alignment_row_to_string(self._c_row))
 
 
@@ -190,49 +204,64 @@
         lib.tai_destruct(self._c_taf_index)  # Clean up the underlying C
 
 
 class AlignmentReader:
     """ Taf or maf alignment parser.
     """
 
-    def __init__(self, file, taf_index=None, sequence_name=None, start=-1, length=-1):
-        """ Use taf_not_maf to switch between MAF or TAF parsing.
-
-        file can be either a Python file handle or a string giving a path to the file.
-        Handing in the file name is much faster as it avoids using a Python file object. If using
-        with a file string remember to close the file, either the with keyword or with the close method.
-
-        If file is compressed with zip or bgzip will automatically detect that the file is compressed and read it okay.
-
-        Use the taf_index and sequence_name, start and length if you want to extract a region from a taf file using
-        a taf index. Also works with compressed files.
+    def __init__(self, file, taf_index=None,  sequence_intervals=None):
+        """
+        :param file: File can be either a Python file handle or a string giving a path to the file.
+        The underlying file can be either maf or taf. Handing in the file name is much faster as it avoids using a
+        Python file object. If using with a file string remember to close the file, either the with keyword or with
+        the close method. If file is compressed with zip or bgzip will automatically detect that the file is
+        compressed and read it okay.
+        :param taf_index: A taf index object, which is specified allows the retrieval of subranges of the alignment.
+        :param sequence_intervals: A sequence of one or more tuples, each of the form (sequence_name, start, length)
+        that specify the range to retrieve. Will be retrieved in order.
         """
         self.p_c_alignment = ffi.NULL  # The previous C alignment returned
         self.p_c_rows_to_py_rows = {}  # Hash from C rows to Python rows of the previous
         # alignment block, allowing linking of rows between blocks
+        self.file = file
         self.c_file_handle = _get_c_file_handle(file)
         self.file_string_not_handle = isinstance(file, str)  # Will be true if the file is a string, not a file handle
         self.c_li_handle = lib.LI_construct(self.c_file_handle)
         i = lib.check_input_format(lib.LI_peek_at_next_line(self.c_li_handle))
         if i not in (0, 1):
             raise RuntimeError("Input file is not a TAF or MAF file")
         self.taf_not_maf = i == 0  # Sniff the file header to determine if a taf file
         self.taf_index = taf_index  # Store the taf index (if there is one)
         self.header_tags = self._read_header()  # Read the header tags
-        self.use_run_length_encoding = "run_length_encode_bases" in self.header_tags  # Use run length encoding
+
+        # Parse run length encoding
+        self.use_run_length_encoding = False
+        if "run_length_encode_bases" in self.header_tags:
+            assert self.header_tags["run_length_encode_bases"] in ("0", "1")
+            self.use_run_length_encoding = self.header_tags["run_length_encode_bases"] == "1"
+
+        self.sequence_intervals = sequence_intervals
+        self.sequence_interval_index = 0
 
         if taf_index:
-            assert self.taf_not_maf  # Can not be trying to parse maf with a taf index
-            assert sequence_name  # The contig name can not be none if using a taf index
-            assert start >= 0  # The start coordinate must be valid
-            assert length >= 0  # The length must be valid
-            self._c_taf_index_it = lib.tai_iterator(taf_index._c_taf_index,
-                                                    self.c_li_handle,
-                                                    self.use_run_length_encoding,
-                                                    _to_c_string(sequence_name), start, length)
+            assert self.sequence_intervals is not None  # Must not be None
+            if len(self.sequence_intervals) > 0:
+                sequence_name, start, length = sequence_intervals[0]
+                assert sequence_name  # The contig name can not be none if using a taf index
+                assert start >= 0  # The start coordinate must be valid
+                assert length >= 0  # The length must be valid
+                assert len(sequence_intervals) > 0  # Must contain at least one interval
+                self._c_taf_index_it = lib.tai_iterator(taf_index._c_taf_index,
+                                                        self.c_li_handle,
+                                                        self.use_run_length_encoding,
+                                                        _to_c_string(sequence_name), start, length)
+            else:
+                self._c_taf_index_it = None  # Case we have an empty iteration
+        else:
+            assert not sequence_intervals  # Sequence intervals should not be specified if taf index not provided
 
     def get_header(self):
         """ Get tags from the header line as a dictionary of key:value pairs.
         Must be called if a header is present in the file before blocks are retrieved """
         return dict(self.header_tags)  # Make a copy
 
     def _read_header(self):
@@ -240,58 +269,66 @@
         c_tag = lib.taf_read_header(self.c_li_handle) if self.taf_not_maf else lib.maf_read_header(self.c_li_handle)
         p_tags = _c_tags_to_dictionary(c_tag)
         lib.tag_destruct(c_tag)  # Clean up tag
         return p_tags
 
     def __next__(self):
         """ Get the next alignment block """
+        if self.taf_index and not self.sequence_intervals:  # Case we have a taf index but no sequence intervals, we're
+            # immediately done
+            raise StopIteration  # We're done
+
         # Read a taf/maf block
         if self.taf_not_maf:  # Is a taf block
             # Use the taf index if present
             c_alignment = lib.tai_next(self._c_taf_index_it, self.c_li_handle) if self.taf_index else \
-                lib.taf_read_block(self.p_c_alignment, 0, self.c_li_handle)
+                lib.taf_read_block(self.p_c_alignment, self.use_run_length_encoding, self.c_li_handle)
         else:  # Is a maf block
-            c_alignment = lib.maf_read_block(self.c_li_handle)
+            c_alignment = lib.tai_next(self._c_taf_index_it, self.c_li_handle) if self.taf_index else \
+                lib.maf_read_block(self.c_li_handle)
 
         if c_alignment == ffi.NULL:  # If the c_alignment is null
-            raise StopIteration  # We're done
+            self.sequence_interval_index += 1
+            if self.sequence_intervals is None or self.sequence_interval_index >= len(self.sequence_intervals):
+                raise StopIteration  # We're done
+            # Otherwise, get next interval
+            sequence_name, start, length = self.sequence_intervals[self.sequence_interval_index]
+            # Make new iterator for next interval
+            self.p_c_alignment = ffi.NULL  # Remove reference to prior alignment
+            lib.tai_iterator_destruct(self._c_taf_index_it)  # Cleanup old iterator
+            self._c_taf_index_it = lib.tai_iterator(self.taf_index._c_taf_index,
+                                                    self.c_li_handle,
+                                                    self.use_run_length_encoding,
+                                                    _to_c_string(sequence_name), start, length)
+            return self.__next__()
 
         # If maf use O(ND) algorithm to link to any prior alignment block
         if (not self.taf_not_maf) and self.p_c_alignment != ffi.NULL:
             lib.alignment_link_adjacent(self.p_c_alignment, c_alignment, 1)
 
         # Now add in the rows
-        c_row, p_py_row, c_rows_to_py_rows = c_alignment.row, None, {}
+        c_row, p_py_row, first_py_row = c_alignment.row, None, None
         while c_row != ffi.NULL:
-            # The previous py row
-
-            # Make the Python row object
-            if c_row.l_row == ffi.NULL:  # If there is no prior left row to connect to
-                py_row = Row(c_row=c_row)
-            else:  # Otherwise, there is a prior left row to connect to
-                l_py_row = self.p_c_rows_to_py_rows[c_row.l_row]
-                py_row = Row(c_row=c_row, l_row=l_py_row)
-                l_py_row._r_row = py_row
-
-            # Add to the map of c rows to python rows
-            c_rows_to_py_rows[c_row] = py_row
+            # Make the Pythob row
+            py_row = Row(c_row=c_row)
+            if first_py_row is None:
+                first_py_row = py_row
 
             # Connect the row object to the chain of row objects for the block
             if p_py_row is not None:
                 p_py_row._n_row = py_row
 
             p_py_row = py_row  # Update the previous python row object
             c_row = c_row.n_row  # Move to the next row
 
         # Now convert the new alignment into Python
-        py_alignment = Alignment(c_alignment=c_alignment, py_row=c_rows_to_py_rows[c_alignment.row])
+        py_alignment = Alignment(c_alignment=c_alignment, py_row=first_py_row)
 
         # Set the new prior alignment / rows
         self.p_c_alignment = c_alignment
-        self.p_c_rows_to_py_rows = c_rows_to_py_rows
 
         return py_alignment
 
     def __iter__(self):
         return self  # Making this an iterable
 
     def close(self):
@@ -305,25 +342,188 @@
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         self.close()
 
 
-def get_column_iterator(alignment_reader):
+def get_reference_sequence_intervals(alignment_reader):
+    """ Generates a sequence of reference sequence intervals by scanning through the alignment_reader.
+    Each generated value is of the form (seq_name, start, length). Length is the number of
+    reference bases in blocks within the interval (e.g. ignores unaligned ref gaps).
+    """
+    seq_intervals = []
+    p_ref_seq, p_ref_start, p_ref_length = None, 0, 0
+    for alignment in alignment_reader:  # For each alignment block
+        # Get the reference row so we can keep track of the reference coordinates
+        ref_row = alignment.first_row()
+        if ref_row is None:  # Weird case we are on an empty block - technically possible in taf
+            continue
+        seq_name = ref_row.sequence_name()  # Get the sequence name
+        assert seq_name is not None  # Seq name can not be unspecified
+        if seq_name != p_ref_seq:  # If we have a new reference sequence
+            if p_ref_seq is not None:  # If there is a previous reference sequence, add it to the list
+                yield p_ref_seq, p_ref_start, p_ref_length
+            p_ref_seq = seq_name  # Set the new reference sequence interval
+            p_ref_start = ref_row.start()
+            p_ref_length = ref_row.length()
+        else:
+            p_ref_length += ref_row.length()  # If not a new ref sequence, just add the number of ref bases
+            # in the block
+    if p_ref_seq is not None:
+        yield p_ref_seq, p_ref_start, p_ref_length
+
+
+def get_column_iterator(alignment_reader,
+                        include_sequence_names=True,
+                        include_non_ref_columns=True,
+                        include_column_tags=False,
+                        column_as_int_array=False,
+                        column_as_int_array_one_hot=False):
     """ Create an alignment column iterator which returns successive
     columns from the alignment from an AlignmentReader object.
 
-    Each is returned as an array of sequence names and a string representing the bases
-    in the column
+    If alignment_reader was created given a sequence interval only the columns from that given reference
+    interval will be returned.
+
+    Each column returned is a column string and a tuple representing the "label" of the column.
+    The label tuple is a composed of the reference index of the column and:
+        If include_sequence_names is True then the second value is an array of sequence names for the columns.
+        If include_column_tags is True then the last value in the label tuple will be a dictionary of any tags.
+
+    If include_non_ref_columns is True then columns not including the reference in the interval will also be returned.
+
+    If column_as_int_array is True then columns will be returned as numpy arrays, see Alignment.get_column_as_np_array()
     """
+    if column_as_int_array:
+        assert not column_as_int_array_one_hot
     for alignment in alignment_reader:  # For each alignment block
-        sequence_names = alignment.get_column_sequences()
-        for i in range(alignment.column_number()):  # For each column
-            yield sequence_names, alignment.get_column(i)
+        # Get the reference row so we can keep track of the reference coordinates
+        ref_row = alignment.first_row()
+        if ref_row is None:  # Weird case we are on an empty block - technically possible in taf
+            continue
+        ref_index = ref_row.start()
+        ref_bases = ref_row.bases()
+
+        # Determine the kind of column to return
+        if column_as_int_array:
+            get_column = alignment.get_column_as_np_array
+        elif column_as_int_array_one_hot:
+            get_column = alignment.get_column_as_np_array_one_hot
+        else:
+            get_column = alignment.get_column
+
+        # If the output wants to match the column entries to the sequences
+        if include_sequence_names:
+            sequence_names = alignment.get_column_sequences()
+            if include_non_ref_columns:
+                if include_column_tags:
+                    for i in range(alignment.column_number()):
+                        yield get_column(i), (ref_index, sequence_names, alignment.column_tags(i))
+                        if ref_bases[i] != '-':
+                            ref_index += 1
+                else:
+                    for i in range(alignment.column_number()):
+                        yield get_column(i), (ref_index, sequence_names)
+                        if ref_bases[i] != '-':
+                            ref_index += 1
+            else:
+                if include_column_tags:
+                    for i in range(alignment.column_number()):
+                        if ref_bases[i] != '-':
+                            yield get_column(i), (ref_index, sequence_names, alignment.column_tags(i))
+                            ref_index += 1
+                else:
+                    for i in range(alignment.column_number()):
+                        if ref_bases[i] != '-':
+                            yield get_column(i), (ref_index, sequence_names)
+                            ref_index += 1
+        else:
+            if include_non_ref_columns:
+                if include_column_tags:
+                    for i in range(alignment.column_number()):
+                        yield get_column(i), (ref_index, alignment.column_tags(i))
+                        if ref_bases[i] != '-':
+                            ref_index += 1
+                else:
+                    for i in range(alignment.column_number()):
+                        yield get_column(i), (ref_index,)
+                        if ref_bases[i] != '-':
+                            ref_index += 1
+            else:
+                if include_column_tags:
+                    for i in range(alignment.column_number()):
+                        if ref_bases[i] != '-':
+                            yield get_column(i), (ref_index, alignment.column_tags(i))
+                            ref_index += 1
+                else:
+                    for i in range(alignment.column_number()):
+                        if ref_bases[i] != '-':
+                            yield get_column(i), (ref_index,)
+                            ref_index += 1
+
+
+def get_window_iterator(alignment_reader,
+                        window_length=10, step=1,
+                        include_sequence_names=True,
+                        include_non_ref_columns=True,
+                        include_column_tags=False,
+                        column_as_int_array=False,
+                        column_as_int_array_one_hot=False):
+    """ Iterate over (overlapping) windows of the alignment. If columns are numpy arrays the return value
+    will be a multidimensional matrix with the first index being the columns. Otherwise columns are returned
+    as an array.
+
+    :param alignment_reader: An alignment reader to iterate from
+    :param window_length: The number of successive columns to include in a window, must be > 0
+    :param step: The number of columns between successive windows, must be 0 < step <= window_length.
+    If equal to the window length will mean windows are non-overlapping
+    :param include_sequence_names: See get_column_iterator()
+    :param include_non_ref_columns: See get_column_iterator()
+    :param include_column_tags: See get_column_iterator()
+    :param column_as_int_array: See get_column_iterator()
+    :param column_as_int_array_one_hot: See get_column_iterator()
+    :return: A numpy array of columns, each column from get_column_iterator(), and another numpy array of labels
+    """
+    assert window_length > 0  # Window length must be positive integer
+    assert step <= window_length  # Step can not exceed the window length
+    assert step >= 1  # Step can not be negative or 0
+    q = deque()
+    # If we have numpy arrays then we can concatenate them to create a single tensor
+    column_it = get_column_iterator(alignment_reader,
+                                    include_sequence_names=include_sequence_names,
+                                    include_non_ref_columns=include_non_ref_columns,
+                                    include_column_tags=include_column_tags,
+                                    column_as_int_array=column_as_int_array,
+                                    column_as_int_array_one_hot=column_as_int_array_one_hot)
+    if column_as_int_array or column_as_int_array_one_hot:
+        for column, labels in column_it:
+            column.shape = (1,) + column.shape  # As we will be joining the column we add an extra "prefix" dimension
+            q.append((column, labels))  # Add to the right end of the window
+            assert len(q) <= window_length
+            if len(q) == window_length:
+                labels = np.empty(window_length, dtype=object)
+                for i in range(window_length):  # Fill out the column and label arrays
+                    labels[i] = q[i][1]
+                columns = np.concatenate(tuple(i[0] for i in q))  # Concatenate together the column arrays
+                yield columns, labels
+                for i in range(step):
+                    q.popleft()  # Remove from the left end of the window
+    else:  # Otherwise, the columns are strings, and we return them as a 1-d array of strings for each window
+        for column, labels in column_it:
+            q.append((column, labels))  # Add to the right end of the window
+            assert len(q) <= window_length
+            if len(q) == window_length:
+                columns, labels = np.empty(window_length, dtype=object), np.empty(window_length, dtype=object)
+                for i in range(window_length):  # Fill out the column and label arrays
+                    columns[i] = q[i][0]
+                    labels[i] = q[i][1]
+                yield columns, labels
+                for i in range(step):
+                    q.popleft()  # Remove from the left end of the window
 
 
 def write_taf_index_file(taf_file, index_file, index_block_size=10000):
     """ Create a taf index file """
     c_taf_file_handle = _get_c_file_handle(taf_file)
     c_li_handle = lib.LI_construct(c_taf_file_handle)
     c_index_file_handle = _get_c_file_handle(index_file, "w")
@@ -384,7 +584,8 @@
         lib.LW_destruct(self.c_lw_handle, self.file_string_not_handle)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         self.close()
+
```

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/avl.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/avl.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/bioioC.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/bioioC.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/commonC.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/commonC.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/fastCMaths.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/fastCMaths.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/hashTableC.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/hashTableC.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/hashTableC_itr.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/hashTableC_itr.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/jsmn.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/jsmn.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/lz4.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/lz4.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/lz4.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/lz4.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/lz4hc.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/lz4hc.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/lz4hc.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/lz4hc.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/pairwiseAlignment.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/pairwiseAlignment.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibCache.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibCache.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibCommon.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibCommon.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibCompression.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibCompression.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibConnectivity.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibConnectivity.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibEulerTour.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibEulerTour.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibExcept.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibExcept.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibFile.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibFile.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibGlobalsInternal.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibGlobalsInternal.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibHash.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibHash.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibKVDatabase.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibKVDatabase.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibKVDatabaseConf.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibKVDatabaseConf.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibKVDatabasePrivate.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibKVDatabasePrivate.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibKVDatabase_BigRecordFile.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibKVDatabase_BigRecordFile.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibKVDatabase_MySql.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibKVDatabase_MySql.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibKVDatabase_Redis.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibKVDatabase_Redis.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibKVDatabase_TokyoCabinet.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibKVDatabase_TokyoCabinet.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibList.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibList.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibMath.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibMath.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibNaiveConnectivity.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibNaiveConnectivity.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibRandom.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibRandom.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibSet.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibSet.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibSortedSet.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibSortedSet.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibString.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibString.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibTreap.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibTreap.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibTree.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibTree.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/sonLibTuples.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/sonLibTuples.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/stGraph.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/stGraph.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/stJson.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/stJson.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/stMatrix.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/stMatrix.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/stPhylogeny.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/stPhylogeny.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/stPosetAlignment.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/stPosetAlignment.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/stSafeC.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/stSafeC.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/stThreadPool.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/stThreadPool.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/impl/stUnionFind.c` & `taffy-0.0.3/taffy/submodules/sonLib/C/impl/stUnionFind.c`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/avl.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/avl.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/bioioC.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/bioioC.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/commonC.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/commonC.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/fastCMaths.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/fastCMaths.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/hashTableC.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/hashTableC.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/hashTableC_itr.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/hashTableC_itr.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/hashTablePrivateC.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/hashTablePrivateC.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/jsmn.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/jsmn.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/pairwiseAlignment.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/pairwiseAlignment.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/safesort.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/safesort.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLib.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLib.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibCache.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibCache.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibCommon.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibCommon.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibCompression.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibCompression.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibConnectivity.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibConnectivity.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibEulerTour.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibEulerTour.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibExcept.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibExcept.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibFile.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibFile.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibHash.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibHash.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibKVDatabase.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibKVDatabase.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibKVDatabaseConf.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibKVDatabaseConf.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibList.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibList.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibMath.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibMath.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibNaiveConnectivity.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibNaiveConnectivity.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibRandom.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibRandom.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibSet.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibSet.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibSortedSet.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibSortedSet.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibString.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibString.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibTreap.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibTreap.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibTree.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibTree.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibTuples.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibTuples.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/sonLibTypes.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/sonLibTypes.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/stGraph.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/stGraph.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/stJson.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/stJson.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/stMatrix.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/stMatrix.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/stPhylogeny.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/stPhylogeny.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/stPosetAlignment.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/stPosetAlignment.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/stSafeC.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/stSafeC.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/stSpimapLayer.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/stSpimapLayer.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/stThreadPool.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/stThreadPool.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/C/inc/stUnionFind.h` & `taffy-0.0.3/taffy/submodules/sonLib/C/inc/stUnionFind.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy/submodules/sonLib/externalTools/cutest/CuTest.h` & `taffy-0.0.3/taffy/submodules/sonLib/externalTools/cutest/CuTest.h`

 * *Files identical despite different names*

### Comparing `taffy-0.0.2/taffy.egg-info/SOURCES.txt` & `taffy-0.0.3/taffy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,32 +2,37 @@
 README.md
 pyproject.toml
 setup.py
 taffy/__init__.py
 taffy/_taffy_build.py
 taffy/lib.py
 taffy/ml.py
+taffy/newick.py
+taffy/wiggle.py
 taffy.egg-info/PKG-INFO
 taffy.egg-info/SOURCES.txt
 taffy.egg-info/dependency_links.txt
 taffy.egg-info/requires.txt
 taffy.egg-info/top_level.txt
 taffy/impl/alignment_block.c
 taffy/impl/line_iterator.c
 taffy/impl/maf.c
 taffy/impl/merge_adjacent_alignments.c
 taffy/impl/ond.c
 taffy/impl/paf.c
 taffy/impl/prefix_sort.c
 taffy/impl/taf.c
 taffy/impl/tai.c
+taffy/impl/wiggle.c
 taffy/inc/line_iterator.h
 taffy/inc/ond.h
 taffy/inc/taf.h
 taffy/inc/tai.h
+taffy/submodules/abPOA/include/abpoa.h
+taffy/submodules/abPOA/include/simd_instruction.h
 taffy/submodules/sonLib/C/impl/avl.c
 taffy/submodules/sonLib/C/impl/bioioC.c
 taffy/submodules/sonLib/C/impl/commonC.c
 taffy/submodules/sonLib/C/impl/fastCMaths.c
 taffy/submodules/sonLib/C/impl/hashTableC.c
 taffy/submodules/sonLib/C/impl/hashTableC_itr.c
 taffy/submodules/sonLib/C/impl/jsmn.c
```

