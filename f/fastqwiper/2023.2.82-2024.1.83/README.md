# Comparing `tmp/fastqwiper-2023.2.82-py3-none-any.whl.zip` & `tmp/fastqwiper-2024.1.83-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 14838 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1898 b- defN 23-Oct-30 19:58 fastq_wiper/__init__.py
--rw-r--r--  2.0 unx     2078 b- defN 23-Oct-30 19:58 fastq_wiper/color_log_formatter.py
--rw-r--r--  2.0 unx    12820 b- defN 23-Oct-30 19:58 fastq_wiper/wiper.py
--rw-r--r--  2.0 unx        0 b- defN 23-Oct-30 19:58 tests/__init__.py
--rw-r--r--  2.0 unx      816 b- defN 23-Oct-30 19:58 tests/test_wiper.py
--rw-r--r--  2.0 unx     7601 b- defN 23-Oct-30 19:59 fastqwiper-2023.2.82.dist-info/LICENSE
--rw-r--r--  2.0 unx    12946 b- defN 23-Oct-30 19:59 fastqwiper-2023.2.82.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Oct-30 19:59 fastqwiper-2023.2.82.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 23-Oct-30 19:59 fastqwiper-2023.2.82.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 23-Oct-30 19:59 fastqwiper-2023.2.82.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      919 b- defN 23-Oct-30 19:59 fastqwiper-2023.2.82.dist-info/RECORD
-11 files, 39248 bytes uncompressed, 13272 bytes compressed:  66.2%
+Zip file size: 15025 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1898 b- defN 24-May-18 16:36 fastq_wiper/__init__.py
+-rw-r--r--  2.0 unx     2078 b- defN 24-May-18 16:36 fastq_wiper/color_log_formatter.py
+-rw-r--r--  2.0 unx    12820 b- defN 24-May-18 16:36 fastq_wiper/wiper.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-18 16:36 tests/__init__.py
+-rw-r--r--  2.0 unx      816 b- defN 24-May-18 16:36 tests/test_wiper.py
+-rw-r--r--  2.0 unx     7601 b- defN 24-May-18 16:36 fastqwiper-2024.1.83.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13353 b- defN 24-May-18 16:36 fastqwiper-2024.1.83.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-18 16:36 fastqwiper-2024.1.83.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 24-May-18 16:36 fastqwiper-2024.1.83.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 24-May-18 16:36 fastqwiper-2024.1.83.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      919 b- defN 24-May-18 16:36 fastqwiper-2024.1.83.dist-info/RECORD
+11 files, 39655 bytes uncompressed, 13459 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_wiper.py
 Comment: 
 
-Filename: fastqwiper-2023.2.82.dist-info/LICENSE
+Filename: fastqwiper-2024.1.83.dist-info/LICENSE
 Comment: 
 
-Filename: fastqwiper-2023.2.82.dist-info/METADATA
+Filename: fastqwiper-2024.1.83.dist-info/METADATA
 Comment: 
 
-Filename: fastqwiper-2023.2.82.dist-info/WHEEL
+Filename: fastqwiper-2024.1.83.dist-info/WHEEL
 Comment: 
 
-Filename: fastqwiper-2023.2.82.dist-info/entry_points.txt
+Filename: fastqwiper-2024.1.83.dist-info/entry_points.txt
 Comment: 
 
-Filename: fastqwiper-2023.2.82.dist-info/top_level.txt
+Filename: fastqwiper-2024.1.83.dist-info/top_level.txt
 Comment: 
 
-Filename: fastqwiper-2023.2.82.dist-info/RECORD
+Filename: fastqwiper-2024.1.83.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fastqwiper-2023.2.82.dist-info/LICENSE` & `fastqwiper-2024.1.83.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fastqwiper-2023.2.82.dist-info/METADATA` & `fastqwiper-2024.1.83.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastqwiper
-Version: 2023.2.82
+Version: 2024.1.83
 Summary: An ensamble method to recover corrupted FASTQ files, drop or fix pesky lines, remove unpaired reads, and fix reads interleaving
 Home-page: https://github.com/mazzalab/fastqwiper
 Author: Tommaso Mazza
 Author-email: bioinformatics@css-mendel.it
 License: MIT
 Project-URL: Source, https://github.com/mazzalab/fastqwiper
 Project-URL: Tracker, https://github.com/mazzalab/fastqwiper/issues
