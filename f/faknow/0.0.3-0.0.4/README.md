# Comparing `tmp/faknow-0.0.3.tar.gz` & `tmp/faknow-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faknow-0.0.3.tar", last modified: Thu Feb  1 12:54:49 2024, max compression
+gzip compressed data, was "faknow-0.0.4.tar", last modified: Sat May 18 09:16:30 2024, max compression
```

## Comparing `faknow-0.0.3.tar` & `faknow-0.0.4.tar`

### file list

```diff
@@ -1,134 +1,137 @@
-drwxrwxrwx   0        0        0        0 2024-02-01 12:54:49.209845 faknow-0.0.3/
--rw-rw-rw-   0        0        0     1081 2023-10-11 07:37:29.000000 faknow-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       39 2023-10-11 07:37:29.000000 faknow-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0    16540 2024-02-01 12:54:49.207851 faknow-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    15836 2024-02-01 09:44:26.000000 faknow-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-02-01 12:54:48.122566 faknow-0.0.3/faknow/
--rw-rw-rw-   0        0        0       23 2024-01-31 05:39:48.000000 faknow-0.0.3/faknow/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-01 12:54:48.199358 faknow-0.0.3/faknow/data/
--rw-rw-rw-   0        0        0        0 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-01 12:54:48.336608 faknow-0.0.3/faknow/data/dataset/
--rw-rw-rw-   0        0        0        0 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/data/dataset/__init__.py
--rw-rw-rw-   0        0        0     2434 2023-11-29 07:12:09.000000 faknow-0.0.3/faknow/data/dataset/bigcn_dataset.py
--rw-rw-rw-   0        0        0      803 2023-12-13 07:17:54.000000 faknow-0.0.3/faknow/data/dataset/cafe_dataset.py
--rw-rw-rw-   0        0        0      392 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/data/dataset/dataset.py
--rw-rw-rw-   0        0        0    14972 2024-01-30 08:32:35.000000 faknow-0.0.3/faknow/data/dataset/dudef_dataset.py
--rw-rw-rw-   0        0        0    12934 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/data/dataset/fang_dataset.py
--rw-rw-rw-   0        0        0     4066 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/data/dataset/m3fend_dataset.py
--rw-rw-rw-   0        0        0     4969 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/data/dataset/multi_modal.py
--rw-rw-rw-   0        0        0     1041 2024-01-30 08:32:21.000000 faknow-0.0.3/faknow/data/dataset/safe_dataset.py
--rw-rw-rw-   0        0        0     3179 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/data/dataset/spotfake_dataset.py
--rw-rw-rw-   0        0        0     5237 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/data/dataset/text.py
--rw-rw-rw-   0        0        0     3311 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/data/dataset/trustrd_dataset.py
-drwxrwxrwx   0        0        0        0 2024-02-01 12:54:48.370042 faknow-0.0.3/faknow/data/process/
--rw-rw-rw-   0        0        0        0 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/data/process/__init__.py
--rw-rw-rw-   0        0        0     9175 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/data/process/process.py
--rw-rw-rw-   0        0        0     3868 2023-11-29 07:12:09.000000 faknow-0.0.3/faknow/data/process/text_process.py
-drwxrwxrwx   0        0        0        0 2024-02-01 12:54:48.389988 faknow-0.0.3/faknow/evaluate/
--rw-rw-rw-   0        0        0        0 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/evaluate/__init__.py
--rw-rw-rw-   0        0        0     2352 2023-11-06 14:48:23.000000 faknow-0.0.3/faknow/evaluate/evaluator.py
--rw-rw-rw-   0        0        0     3009 2023-11-06 14:48:24.000000 faknow-0.0.3/faknow/evaluate/metrics.py
-drwxrwxrwx   0        0        0        0 2024-02-01 12:54:48.403461 faknow-0.0.3/faknow/model/
--rw-rw-rw-   0        0        0        0 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-01 12:54:48.463678 faknow-0.0.3/faknow/model/content_based/
--rw-rw-rw-   0        0        0        0 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/model/content_based/__init__.py
--rw-rw-rw-   0        0        0     5990 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/model/content_based/endef.py
--rw-rw-rw-   0        0        0    16354 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/model/content_based/m3fend.py
--rw-rw-rw-   0        0        0     6380 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/model/content_based/mdfend.py
-drwxrwxrwx   0        0        0        0 2024-02-01 12:54:48.571772 faknow-0.0.3/faknow/model/content_based/multi_modal/
--rw-rw-rw-   0        0        0        0 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/model/content_based/multi_modal/__init__.py
--rw-rw-rw-   0        0        0    16896 2023-12-13 07:17:54.000000 faknow-0.0.3/faknow/model/content_based/multi_modal/cafe.py
--rw-rw-rw-   0        0        0     5172 2023-10-16 12:41:05.000000 faknow-0.0.3/faknow/model/content_based/multi_modal/eann.py
--rw-rw-rw-   0        0        0    12660 2023-12-04 07:43:35.000000 faknow-0.0.3/faknow/model/content_based/multi_modal/hmcan.py
--rw-rw-rw-   0        0        0    14474 2023-12-04 07:49:47.000000 faknow-0.0.3/faknow/model/content_based/multi_modal/mcan.py
--rw-rw-rw-   0        0        0    11087 2023-11-17 10:12:40.000000 faknow-0.0.3/faknow/model/content_based/multi_modal/mfan.py
--rw-rw-rw-   0        0        0     6645 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/model/content_based/multi_modal/safe.py
--rw-rw-rw-   0        0        0    10665 2023-11-23 06:17:06.000000 faknow-0.0.3/faknow/model/content_based/multi_modal/spotfake.py
--rw-rw-rw-   0        0        0     3101 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/model/content_based/textcnn.py
-drwxrwxrwx   0        0        0        0 2024-02-01 12:54:48.619605 faknow-0.0.3/faknow/model/layers/
--rw-rw-rw-   0        0        0        0 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/model/layers/__init__.py
--rw-rw-rw-   0        0        0     3979 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/model/layers/dct.py
--rw-rw-rw-   0        0        0    11687 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/model/layers/layer.py
--rw-rw-rw-   0        0        0     4407 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/model/layers/layers_m3fend.py
--rw-rw-rw-   0        0        0    13662 2023-11-29 07:12:09.000000 faknow-0.0.3/faknow/model/layers/transformer.py
--rw-rw-rw-   0        0        0     1177 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/model/model.py
-drwxrwxrwx   0        0        0        0 2024-02-01 12:54:48.746111 faknow-0.0.3/faknow/model/social_context/
--rw-rw-rw-   0        0        0        0 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/model/social_context/__init__.py
--rw-rw-rw-   0        0        0     4837 2023-11-06 14:48:24.000000 faknow-0.0.3/faknow/model/social_context/base_gnn.py
--rw-rw-rw-   0        0        0     5431 2023-10-31 12:00:48.000000 faknow-0.0.3/faknow/model/social_context/bigcn.py
--rw-rw-rw-   0        0        0     3046 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/model/social_context/dudef.py
--rw-rw-rw-   0        0        0    10716 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/model/social_context/ebgcn.py
--rw-rw-rw-   0        0        0     5954 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/model/social_context/eddfn.py
--rw-rw-rw-   0        0        0    26373 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/model/social_context/fang.py
--rw-rw-rw-   0        0        0     4302 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/model/social_context/gcnfn.py
--rw-rw-rw-   0        0        0     4938 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/model/social_context/gnncl.py
--rw-rw-rw-   0        0        0    15293 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/model/social_context/trustrd.py
--rw-rw-rw-   0        0        0     2772 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/model/social_context/upfd.py
-drwxrwxrwx   0        0        0        0 2024-02-01 12:54:48.820865 faknow-0.0.3/faknow/properties/
--rw-rw-rw-   0        0        0       62 2023-10-16 12:41:05.000000 faknow-0.0.3/faknow/properties/bigcn.yaml
--rw-rw-rw-   0        0        0       32 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/properties/config.yaml
--rw-rw-rw-   0        0        0      306 2023-10-20 07:06:40.000000 faknow-0.0.3/faknow/properties/eann.yaml
--rw-rw-rw-   0        0        0      226 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/properties/eddfn.yaml
--rw-rw-rw-   0        0        0      138 2023-12-08 06:46:17.000000 faknow-0.0.3/faknow/properties/endef.yaml
--rw-rw-rw-   0        0        0      200 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/properties/finerfact.yaml
--rw-rw-rw-   0        0        0       65 2023-12-04 11:52:04.000000 faknow-0.0.3/faknow/properties/gcnfn.yaml
--rw-rw-rw-   0        0        0       65 2023-12-04 11:41:06.000000 faknow-0.0.3/faknow/properties/gnncl.yaml
--rw-rw-rw-   0        0        0      125 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/properties/m3fend.yaml
--rw-rw-rw-   0        0        0      108 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/properties/mcan.yaml
--rw-rw-rw-   0        0        0       96 2023-10-20 07:06:40.000000 faknow-0.0.3/faknow/properties/mdfend.yaml
--rw-rw-rw-   0        0        0      309 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/properties/mfan.yaml
--rw-rw-rw-   0        0        0       73 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/properties/nep.yaml
--rw-rw-rw-   0        0        0       90 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/properties/safe.yaml
--rw-rw-rw-   0        0        0      170 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/properties/spotfake.yaml
--rw-rw-rw-   0        0        0      391 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/properties/textcnn.yaml
--rw-rw-rw-   0        0        0       62 2023-12-04 11:48:25.000000 faknow-0.0.3/faknow/properties/upfd.yaml
-drwxrwxrwx   0        0        0        0 2024-02-01 12:54:48.823857 faknow-0.0.3/faknow/run/
--rw-rw-rw-   0        0        0      128 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/run/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-01 12:54:48.874722 faknow-0.0.3/faknow/run/content_based/
--rw-rw-rw-   0        0        0      331 2023-11-23 06:17:06.000000 faknow-0.0.3/faknow/run/content_based/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-01 12:54:48.976807 faknow-0.0.3/faknow/run/content_based/multimodal/
--rw-rw-rw-   0        0        0      753 2023-11-23 06:17:06.000000 faknow-0.0.3/faknow/run/content_based/multimodal/__init__.py
--rw-rw-rw-   0        0        0     3139 2023-12-13 07:17:54.000000 faknow-0.0.3/faknow/run/content_based/multimodal/run_cafe.py
--rw-rw-rw-   0        0        0     7647 2023-11-06 14:48:24.000000 faknow-0.0.3/faknow/run/content_based/multimodal/run_eann.py
--rw-rw-rw-   0        0        0     4716 2023-12-04 07:43:35.000000 faknow-0.0.3/faknow/run/content_based/multimodal/run_hmcan.py
--rw-rw-rw-   0        0        0    11913 2023-11-29 07:12:09.000000 faknow-0.0.3/faknow/run/content_based/multimodal/run_mcan.py
--rw-rw-rw-   0        0        0     7840 2023-11-29 07:12:09.000000 faknow-0.0.3/faknow/run/content_based/multimodal/run_mfan.py
--rw-rw-rw-   0        0        0     3597 2023-10-20 07:27:37.000000 faknow-0.0.3/faknow/run/content_based/multimodal/run_safe.py
--rw-rw-rw-   0        0        0     6490 2023-11-29 07:12:09.000000 faknow-0.0.3/faknow/run/content_based/multimodal/run_spotfake.py
--rw-rw-rw-   0        0        0     5307 2023-12-08 06:33:25.000000 faknow-0.0.3/faknow/run/content_based/run_endef.py
--rw-rw-rw-   0        0        0     7932 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/run/content_based/run_m3fend.py
--rw-rw-rw-   0        0        0     3617 2023-11-29 07:12:09.000000 faknow-0.0.3/faknow/run/content_based/run_mdfend.py
--rw-rw-rw-   0        0        0     6648 2023-11-06 14:48:24.000000 faknow-0.0.3/faknow/run/content_based/run_textcnn.py
--rw-rw-rw-   0        0        0      697 2023-12-04 11:30:17.000000 faknow-0.0.3/faknow/run/run.py
-drwxrwxrwx   0        0        0        0 2024-02-01 12:54:49.059740 faknow-0.0.3/faknow/run/social_context/
--rw-rw-rw-   0        0        0      397 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/run/social_context/__init__.py
--rw-rw-rw-   0        0        0     4782 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/run/social_context/run_bigcn.py
--rw-rw-rw-   0        0        0     3055 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/run/social_context/run_dudef.py
--rw-rw-rw-   0        0        0     5028 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/run/social_context/run_ebgcn.py
--rw-rw-rw-   0        0        0     3234 2023-11-06 14:48:24.000000 faknow-0.0.3/faknow/run/social_context/run_eddfn.py
--rw-rw-rw-   0        0        0     4194 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/run/social_context/run_fang.py
--rw-rw-rw-   0        0        0     4210 2023-10-20 07:27:37.000000 faknow-0.0.3/faknow/run/social_context/run_gcnfn.py
--rw-rw-rw-   0        0        0     4688 2023-10-20 07:27:37.000000 faknow-0.0.3/faknow/run/social_context/run_gnncl.py
--rw-rw-rw-   0        0        0     5272 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/run/social_context/run_trustrd.py
--rw-rw-rw-   0        0        0     4756 2023-10-20 07:27:37.000000 faknow-0.0.3/faknow/run/social_context/run_upfd.py
-drwxrwxrwx   0        0        0        0 2024-02-01 12:54:49.154595 faknow-0.0.3/faknow/train/
--rw-rw-rw-   0        0        0      111 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/train/__init__.py
--rw-rw-rw-   0        0        0     1057 2023-10-11 07:37:38.000000 faknow-0.0.3/faknow/train/base_gnn_trainer.py
--rw-rw-rw-   0        0        0     3487 2023-12-13 07:17:54.000000 faknow-0.0.3/faknow/train/cafe_trainer.py
--rw-rw-rw-   0        0        0     1115 2023-10-11 07:37:39.000000 faknow-0.0.3/faknow/train/dense_gnn_trainer.py
--rw-rw-rw-   0        0        0     1553 2023-10-11 07:37:39.000000 faknow-0.0.3/faknow/train/pgd_trainer.py
--rw-rw-rw-   0        0        0    20444 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/train/trainer.py
--rw-rw-rw-   0        0        0     9463 2023-10-11 07:37:39.000000 faknow-0.0.3/faknow/train/trainer_gpu.py
-drwxrwxrwx   0        0        0        0 2024-02-01 12:54:49.190187 faknow-0.0.3/faknow/utils/
--rw-rw-rw-   0        0        0        0 2023-10-11 07:37:39.000000 faknow-0.0.3/faknow/utils/__init__.py
--rw-rw-rw-   0        0        0     3093 2023-10-11 07:37:39.000000 faknow-0.0.3/faknow/utils/pgd.py
--rw-rw-rw-   0        0        0     4602 2024-01-25 13:59:24.000000 faknow-0.0.3/faknow/utils/util.py
-drwxrwxrwx   0        0        0        0 2024-02-01 12:54:49.205855 faknow-0.0.3/faknow.egg-info/
--rw-rw-rw-   0        0        0    16540 2024-02-01 12:54:47.000000 faknow-0.0.3/faknow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3836 2024-02-01 12:54:47.000000 faknow-0.0.3/faknow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-01 12:54:47.000000 faknow-0.0.3/faknow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-10-17 15:48:22.000000 faknow-0.0.3/faknow.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      185 2024-02-01 12:54:47.000000 faknow-0.0.3/faknow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-02-01 12:54:47.000000 faknow-0.0.3/faknow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-01 12:54:49.210842 faknow-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1541 2024-01-31 05:39:55.000000 faknow-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:16:30.881371 faknow-0.0.4/
+-rw-rw-rw-   0        0        0     1081 2023-11-09 08:13:31.000000 faknow-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-11-09 08:13:31.000000 faknow-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    16180 2024-05-18 09:16:30.881371 faknow-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    15837 2024-05-18 08:49:33.000000 faknow-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 09:16:29.733675 faknow-0.0.4/faknow/
+-rw-rw-rw-   0        0        0       23 2024-05-18 08:38:08.000000 faknow-0.0.4/faknow/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:16:29.824157 faknow-0.0.4/faknow/data/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:51:26.000000 faknow-0.0.4/faknow/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:16:30.004335 faknow-0.0.4/faknow/data/dataset/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:51:26.000000 faknow-0.0.4/faknow/data/dataset/__init__.py
+-rw-rw-rw-   0        0        0     2434 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/data/dataset/bigcn_dataset.py
+-rw-rw-rw-   0        0        0      803 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/data/dataset/cafe_dataset.py
+-rw-rw-rw-   0        0        0      392 2023-05-04 11:51:26.000000 faknow-0.0.4/faknow/data/dataset/dataset.py
+-rw-rw-rw-   0        0        0    14972 2024-01-17 12:51:18.000000 faknow-0.0.4/faknow/data/dataset/dudef_dataset.py
+-rw-rw-rw-   0        0        0    12934 2024-01-20 11:37:04.000000 faknow-0.0.4/faknow/data/dataset/fang_dataset.py
+-rw-rw-rw-   0        0        0     4066 2024-01-20 11:37:04.000000 faknow-0.0.4/faknow/data/dataset/m3fend_dataset.py
+-rw-rw-rw-   0        0        0     4969 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/data/dataset/multi_modal.py
+-rw-rw-rw-   0        0        0     1041 2024-03-06 13:03:38.000000 faknow-0.0.4/faknow/data/dataset/safe_dataset.py
+-rw-rw-rw-   0        0        0     3179 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/data/dataset/spotfake_dataset.py
+-rw-rw-rw-   0        0        0     5237 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/data/dataset/text.py
+-rw-rw-rw-   0        0        0     3311 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/data/dataset/trustrd_dataset.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:16:30.032613 faknow-0.0.4/faknow/data/process/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:51:26.000000 faknow-0.0.4/faknow/data/process/__init__.py
+-rw-rw-rw-   0        0        0     9175 2024-01-21 11:04:06.000000 faknow-0.0.4/faknow/data/process/process.py
+-rw-rw-rw-   0        0        0     3868 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/data/process/text_process.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:16:30.061356 faknow-0.0.4/faknow/evaluate/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:51:26.000000 faknow-0.0.4/faknow/evaluate/__init__.py
+-rw-rw-rw-   0        0        0     2352 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/evaluate/evaluator.py
+-rw-rw-rw-   0        0        0     3009 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/evaluate/metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:16:30.073898 faknow-0.0.4/faknow/model/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:51:26.000000 faknow-0.0.4/faknow/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:16:30.186399 faknow-0.0.4/faknow/model/content_based/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:51:26.000000 faknow-0.0.4/faknow/model/content_based/__init__.py
+-rw-rw-rw-   0        0        0     5990 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/model/content_based/endef.py
+-rw-rw-rw-   0        0        0    16354 2024-01-20 13:14:22.000000 faknow-0.0.4/faknow/model/content_based/m3fend.py
+-rw-rw-rw-   0        0        0     6380 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/model/content_based/mdfend.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:16:30.273632 faknow-0.0.4/faknow/model/content_based/multi_modal/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:51:26.000000 faknow-0.0.4/faknow/model/content_based/multi_modal/__init__.py
+-rw-rw-rw-   0        0        0    17060 2024-03-06 13:02:42.000000 faknow-0.0.4/faknow/model/content_based/multi_modal/cafe.py
+-rw-rw-rw-   0        0        0     5172 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/model/content_based/multi_modal/eann.py
+-rw-rw-rw-   0        0        0    12660 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/model/content_based/multi_modal/hmcan.py
+-rw-rw-rw-   0        0        0    14474 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/model/content_based/multi_modal/mcan.py
+-rw-rw-rw-   0        0        0    11087 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/model/content_based/multi_modal/mfan.py
+-rw-rw-rw-   0        0        0     6645 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/model/content_based/multi_modal/safe.py
+-rw-rw-rw-   0        0        0    10665 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/model/content_based/multi_modal/spotfake.py
+-rw-rw-rw-   0        0        0     3101 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/model/content_based/textcnn.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:16:30.324105 faknow-0.0.4/faknow/model/layers/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:51:26.000000 faknow-0.0.4/faknow/model/layers/__init__.py
+-rw-rw-rw-   0        0        0     3979 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/model/layers/dct.py
+-rw-rw-rw-   0        0        0    11687 2024-01-21 11:09:39.000000 faknow-0.0.4/faknow/model/layers/layer.py
+-rw-rw-rw-   0        0        0     4407 2024-01-20 11:45:38.000000 faknow-0.0.4/faknow/model/layers/layers_m3fend.py
+-rw-rw-rw-   0        0        0    13662 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/model/layers/transformer.py
+-rw-rw-rw-   0        0        0     1177 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/model/model.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:16:30.466543 faknow-0.0.4/faknow/model/social_context/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:51:26.000000 faknow-0.0.4/faknow/model/social_context/__init__.py
+-rw-rw-rw-   0        0        0     4837 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/model/social_context/base_gnn.py
+-rw-rw-rw-   0        0        0     5431 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/model/social_context/bigcn.py
+-rw-rw-rw-   0        0        0     3046 2024-01-17 12:47:11.000000 faknow-0.0.4/faknow/model/social_context/dudef.py
+-rw-rw-rw-   0        0        0    10716 2024-01-20 13:22:25.000000 faknow-0.0.4/faknow/model/social_context/ebgcn.py
+-rw-rw-rw-   0        0        0     5954 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/model/social_context/eddfn.py
+-rw-rw-rw-   0        0        0    26373 2024-01-20 11:37:04.000000 faknow-0.0.4/faknow/model/social_context/fang.py
+-rw-rw-rw-   0        0        0     4302 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/model/social_context/gcnfn.py
+-rw-rw-rw-   0        0        0     4938 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/model/social_context/gnncl.py
+-rw-rw-rw-   0        0        0    15293 2023-12-16 14:13:04.000000 faknow-0.0.4/faknow/model/social_context/trustrd.py
+-rw-rw-rw-   0        0        0     2772 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/model/social_context/upfd.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:16:30.501577 faknow-0.0.4/faknow/properties/
+-rw-rw-rw-   0        0        0       62 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/properties/bigcn.yaml
+-rw-rw-rw-   0        0        0       32 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/properties/config.yaml
+-rw-rw-rw-   0        0        0      306 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/properties/eann.yaml
+-rw-rw-rw-   0        0        0      226 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/properties/eddfn.yaml
+-rw-rw-rw-   0        0        0      138 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/properties/endef.yaml
+-rw-rw-rw-   0        0        0      200 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/properties/finerfact.yaml
+-rw-rw-rw-   0        0        0       65 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/properties/gcnfn.yaml
+-rw-rw-rw-   0        0        0       65 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/properties/gnncl.yaml
+-rw-rw-rw-   0        0        0      125 2024-01-20 11:37:04.000000 faknow-0.0.4/faknow/properties/m3fend.yaml
+-rw-rw-rw-   0        0        0      108 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/properties/mcan.yaml
+-rw-rw-rw-   0        0        0       96 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/properties/mdfend.yaml
+-rw-rw-rw-   0        0        0      309 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/properties/mfan.yaml
+-rw-rw-rw-   0        0        0       73 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/properties/nep.yaml
+-rw-rw-rw-   0        0        0       90 2023-12-06 10:25:53.000000 faknow-0.0.4/faknow/properties/safe.yaml
+-rw-rw-rw-   0        0        0      170 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/properties/spotfake.yaml
+-rw-rw-rw-   0        0        0      391 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/properties/textcnn.yaml
+-rw-rw-rw-   0        0        0       62 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/properties/upfd.yaml
+drwxrwxrwx   0        0        0        0 2024-05-18 09:16:30.508212 faknow-0.0.4/faknow/run/
+-rw-rw-rw-   0        0        0      128 2024-01-21 11:00:27.000000 faknow-0.0.4/faknow/run/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:16:30.555421 faknow-0.0.4/faknow/run/content_based/
+-rw-rw-rw-   0        0        0      331 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/run/content_based/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:16:30.634762 faknow-0.0.4/faknow/run/content_based/multimodal/
+-rw-rw-rw-   0        0        0      753 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/run/content_based/multimodal/__init__.py
+-rw-rw-rw-   0        0        0     3139 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/run/content_based/multimodal/run_cafe.py
+-rw-rw-rw-   0        0        0     7647 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/run/content_based/multimodal/run_eann.py
+-rw-rw-rw-   0        0        0     4716 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/run/content_based/multimodal/run_hmcan.py
+-rw-rw-rw-   0        0        0    11913 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/run/content_based/multimodal/run_mcan.py
+-rw-rw-rw-   0        0        0     7840 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/run/content_based/multimodal/run_mfan.py
+-rw-rw-rw-   0        0        0     3597 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/run/content_based/multimodal/run_safe.py
+-rw-rw-rw-   0        0        0     6490 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/run/content_based/multimodal/run_spotfake.py
+-rw-rw-rw-   0        0        0     5307 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/run/content_based/run_endef.py
+-rw-rw-rw-   0        0        0     7932 2024-01-20 11:38:10.000000 faknow-0.0.4/faknow/run/content_based/run_m3fend.py
+-rw-rw-rw-   0        0        0     3617 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/run/content_based/run_mdfend.py
+-rw-rw-rw-   0        0        0     6648 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/run/content_based/run_textcnn.py
+-rw-rw-rw-   0        0        0      655 2024-05-18 08:38:08.000000 faknow-0.0.4/faknow/run/run.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:16:30.731691 faknow-0.0.4/faknow/run/social_context/
+-rw-rw-rw-   0        0        0      397 2024-01-21 10:59:22.000000 faknow-0.0.4/faknow/run/social_context/__init__.py
+-rw-rw-rw-   0        0        0     4782 2024-01-20 11:37:04.000000 faknow-0.0.4/faknow/run/social_context/run_bigcn.py
+-rw-rw-rw-   0        0        0     3055 2024-01-17 12:51:18.000000 faknow-0.0.4/faknow/run/social_context/run_dudef.py
+-rw-rw-rw-   0        0        0     5028 2023-12-16 14:07:05.000000 faknow-0.0.4/faknow/run/social_context/run_ebgcn.py
+-rw-rw-rw-   0        0        0     3234 2023-12-16 14:07:06.000000 faknow-0.0.4/faknow/run/social_context/run_eddfn.py
+-rw-rw-rw-   0        0        0     4194 2024-01-20 11:37:04.000000 faknow-0.0.4/faknow/run/social_context/run_fang.py
+-rw-rw-rw-   0        0        0     4210 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/run/social_context/run_gcnfn.py
+-rw-rw-rw-   0        0        0     4688 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/run/social_context/run_gnncl.py
+-rw-rw-rw-   0        0        0     5272 2023-12-16 14:07:06.000000 faknow-0.0.4/faknow/run/social_context/run_trustrd.py
+-rw-rw-rw-   0        0        0     4756 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/run/social_context/run_upfd.py
+-rw-rw-rw-   0        0        0     4151 2024-01-10 12:38:33.000000 faknow-0.0.4/faknow/run/test.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:16:30.798262 faknow-0.0.4/faknow/train/
+-rw-rw-rw-   0        0        0      111 2023-05-04 11:51:26.000000 faknow-0.0.4/faknow/train/__init__.py
+-rw-rw-rw-   0        0        0     1057 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/train/base_gnn_trainer.py
+-rw-rw-rw-   0        0        0     3487 2023-12-16 14:07:06.000000 faknow-0.0.4/faknow/train/cafe_trainer.py
+-rw-rw-rw-   0        0        0     1115 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/train/dense_gnn_trainer.py
+-rw-rw-rw-   0        0        0     1553 2023-11-09 08:13:41.000000 faknow-0.0.4/faknow/train/pgd_trainer.py
+-rw-rw-rw-   0        0        0    20444 2024-01-20 11:37:04.000000 faknow-0.0.4/faknow/train/trainer.py
+-rw-rw-rw-   0        0        0     9463 2023-11-09 08:13:42.000000 faknow-0.0.4/faknow/train/trainer_gpu.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:16:30.833754 faknow-0.0.4/faknow/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:51:26.000000 faknow-0.0.4/faknow/utils/__init__.py
+-rw-rw-rw-   0        0        0     3093 2023-11-09 08:13:42.000000 faknow-0.0.4/faknow/utils/pgd.py
+-rw-rw-rw-   0        0        0     4602 2024-01-20 11:41:05.000000 faknow-0.0.4/faknow/utils/util.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:16:29.822163 faknow-0.0.4/faknow.egg-info/
+-rw-rw-rw-   0        0        0    16180 2024-05-18 09:16:28.000000 faknow-0.0.4/faknow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3868 2024-05-18 09:16:29.000000 faknow-0.0.4/faknow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 09:16:28.000000 faknow-0.0.4/faknow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-06 07:29:15.000000 faknow-0.0.4/faknow.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      185 2024-05-18 09:16:28.000000 faknow-0.0.4/faknow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-18 09:16:28.000000 faknow-0.0.4/faknow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 09:16:30.881371 faknow-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1541 2024-05-18 08:38:08.000000 faknow-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:16:30.874281 faknow-0.0.4/test/
+-rw-rw-rw-   0        0        0      330 2023-11-29 06:12:09.000000 faknow-0.0.4/test/test.py
```

### Comparing `faknow-0.0.3/LICENSE` & `faknow-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/PKG-INFO` & `faknow-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,34 @@
 Metadata-Version: 2.1
 Name: faknow
