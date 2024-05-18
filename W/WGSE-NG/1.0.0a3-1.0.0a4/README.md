# Comparing `tmp/wgse_ng-1.0.0a3.tar.gz` & `tmp/wgse_ng-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wgse_ng-1.0.0a3.tar", last modified: Fri May 17 20:10:04 2024, max compression
+gzip compressed data, was "wgse_ng-1.0.0a4.tar", last modified: Sat May 18 06:28:10 2024, max compression
```

## Comparing `wgse_ng-1.0.0a3.tar` & `wgse_ng-1.0.0a4.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.590823 wgse_ng-1.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-17 20:10:04.590823 wgse_ng-1.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.590823 wgse_ng-1.0.0a3/WGSE_NG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-17 20:10:04.000000 wgse_ng-1.0.0a3/WGSE_NG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-17 20:10:04.000000 wgse_ng-1.0.0a3/WGSE_NG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 20:10:04.000000 wgse_ng-1.0.0a3/WGSE_NG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-17 20:10:04.000000 wgse_ng-1.0.0a3/WGSE_NG.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-17 20:10:04.000000 wgse_ng-1.0.0a3/WGSE_NG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-17 20:10:04.000000 wgse_ng-1.0.0a3/WGSE_NG.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 20:10:04.590823 wgse_ng-1.0.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.558822 wgse_ng-1.0.0a3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/test/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/test/test_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/test/test_fasta_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/test/test_microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/test/test_raw_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/test/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/test/test_unknown_bases_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.558822 wgse_ng-1.0.0a3/wgse/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/VERSION.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.558822 wgse_ng-1.0.0a3/wgse/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/adapters/alignment_map_file_info_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/adapters/alignment_stats_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/adapters/header_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/adapters/index_stats_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/adapters/reference_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.558822 wgse_ng-1.0.0a3/wgse/alignment_map/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/alignment_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/alignment_map/alignment_map_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/alignment_map/alignment_map_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/alignment_map/alignment_map_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/alignment_map/alignment_stats_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/alignment_map/depth_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/alignment_map/index_stats_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.562822 wgse_ng-1.0.0a3/wgse/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/alignment_map_file_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/alignment_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/chromosome_name_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/file_type.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/gender.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/genome.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/mitochondrial_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/mitochondrial_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/mitochondrial_name_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/read_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/sequence_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/tabular_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.562822 wgse_ng-1.0.0a3/wgse/fasta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/fasta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/fasta/fasta_letter_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/fasta/fasta_stats_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/fasta/letter_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/fasta/letter_run_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/fasta/letter_run_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/fasta/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.566823 wgse_ng-1.0.0a3/wgse/fastq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/fastq/fastq_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.566823 wgse_ng-1.0.0a3/wgse/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/gui/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    12048 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/gui/microarray_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/gui/table_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/gui/ui_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/gui/ui_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.570823 wgse_ng-1.0.0a3/wgse/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.582823 wgse_ng-1.0.0a3/wgse/metadata/bed_templates/
--rw-r--r--   0 runner    (1001) docker     (127)  4482835 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/metadata/bed_templates/19_wes.csv
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/metadata/bed_templates/19_y_mt.csv
--rw-r--r--   0 runner    (1001) docker     (127)  4687904 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/metadata/bed_templates/38_wes.csv
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/metadata/bed_templates/38_y_mt.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/metadata/bed_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/metadata/builds.json
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/metadata/mtdna.json
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/metadata/ploidy.txt
--rw-r--r--   0 runner    (1001) docker     (127)  4213156 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/metadata/references.json
--rw-r--r--   0 runner    (1001) docker     (127)    17094 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/metadata/references_template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.586823 wgse_ng-1.0.0a3/wgse/metadata/report_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/metadata/report_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/metadata/report_templates/table_macro.html
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/metadata/report_templates/table_simple.html
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/metadata/report_templates/table_tab.html
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/metadata/sequencers.json
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/metadata/sources.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.586823 wgse_ng-1.0.0a3/wgse/microarray/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/microarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/microarray/microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/microarray/microarray_line_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/microarray/raw_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.586823 wgse_ng-1.0.0a3/wgse/mtDNA/
--rw-r--r--   0 runner    (1001) docker     (127)    16961 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/mtDNA/CRS.fasta
--rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/mtDNA/RSRS.fasta
--rw-r--r--   0 runner    (1001) docker     (127)    16863 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/mtDNA/Yoruba.fasta
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/mtDNA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/mtDNA/rCRS.fasta
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.586823 wgse_ng-1.0.0a3/wgse/reference_genome/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/reference_genome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/reference_genome/bgzip_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/reference_genome/decompressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/reference_genome/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/reference_genome/genome_metadata_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8456 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/reference_genome/repository_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.586823 wgse_ng-1.0.0a3/wgse/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/renderers/csv_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/renderers/html_aligned_file_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/renderers/html_simple_table_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.590823 wgse_ng-1.0.0a3/wgse/utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/check_prerequisites.py
--rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/external.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/file_type_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/mt_dna.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/sequence_orderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/sequencers.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/unit_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/variant_caller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:28:10.171001 wgse_ng-1.0.0a4/
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-18 06:28:10.171001 wgse_ng-1.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:28:10.171001 wgse_ng-1.0.0a4/WGSE_NG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-18 06:28:10.000000 wgse_ng-1.0.0a4/WGSE_NG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-18 06:28:10.000000 wgse_ng-1.0.0a4/WGSE_NG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 06:28:10.000000 wgse_ng-1.0.0a4/WGSE_NG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-18 06:28:10.000000 wgse_ng-1.0.0a4/WGSE_NG.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-18 06:28:10.000000 wgse_ng-1.0.0a4/WGSE_NG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 06:28:10.000000 wgse_ng-1.0.0a4/WGSE_NG.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 06:28:10.171001 wgse_ng-1.0.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:28:10.139001 wgse_ng-1.0.0a4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/test/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/test/test_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/test/test_fasta_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/test/test_microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/test/test_raw_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/test/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/test/test_unknown_bases_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:28:10.139001 wgse_ng-1.0.0a4/wgse/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:28:10.139001 wgse_ng-1.0.0a4/wgse/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/adapters/alignment_map_file_info_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/adapters/alignment_stats_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/adapters/header_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/adapters/index_stats_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/adapters/reference_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:28:10.139001 wgse_ng-1.0.0a4/wgse/alignment_map/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/alignment_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/alignment_map/alignment_map_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/alignment_map/alignment_map_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/alignment_map/alignment_map_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/alignment_map/alignment_stats_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/alignment_map/depth_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/alignment_map/index_stats_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:28:10.143001 wgse_ng-1.0.0a4/wgse/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/data/alignment_map_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/data/alignment_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/data/chromosome_name_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/data/file_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/data/gender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/data/genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/data/microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/data/mitochondrial_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/data/mitochondrial_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/data/mitochondrial_name_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/data/read_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/data/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/data/sequence_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/data/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/data/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/data/tabular_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:28:10.143001 wgse_ng-1.0.0a4/wgse/fasta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/fasta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/fasta/fasta_letter_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/fasta/fasta_stats_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/fasta/letter_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/fasta/letter_run_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/fasta/letter_run_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/fasta/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:28:10.143001 wgse_ng-1.0.0a4/wgse/fastq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/fastq/fastq_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:28:10.147001 wgse_ng-1.0.0a4/wgse/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/gui/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12048 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/gui/microarray_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/gui/table_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/gui/ui_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/gui/ui_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:28:10.151001 wgse_ng-1.0.0a4/wgse/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:28:10.163001 wgse_ng-1.0.0a4/wgse/metadata/bed_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)  4482835 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/metadata/bed_templates/19_wes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/metadata/bed_templates/19_y_mt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  4687904 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/metadata/bed_templates/38_wes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/metadata/bed_templates/38_y_mt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/metadata/bed_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/metadata/builds.json
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/metadata/mtdna.json
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/metadata/ploidy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  4213156 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/metadata/references.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17094 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/metadata/references_template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:28:10.163001 wgse_ng-1.0.0a4/wgse/metadata/report_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/metadata/report_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/metadata/report_templates/table_macro.html
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/metadata/report_templates/table_simple.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/metadata/report_templates/table_tab.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/metadata/sequencers.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/metadata/sources.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:28:10.167001 wgse_ng-1.0.0a4/wgse/microarray/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/microarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/microarray/microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/microarray/microarray_line_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/microarray/raw_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:28:10.167001 wgse_ng-1.0.0a4/wgse/mtDNA/
+-rw-r--r--   0 runner    (1001) docker     (127)    16961 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/mtDNA/CRS.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/mtDNA/RSRS.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)    16863 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/mtDNA/Yoruba.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/mtDNA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/mtDNA/rCRS.fasta
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:28:10.167001 wgse_ng-1.0.0a4/wgse/reference_genome/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/reference_genome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/reference_genome/bgzip_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/reference_genome/decompressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/reference_genome/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/reference_genome/genome_metadata_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8456 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/reference_genome/repository_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:28:10.167001 wgse_ng-1.0.0a4/wgse/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/renderers/csv_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/renderers/html_aligned_file_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/renderers/html_simple_table_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 06:28:10.171001 wgse_ng-1.0.0a4/wgse/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/utility/check_prerequisites.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/utility/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/utility/file_type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/utility/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/utility/mt_dna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/utility/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/utility/sequence_orderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/utility/sequencers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/utility/unit_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/utility/updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-18 06:27:58.000000 wgse_ng-1.0.0a4/wgse/variant_caller.py
```

### Comparing `wgse_ng-1.0.0a3/PKG-INFO` & `wgse_ng-1.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WGSE-NG
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Whole Genome Sequencing data manipulation tool
 Home-page: https://github.com/WGSE-NG/WGSE-NG
 Author: Multiple
 Author-email: 
 Keywords: bioinformatics,genetics,wgs,microarray,science
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `wgse_ng-1.0.0a3/README.md` & `wgse_ng-1.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/WGSE_NG.egg-info/PKG-INFO` & `wgse_ng-1.0.0a4/WGSE_NG.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WGSE-NG
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Whole Genome Sequencing data manipulation tool
 Home-page: https://github.com/WGSE-NG/WGSE-NG
 Author: Multiple
 Author-email: 
 Keywords: bioinformatics,genetics,wgs,microarray,science
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `wgse_ng-1.0.0a3/WGSE_NG.egg-info/SOURCES.txt` & `wgse_ng-1.0.0a4/WGSE_NG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/setup.py` & `wgse_ng-1.0.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/test/test_buckets.py` & `wgse_ng-1.0.0a4/test/test_buckets.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/test/test_fasta.py` & `wgse_ng-1.0.0a4/test/test_fasta.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/test/test_fasta_dictionary.py` & `wgse_ng-1.0.0a4/test/test_fasta_dictionary.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/test/test_microarray_converter.py` & `wgse_ng-1.0.0a4/test/test_microarray_converter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/test/test_raw_file.py` & `wgse_ng-1.0.0a4/test/test_raw_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/test/test_sequence.py` & `wgse_ng-1.0.0a4/test/test_sequence.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/test/test_unknown_bases_stats.py` & `wgse_ng-1.0.0a4/test/test_unknown_bases_stats.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/__init__.py` & `wgse_ng-1.0.0a4/wgse/__init__.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/adapters/alignment_map_file_info_adapter.py` & `wgse_ng-1.0.0a4/wgse/adapters/alignment_map_file_info_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/adapters/alignment_stats_adapter.py` & `wgse_ng-1.0.0a4/wgse/adapters/alignment_stats_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/adapters/header_adapter.py` & `wgse_ng-1.0.0a4/wgse/adapters/header_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/adapters/index_stats_adapter.py` & `wgse_ng-1.0.0a4/wgse/adapters/index_stats_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/adapters/reference_adapter.py` & `wgse_ng-1.0.0a4/wgse/adapters/reference_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/alignment_map/alignment_map_file.py` & `wgse_ng-1.0.0a4/wgse/alignment_map/alignment_map_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/alignment_map/alignment_map_header.py` & `wgse_ng-1.0.0a4/wgse/alignment_map/alignment_map_header.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/alignment_map/alignment_map_row.py` & `wgse_ng-1.0.0a4/wgse/alignment_map/alignment_map_row.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/alignment_map/alignment_stats_calculator.py` & `wgse_ng-1.0.0a4/wgse/alignment_map/alignment_stats_calculator.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/alignment_map/depth_analyzer.py` & `wgse_ng-1.0.0a4/wgse/alignment_map/depth_analyzer.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/alignment_map/index_stats_calculator.py` & `wgse_ng-1.0.0a4/wgse/alignment_map/index_stats_calculator.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/configuration.py` & `wgse_ng-1.0.0a4/wgse/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
         metadata (Path): Root folder for metadata.
         mtdna (Path): Root folder for mtDNA files.
     """
 
     def __init__(self) -> None:
         self.genomes: Path = Path(WGSEDefaults.LOCAL_FOLDER, "genomes")
         self.temporary: Path = Path(WGSEDefaults.LOCAL_FOLDER, "temp")
+        self.log_path: Path = Path(WGSEDefaults.LOCAL_FOLDER,"logs")
         self.metadata: Path = Path(metadata.__file__).parent
         self.mtdna: Path = Path(mtDNA.__file__).parent
 
 
 class AlignmentStatsConfig:
     """Configuration for alignment stats calculation.