@@ -93,37 +93,37 @@
 #### One quick way (Docker)
 1. Pull the Docker image from DockerHub:
 
 `docker pull mazzalab/fastqwiper`
 
 2. Once downloaded the image, type:
 
-CMD: `docker run --rm -ti --name fastqwiper -v "YOUR_LOCAL_PATH_TO_DATA_FOLDER:/fastqwiper/data" mazzalab/fastqwiper paired 8 sample 50000000`
+CMD: `docker run --rm -ti --name fastqwiper -v "YOUR_LOCAL_PATH_TO_DATA_FOLDER:/fastqwiper/data" mazzalab/fastqwiper paired 8 sample 50000000 33`
 
 #### Another quick way (Singularity)
 1. Pull the Singularity image from the Cloud Library:
 
 `singularity pull library://mazzalab/fastqwiper/fastqwiper.sif`
 
 2. Once downloaded the image (e.g., fastqwiper.sif_2023.2.70.sif), type:
 
-CMD `singularity run --bind /scratch/tom/fastqwiper_singularity/data:/fastqwiper/data --writable-tmpfs fastqwiper.sif_2023.2.70.sif paired 8 sample 50000000`
+CMD `singularity run --bind /scratch/tom/fastqwiper_singularity/data:/fastqwiper/data --writable-tmpfs fastqwiper.sif_2023.2.70.sif paired 8 sample 50000000 33`
 
 If you want to bind the `.singularity` cache folder and the `logs` folder, you can omit `--writable-tmpfs`, create the folders `.singularity` and `logs` (`mkdir .singularity logs`) on the host system, and use this command instead:
 
-CMD: `singularity run --bind YOUR_LOCAL_PATH_TO_DATA_FOLDER/:/fastqwiper/data --bind YOUR_LOCAL_PATH_TO_.singularity_FOLDER/:/fastqwiper/.snakemake --bind YOUR_LOCAL_PATH_TO_LOGS_FOLDER/:/fastqwiper/logs fastqwiper.sif_2023.2.70.sif paired 8 sample 50000000`
+CMD: `singularity run --bind YOUR_LOCAL_PATH_TO_DATA_FOLDER/:/fastqwiper/data --bind YOUR_LOCAL_PATH_TO_.singularity_FOLDER/:/fastqwiper/.snakemake --bind YOUR_LOCAL_PATH_TO_LOGS_FOLDER/:/fastqwiper/logs fastqwiper.sif_2023.2.70.sif paired 8 sample 50000000 33`
 
 For both **Docker** and **Singularity**:
 
 - `YOUR_LOCAL_PATH_TO_DATA_FOLDER` is the path of the folder where the fastq.gz files to be wiped are located;
 - `paired` triggers the cleaning of R1 and R2. Alternatively, `single` will trigger the wipe of individual FASTQ files;
 - `8` is the number of your choice of computing cores to be spawned;
 - `sample` is part of the names of the FASTQ files to be wiped. <b>Be aware</b> that: for <b>paired-end</b> files (e.g., "sample_R1.fastq.gz" and "sample_R2.fastq.gz"), your files must finish with `_R1.fastq.gz` and `_R2.fastq.gz`. Therefore, the argument to pass is everything before these texts: `sample` in this case. For <b>single end</b>/individual files (e.g., "excerpt_R1_001.fastq.gz"), your file must end with the string `.fastq.gz`; the preceding text, i.e., "excerpt_R1_001" in this case, will be the text to be passed to the command as an argument. 