-Version: 0.0.3
+Version: 0.0.4
 Summary: A unified library for fake news detection.
 Home-page: https://github.com/NPURG/FaKnow
 Author: NPURG
 Author-email: faknow@outlook.com
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: transformers>=4.26.1
-Requires-Dist: numpy>=1.23.4
-Requires-Dist: pandas>=1.5.2
-Requires-Dist: scikit_learn>=1.1.3
-Requires-Dist: tensorboard>=2.10.0
-Requires-Dist: tqdm>=4.64.1
-Requires-Dist: jieba>=0.42.1
-Requires-Dist: gensim>=4.2.0
-Requires-Dist: pillow>=9.3.0
-Requires-Dist: nltk>=3.7
-Requires-Dist: sphinx-markdown-tables>=0.0.17
 
 # FaKnow
 
 <p align="center">
     <a href="https://npurg.github.io/FaKnowDoc/">
         <img alt="doc" src="https://img.shields.io/badge/doc-sphinx-blue.svg">
     </a>
     <a href="https://github.com/NPURG/FaKnow/blob/master/LICENSE">
         <img alt="license" src="https://img.shields.io/badge/license-MIT-green.svg">
     </a>
     <a href="https://github.com/NPURG/FaKnow/releases">
-        <img alt="release" src="https://img.shields.io/badge/relase-v0.0.3-yellow.svg">
+        <img alt="release" src="https://img.shields.io/badge/release-v0.0.3-yellow.svg">
     </a>
     <!-- <a href="https://github.com/huggingface/transformers/releases">