```

### Comparing `wgse_ng-1.0.0a3/wgse/data/alignment_map_file_info.py` & `wgse_ng-1.0.0a4/wgse/data/alignment_map_file_info.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/data/alignment_stats.py` & `wgse_ng-1.0.0a4/wgse/data/alignment_stats.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/data/genome.py` & `wgse_ng-1.0.0a4/wgse/data/genome.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/data/microarray_converter.py` & `wgse_ng-1.0.0a4/wgse/data/microarray_converter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/data/mitochondrial_model.py` & `wgse_ng-1.0.0a4/wgse/data/mitochondrial_model.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/data/sequence.py` & `wgse_ng-1.0.0a4/wgse/data/sequence.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/fasta/fasta_letter_counter.py` & `wgse_ng-1.0.0a4/wgse/fasta/fasta_letter_counter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/fasta/fasta_stats_files.py` & `wgse_ng-1.0.0a4/wgse/fasta/fasta_stats_files.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/fasta/letter_run_buckets.py` & `wgse_ng-1.0.0a4/wgse/fasta/letter_run_buckets.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/fasta/letter_run_collection.py` & `wgse_ng-1.0.0a4/wgse/fasta/letter_run_collection.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/fasta/reference.py` & `wgse_ng-1.0.0a4/wgse/fasta/reference.py`

 * *Files 10% similar despite different names*

```diff
@@ -89,31 +89,26 @@
 
         Returns:
             list[Genome]: list of matching genomes.
         """
         match_list = []
         for genome, matches in self._genome_map.items():
             matching = True
-            logger.debug(f"{genome!s}: matching {len(matches.keys())}/{len([x for x in matches.values()if x is not None])}")
             for genome_sequence, query_sequence in matches.items():
                 if query_sequence is None:
-                    logger.debug(f"Discarding genome {genome!s} because {genome_sequence.name} does not have a match.")
                     matching = False
                     break
                 if genome_sequence.name != query_sequence.name:
-                    logger.debug(f"Discarding genome {genome!s} because {genome_sequence.name} is different from {query_sequence.name}.")
                     matching = False
                     break
                 if query_sequence.md5 is not None:
                     if genome_sequence.md5 != query_sequence.md5:
-                        logger.debug(f"Discarding genome {genome!s} because {genome_sequence.md5} is different from {query_sequence.md5}.")
                         matching = False
                         break
                 if query_sequence.length != query_sequence.length:
-                    logger.debug(f"Discarding genome {genome!s} because {genome_sequence.length} is different from {query_sequence.length}.")
                     matching = False
                     break
             if matching:
                 logger.info(f"{genome!s} is a perfect match.")
                 match_list.append(genome)
         return match_list
```

### Comparing `wgse_ng-1.0.0a3/wgse/fastq/fastq_file.py` & `wgse_ng-1.0.0a4/wgse/fastq/fastq_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/gui/extract.py` & `wgse_ng-1.0.0a4/wgse/gui/extract.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/gui/main.py` & `wgse_ng-1.0.0a4/wgse/gui/main.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/gui/microarray_format.py` & `wgse_ng-1.0.0a4/wgse/gui/microarray_format.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/gui/table_dialog.py` & `wgse_ng-1.0.0a4/wgse/gui/table_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/gui/ui_extract.py` & `wgse_ng-1.0.0a4/wgse/gui/ui_extract.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/gui/ui_form.py` & `wgse_ng-1.0.0a4/wgse/gui/ui_form.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/metadata/bed_templates/19_wes.csv` & `wgse_ng-1.0.0a4/wgse/metadata/bed_templates/19_wes.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/metadata/bed_templates/38_wes.csv` & `wgse_ng-1.0.0a4/wgse/metadata/bed_templates/38_wes.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/metadata/bed_templates/38_y_mt.csv` & `wgse_ng-1.0.0a4/wgse/metadata/bed_templates/38_y_mt.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/metadata/mtdna.json` & `wgse_ng-1.0.0a4/wgse/metadata/mtdna.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/metadata/references.json` & `wgse_ng-1.0.0a4/wgse/metadata/references.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/metadata/references_template.json` & `wgse_ng-1.0.0a4/wgse/metadata/references_template.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/metadata/report_templates/table_macro.html` & `wgse_ng-1.0.0a4/wgse/metadata/report_templates/table_macro.html`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/metadata/report_templates/table_simple.html` & `wgse_ng-1.0.0a4/wgse/metadata/report_templates/table_simple.html`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/metadata/report_templates/table_tab.html` & `wgse_ng-1.0.0a4/wgse/metadata/report_templates/table_tab.html`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/metadata/sequencers.json` & `wgse_ng-1.0.0a4/wgse/metadata/sequencers.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/metadata/sources.json` & `wgse_ng-1.0.0a4/wgse/metadata/sources.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/microarray/microarray_converter.py` & `wgse_ng-1.0.0a4/wgse/microarray/microarray_converter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/microarray/microarray_line_formatter.py` & `wgse_ng-1.0.0a4/wgse/microarray/microarray_line_formatter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/microarray/raw_file.py` & `wgse_ng-1.0.0a4/wgse/microarray/raw_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/mtDNA/CRS.fasta` & `wgse_ng-1.0.0a4/wgse/mtDNA/CRS.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/mtDNA/RSRS.fasta` & `wgse_ng-1.0.0a4/wgse/mtDNA/RSRS.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/mtDNA/Yoruba.fasta` & `wgse_ng-1.0.0a4/wgse/mtDNA/Yoruba.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/mtDNA/rCRS.fasta` & `wgse_ng-1.0.0a4/wgse/mtDNA/rCRS.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/reference_genome/bgzip_compressor.py` & `wgse_ng-1.0.0a4/wgse/reference_genome/bgzip_compressor.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/reference_genome/decompressor.py` & `wgse_ng-1.0.0a4/wgse/reference_genome/decompressor.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/reference_genome/downloader.py` & `wgse_ng-1.0.0a4/wgse/reference_genome/downloader.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/reference_genome/genome_metadata_loader.py` & `wgse_ng-1.0.0a4/wgse/reference_genome/genome_metadata_loader.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/reference_genome/repository_manager.py` & `wgse_ng-1.0.0a4/wgse/reference_genome/repository_manager.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/renderers/html_aligned_file_report.py` & `wgse_ng-1.0.0a4/wgse/renderers/html_aligned_file_report.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/renderers/html_simple_table_report.py` & `wgse_ng-1.0.0a4/wgse/renderers/html_simple_table_report.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/utility/external.py` & `wgse_ng-1.0.0a4/wgse/utility/external.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,19 @@
 
         if wait:
             # Force stdout/stderr to be PIPE as we
             # need to collect the output
             stdout = subprocess.PIPE
             stderr = subprocess.PIPE
         logger.debug(f"Calling: {shlex.join(args)}")
-
-        output = subprocess.Popen(args, stdout=stdout, stdin=stdin, stderr=stderr)
+        si=None
+        if "win" in sys.platform:
+            si = subprocess.STARTUPINFO()
+            si.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        output = subprocess.Popen(args, stdout=stdout, stdin=stdin, stderr=stderr, startupinfo=si)
         if wait == True:
             out, err = output.communicate()
             if output.returncode != 0:
                 raise RuntimeError(f"Call to {f.__name__} failed: {err.decode()}")
             return out
         return output
```

### Comparing `wgse_ng-1.0.0a3/wgse/utility/file_type_checker.py` & `wgse_ng-1.0.0a4/wgse/utility/file_type_checker.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/utility/mt_dna.py` & `wgse_ng-1.0.0a4/wgse/utility/mt_dna.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/utility/regions.py` & `wgse_ng-1.0.0a4/wgse/utility/regions.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/utility/sequence_orderer.py` & `wgse_ng-1.0.0a4/wgse/utility/sequence_orderer.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/utility/sequencers.py` & `wgse_ng-1.0.0a4/wgse/utility/sequencers.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/utility/updater.py` & `wgse_ng-1.0.0a4/wgse/utility/updater.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a3/wgse/variant_caller.py` & `wgse_ng-1.0.0a4/wgse/variant_caller.py`

 * *Files identical despite different names*