-- `50000000` is the number of rows-per-chunk (used when cores>1. It must be a number multiple of 4)
-
+- `50000000` (optional) is the number of rows-per-chunk (used when cores>1. It must be a number multiple of 4). Increasing this number too much would reduce the parallelism advantage. Decreasing this number too much would increase the number of chunks more than the number of available cpus, making parallelism unefficient. Choose this number wisely depending on the total number of reads in your starting file.
+- `33` (optional) is the ASCII offset (33=Sanger, 64=old Solexa) 
 
 #### The slow way (Linux & Mac OS)
 To enable the use of preconfigured [pipelines](https://github.com/mazzalab/fastqwiper/tree/main/pipeline), you need to install **Snakemake**. The recommended way to install Snakemake is via Conda, because it enables **Snakemake** to [handle software dependencies of your workflow](https://snakemake.readthedocs.io/en/stable/snakefiles/deployment.html#integrated-package-management).
 However, the default conda solver is slow and often hangs. Therefore, we recommend installing [Mamba](https://github.com/mamba-org/mamba) as a drop-in replacement via
 
 `$ conda install -c conda-forge mamba`
 
@@ -169,22 +169,22 @@
 ### Commands:
 Copy the fastq files you want to fix in the `data` folder.
 **N.b.**: In all commands above, you will pass to the workflow the name of the sample to be analyzed through the config argument: `sample_name`. Remember that your fastq files' names must finish with `_R1.fastq.gz` and `_R2.fastq.gz`, for paired fastq files, and with `.fastq.gz`, for individual fastq files, and, therefore, the text to be assigned to the variable `sample_name` must be everything before them. E.g., if your files are `my_sample_R1.fastq.gz` and `my_sample_R2.fastq.gz`, then `--config sample_name=my_sample`.
 
 #### Paired-end files
 
 - **Get a dry run** of a pipeline (e.g., `fix_wipe_pairs_reads_sequential.smk`):<br />
-`snakemake --config sample_name=my_sample -s pipeline/fix_wipe_pairs_reads_sequential.smk --use-conda --cores 4`
+`snakemake --config sample_name=my_sample qin=33 -s pipeline/fix_wipe_pairs_reads_sequential.smk --use-conda --cores 4`
 
 - **Generate the planned DAG**:<br />
-`snakemake --config sample_name=my_sample -s pipeline/fix_wipe_pairs_reads_sequential.smk --dag | dot -Tpdf > dag.pdf`<br /> <br />
+`snakemake --config sample_name=my_sample qin=33 -s pipeline/fix_wipe_pairs_reads_sequential.smk --dag | dot -Tpdf > dag.pdf`<br /> <br />
 <img src="https://github.com/mazzalab/fastqwiper/blob/main/pipeline/fix_wipe_pairs_reads.png?raw=true" width="400">
 
 - **Run the pipeline** (n.b., during the first execution, Snakemake will download and install some required remote packages and may take longer). The number of computing cores can be tuned accordingly:<br />
-`snakemake --config sample_name=my_sample -s pipeline/fix_wipe_single_reads_sequential.smk --use-conda --cores 2`
+`snakemake --config sample_name=my_sample qin=33 -s pipeline/fix_wipe_single_reads_sequential.smk --use-conda --cores 2`
 
 Fixed files will be copied in the `data` folder and will be suffixed with the string `_fixed_wiped_paired_interleaving`.
 We remind that the `fix_wipe_pairs_reads_sequential.smk` and `fix_wipe_pairs_reads_parallel.smk` pipelines perform the following actions:
 - execute `gzrt` on corrupted fastq.gz files (i.e., that cannot be unzipped because of errors) and recover readable reads;
 - execute `FastqWiper` on recovered reads to make them compliant with the FASTQ format (source: [Wipipedia](https://en.wikipedia.org/wiki/FASTQ_format))
 - execute `Trimmomatic` on wiped reads to remove residual unpaired reads
 - execute `BBmap (repair.sh)` on paired reads to fix the correct interleaving and sort fastq files.
```