-        <img alt="doi" src="https://img.shields.io/badge/doi-xxx-orange.svg"> -->
-    </a>
+        <img alt="doi" src="https://img.shields.io/badge/doi-xxx-orange.svg">
+    </a> -->
 </p>
 
 
 **FaKnow** (**Fa**ke **Know**), a unified *Fake News Detection* algorithms library based on PyTorch, is designed for
 reproducing and developing fake news detection algorithms. It includes **22 models**(see at **Integrated Models**), covering **2 categories**:
 
 - content based
```

#### html2text {}

```diff
@@ -1,16 +1,12 @@
-Metadata-Version: 2.1 Name: faknow Version: 0.0.3 Summary: A unified library
+Metadata-Version: 2.1 Name: faknow Version: 0.0.4 Summary: A unified library
 for fake news detection. Home-page: https://github.com/NPURG/FaKnow Author:
 NPURG Author-email: faknow@outlook.com Classifier: License :: OSI Approved ::
 MIT License Requires-Python: >=3.8.0 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: transformers>=4.26.1 Requires-Dist:
-numpy>=1.23.4 Requires-Dist: pandas>=1.5.2 Requires-Dist: scikit_learn>=1.1.3
-Requires-Dist: tensorboard>=2.10.0 Requires-Dist: tqdm>=4.64.1 Requires-Dist:
-jieba>=0.42.1 Requires-Dist: gensim>=4.2.0 Requires-Dist: pillow>=9.3.0
-Requires-Dist: nltk>=3.7 Requires-Dist: sphinx-markdown-tables>=0.0.17 # FaKnow
+License-File: LICENSE # FaKnow
                             _[_d_o_c_]_[_l_i_c_e_n_s_e_]_[_r_e_l_e_a_s_e_]
 **FaKnow** (**Fa**ke **Know**), a unified *Fake News Detection* algorithms
 library based on PyTorch, is designed for reproducing and developing fake news
 detection algorithms. It includes **22 models**(see at **Integrated Models**),
 covering **2 categories**: - content based - social context ## Features -
 **Unified Framework**: provide a unified interface to cover a series of
 algorithm development processes, including data processing, model developing,
```

### Comparing `faknow-0.0.3/README.md` & `faknow-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,19 @@
     <a href="https://npurg.github.io/FaKnowDoc/">
         <img alt="doc" src="https://img.shields.io/badge/doc-sphinx-blue.svg">
     </a>
     <a href="https://github.com/NPURG/FaKnow/blob/master/LICENSE">
         <img alt="license" src="https://img.shields.io/badge/license-MIT-green.svg">
     </a>
     <a href="https://github.com/NPURG/FaKnow/releases">
-        <img alt="release" src="https://img.shields.io/badge/relase-v0.0.3-yellow.svg">
+        <img alt="release" src="https://img.shields.io/badge/release-v0.0.3-yellow.svg">
     </a>
     <!-- <a href="https://github.com/huggingface/transformers/releases">
-        <img alt="doi" src="https://img.shields.io/badge/doi-xxx-orange.svg"> -->
-    </a>
+        <img alt="doi" src="https://img.shields.io/badge/doi-xxx-orange.svg">
+    </a> -->
 </p>
 
 
 **FaKnow** (**Fa**ke **Know**), a unified *Fake News Detection* algorithms library based on PyTorch, is designed for
 reproducing and developing fake news detection algorithms. It includes **22 models**(see at **Integrated Models**), covering **2 categories**:
 
 - content based
```

### Comparing `faknow-0.0.3/faknow/data/dataset/bigcn_dataset.py` & `faknow-0.0.4/faknow/data/dataset/bigcn_dataset.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/data/dataset/cafe_dataset.py` & `faknow-0.0.4/faknow/data/dataset/cafe_dataset.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/data/dataset/dudef_dataset.py` & `faknow-0.0.4/faknow/data/dataset/dudef_dataset.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/data/dataset/fang_dataset.py` & `faknow-0.0.4/faknow/data/dataset/fang_dataset.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/data/dataset/m3fend_dataset.py` & `faknow-0.0.4/faknow/data/dataset/m3fend_dataset.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/data/dataset/multi_modal.py` & `faknow-0.0.4/faknow/data/dataset/multi_modal.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/data/dataset/safe_dataset.py` & `faknow-0.0.4/faknow/data/dataset/safe_dataset.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/data/dataset/spotfake_dataset.py` & `faknow-0.0.4/faknow/data/dataset/spotfake_dataset.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/data/dataset/text.py` & `faknow-0.0.4/faknow/data/dataset/text.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/data/dataset/trustrd_dataset.py` & `faknow-0.0.4/faknow/data/dataset/trustrd_dataset.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/data/process/process.py` & `faknow-0.0.4/faknow/data/process/process.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/data/process/text_process.py` & `faknow-0.0.4/faknow/data/process/text_process.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/evaluate/evaluator.py` & `faknow-0.0.4/faknow/evaluate/evaluator.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/evaluate/metrics.py` & `faknow-0.0.4/faknow/evaluate/metrics.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/content_based/endef.py` & `faknow-0.0.4/faknow/model/content_based/endef.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/content_based/m3fend.py` & `faknow-0.0.4/faknow/model/content_based/m3fend.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/content_based/mdfend.py` & `faknow-0.0.4/faknow/model/content_based/mdfend.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/content_based/multi_modal/cafe.py` & `faknow-0.0.4/faknow/model/content_based/multi_modal/cafe.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,18 +55,17 @@
         corre_final = weight_corre * correlation
         final_corre = torch.cat([text_final, img_final, corre_final], 1)
         out = self.classifier(final_corre)
         return out
 
     def calculate_loss(self, data: Dict[str, Tensor]) -> Tensor:
         """
-        process raw data using similarity_module
         calculate loss via CrossEntropyLoss
         Args:
-            data (Tuple[Tensor]): batch data tuple,including text, image and label
+            data (Dict[str, Tensor]): batch data with text, image, label
         Returns:
             torch.Tensor: loss
         """
         text = data['text']
         image = data['image']
         label = data['label']
         pre_detection = self.forward(text, image)
@@ -163,15 +162,15 @@
         text_shared = self.shared_text_linear(text_encoding)
         image_shared = self.shared_image(image)
         return text_shared, image_shared
 
 
 class _SimilarityModule(AbstractModel):
     """
-    Cross modal aligment and calculate cosine embedding loss
+    Cross modal aligment via contrastive learning
     """
     def __init__(self, shared_dim=128, sim_dim=64):
         """
         Args:
             shared_dim (int): dimension of aligner node feature
             sim_dim (int): dimension of similarity node feature
         """
@@ -207,24 +206,24 @@
         text_encoding, image_encoding = self.encoding(text, image)
         text_aligned = self.text_aligner(text_encoding)
         image_aligned = self.image_aligner(image_encoding)
         sim_feature = torch.cat([text_aligned, image_aligned], 1)
         pred_similarity = self.sim_classifier(sim_feature)
         return text_aligned, image_aligned, pred_similarity
 
-    def calculate_loss(self, data: Tuple[Tensor]) -> Tensor:
+    def calculate_loss(self, data: Dict[str, Tensor]) -> Tensor:
         """
         calculate loss via CosineEmbeddingLoss
         Args:
-            data Tuple[Tensor]: batch data, including text, image, label
+            data (Dict[str, Tensor]): batch data with text, image, label
         Returns:
             torch.Tensor: CosineEmbeddingLoss
         """
         fixed_text, matched_image, unmatched_image = self.sample_data_pairs(
-            data)
+            **data)
 
         text_aligned_match, image_aligned_match, similarity_match = self.forward(
             fixed_text, matched_image)
         text_aligned_unmatch, image_aligned_unmatch, similarity_unmatch = self.forward(
             fixed_text, unmatched_image)
 
         similarity_label = torch.cat([
@@ -239,31 +238,35 @@
         image_aligned = torch.cat([image_aligned_match, image_aligned_unmatch],
                                   dim=0)
         loss_similarity = self.loss_func_similarity(text_aligned,
                                                     image_aligned,
                                                     similarity_label)
         return loss_similarity
 
-    def sample_data_pairs(self, data: Dict[str, Tensor]) -> Tuple[Tensor]:
+    def sample_data_pairs(self,
+                          text,
+                          image,
+                          label,
+                          true_label=1) -> Tuple[Tensor]:
         """
         randomly sample positive text-image pairs and negative text-image pairs
 
         Args:
-            data (Tuple[Tensor, any]): batch data, including text, image, label
+            text (Tensor): raw text data, shape=(batch_size, 30, 200)
+            image (Tensor): raw image data, shape=(batch_size, 512)
+            label (Tensor): raw label data, shape=(batch_size,)
+            true_label (int): label of positive data, default=1
         Returns:
             fixed_text (Tensor): processed text data, shape=(sample_num, 30, 200)
             matched_image (Tensor): processed match image data, shape=(sample_num ,512)
             unmatched_image (Tensor): processed unmatch image data, shape=(sample_num, 512)
         """
-        text = data['text']
-        image = data['image']
-        label = data['label']
 
         # index of batch news data whose label=1
-        index = [i for i, l in enumerate(label) if l == 1]
+        index = [i for i, l in enumerate(label) if l == true_label]
         sample_text = text[index]
         sample_image = image[index]
         fixed_text = copy.deepcopy(sample_text)
         matched_image = copy.deepcopy(sample_image)
         unmatched_image = copy.deepcopy(sample_image).roll(shifts=3, dims=0)
         return fixed_text, matched_image, unmatched_image
 
@@ -306,15 +309,15 @@
         mu, sigma = params[:, :self.z_dim], params[:, self.z_dim:]
         sigma = softplus(sigma) + 1e-7
         return Independent(Normal(loc=mu, scale=sigma), 1)
 
 
 class _AmbiguityModule(nn.Module):
     """
-    Cross modal ambiguity learning moddule,
+    Cross modal ambiguity learning module,
     capture the ambiguity between text and image via KL divergence
     """
     def __init__(self):
         super(_AmbiguityModule, self).__init__()
         self.encoder_text = _GaussianSample()
         self.encoder_image = _GaussianSample()
 
@@ -380,17 +383,16 @@
         Args:
             corre_out_dim (int): output dim of correlation, default=64
         """
         super(_CrossModalModule, self).__init__()
         self.softmax = nn.Softmax(-1)
         self.corre_dim = 64
         self.pooling = nn.AdaptiveMaxPool1d(1)
-        self.fc = nn.Sequential(
-            nn.Linear(self.corre_dim, corre_out_dim),
-            nn.BatchNorm1d(corre_out_dim), nn.ReLU())
+        self.fc = nn.Sequential(nn.Linear(self.corre_dim, corre_out_dim),
+                                nn.BatchNorm1d(corre_out_dim), nn.ReLU())
 
     def forward(self, text: Tensor, image: Tensor):
         """
         Args:
             text (Tensor): batch text data, shape=(batch_size, 64)
             image (Tensor): batch image data, shape=(batch_size, 64)
         Returns:
```

### Comparing `faknow-0.0.3/faknow/model/content_based/multi_modal/eann.py` & `faknow-0.0.4/faknow/model/content_based/multi_modal/eann.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/content_based/multi_modal/hmcan.py` & `faknow-0.0.4/faknow/model/content_based/multi_modal/hmcan.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/content_based/multi_modal/mcan.py` & `faknow-0.0.4/faknow/model/content_based/multi_modal/mcan.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/content_based/multi_modal/mfan.py` & `faknow-0.0.4/faknow/model/content_based/multi_modal/mfan.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/content_based/multi_modal/safe.py` & `faknow-0.0.4/faknow/model/content_based/multi_modal/safe.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/content_based/multi_modal/spotfake.py` & `faknow-0.0.4/faknow/model/content_based/multi_modal/spotfake.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/content_based/textcnn.py` & `faknow-0.0.4/faknow/model/content_based/textcnn.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/layers/dct.py` & `faknow-0.0.4/faknow/model/layers/dct.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/layers/layer.py` & `faknow-0.0.4/faknow/model/layers/layer.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/layers/layers_m3fend.py` & `faknow-0.0.4/faknow/model/layers/layers_m3fend.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/layers/transformer.py` & `faknow-0.0.4/faknow/model/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/model.py` & `faknow-0.0.4/faknow/model/model.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/social_context/base_gnn.py` & `faknow-0.0.4/faknow/model/social_context/base_gnn.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/social_context/bigcn.py` & `faknow-0.0.4/faknow/model/social_context/bigcn.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/social_context/dudef.py` & `faknow-0.0.4/faknow/model/social_context/dudef.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/social_context/ebgcn.py` & `faknow-0.0.4/faknow/model/social_context/ebgcn.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/social_context/eddfn.py` & `faknow-0.0.4/faknow/model/social_context/eddfn.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/social_context/fang.py` & `faknow-0.0.4/faknow/model/social_context/fang.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/social_context/gcnfn.py` & `faknow-0.0.4/faknow/model/social_context/gcnfn.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/social_context/gnncl.py` & `faknow-0.0.4/faknow/model/social_context/gnncl.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/social_context/trustrd.py` & `faknow-0.0.4/faknow/model/social_context/trustrd.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/model/social_context/upfd.py` & `faknow-0.0.4/faknow/model/social_context/upfd.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/content_based/multimodal/__init__.py` & `faknow-0.0.4/faknow/run/content_based/multimodal/__init__.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/content_based/multimodal/run_cafe.py` & `faknow-0.0.4/faknow/run/content_based/multimodal/run_cafe.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/content_based/multimodal/run_eann.py` & `faknow-0.0.4/faknow/run/content_based/multimodal/run_eann.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/content_based/multimodal/run_hmcan.py` & `faknow-0.0.4/faknow/run/content_based/multimodal/run_hmcan.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/content_based/multimodal/run_mcan.py` & `faknow-0.0.4/faknow/run/content_based/multimodal/run_mcan.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/content_based/multimodal/run_mfan.py` & `faknow-0.0.4/faknow/run/content_based/multimodal/run_mfan.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/content_based/multimodal/run_safe.py` & `faknow-0.0.4/faknow/run/content_based/multimodal/run_safe.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/content_based/multimodal/run_spotfake.py` & `faknow-0.0.4/faknow/run/content_based/multimodal/run_spotfake.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/content_based/run_endef.py` & `faknow-0.0.4/faknow/run/content_based/run_endef.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/content_based/run_m3fend.py` & `faknow-0.0.4/faknow/run/content_based/run_m3fend.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/content_based/run_mdfend.py` & `faknow-0.0.4/faknow/run/content_based/run_mdfend.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/content_based/run_textcnn.py` & `faknow-0.0.4/faknow/run/content_based/run_textcnn.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/run.py` & `faknow-0.0.4/faknow/run/run.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from faknow.run.content_based import *
 from faknow.run.social_context import *
-from faknow.run.knowledge_aware import *
 
 __all__ = ['run', 'run_from_yaml']
 
 
 def run(model: str, **kwargs):
     """
     run the model with the given keyword arguments
```

### Comparing `faknow-0.0.3/faknow/run/social_context/run_bigcn.py` & `faknow-0.0.4/faknow/run/social_context/run_bigcn.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/social_context/run_dudef.py` & `faknow-0.0.4/faknow/run/social_context/run_dudef.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/social_context/run_ebgcn.py` & `faknow-0.0.4/faknow/run/social_context/run_ebgcn.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/social_context/run_eddfn.py` & `faknow-0.0.4/faknow/run/social_context/run_eddfn.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/social_context/run_fang.py` & `faknow-0.0.4/faknow/run/social_context/run_fang.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/social_context/run_gcnfn.py` & `faknow-0.0.4/faknow/run/social_context/run_gcnfn.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/social_context/run_gnncl.py` & `faknow-0.0.4/faknow/run/social_context/run_gnncl.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/social_context/run_trustrd.py` & `faknow-0.0.4/faknow/run/social_context/run_trustrd.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/run/social_context/run_upfd.py` & `faknow-0.0.4/faknow/run/social_context/run_upfd.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/train/base_gnn_trainer.py` & `faknow-0.0.4/faknow/train/base_gnn_trainer.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/train/cafe_trainer.py` & `faknow-0.0.4/faknow/train/cafe_trainer.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/train/dense_gnn_trainer.py` & `faknow-0.0.4/faknow/train/dense_gnn_trainer.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/train/pgd_trainer.py` & `faknow-0.0.4/faknow/train/pgd_trainer.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/train/trainer.py` & `faknow-0.0.4/faknow/train/trainer.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/train/trainer_gpu.py` & `faknow-0.0.4/faknow/train/trainer_gpu.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/utils/pgd.py` & `faknow-0.0.4/faknow/utils/pgd.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow/utils/util.py` & `faknow-0.0.4/faknow/utils/util.py`

 * *Files identical despite different names*

### Comparing `faknow-0.0.3/faknow.egg-info/PKG-INFO` & `faknow-0.0.4/faknow.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,34 @@
 Metadata-Version: 2.1
 Name: faknow
-Version: 0.0.3
+Version: 0.0.4
 Summary: A unified library for fake news detection.
 Home-page: https://github.com/NPURG/FaKnow
 Author: NPURG
 Author-email: faknow@outlook.com
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: transformers>=4.26.1
-Requires-Dist: numpy>=1.23.4
-Requires-Dist: pandas>=1.5.2
-Requires-Dist: scikit_learn>=1.1.3
-Requires-Dist: tensorboard>=2.10.0
-Requires-Dist: tqdm>=4.64.1
-Requires-Dist: jieba>=0.42.1
-Requires-Dist: gensim>=4.2.0
-Requires-Dist: pillow>=9.3.0
-Requires-Dist: nltk>=3.7
-Requires-Dist: sphinx-markdown-tables>=0.0.17
 
 # FaKnow
 
 <p align="center">
     <a href="https://npurg.github.io/FaKnowDoc/">
         <img alt="doc" src="https://img.shields.io/badge/doc-sphinx-blue.svg">
     </a>
     <a href="https://github.com/NPURG/FaKnow/blob/master/LICENSE">
         <img alt="license" src="https://img.shields.io/badge/license-MIT-green.svg">
     </a>
     <a href="https://github.com/NPURG/FaKnow/releases">
-        <img alt="release" src="https://img.shields.io/badge/relase-v0.0.3-yellow.svg">
+        <img alt="release" src="https://img.shields.io/badge/release-v0.0.3-yellow.svg">
     </a>
     <!-- <a href="https://github.com/huggingface/transformers/releases">
-        <img alt="doi" src="https://img.shields.io/badge/doi-xxx-orange.svg"> -->
-    </a>
+        <img alt="doi" src="https://img.shields.io/badge/doi-xxx-orange.svg">
+    </a> -->
 </p>
 
 
 **FaKnow** (**Fa**ke **Know**), a unified *Fake News Detection* algorithms library based on PyTorch, is designed for
 reproducing and developing fake news detection algorithms. It includes **22 models**(see at **Integrated Models**), covering **2 categories**:
 
 - content based
```

#### html2text {}

```diff
@@ -1,16 +1,12 @@
-Metadata-Version: 2.1 Name: faknow Version: 0.0.3 Summary: A unified library
+Metadata-Version: 2.1 Name: faknow Version: 0.0.4 Summary: A unified library
 for fake news detection. Home-page: https://github.com/NPURG/FaKnow Author:
 NPURG Author-email: faknow@outlook.com Classifier: License :: OSI Approved ::
 MIT License Requires-Python: >=3.8.0 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: transformers>=4.26.1 Requires-Dist:
-numpy>=1.23.4 Requires-Dist: pandas>=1.5.2 Requires-Dist: scikit_learn>=1.1.3
-Requires-Dist: tensorboard>=2.10.0 Requires-Dist: tqdm>=4.64.1 Requires-Dist:
-jieba>=0.42.1 Requires-Dist: gensim>=4.2.0 Requires-Dist: pillow>=9.3.0
-Requires-Dist: nltk>=3.7 Requires-Dist: sphinx-markdown-tables>=0.0.17 # FaKnow
+License-File: LICENSE # FaKnow
                             _[_d_o_c_]_[_l_i_c_e_n_s_e_]_[_r_e_l_e_a_s_e_]
 **FaKnow** (**Fa**ke **Know**), a unified *Fake News Detection* algorithms
 library based on PyTorch, is designed for reproducing and developing fake news
 detection algorithms. It includes **22 models**(see at **Integrated Models**),
 covering **2 categories**: - content based - social context ## Features -
 **Unified Framework**: provide a unified interface to cover a series of
 algorithm development processes, including data processing, model developing,
```

### Comparing `faknow-0.0.3/faknow.egg-info/SOURCES.txt` & `faknow-0.0.4/faknow.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 faknow/properties/nep.yaml
 faknow/properties/safe.yaml
 faknow/properties/spotfake.yaml
 faknow/properties/textcnn.yaml
 faknow/properties/upfd.yaml
 faknow/run/__init__.py
 faknow/run/run.py
+faknow/run/test.py
 faknow/run/content_based/__init__.py
 faknow/run/content_based/run_endef.py
 faknow/run/content_based/run_m3fend.py
 faknow/run/content_based/run_mdfend.py
 faknow/run/content_based/run_textcnn.py
 faknow/run/content_based/multimodal/__init__.py
 faknow/run/content_based/multimodal/run_cafe.py
@@ -106,8 +107,9 @@
 faknow/train/cafe_trainer.py
 faknow/train/dense_gnn_trainer.py
 faknow/train/pgd_trainer.py
 faknow/train/trainer.py
 faknow/train/trainer_gpu.py
 faknow/utils/__init__.py
 faknow/utils/pgd.py
-faknow/utils/util.py
+faknow/utils/util.py
+test/test.py
```

### Comparing `faknow-0.0.3/setup.py` & `faknow-0.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 if on_rtd:
     install_requires.extend(setup_requires)
 
 filepath = os.path.join(os.path.dirname(__file__), "README.md")
 
 setup(
     name="faknow",
-    version="0.0.3",  # edit faknow/__init__.py in response
+    version="0.0.4",  # edit faknow/__init__.py in response
     description="A unified library for fake news detection.",
     long_description=open(filepath, encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/NPURG/FaKnow",
     author="NPURG",
     author_email="faknow@outlook.com",
     python_requires=">=3.8.0",
```

