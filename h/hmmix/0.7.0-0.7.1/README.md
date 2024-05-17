# Comparing `tmp/hmmix-0.7.0.tar.gz` & `tmp/hmmix-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hmmix-0.7.0.tar", last modified: Mon May 13 01:32:28 2024, max compression
+gzip compressed data, was "dist/hmmix-0.7.1.tar", last modified: Fri May 17 22:36:02 2024, max compression
```

## Comparing `hmmix-0.7.0.tar` & `hmmix-0.7.1.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2024-05-13 01:32:28.000000 hmmix-0.7.0/
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    35149 2022-05-11 17:42:22.000000 hmmix-0.7.0/LICENSE.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    37194 2024-05-13 01:32:28.000000 hmmix-0.7.0/PKG-INFO
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    36660 2024-05-13 00:59:09.000000 hmmix-0.7.0/README.md
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       38 2024-05-13 01:32:28.000000 hmmix-0.7.0/setup.cfg
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      994 2024-05-13 01:32:07.000000 hmmix-0.7.0/setup.py
-drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2024-05-13 01:32:28.000000 hmmix-0.7.0/src/
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     8599 2024-05-10 23:31:25.000000 hmmix-0.7.0/src/bcf_vcf.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    17028 2024-05-13 01:21:08.000000 hmmix-0.7.0/src/helper_functions.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    18509 2024-05-13 01:27:31.000000 hmmix-0.7.0/src/hmm_functions.py
-drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2024-05-13 01:32:28.000000 hmmix-0.7.0/src/hmmix.egg-info/
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    37194 2024-05-13 01:32:27.000000 hmmix-0.7.0/src/hmmix.egg-info/PKG-INFO
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      411 2024-05-13 01:32:28.000000 hmmix-0.7.0/src/hmmix.egg-info/SOURCES.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)        1 2024-05-13 01:32:27.000000 hmmix-0.7.0/src/hmmix.egg-info/dependency_links.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       36 2024-05-13 01:32:28.000000 hmmix-0.7.0/src/hmmix.egg-info/entry_points.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       29 2024-05-13 01:32:28.000000 hmmix-0.7.0/src/hmmix.egg-info/requires.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       77 2024-05-13 01:32:28.000000 hmmix-0.7.0/src/hmmix.egg-info/top_level.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    21088 2024-05-13 01:31:55.000000 hmmix-0.7.0/src/main.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     2007 2022-10-25 01:10:14.000000 hmmix-0.7.0/src/make_mutationrate.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     4560 2024-05-12 23:11:55.000000 hmmix-0.7.0/src/make_test_data.py
-drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2024-05-13 01:32:28.000000 hmmix-0.7.0/test/
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     1280 2024-05-13 00:59:38.000000 hmmix-0.7.0/test/test.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     3106 2022-06-02 06:35:33.000000 hmmix-0.7.0/test/test2.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      541 2022-06-08 21:55:04.000000 hmmix-0.7.0/test/test_main.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)        0 2022-07-12 05:40:51.000000 hmmix-0.7.0/test/testfred.py
+drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2024-05-17 22:36:02.000000 hmmix-0.7.1/
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    35149 2022-05-11 17:42:22.000000 hmmix-0.7.1/LICENSE.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    41064 2024-05-17 22:36:02.000000 hmmix-0.7.1/PKG-INFO
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    40530 2024-05-17 22:33:23.000000 hmmix-0.7.1/README.md
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       38 2024-05-17 22:36:02.000000 hmmix-0.7.1/setup.cfg
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      994 2024-05-17 22:35:48.000000 hmmix-0.7.1/setup.py
+drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2024-05-17 22:36:02.000000 hmmix-0.7.1/src/
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     8599 2024-05-17 18:48:53.000000 hmmix-0.7.1/src/bcf_vcf.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    17258 2024-05-17 22:29:01.000000 hmmix-0.7.1/src/helper_functions.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    18509 2024-05-15 21:18:28.000000 hmmix-0.7.1/src/hmm_functions.py
+drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2024-05-17 22:36:02.000000 hmmix-0.7.1/src/hmmix.egg-info/
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    41064 2024-05-17 22:36:01.000000 hmmix-0.7.1/src/hmmix.egg-info/PKG-INFO
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      380 2024-05-17 22:36:02.000000 hmmix-0.7.1/src/hmmix.egg-info/SOURCES.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)        1 2024-05-17 22:36:01.000000 hmmix-0.7.1/src/hmmix.egg-info/dependency_links.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       36 2024-05-17 22:36:01.000000 hmmix-0.7.1/src/hmmix.egg-info/entry_points.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       29 2024-05-17 22:36:01.000000 hmmix-0.7.1/src/hmmix.egg-info/requires.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       77 2024-05-17 22:36:01.000000 hmmix-0.7.1/src/hmmix.egg-info/top_level.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    21120 2024-05-17 22:35:42.000000 hmmix-0.7.1/src/main.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     2007 2024-05-15 21:18:33.000000 hmmix-0.7.1/src/make_mutationrate.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     4431 2024-05-15 22:49:25.000000 hmmix-0.7.1/src/make_test_data.py
+drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2024-05-17 22:36:02.000000 hmmix-0.7.1/test/
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     1280 2024-05-13 00:59:38.000000 hmmix-0.7.1/test/test.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      541 2022-06-08 21:55:04.000000 hmmix-0.7.1/test/test_main.py
```

### Comparing `hmmix-0.7.0/LICENSE.txt` & `hmmix-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hmmix-0.7.0/PKG-INFO` & `hmmix-0.7.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 Metadata-Version: 2.1
 Name: hmmix
-Version: 0.7.0
+Version: 0.7.1
 Summary: Find introgressed segments
 Home-page: https://github.com/LauritsSkov/Introgression-detection
 Author: Laurits Skov and Moises Coll Macia
 Author-email: lauritsskov2@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Contact
-https://sites.google.com/view/laurits-skov
+# Introgression detection
+
+## Contact
+
+<https://sites.google.com/view/laurits-skov>
 
 ---
 
-# Helpful files
-The outgroup files, mutation rate files and callability files and ancestral allele files are now premade! 
+## Helpful files
 
-https://doi.org/10.5281/zenodo.10806733 (hg19 and hg38)
+The outgroup files, mutation rate files, reference genomes, ancestral alleles and callability files and ancestral allele files are now premade!
 
-VCF file containing 4 high coverage archaic genomes (Altai, Vindija and Chagyrskaya Neanderthals and Denisovan) here: 
+<https://doi.org/10.5281/zenodo.11212339> (hg19 and hg38)
+Note the old version (<https://doi.org/10.5281/zenodo.10806733>) did not contain the ancestral alleles or reference genome and there was some missing data on the X chromosome.
 
-https://zenodo.org/records/7246376 (hg19)
+VCF file containing 4 high coverage archaic genomes (Altai, Vindija and Chagyrskaya Neanderthals and Denisovan) here:
 
-https://zenodo.org/records/10806726 (hg38)
+<https://zenodo.org/records/7246376> (hg19)
 
----
+<https://zenodo.org/records/10806726> (hg38)
 
-# Introgression detection
+---
 
 If you are working with archaic introgression into present-day humans of non-African ancestry you can use these files and skip the following steps:
-Find derived variants in outgroup and Estimate local mutation rate. 
+Find derived variants in outgroup and Estimate local mutation rate.
 
 These are the scripts needed to infere archaic introgression in modern populations using an unadmixed outgroup.
 
 1. [Installation](#installation)
 2. [Usage](#usage)
 3. [Quick tutorial](#quick-tutorial)
 4. [1000 genomes tutorial](#example-with-1000-genomes-data)
@@ -146,15 +149,15 @@
 
 > inhomogeneous                
     -obs                [required] file with observation data
     -chrom              Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3 (default is use all chromosomes)
     -weights            file with callability (defaults to all positions being called)
     -mutrates           file with mutation rates (default is mutation rate is uniform)
     -param              markov parameters file (default is human/neanderthal like parameters)
-    -out                outputfile prefix <out>.hap1.txt and <out>.hap2.txt if -haploid option is used or <out>.diploid.txt (default is stdout)
+    -out                outputfile prefix <out>.hap1_sim(0-n).txt and <out>.hap2_sim(0-n).txt if -haploid option is used or <out>.diploid_(0-n).txt (default is stdout)
     -window_size        size of bins (default is 1000 bp)
     -haploid            Change from using diploid data to haploid data (default is diploid)
     -samples            Number of simulated paths for the inhomogeneous markov chain (default is 100)
     -admixpop           Annotate using vcffile with admixing population (default is none)
     -extrainfo          Add variant position for each SNP (default is off)
 ```
 
@@ -290,21 +293,24 @@
 ---
 
 ## Example with 1000 genomes data
 
 ---
 
 The whole pipeline we will run looks like this. In the following section we will go through all the steps on the way
-NOTE: The outgroup files, mutation rate files and callability files are now premade! They can be downloaded in hg38 and hg19 here: https://doi.org/10.5281/zenodo.10806733
+
+NOTE: The outgroup files, mutation rate files, reference genomes, ancestral alleles and callability files and ancestral allele files are now premade!
+They can be downloaded in hg38 and hg19 here: <https://doi.org/10.5281/zenodo.11212339>
+
 But keep reading along if you want to know HOW the files were generated!
 
 ```note
-hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa -refgenome=referencegenome/*fa
+hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa -refgenome=hg19_refgenome/*fa
 hmmix mutation_rate -outgroup=outgroup.txt  -weights=strickmask.bed -window_size=1000000 -out mutationrate.bed
-hmmix create_ingroup  -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa
+hmmix create_ingroup  -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa
 hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.json 
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json 
 ```
 
 ### Getting data
 
 I thought it would be nice to have an entire reproduceble example of how to use this model. From a common starting point such as a VCF file (well a BCF file in this case) to the final output.  The reason for using BCF files is because it is MUCH faster to extract data for each individual. You can convert a vcf file to a bcf file like this:
@@ -327,25 +333,25 @@
 ftp.1000genomes.ebi.ac.uk/vol1/ftp/release/20130502/supporting/accessible_genome_masks/20141020.strict_mask.whole_genome.bed
 sed 's/^chr\|%$//g' 20141020.strict_mask.whole_genome.bed | awk '{print $1"\t"$2"\t"$3}' > strickmask.bed
 
 # outgroup information
 ftp://ftp.1000genomes.ebi.ac.uk/vol1/ftp/release/20130502/integrated_call_samples_v3.20130502.ALL.panel
 
 # Ancestral information
-ftp://ftp.ensembl.org/pub/release-74/fasta/ancestral_alleles/homo_sapiens_ancestor_GRCh37_e71.tar.bz2
+ftp://ftp.ensembl.org/pub/release-74/fasta/ancestral_alleles/hg19_ancestral.tar.bz2
 
 # Reference genome
 wget 'ftp://hgdownload.soe.ucsc.edu/goldenPath/hg19/bigZips/chromFa.tar.gz' -O chromFa.tar.gz
 
 # Archaic variants (Altai, Vindija, Chagyrskaya and Denisova in hg19)
 https://zenodo.org/records/7246376
 
 ```
 
-For this example we will use all individuals from 'YRI','MSL' and 'ESN' as outgroup individuals. While we will only be decoding hG00096 in this example you can add as many individuals as you want to the ingroup.  
+For this example we will use all individuals from 'YRI','MSL' and 'ESN' as outgroup individuals. While we will only be decoding HG00096 in this example you can add as many individuals as you want to the ingroup.  
 
 ```json
 {
   "ingroup": [
     "HG00096",
     "HG00097"
   ],
@@ -358,36 +364,57 @@
 }
 ```
 
 ---
 
 ### Finding snps which are derived in the outgroup
 
-First we need to find a set of variants found in the outgroup. We can use the wildcard character to loop through all bcf files. If you dont have ancestral information you can skip the ancestral argument.
-
-```bash
-(took an hour) > hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa 
-
-# Alternative usage (if you only have a few individual in the outgroup you can also provide a comma separated list)
-> hmmix create_outgroup -ind=HG02922,HG02923,HG02938 -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa 
-
-# Alternative usage (if you have no ancestral information)
-> hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt 
+First we need to find a set of variants found in the outgroup. We can use the wildcard character to loop through all bcf files. It is best if you have files with the ancestral alleles (in FASTA format) and the reference genome (in FASTA format) but the program will run without.
 
-# Alternative usage (if you only want to run the model on a subset of chromosomes, with or without ancestral information)
-> hmmix create_outgroup -ind=individuals.json -vcf=chr1.bcf,chr2.bcf -weights=strickmask.bed -out=outgroup.txt
+Something to note is that if you use an outgroup vcffile (like 1000 genomes) and an ingroup vcf file from a different dataset (like SGDP) there is an edge case which could occur. There could be recurrent mutations where every individual in 1000 genome has the derived variant and one individual in SGDP where the derived variant has mutated back to the ancestral allele. This means that this position will not be present in the outgroup file. However if a recurrent mutation occurs it will look like multiple individuals in the ingroup file have the mutation. This does not happen often but that is why I recommend having files with the ancestral allele and reference genome information.
 
-> hmmix create_outgroup -ind=individuals.json -vcf=chr1.bcf,chr2.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_1.fa,homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_2.fa
+```note
+# Recommended usage (if you want to remove sites which are fixed derived in your outgroup/ingroup). This is the file from zenodo. 
+(took two hours) > hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa -refgenome=hg19_refgenome/*fa
+----------------------------------------
+> Outgroup individuals: 292
+> Using vcf and ancestral files
+vcffile: chr1.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_1.fa reffile:  hg19_refgenome/chr1.fa
+vcffile: chr2.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_2.fa reffile:  hg19_refgenome/chr2.fa
+vcffile: chr3.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_3.fa reffile:  hg19_refgenome/chr3.fa
+vcffile: chr4.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_4.fa reffile:  hg19_refgenome/chr4.fa
+vcffile: chr5.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_5.fa reffile:  hg19_refgenome/chr5.fa
+vcffile: chr6.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_6.fa reffile:  hg19_refgenome/chr6.fa
+vcffile: chr7.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_7.fa reffile:  hg19_refgenome/chr7.fa
+vcffile: chr8.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_8.fa reffile:  hg19_refgenome/chr8.fa
+vcffile: chr9.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_9.fa reffile:  hg19_refgenome/chr9.fa
+vcffile: chr10.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_10.fa reffile: hg19_refgenome/chr10.fa
+vcffile: chr11.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_11.fa reffile: hg19_refgenome/chr11.fa
+vcffile: chr12.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_12.fa reffile: hg19_refgenome/chr12.fa
+vcffile: chr13.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_13.fa reffile: hg19_refgenome/chr13.fa
+vcffile: chr14.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_14.fa reffile: hg19_refgenome/chr14.fa
+vcffile: chr15.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_15.fa reffile: hg19_refgenome/chr15.fa
+vcffile: chr16.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_16.fa reffile: hg19_refgenome/chr16.fa
+vcffile: chr17.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_17.fa reffile: hg19_refgenome/chr17.fa
+vcffile: chr18.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_18.fa reffile: hg19_refgenome/chr18.fa
+vcffile: chr19.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_19.fa reffile: hg19_refgenome/chr19.fa
+vcffile: chr20.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_20.fa reffile: hg19_refgenome/chr20.fa
+vcffile: chr21.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_21.fa reffile: hg19_refgenome/chr21.fa
+vcffile: chr22.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_22.fa reffile: hg19_refgenome/chr22.fa
+vcffile: chrX.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_X.fa reffile:  hg19_refgenome/chrX.fa
+
+> Callability file: strickmask.bed
+> Writing output to: outgroup.txt
+----------------------------------------
 ```
 
-Something to note is that if you use an outgroup vcffile (like 1000 genomes) and an ingroup vcf file from a different dataset (like SGDP) there is an edge case which could occur. There could be recurrent mutations where every individual in 1000 genome has the derived variant and one individual in SGDP where the derived variant has mutated back to the ancestral allele. This means that this position will not be present in the outgroup file. However if a recurrent mutation occurs it will look like multiple individuals in the ingroup file have the mutation. This does not happen often but just in case you can create the outgroup file and adding the sites which are fixed derived in all individuals using the reference genome:
+Here it is important to check that hmmix matches up the reference, ancestral and vcffiles correctly e.g. chr1.bcf should fit with hg19_ancestral/homo_sapiens_ancestor_1.fa and hg19_refgenome/chr1.fa for instance. If you see an issue here its better to give the files as commaseparated values.
 
-```bash
-# Recommended usage (if you want to remove sites which are fixed derived in your outgroup/ingroup)
-> hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa -refgenome=*fa
+```note
+hmmix create_outgroup -ind=individuals.json -vcf=chr1.bcf,chr2.bcf,chr3.bcf,chr4.bcf,chr5.bcf,chr6.bcf,chr7.bcf,chr8.bcf,chr9.bcf,chr10.bcf,chr11.bcf,chr12.bcf,chr13.bcf,chr14.bcf,chr15.bcf,chr16.bcf,chr17.bcf,chr18.bcf,chr19.bcf,chr20.bcf,chr21.bcf,chr22.bcf,chrX.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_1.fa,hg19_ancestral/homo_sapiens_ancestor_2.fa,hg19_ancestral/homo_sapiens_ancestor_3.fa,hg19_ancestral/homo_sapiens_ancestor_4.fa,hg19_ancestral/homo_sapiens_ancestor_5.fa,hg19_ancestral/homo_sapiens_ancestor_6.fa,hg19_ancestral/homo_sapiens_ancestor_7.fa,hg19_ancestral/homo_sapiens_ancestor_8.fa,hg19_ancestral/homo_sapiens_ancestor_9.fa,hg19_ancestral/homo_sapiens_ancestor_10.fa,hg19_ancestral/homo_sapiens_ancestor_11.fa,hg19_ancestral/homo_sapiens_ancestor_12.fa,hg19_ancestral/homo_sapiens_ancestor_13.fa,hg19_ancestral/homo_sapiens_ancestor_14.fa,hg19_ancestral/homo_sapiens_ancestor_15.fa,hg19_ancestral/homo_sapiens_ancestor_16.fa,hg19_ancestral/homo_sapiens_ancestor_17.fa,hg19_ancestral/homo_sapiens_ancestor_18.fa,hg19_ancestral/homo_sapiens_ancestor_19.fa,hg19_ancestral/homo_sapiens_ancestor_20.fa,hg19_ancestral/homo_sapiens_ancestor_21.fa,hg19_ancestral/homo_sapiens_ancestor_22.fa,hg19_ancestral/homo_sapiens_ancestor_X.fa -refgenome=hg19_refgenome/chr1.fa,hg19_refgenome/chr2.fa,hg19_refgenome/chr3.fa,hg19_refgenome/chr4.fa,hg19_refgenome/chr5.fa,hg19_refgenome/chr6.fa,hg19_refgenome/chr7.fa,hg19_refgenome/chr8.fa,hg19_refgenome/chr9.fa,hg19_refgenome/chr10.fa,hg19_refgenome/chr11.fa,hg19_refgenome/chr12.fa,hg19_refgenome/chr13.fa,hg19_refgenome/chr14.fa,hg19_refgenome/chr15.fa,hg19_refgenome/chr16.fa,hg19_refgenome/chr17.fa,hg19_refgenome/chr18.fa,hg19_refgenome/chr19.fa,hg19_refgenome/chr20.fa,hg19_refgenome/chr21.fa,hg19_refgenome/chr22.fa,hg19_refgenome/chrX.fa
 ```
 
 ---
 
 ### Estimating mutation rate across genome
 
 We can use the number of variants in the outgroup to estimate the substitution rate as a proxy for mutation rate.
@@ -405,54 +432,55 @@
 ---
 
 ### Find a set of variants which are not derived in the outgroup
 
 Keep variants that are not found to be derived in the outgroup for each individual in ingroup. You can also speficy a single individual or a comma separated list of individuals.
 
 ```note
-(took 20 min) > hmmix create_ingroup  -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa
+(took 20 min) > hmmix create_ingroup  -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa
 ----------------------------------------
 > Ingroup individuals: 2
 > Using vcf and ancestral files
-vcffile: chr1.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_1.fa
-vcffile: chr2.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_2.fa
-vcffile: chr3.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_3.fa
-vcffile: chr4.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_4.fa
-vcffile: chr5.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_5.fa
-vcffile: chr6.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_6.fa
-vcffile: chr7.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_7.fa
-vcffile: chr8.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_8.fa
-vcffile: chr9.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_9.fa
-vcffile: chr10.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_10.fa
-vcffile: chr11.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_11.fa
-vcffile: chr12.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_12.fa
-vcffile: chr13.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_13.fa
-vcffile: chr14.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_14.fa
-vcffile: chr15.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_15.fa
-vcffile: chr16.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_16.fa
-vcffile: chr17.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_17.fa
-vcffile: chr18.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_18.fa
-vcffile: chr19.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_19.fa
-vcffile: chr20.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_20.fa
-vcffile: chr21.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_21.fa
-vcffile: chr22.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_22.fa
+vcffile: chr1.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_1.fa
+vcffile: chr2.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_2.fa
+vcffile: chr3.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_3.fa
+vcffile: chr4.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_4.fa
+vcffile: chr5.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_5.fa
+vcffile: chr6.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_6.fa
+vcffile: chr7.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_7.fa
+vcffile: chr8.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_8.fa
+vcffile: chr9.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_9.fa
+vcffile: chr10.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_10.fa
+vcffile: chr11.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_11.fa
+vcffile: chr12.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_12.fa
+vcffile: chr13.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_13.fa
+vcffile: chr14.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_14.fa
+vcffile: chr15.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_15.fa
+vcffile: chr16.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_16.fa
+vcffile: chr17.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_17.fa
+vcffile: chr18.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_18.fa
+vcffile: chr19.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_19.fa
+vcffile: chr20.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_20.fa
+vcffile: chr21.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_21.fa
+vcffile: chr22.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_22.fa
+vcffile: chrX.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_X.fa
 
 > Using outgroup variants from: outgroup.txt 
 > Callability file: strickmask.bed 
 > Writing output to file with prefix: obs.<individual>.txt
 
 ----------------------------------------
 Running command:
 bcftools view -m2 -M2 -v snps -s HG00096 -T strickmask.bed chr1.bcf | vcftools --vcf - --exclude-positions outgroup.txt --recode --stdout 
 ...
 bcftools view -m2 -M2 -v snps -s HG00097 -T strickmask.bed chr22.bcf | vcftools --vcf - --exclude-positions outgroup.txt --recode --stdout 
 
 
 # Different way to define which individuals are in the ingroup
-(took 20 min) > hmmix create_ingroup  -ind=HG00096,HG00097 -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa
+(took 20 min) > hmmix create_ingroup  -ind=HG00096,HG00097 -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa
 ```
 
 ---
 
 ### Training
 
 Now for training the HMM parameters and decoding
@@ -461,160 +489,160 @@
 (took 2 min) > hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.json 
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.98, 0.02]
 > transitions = [[1.0, 0.0], [0.02, 0.98]]
 > emissions = [0.04, 0.4]
 > chromosomes to use: All
-> number of windows: 2877010 . Number of snps =  129734
+> number of windows: 3032224 . Number of snps =  129803
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output is trained.HG00096.json
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 iteration  loglikelihood  start1  start2  emis1   emis2   trans1_1  trans2_2
-0          -492287.8643   0.98    0.02    0.04    0.4     0.9999    0.98
-1          -488898.6051   0.961   0.039   0.0483  0.3913  0.9994    0.986
-2          -488754.2455   0.958   0.042   0.0481  0.3911  0.9993    0.9835
+0          -495665.7379   0.98    0.02    0.04    0.4     0.9999    0.98
+1          -493092.9242   0.964   0.036   0.0459  0.3894  0.9995    0.9859
+2          -492917.6235   0.959   0.041   0.0455  0.3847  0.9993    0.9834
 ...
-19         -488641.0769   0.954   0.046   0.047   0.3862  0.9989    0.9771
-20         -488641.0755   0.954   0.046   0.047   0.3862  0.9989    0.9771
-21         -488641.0748   0.954   0.046   0.047   0.3862  0.9989    0.9771
+20         -492775.4072   0.954   0.046   0.0442  0.3725  0.9989    0.9768
+21         -492775.4058   0.954   0.046   0.0442  0.3725  0.9989    0.9768
+22         -492775.4049   0.954   0.046   0.0442  0.3725  0.9989    0.9768
 ```
 
 ---
 
 ### Decoding
 
 ```note
 (took 30 sec) > hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json 
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.954, 0.046]
 > transitions = [[0.999, 0.001], [0.023, 0.977]]
-> emissions = [0.047, 0.386]
+> emissions = [0.044, 0.372]
 > chromosomes to use: All
-> number of windows: 2877010 . Number of snps =  129734
+> number of windows: 3032224 . Number of snps =  129803
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 chrom  start    end      length   state    mean_prob  snps
-1      0        2988000  2988000  Human    0.98484    91
-1      2988000  2997000  9000     Archaic  0.71819    6
-1      2997000  3425000  428000   Human    0.98944    30
-1      3425000  3452000  27000    Archaic  0.95652    22
-1      3452000  4302000  850000   Human    0.98203    36
-1      4302000  4361000  59000    Archaic  0.84636    20
-1      4361000  4500000  139000   Human    0.97136    4
-1      4500000  4510000  10000    Archaic  0.84457    7
+1      0        2988000  2988000  Human    0.98429    91
+1      2988000  2997000  9000     Archaic  0.76217    6
+1      2997000  3425000  428000   Human    0.98776    30
+1      3425000  3452000  27000    Archaic  0.95816    22
+1      3452000  4302000  850000   Human    0.97917    36
+1      4302000  4361000  59000    Archaic  0.867      20
+1      4361000  4500000  139000   Human    0.96854    4
+1      4500000  4510000  10000    Archaic  0.8552     7
 ```
 
 You can also save to an output file with the command:
 
 ```note
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json -out=HG00096.decoded
 ```
 
 This will create a file named HG00096.decoded.diploid.txt because the default option is treating the data as diploid (more on haploid decoding in next chapter)
 
 ---
 
 ### Training and decoding with phased data
 
-It is also possible to tell the model that the data is phased with the -haploid parameter. For that we first need to train the parameters for haploid data and then decode. Training the model on phased data is done like this - and we also remember to change the name of the parameter file to include phased so future versions of ourselves don't forget. Another thing to note is that the number of snps is bigger than before 135411 vs 129734. This is because the program is counting snps on both haplotypes and homozygotes will be counted twice!
+It is also possible to tell the model that the data is phased with the -haploid parameter. For that we first need to train the parameters for haploid data and then decode. Training the model on phased data is done like this - and we also remember to change the name of the parameter file to include phased so future versions of ourselves don't forget. Another thing to note is that the number of snps is bigger than before 135483 vs 129803. This is because the program is counting snps on both haplotypes and homozygotes will be counted twice!
 
 ```note
 (took 4 min) > hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.phased.json -haploid
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.98, 0.02]
 > transitions = [[1.0, 0.0], [0.02, 0.98]]
 > emissions = [0.04, 0.4]
 > chromosomes to use: All
-> number of windows: 5754020 . Number of snps =  135411
+> number of windows: 6064448 . Number of snps =  135483
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output is trained.HG00096.phased.json
 > Window size is 1000 bp
 > Haploid True
 ----------------------------------------
 iteration  loglikelihood  start1  start2  emis1   emis2   trans1_1  trans2_2
-0          -597750.7043   0.98    0.02    0.04    0.4     0.9999    0.98
-1          -585028.8828   0.983   0.017   0.0261  0.4026  0.9998    0.9853
-2          -584447.5809   0.979   0.021   0.0252  0.373   0.9996    0.9826
+0          -605433.1928   0.98    0.02    0.04    0.4     0.9999    0.98
+1          -589492.2      0.985   0.015   0.0248  0.3999  0.9998    0.9852
+2          -588823.124    0.98    0.02    0.0238  0.3671  0.9996    0.9825
 ...
-19         -584131.0153   0.972   0.028   0.0241  0.3367  0.9993    0.9758
-20         -584131.0138   0.972   0.028   0.0241  0.3367  0.9993    0.9758
-21         -584131.013    0.972   0.028   0.0241  0.3366  0.9993    0.9758
+20         -588456.6027   0.973   0.027   0.0228  0.3267  0.9993    0.9755
+21         -588456.6015   0.973   0.027   0.0228  0.3266  0.9993    0.9755
+22         -588456.6009   0.973   0.027   0.0228  0.3266  0.9993    0.9755
 ```
 
-Below I am only showing the first archaic segments on chromosome 1 for each haplotype (note you have to scroll down after chrom 22 before the new haplotype begins). The seem to fall more or less in the same places as when we used diploid data.
+Below I am only showing the first archaic segments on chromosome 1 for each haplotype (note you have to scroll down after chrom X before the new haplotype begins). The seem to fall more or less in the same places as when we used diploid data.
 
 ```note
 (took 30 sec) > hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.phased.json -haploid
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
-> starting_probabilities = [0.972, 0.028]
+> starting_probabilities = [0.973, 0.027]
 > transitions = [[0.999, 0.001], [0.024, 0.976]]
-> emissions = [0.024, 0.337]
+> emissions = [0.023, 0.327]
 > chromosomes to use: All
-> number of windows: 5754020 . Number of snps =  135411
+> number of windows: 6064448 . Number of snps =  135483
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid True
 ----------------------------------------
 hap1
 chrom  start    end      length  state    mean_prob  snps
-1      2162000  2185000  23000   Archaic  0.61054    6
-1      3425000  3452000  27000   Archaic  0.96595    22
+1      2156000  2185000  29000   Archaic  0.64711    6
+1      3425000  3452000  27000   Archaic  0.96701    22
 
 ...
 hap2
-1      2780000  2803000  23000   Archaic  0.61948    7
-1      4302000  4337000  35000   Archaic  0.94008    13
-1      4500000  4511000  11000   Archaic  0.87592    7
-1      4989000  5000000  11000   Archaic  0.579      4
+1      2780000  2803000  23000   Archaic  0.68285    7
+1      4302000  4337000  35000   Archaic  0.94244    13
+1      4500000  4511000  11000   Archaic  0.87938    7
+1      4989000  5001000  12000   Archaic  0.61874    5
 ```
 
 You can also save to an output file with the command:
 
 ```note
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.phased.json -haploid -out=HG00096.decoded
 ```
 
 This will create two files named HG00096.decoded.hap1.txt and HG00096.decoded.hap2.txt
 
 ---
 
 ### Annotate with known admixing population
 
-Even though this method does not use archaic reference genomes for finding segments you can still use them to annotate your segments. 
+Even though this method does not use archaic reference genomes for finding segments you can still use them to annotate your segments.
 I have uploaded a VCF file containing 4 high coverage archaic genomes (3 Neanderthals and 1 Denisovan) here:
 
-https://zenodo.org/records/7246376 (hg19 - the one I use in this example)
+<https://zenodo.org/records/7246376> (hg19 - the one I use in this example)
 
-https://zenodo.org/records/10806726 (hg38)
+<https://zenodo.org/records/10806726> (hg38)
 
 If you have a vcf from the population that admixed in VCF/BCF format you can write this:
 
 ```note
 > hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json -admixpop=archaicvar/*bcf
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.954, 0.046]
 > transitions = [[0.999, 0.001], [0.023, 0.977]]
-> emissions = [0.047, 0.386]
+> emissions = [0.044, 0.372]
 > chromosomes to use: All
-> number of windows: 2877010 . Number of snps =  129734
+> number of windows: 3032224 . Number of snps =  129803
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_9.bcf
@@ -638,22 +666,22 @@
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_5.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_8.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_11.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_12.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_13.bcf
 
 chrom  start     end       length  state    mean_prob  snps  admixpopvariants  AltaiNeandertal  Vindija33.19  Denisova  Chagyrskaya-Phalanx
-1      2988000   2997000   9000    Archaic  0.71819    6     4                 4                4             1         4
-1      3425000   3452000   27000   Archaic  0.95652    22    17                17               15            3         17
-1      4302000   4361000   59000   Archaic  0.84636    20    12                11               12            11        11
-1      4500000   4510000   10000   Archaic  0.84457    7     5                 4                5             4         5
-1      5339000   5347000   8000    Archaic  0.58914    4     3                 2                3             0         3
-1      9322000   9355000   33000   Archaic  0.84751    9     0                 0                0             0         0
-1      12599000  12654000  55000   Archaic  0.9142     18    11                4                11            0         10
-
+1      2988000   2997000   9000    Archaic  0.76217    6     4                 4                4             1         4
+1      3425000   3452000   27000   Archaic  0.95816    22    17                17               15            3         17
+1      4302000   4361000   59000   Archaic  0.867      20    12                11               12            11        11
+1      4500000   4510000   10000   Archaic  0.8552     7     5                 4                5             4         5
+1      5306000   5319000   13000   Archaic  0.55584    4     1                 1                1             0         1
+1      5338000   5348000   10000   Archaic  0.65033    5     3                 2                3             0         3
+1      9321000   9355000   34000   Archaic  0.86414    9     0                 0                0             0         0
+1      12599000  12655000  56000   Archaic  0.91159    18    11                4                11            0         10
 ```
 
 For the first segment there are 6 derived snps. Of these snps 4 are shared with Altai,Vindija, Denisova and Chagyrskaya. Only 1 is shared with Denisova so this segment likeli introgressed from Neanderthals
 
 ---
 
 ### Run in python
```

### Comparing `hmmix-0.7.0/README.md` & `hmmix-0.7.1/src/hmmix.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,48 @@
-# Contact
-https://sites.google.com/view/laurits-skov
+Metadata-Version: 2.1
+Name: hmmix
+Version: 0.7.1
+Summary: Find introgressed segments
+Home-page: https://github.com/LauritsSkov/Introgression-detection
+Author: Laurits Skov and Moises Coll Macia
+Author-email: lauritsskov2@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Introgression detection
+
+## Contact
+
+<https://sites.google.com/view/laurits-skov>
 
 ---
 
-# Helpful files
-The outgroup files, mutation rate files and callability files and ancestral allele files are now premade! 
+## Helpful files
 
-https://doi.org/10.5281/zenodo.10806733 (hg19 and hg38)
+The outgroup files, mutation rate files, reference genomes, ancestral alleles and callability files and ancestral allele files are now premade!
 
-VCF file containing 4 high coverage archaic genomes (Altai, Vindija and Chagyrskaya Neanderthals and Denisovan) here: 
+<https://doi.org/10.5281/zenodo.11212339> (hg19 and hg38)
+Note the old version (<https://doi.org/10.5281/zenodo.10806733>) did not contain the ancestral alleles or reference genome and there was some missing data on the X chromosome.
 
-https://zenodo.org/records/7246376 (hg19)
+VCF file containing 4 high coverage archaic genomes (Altai, Vindija and Chagyrskaya Neanderthals and Denisovan) here:
 
-https://zenodo.org/records/10806726 (hg38)
+<https://zenodo.org/records/7246376> (hg19)
 
----
+<https://zenodo.org/records/10806726> (hg38)
 
-# Introgression detection
+---
 
 If you are working with archaic introgression into present-day humans of non-African ancestry you can use these files and skip the following steps:
-Find derived variants in outgroup and Estimate local mutation rate. 
+Find derived variants in outgroup and Estimate local mutation rate.
 
 These are the scripts needed to infere archaic introgression in modern populations using an unadmixed outgroup.
 
 1. [Installation](#installation)
 2. [Usage](#usage)
 3. [Quick tutorial](#quick-tutorial)
 4. [1000 genomes tutorial](#example-with-1000-genomes-data)
@@ -130,15 +149,15 @@
 
 > inhomogeneous                
     -obs                [required] file with observation data
     -chrom              Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3 (default is use all chromosomes)
     -weights            file with callability (defaults to all positions being called)
     -mutrates           file with mutation rates (default is mutation rate is uniform)
     -param              markov parameters file (default is human/neanderthal like parameters)
-    -out                outputfile prefix <out>.hap1.txt and <out>.hap2.txt if -haploid option is used or <out>.diploid.txt (default is stdout)
+    -out                outputfile prefix <out>.hap1_sim(0-n).txt and <out>.hap2_sim(0-n).txt if -haploid option is used or <out>.diploid_(0-n).txt (default is stdout)
     -window_size        size of bins (default is 1000 bp)
     -haploid            Change from using diploid data to haploid data (default is diploid)
     -samples            Number of simulated paths for the inhomogeneous markov chain (default is 100)
     -admixpop           Annotate using vcffile with admixing population (default is none)
     -extrainfo          Add variant position for each SNP (default is off)
 ```
 
@@ -274,21 +293,24 @@
 ---
 
 ## Example with 1000 genomes data
 
 ---
 
 The whole pipeline we will run looks like this. In the following section we will go through all the steps on the way
-NOTE: The outgroup files, mutation rate files and callability files are now premade! They can be downloaded in hg38 and hg19 here: https://doi.org/10.5281/zenodo.10806733
+
+NOTE: The outgroup files, mutation rate files, reference genomes, ancestral alleles and callability files and ancestral allele files are now premade!
+They can be downloaded in hg38 and hg19 here: <https://doi.org/10.5281/zenodo.11212339>
+
 But keep reading along if you want to know HOW the files were generated!
 
 ```note
-hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa -refgenome=referencegenome/*fa
+hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa -refgenome=hg19_refgenome/*fa
 hmmix mutation_rate -outgroup=outgroup.txt  -weights=strickmask.bed -window_size=1000000 -out mutationrate.bed
-hmmix create_ingroup  -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa
+hmmix create_ingroup  -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa
 hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.json 
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json 
 ```
 
 ### Getting data
 
 I thought it would be nice to have an entire reproduceble example of how to use this model. From a common starting point such as a VCF file (well a BCF file in this case) to the final output.  The reason for using BCF files is because it is MUCH faster to extract data for each individual. You can convert a vcf file to a bcf file like this:
@@ -311,25 +333,25 @@
 ftp.1000genomes.ebi.ac.uk/vol1/ftp/release/20130502/supporting/accessible_genome_masks/20141020.strict_mask.whole_genome.bed
 sed 's/^chr\|%$//g' 20141020.strict_mask.whole_genome.bed | awk '{print $1"\t"$2"\t"$3}' > strickmask.bed
 
 # outgroup information
 ftp://ftp.1000genomes.ebi.ac.uk/vol1/ftp/release/20130502/integrated_call_samples_v3.20130502.ALL.panel
 
 # Ancestral information
-ftp://ftp.ensembl.org/pub/release-74/fasta/ancestral_alleles/homo_sapiens_ancestor_GRCh37_e71.tar.bz2
+ftp://ftp.ensembl.org/pub/release-74/fasta/ancestral_alleles/hg19_ancestral.tar.bz2
 
 # Reference genome
 wget 'ftp://hgdownload.soe.ucsc.edu/goldenPath/hg19/bigZips/chromFa.tar.gz' -O chromFa.tar.gz
 
 # Archaic variants (Altai, Vindija, Chagyrskaya and Denisova in hg19)
 https://zenodo.org/records/7246376
 
 ```
 
-For this example we will use all individuals from 'YRI','MSL' and 'ESN' as outgroup individuals. While we will only be decoding hG00096 in this example you can add as many individuals as you want to the ingroup.  
+For this example we will use all individuals from 'YRI','MSL' and 'ESN' as outgroup individuals. While we will only be decoding HG00096 in this example you can add as many individuals as you want to the ingroup.  
 
 ```json
 {
   "ingroup": [
     "HG00096",
     "HG00097"
   ],
@@ -342,36 +364,57 @@
 }
 ```
 
 ---
 
 ### Finding snps which are derived in the outgroup
 
-First we need to find a set of variants found in the outgroup. We can use the wildcard character to loop through all bcf files. If you dont have ancestral information you can skip the ancestral argument.
-
-```bash
-(took an hour) > hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa 
+First we need to find a set of variants found in the outgroup. We can use the wildcard character to loop through all bcf files. It is best if you have files with the ancestral alleles (in FASTA format) and the reference genome (in FASTA format) but the program will run without.
 
-# Alternative usage (if you only have a few individual in the outgroup you can also provide a comma separated list)
-> hmmix create_outgroup -ind=HG02922,HG02923,HG02938 -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa 
+Something to note is that if you use an outgroup vcffile (like 1000 genomes) and an ingroup vcf file from a different dataset (like SGDP) there is an edge case which could occur. There could be recurrent mutations where every individual in 1000 genome has the derived variant and one individual in SGDP where the derived variant has mutated back to the ancestral allele. This means that this position will not be present in the outgroup file. However if a recurrent mutation occurs it will look like multiple individuals in the ingroup file have the mutation. This does not happen often but that is why I recommend having files with the ancestral allele and reference genome information.
 
-# Alternative usage (if you have no ancestral information)
-> hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt 
-
-# Alternative usage (if you only want to run the model on a subset of chromosomes, with or without ancestral information)
-> hmmix create_outgroup -ind=individuals.json -vcf=chr1.bcf,chr2.bcf -weights=strickmask.bed -out=outgroup.txt
-
-> hmmix create_outgroup -ind=individuals.json -vcf=chr1.bcf,chr2.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_1.fa,homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_2.fa
+```note
+# Recommended usage (if you want to remove sites which are fixed derived in your outgroup/ingroup). This is the file from zenodo. 
+(took two hours) > hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa -refgenome=hg19_refgenome/*fa
+----------------------------------------
+> Outgroup individuals: 292
+> Using vcf and ancestral files
+vcffile: chr1.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_1.fa reffile:  hg19_refgenome/chr1.fa
+vcffile: chr2.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_2.fa reffile:  hg19_refgenome/chr2.fa
+vcffile: chr3.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_3.fa reffile:  hg19_refgenome/chr3.fa
+vcffile: chr4.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_4.fa reffile:  hg19_refgenome/chr4.fa
+vcffile: chr5.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_5.fa reffile:  hg19_refgenome/chr5.fa
+vcffile: chr6.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_6.fa reffile:  hg19_refgenome/chr6.fa
+vcffile: chr7.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_7.fa reffile:  hg19_refgenome/chr7.fa
+vcffile: chr8.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_8.fa reffile:  hg19_refgenome/chr8.fa
+vcffile: chr9.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_9.fa reffile:  hg19_refgenome/chr9.fa
+vcffile: chr10.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_10.fa reffile: hg19_refgenome/chr10.fa
+vcffile: chr11.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_11.fa reffile: hg19_refgenome/chr11.fa
+vcffile: chr12.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_12.fa reffile: hg19_refgenome/chr12.fa
+vcffile: chr13.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_13.fa reffile: hg19_refgenome/chr13.fa
+vcffile: chr14.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_14.fa reffile: hg19_refgenome/chr14.fa
+vcffile: chr15.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_15.fa reffile: hg19_refgenome/chr15.fa
+vcffile: chr16.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_16.fa reffile: hg19_refgenome/chr16.fa
+vcffile: chr17.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_17.fa reffile: hg19_refgenome/chr17.fa
+vcffile: chr18.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_18.fa reffile: hg19_refgenome/chr18.fa
+vcffile: chr19.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_19.fa reffile: hg19_refgenome/chr19.fa
+vcffile: chr20.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_20.fa reffile: hg19_refgenome/chr20.fa
+vcffile: chr21.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_21.fa reffile: hg19_refgenome/chr21.fa
+vcffile: chr22.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_22.fa reffile: hg19_refgenome/chr22.fa
+vcffile: chrX.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_X.fa reffile:  hg19_refgenome/chrX.fa
+
+> Callability file: strickmask.bed
+> Writing output to: outgroup.txt
+----------------------------------------
 ```
 
-Something to note is that if you use an outgroup vcffile (like 1000 genomes) and an ingroup vcf file from a different dataset (like SGDP) there is an edge case which could occur. There could be recurrent mutations where every individual in 1000 genome has the derived variant and one individual in SGDP where the derived variant has mutated back to the ancestral allele. This means that this position will not be present in the outgroup file. However if a recurrent mutation occurs it will look like multiple individuals in the ingroup file have the mutation. This does not happen often but just in case you can create the outgroup file and adding the sites which are fixed derived in all individuals using the reference genome:
+Here it is important to check that hmmix matches up the reference, ancestral and vcffiles correctly e.g. chr1.bcf should fit with hg19_ancestral/homo_sapiens_ancestor_1.fa and hg19_refgenome/chr1.fa for instance. If you see an issue here its better to give the files as commaseparated values.
 
-```bash
-# Recommended usage (if you want to remove sites which are fixed derived in your outgroup/ingroup)
-> hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa -refgenome=*fa
+```note
+hmmix create_outgroup -ind=individuals.json -vcf=chr1.bcf,chr2.bcf,chr3.bcf,chr4.bcf,chr5.bcf,chr6.bcf,chr7.bcf,chr8.bcf,chr9.bcf,chr10.bcf,chr11.bcf,chr12.bcf,chr13.bcf,chr14.bcf,chr15.bcf,chr16.bcf,chr17.bcf,chr18.bcf,chr19.bcf,chr20.bcf,chr21.bcf,chr22.bcf,chrX.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_1.fa,hg19_ancestral/homo_sapiens_ancestor_2.fa,hg19_ancestral/homo_sapiens_ancestor_3.fa,hg19_ancestral/homo_sapiens_ancestor_4.fa,hg19_ancestral/homo_sapiens_ancestor_5.fa,hg19_ancestral/homo_sapiens_ancestor_6.fa,hg19_ancestral/homo_sapiens_ancestor_7.fa,hg19_ancestral/homo_sapiens_ancestor_8.fa,hg19_ancestral/homo_sapiens_ancestor_9.fa,hg19_ancestral/homo_sapiens_ancestor_10.fa,hg19_ancestral/homo_sapiens_ancestor_11.fa,hg19_ancestral/homo_sapiens_ancestor_12.fa,hg19_ancestral/homo_sapiens_ancestor_13.fa,hg19_ancestral/homo_sapiens_ancestor_14.fa,hg19_ancestral/homo_sapiens_ancestor_15.fa,hg19_ancestral/homo_sapiens_ancestor_16.fa,hg19_ancestral/homo_sapiens_ancestor_17.fa,hg19_ancestral/homo_sapiens_ancestor_18.fa,hg19_ancestral/homo_sapiens_ancestor_19.fa,hg19_ancestral/homo_sapiens_ancestor_20.fa,hg19_ancestral/homo_sapiens_ancestor_21.fa,hg19_ancestral/homo_sapiens_ancestor_22.fa,hg19_ancestral/homo_sapiens_ancestor_X.fa -refgenome=hg19_refgenome/chr1.fa,hg19_refgenome/chr2.fa,hg19_refgenome/chr3.fa,hg19_refgenome/chr4.fa,hg19_refgenome/chr5.fa,hg19_refgenome/chr6.fa,hg19_refgenome/chr7.fa,hg19_refgenome/chr8.fa,hg19_refgenome/chr9.fa,hg19_refgenome/chr10.fa,hg19_refgenome/chr11.fa,hg19_refgenome/chr12.fa,hg19_refgenome/chr13.fa,hg19_refgenome/chr14.fa,hg19_refgenome/chr15.fa,hg19_refgenome/chr16.fa,hg19_refgenome/chr17.fa,hg19_refgenome/chr18.fa,hg19_refgenome/chr19.fa,hg19_refgenome/chr20.fa,hg19_refgenome/chr21.fa,hg19_refgenome/chr22.fa,hg19_refgenome/chrX.fa
 ```
 
 ---
 
 ### Estimating mutation rate across genome
 
 We can use the number of variants in the outgroup to estimate the substitution rate as a proxy for mutation rate.
@@ -389,54 +432,55 @@
 ---
 
 ### Find a set of variants which are not derived in the outgroup
 
 Keep variants that are not found to be derived in the outgroup for each individual in ingroup. You can also speficy a single individual or a comma separated list of individuals.
 
 ```note
-(took 20 min) > hmmix create_ingroup  -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa
+(took 20 min) > hmmix create_ingroup  -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa
 ----------------------------------------
 > Ingroup individuals: 2
 > Using vcf and ancestral files
-vcffile: chr1.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_1.fa
-vcffile: chr2.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_2.fa
-vcffile: chr3.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_3.fa
-vcffile: chr4.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_4.fa
-vcffile: chr5.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_5.fa
-vcffile: chr6.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_6.fa
-vcffile: chr7.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_7.fa
-vcffile: chr8.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_8.fa
-vcffile: chr9.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_9.fa
-vcffile: chr10.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_10.fa
-vcffile: chr11.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_11.fa
-vcffile: chr12.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_12.fa
-vcffile: chr13.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_13.fa
-vcffile: chr14.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_14.fa
-vcffile: chr15.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_15.fa
-vcffile: chr16.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_16.fa
-vcffile: chr17.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_17.fa
-vcffile: chr18.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_18.fa
-vcffile: chr19.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_19.fa
-vcffile: chr20.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_20.fa
-vcffile: chr21.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_21.fa
-vcffile: chr22.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_22.fa
+vcffile: chr1.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_1.fa
+vcffile: chr2.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_2.fa
+vcffile: chr3.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_3.fa
+vcffile: chr4.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_4.fa
+vcffile: chr5.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_5.fa
+vcffile: chr6.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_6.fa
+vcffile: chr7.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_7.fa
+vcffile: chr8.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_8.fa
+vcffile: chr9.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_9.fa
+vcffile: chr10.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_10.fa
+vcffile: chr11.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_11.fa
+vcffile: chr12.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_12.fa
+vcffile: chr13.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_13.fa
+vcffile: chr14.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_14.fa
+vcffile: chr15.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_15.fa
+vcffile: chr16.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_16.fa
+vcffile: chr17.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_17.fa
+vcffile: chr18.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_18.fa
+vcffile: chr19.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_19.fa
+vcffile: chr20.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_20.fa
+vcffile: chr21.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_21.fa
+vcffile: chr22.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_22.fa
+vcffile: chrX.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_X.fa
 
 > Using outgroup variants from: outgroup.txt 
 > Callability file: strickmask.bed 
 > Writing output to file with prefix: obs.<individual>.txt
 
 ----------------------------------------
 Running command:
 bcftools view -m2 -M2 -v snps -s HG00096 -T strickmask.bed chr1.bcf | vcftools --vcf - --exclude-positions outgroup.txt --recode --stdout 
 ...
 bcftools view -m2 -M2 -v snps -s HG00097 -T strickmask.bed chr22.bcf | vcftools --vcf - --exclude-positions outgroup.txt --recode --stdout 
 
 
 # Different way to define which individuals are in the ingroup
-(took 20 min) > hmmix create_ingroup  -ind=HG00096,HG00097 -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa
+(took 20 min) > hmmix create_ingroup  -ind=HG00096,HG00097 -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa
 ```
 
 ---
 
 ### Training
 
 Now for training the HMM parameters and decoding
@@ -445,160 +489,160 @@
 (took 2 min) > hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.json 
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.98, 0.02]
 > transitions = [[1.0, 0.0], [0.02, 0.98]]
 > emissions = [0.04, 0.4]
 > chromosomes to use: All
-> number of windows: 2877010 . Number of snps =  129734
+> number of windows: 3032224 . Number of snps =  129803
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output is trained.HG00096.json
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 iteration  loglikelihood  start1  start2  emis1   emis2   trans1_1  trans2_2
-0          -492287.8643   0.98    0.02    0.04    0.4     0.9999    0.98
-1          -488898.6051   0.961   0.039   0.0483  0.3913  0.9994    0.986
-2          -488754.2455   0.958   0.042   0.0481  0.3911  0.9993    0.9835
+0          -495665.7379   0.98    0.02    0.04    0.4     0.9999    0.98
+1          -493092.9242   0.964   0.036   0.0459  0.3894  0.9995    0.9859
+2          -492917.6235   0.959   0.041   0.0455  0.3847  0.9993    0.9834
 ...
-19         -488641.0769   0.954   0.046   0.047   0.3862  0.9989    0.9771
-20         -488641.0755   0.954   0.046   0.047   0.3862  0.9989    0.9771
-21         -488641.0748   0.954   0.046   0.047   0.3862  0.9989    0.9771
+20         -492775.4072   0.954   0.046   0.0442  0.3725  0.9989    0.9768
+21         -492775.4058   0.954   0.046   0.0442  0.3725  0.9989    0.9768
+22         -492775.4049   0.954   0.046   0.0442  0.3725  0.9989    0.9768
 ```
 
 ---
 
 ### Decoding
 
 ```note
 (took 30 sec) > hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json 
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.954, 0.046]
 > transitions = [[0.999, 0.001], [0.023, 0.977]]
-> emissions = [0.047, 0.386]
+> emissions = [0.044, 0.372]
 > chromosomes to use: All
-> number of windows: 2877010 . Number of snps =  129734
+> number of windows: 3032224 . Number of snps =  129803
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 chrom  start    end      length   state    mean_prob  snps
-1      0        2988000  2988000  Human    0.98484    91
-1      2988000  2997000  9000     Archaic  0.71819    6
-1      2997000  3425000  428000   Human    0.98944    30
-1      3425000  3452000  27000    Archaic  0.95652    22
-1      3452000  4302000  850000   Human    0.98203    36
-1      4302000  4361000  59000    Archaic  0.84636    20
-1      4361000  4500000  139000   Human    0.97136    4
-1      4500000  4510000  10000    Archaic  0.84457    7
+1      0        2988000  2988000  Human    0.98429    91
+1      2988000  2997000  9000     Archaic  0.76217    6
+1      2997000  3425000  428000   Human    0.98776    30
+1      3425000  3452000  27000    Archaic  0.95816    22
+1      3452000  4302000  850000   Human    0.97917    36
+1      4302000  4361000  59000    Archaic  0.867      20
+1      4361000  4500000  139000   Human    0.96854    4
+1      4500000  4510000  10000    Archaic  0.8552     7
 ```
 
 You can also save to an output file with the command:
 
 ```note
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json -out=HG00096.decoded
 ```
 
 This will create a file named HG00096.decoded.diploid.txt because the default option is treating the data as diploid (more on haploid decoding in next chapter)
 
 ---
 
 ### Training and decoding with phased data
 
-It is also possible to tell the model that the data is phased with the -haploid parameter. For that we first need to train the parameters for haploid data and then decode. Training the model on phased data is done like this - and we also remember to change the name of the parameter file to include phased so future versions of ourselves don't forget. Another thing to note is that the number of snps is bigger than before 135411 vs 129734. This is because the program is counting snps on both haplotypes and homozygotes will be counted twice!
+It is also possible to tell the model that the data is phased with the -haploid parameter. For that we first need to train the parameters for haploid data and then decode. Training the model on phased data is done like this - and we also remember to change the name of the parameter file to include phased so future versions of ourselves don't forget. Another thing to note is that the number of snps is bigger than before 135483 vs 129803. This is because the program is counting snps on both haplotypes and homozygotes will be counted twice!
 
 ```note
 (took 4 min) > hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.phased.json -haploid
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.98, 0.02]
 > transitions = [[1.0, 0.0], [0.02, 0.98]]
 > emissions = [0.04, 0.4]
 > chromosomes to use: All
-> number of windows: 5754020 . Number of snps =  135411
+> number of windows: 6064448 . Number of snps =  135483
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output is trained.HG00096.phased.json
 > Window size is 1000 bp
 > Haploid True
 ----------------------------------------
 iteration  loglikelihood  start1  start2  emis1   emis2   trans1_1  trans2_2
-0          -597750.7043   0.98    0.02    0.04    0.4     0.9999    0.98
-1          -585028.8828   0.983   0.017   0.0261  0.4026  0.9998    0.9853
-2          -584447.5809   0.979   0.021   0.0252  0.373   0.9996    0.9826
+0          -605433.1928   0.98    0.02    0.04    0.4     0.9999    0.98
+1          -589492.2      0.985   0.015   0.0248  0.3999  0.9998    0.9852
+2          -588823.124    0.98    0.02    0.0238  0.3671  0.9996    0.9825
 ...
-19         -584131.0153   0.972   0.028   0.0241  0.3367  0.9993    0.9758
-20         -584131.0138   0.972   0.028   0.0241  0.3367  0.9993    0.9758
-21         -584131.013    0.972   0.028   0.0241  0.3366  0.9993    0.9758
+20         -588456.6027   0.973   0.027   0.0228  0.3267  0.9993    0.9755
+21         -588456.6015   0.973   0.027   0.0228  0.3266  0.9993    0.9755
+22         -588456.6009   0.973   0.027   0.0228  0.3266  0.9993    0.9755
 ```
 
-Below I am only showing the first archaic segments on chromosome 1 for each haplotype (note you have to scroll down after chrom 22 before the new haplotype begins). The seem to fall more or less in the same places as when we used diploid data.
+Below I am only showing the first archaic segments on chromosome 1 for each haplotype (note you have to scroll down after chrom X before the new haplotype begins). The seem to fall more or less in the same places as when we used diploid data.
 
 ```note
 (took 30 sec) > hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.phased.json -haploid
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
-> starting_probabilities = [0.972, 0.028]
+> starting_probabilities = [0.973, 0.027]
 > transitions = [[0.999, 0.001], [0.024, 0.976]]
-> emissions = [0.024, 0.337]
+> emissions = [0.023, 0.327]
 > chromosomes to use: All
-> number of windows: 5754020 . Number of snps =  135411
+> number of windows: 6064448 . Number of snps =  135483
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid True
 ----------------------------------------
 hap1
 chrom  start    end      length  state    mean_prob  snps
-1      2162000  2185000  23000   Archaic  0.61054    6
-1      3425000  3452000  27000   Archaic  0.96595    22
+1      2156000  2185000  29000   Archaic  0.64711    6
+1      3425000  3452000  27000   Archaic  0.96701    22
 
 ...
 hap2
-1      2780000  2803000  23000   Archaic  0.61948    7
-1      4302000  4337000  35000   Archaic  0.94008    13
-1      4500000  4511000  11000   Archaic  0.87592    7
-1      4989000  5000000  11000   Archaic  0.579      4
+1      2780000  2803000  23000   Archaic  0.68285    7
+1      4302000  4337000  35000   Archaic  0.94244    13
+1      4500000  4511000  11000   Archaic  0.87938    7
+1      4989000  5001000  12000   Archaic  0.61874    5
 ```
 
 You can also save to an output file with the command:
 
 ```note
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.phased.json -haploid -out=HG00096.decoded
 ```
 
 This will create two files named HG00096.decoded.hap1.txt and HG00096.decoded.hap2.txt
 
 ---
 
 ### Annotate with known admixing population
 
-Even though this method does not use archaic reference genomes for finding segments you can still use them to annotate your segments. 
+Even though this method does not use archaic reference genomes for finding segments you can still use them to annotate your segments.
 I have uploaded a VCF file containing 4 high coverage archaic genomes (3 Neanderthals and 1 Denisovan) here:
 
-https://zenodo.org/records/7246376 (hg19 - the one I use in this example)
+<https://zenodo.org/records/7246376> (hg19 - the one I use in this example)
 
-https://zenodo.org/records/10806726 (hg38)
+<https://zenodo.org/records/10806726> (hg38)
 
 If you have a vcf from the population that admixed in VCF/BCF format you can write this:
 
 ```note
 > hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json -admixpop=archaicvar/*bcf
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.954, 0.046]
 > transitions = [[0.999, 0.001], [0.023, 0.977]]
-> emissions = [0.047, 0.386]
+> emissions = [0.044, 0.372]
 > chromosomes to use: All
-> number of windows: 2877010 . Number of snps =  129734
+> number of windows: 3032224 . Number of snps =  129803
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_9.bcf
@@ -622,22 +666,22 @@
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_5.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_8.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_11.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_12.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_13.bcf
 
 chrom  start     end       length  state    mean_prob  snps  admixpopvariants  AltaiNeandertal  Vindija33.19  Denisova  Chagyrskaya-Phalanx
-1      2988000   2997000   9000    Archaic  0.71819    6     4                 4                4             1         4
-1      3425000   3452000   27000   Archaic  0.95652    22    17                17               15            3         17
-1      4302000   4361000   59000   Archaic  0.84636    20    12                11               12            11        11
-1      4500000   4510000   10000   Archaic  0.84457    7     5                 4                5             4         5
-1      5339000   5347000   8000    Archaic  0.58914    4     3                 2                3             0         3
-1      9322000   9355000   33000   Archaic  0.84751    9     0                 0                0             0         0
-1      12599000  12654000  55000   Archaic  0.9142     18    11                4                11            0         10
-
+1      2988000   2997000   9000    Archaic  0.76217    6     4                 4                4             1         4
+1      3425000   3452000   27000   Archaic  0.95816    22    17                17               15            3         17
+1      4302000   4361000   59000   Archaic  0.867      20    12                11               12            11        11
+1      4500000   4510000   10000   Archaic  0.8552     7     5                 4                5             4         5
+1      5306000   5319000   13000   Archaic  0.55584    4     1                 1                1             0         1
+1      5338000   5348000   10000   Archaic  0.65033    5     3                 2                3             0         3
+1      9321000   9355000   34000   Archaic  0.86414    9     0                 0                0             0         0
+1      12599000  12655000  56000   Archaic  0.91159    18    11                4                11            0         10
 ```
 
 For the first segment there are 6 derived snps. Of these snps 4 are shared with Altai,Vindija, Denisova and Chagyrskaya. Only 1 is shared with Denisova so this segment likeli introgressed from Neanderthals
 
 ---
 
 ### Run in python
@@ -694,7 +738,9 @@
 
 ```
 
 And that is it! Now you have run the model and gotten a set of parameters that you can interpret biologically (see my paper) and you have a list of segments that belong to the human and Archaic state.
 
 If you have any questions about the use of the scripts, if you find errors or if you have feedback you can contact my here (make an issue) or write to:
 lauritsskov2@gmail.com
+
+
```

### Comparing `hmmix-0.7.0/setup.py` & `hmmix-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='hmmix', 
-    version = '0.7.0',
+    version = '0.7.1',
     description='Find introgressed segments',
     py_modules=['bcf_vcf', 'helper_functions', 'hmm_functions', 'main', 'make_mutationrate', 'make_test_data'],
     package_dir={'': 'src'},
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

### Comparing `hmmix-0.7.0/src/bcf_vcf.py` & `hmmix-0.7.1/src/bcf_vcf.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.7.0/src/helper_functions.py` & `hmmix-0.7.1/src/helper_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,14 +199,35 @@
     with open(fasta_file) as data:
         for line in data:
             if not line.startswith('>'):
                 fasta_sequence += line.strip().upper()
 
     return fasta_sequence
 
+def sortby(x):
+    '''
+    This function is used in the sorted() function. It will sort first by numeric values, then strings then other symbols
+
+    Usage:
+    mylist = ['1', '12', '2', 3, 'MT', 'Y']
+    sortedlist = sorted(mylist, key=sortby)
+    returns ['1', '2', 3, '12', 'MT', 'Y']
+    '''
+
+    lower_case_letters = 'abcdefghijklmnopqrstuvwxyz'
+    if x.isnumeric():
+        return int(x)
+    elif type(x) == str and len(x) > 0:
+        if x[0].lower() in lower_case_letters:
+            return 1e6 + lower_case_letters.index(x[0].lower())
+        else:
+            return 2e6
+    else:
+        return 3e6
+    
 
 def get_consensus(infiles):
     '''
     Find consensus prefix, postfix and value that changes in set of files:
 
     myfiles = ['chr1.vcf', 'chr2.vcf', 'chr3.vcf']
     prefix, postfix, values = get_consensus(myfiles) 
@@ -236,39 +257,20 @@
         for value in consensus_strings:
 
             if len(value.split('|')) == 2:
                 prefix, postfix = value.split('|')
                 matches = len([x for x in infiles if prefix in x and postfix in x])
 
                 if matches == len(infiles):
-                    values = [x.replace(prefix, '').replace(postfix,'') for x in infiles]
-                    return prefix, postfix, set(values)
+                    values = set([x.replace(prefix, '').replace(postfix,'') for x in infiles])
+                    return prefix, postfix, sorted(values, key=sortby)
     else:
         return None, None, None
 
-def sortby(x):
-    '''
-    This function is used in the sorted() function. It will sort first by numeric values, then strings then other symbols
 
-    Usage:
-    mylist = ['1', '12', '2', 3, 'MT', 'Y']
-    sortedlist = sorted(mylist, key=sortby)
-    returns ['1', '2', 3, '12', 'MT', 'Y']
-    '''
-
-    lower_case_letters = 'abcdefghijklmnopqrstuvwxyz'
-    if x.isnumeric():
-        return int(x)
-    elif type(x) == str and len(x) > 0:
-        if x[0].lower() in lower_case_letters:
-            return 1e6 + lower_case_letters.index(x[0].lower())
-        else:
-            return 2e6
-    else:
-        return 3e6
     
 
 
 
 def sortby_haplotype(x):
     '''
     This function will sort haplotypes by number
@@ -425,30 +427,33 @@
 # Check which type of input we are dealing with
 def combined_files(ancestralfiles, vcffiles):
 
     # Get ancestral and vcf consensus
     prefix1, postfix1, values1 = get_consensus(vcffiles)
     prefix2, postfix2, values2 = get_consensus(ancestralfiles)
 
-    
     # No ancestral files
     if ancestralfiles == ['']:
         ancestralfiles = [None for _ in vcffiles]
+        vcffiles = [f'{prefix1}{x}{postfix1}' for x in values1]
         return ancestralfiles, vcffiles
 
     # Same length
     elif len(ancestralfiles) == len(vcffiles):
+        vcffiles = [f'{prefix1}{x}{postfix1}' for x in values1]
+        ancestralfiles = [f'{prefix2}{x}{postfix2}' for x in values2]
         return ancestralfiles, vcffiles
 
     # diff lengthts (both longer than 1)       
     elif len(ancestralfiles) > 1 and len(vcffiles) > 1:
+
         vcffiles = []
         ancestralfiles = []
 
-        for joined in sorted(values1.intersection(values2), key=sortby):
+        for joined in sorted(set(values1).intersection(set(values2)), key=sortby):
             vcffiles.append(''.join([prefix1, joined, postfix1]))
             ancestralfiles.append(''.join([prefix2, joined, postfix2]))
         return ancestralfiles, vcffiles
 
     # Many ancestral files only one vcf    
     elif len(ancestralfiles) > 1 and len(vcffiles) == 1:
         ancestralfiles = []
```

### Comparing `hmmix-0.7.0/src/hmm_functions.py` & `hmmix-0.7.1/src/hmm_functions.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.7.0/src/hmmix.egg-info/PKG-INFO` & `hmmix-0.7.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,32 @@
-Metadata-Version: 2.1
-Name: hmmix
-Version: 0.7.0
-Summary: Find introgressed segments
-Home-page: https://github.com/LauritsSkov/Introgression-detection
-Author: Laurits Skov and Moises Coll Macia
-Author-email: lauritsskov2@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+# Introgression detection
+
+## Contact
 
-# Contact
-https://sites.google.com/view/laurits-skov
+<https://sites.google.com/view/laurits-skov>
 
 ---
 
-# Helpful files
-The outgroup files, mutation rate files and callability files and ancestral allele files are now premade! 
+## Helpful files
 
-https://doi.org/10.5281/zenodo.10806733 (hg19 and hg38)
+The outgroup files, mutation rate files, reference genomes, ancestral alleles and callability files and ancestral allele files are now premade!
 
-VCF file containing 4 high coverage archaic genomes (Altai, Vindija and Chagyrskaya Neanderthals and Denisovan) here: 
+<https://doi.org/10.5281/zenodo.11212339> (hg19 and hg38)
+Note the old version (<https://doi.org/10.5281/zenodo.10806733>) did not contain the ancestral alleles or reference genome and there was some missing data on the X chromosome.
 
-https://zenodo.org/records/7246376 (hg19)
+VCF file containing 4 high coverage archaic genomes (Altai, Vindija and Chagyrskaya Neanderthals and Denisovan) here:
 
-https://zenodo.org/records/10806726 (hg38)
+<https://zenodo.org/records/7246376> (hg19)
 
----
+<https://zenodo.org/records/10806726> (hg38)
 
-# Introgression detection
+---
 
 If you are working with archaic introgression into present-day humans of non-African ancestry you can use these files and skip the following steps:
-Find derived variants in outgroup and Estimate local mutation rate. 
+Find derived variants in outgroup and Estimate local mutation rate.
 
 These are the scripts needed to infere archaic introgression in modern populations using an unadmixed outgroup.
 
 1. [Installation](#installation)
 2. [Usage](#usage)
 3. [Quick tutorial](#quick-tutorial)
 4. [1000 genomes tutorial](#example-with-1000-genomes-data)
@@ -146,15 +133,15 @@
 
 > inhomogeneous                
     -obs                [required] file with observation data
     -chrom              Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3 (default is use all chromosomes)
     -weights            file with callability (defaults to all positions being called)
     -mutrates           file with mutation rates (default is mutation rate is uniform)
     -param              markov parameters file (default is human/neanderthal like parameters)
-    -out                outputfile prefix <out>.hap1.txt and <out>.hap2.txt if -haploid option is used or <out>.diploid.txt (default is stdout)
+    -out                outputfile prefix <out>.hap1_sim(0-n).txt and <out>.hap2_sim(0-n).txt if -haploid option is used or <out>.diploid_(0-n).txt (default is stdout)
     -window_size        size of bins (default is 1000 bp)
     -haploid            Change from using diploid data to haploid data (default is diploid)
     -samples            Number of simulated paths for the inhomogeneous markov chain (default is 100)
     -admixpop           Annotate using vcffile with admixing population (default is none)
     -extrainfo          Add variant position for each SNP (default is off)
 ```
 
@@ -290,21 +277,24 @@
 ---
 
 ## Example with 1000 genomes data
 
 ---
 
 The whole pipeline we will run looks like this. In the following section we will go through all the steps on the way
-NOTE: The outgroup files, mutation rate files and callability files are now premade! They can be downloaded in hg38 and hg19 here: https://doi.org/10.5281/zenodo.10806733
+
+NOTE: The outgroup files, mutation rate files, reference genomes, ancestral alleles and callability files and ancestral allele files are now premade!
+They can be downloaded in hg38 and hg19 here: <https://doi.org/10.5281/zenodo.11212339>
+
 But keep reading along if you want to know HOW the files were generated!
 
 ```note
-hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa -refgenome=referencegenome/*fa
+hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa -refgenome=hg19_refgenome/*fa
 hmmix mutation_rate -outgroup=outgroup.txt  -weights=strickmask.bed -window_size=1000000 -out mutationrate.bed
-hmmix create_ingroup  -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa
+hmmix create_ingroup  -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa
 hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.json 
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json 
 ```
 
 ### Getting data
 
 I thought it would be nice to have an entire reproduceble example of how to use this model. From a common starting point such as a VCF file (well a BCF file in this case) to the final output.  The reason for using BCF files is because it is MUCH faster to extract data for each individual. You can convert a vcf file to a bcf file like this:
@@ -327,25 +317,25 @@
 ftp.1000genomes.ebi.ac.uk/vol1/ftp/release/20130502/supporting/accessible_genome_masks/20141020.strict_mask.whole_genome.bed
 sed 's/^chr\|%$//g' 20141020.strict_mask.whole_genome.bed | awk '{print $1"\t"$2"\t"$3}' > strickmask.bed
 
 # outgroup information
 ftp://ftp.1000genomes.ebi.ac.uk/vol1/ftp/release/20130502/integrated_call_samples_v3.20130502.ALL.panel
 
 # Ancestral information
-ftp://ftp.ensembl.org/pub/release-74/fasta/ancestral_alleles/homo_sapiens_ancestor_GRCh37_e71.tar.bz2
+ftp://ftp.ensembl.org/pub/release-74/fasta/ancestral_alleles/hg19_ancestral.tar.bz2
 
 # Reference genome
 wget 'ftp://hgdownload.soe.ucsc.edu/goldenPath/hg19/bigZips/chromFa.tar.gz' -O chromFa.tar.gz
 
 # Archaic variants (Altai, Vindija, Chagyrskaya and Denisova in hg19)
 https://zenodo.org/records/7246376
 
 ```
 
-For this example we will use all individuals from 'YRI','MSL' and 'ESN' as outgroup individuals. While we will only be decoding hG00096 in this example you can add as many individuals as you want to the ingroup.  
+For this example we will use all individuals from 'YRI','MSL' and 'ESN' as outgroup individuals. While we will only be decoding HG00096 in this example you can add as many individuals as you want to the ingroup.  
 
 ```json
 {
   "ingroup": [
     "HG00096",
     "HG00097"
   ],
@@ -358,36 +348,57 @@
 }
 ```
 
 ---
 
 ### Finding snps which are derived in the outgroup
 
-First we need to find a set of variants found in the outgroup. We can use the wildcard character to loop through all bcf files. If you dont have ancestral information you can skip the ancestral argument.
-
-```bash
-(took an hour) > hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa 
-
-# Alternative usage (if you only have a few individual in the outgroup you can also provide a comma separated list)
-> hmmix create_outgroup -ind=HG02922,HG02923,HG02938 -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa 
+First we need to find a set of variants found in the outgroup. We can use the wildcard character to loop through all bcf files. It is best if you have files with the ancestral alleles (in FASTA format) and the reference genome (in FASTA format) but the program will run without.
 
-# Alternative usage (if you have no ancestral information)
-> hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt 
+Something to note is that if you use an outgroup vcffile (like 1000 genomes) and an ingroup vcf file from a different dataset (like SGDP) there is an edge case which could occur. There could be recurrent mutations where every individual in 1000 genome has the derived variant and one individual in SGDP where the derived variant has mutated back to the ancestral allele. This means that this position will not be present in the outgroup file. However if a recurrent mutation occurs it will look like multiple individuals in the ingroup file have the mutation. This does not happen often but that is why I recommend having files with the ancestral allele and reference genome information.
 
-# Alternative usage (if you only want to run the model on a subset of chromosomes, with or without ancestral information)
-> hmmix create_outgroup -ind=individuals.json -vcf=chr1.bcf,chr2.bcf -weights=strickmask.bed -out=outgroup.txt
-
-> hmmix create_outgroup -ind=individuals.json -vcf=chr1.bcf,chr2.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_1.fa,homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_2.fa
+```note
+# Recommended usage (if you want to remove sites which are fixed derived in your outgroup/ingroup). This is the file from zenodo. 
+(took two hours) > hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa -refgenome=hg19_refgenome/*fa
+----------------------------------------
+> Outgroup individuals: 292
+> Using vcf and ancestral files
+vcffile: chr1.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_1.fa reffile:  hg19_refgenome/chr1.fa
+vcffile: chr2.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_2.fa reffile:  hg19_refgenome/chr2.fa
+vcffile: chr3.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_3.fa reffile:  hg19_refgenome/chr3.fa
+vcffile: chr4.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_4.fa reffile:  hg19_refgenome/chr4.fa
+vcffile: chr5.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_5.fa reffile:  hg19_refgenome/chr5.fa
+vcffile: chr6.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_6.fa reffile:  hg19_refgenome/chr6.fa
+vcffile: chr7.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_7.fa reffile:  hg19_refgenome/chr7.fa
+vcffile: chr8.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_8.fa reffile:  hg19_refgenome/chr8.fa
+vcffile: chr9.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_9.fa reffile:  hg19_refgenome/chr9.fa
+vcffile: chr10.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_10.fa reffile: hg19_refgenome/chr10.fa
+vcffile: chr11.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_11.fa reffile: hg19_refgenome/chr11.fa
+vcffile: chr12.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_12.fa reffile: hg19_refgenome/chr12.fa
+vcffile: chr13.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_13.fa reffile: hg19_refgenome/chr13.fa
+vcffile: chr14.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_14.fa reffile: hg19_refgenome/chr14.fa
+vcffile: chr15.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_15.fa reffile: hg19_refgenome/chr15.fa
+vcffile: chr16.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_16.fa reffile: hg19_refgenome/chr16.fa
+vcffile: chr17.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_17.fa reffile: hg19_refgenome/chr17.fa
+vcffile: chr18.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_18.fa reffile: hg19_refgenome/chr18.fa
+vcffile: chr19.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_19.fa reffile: hg19_refgenome/chr19.fa
+vcffile: chr20.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_20.fa reffile: hg19_refgenome/chr20.fa
+vcffile: chr21.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_21.fa reffile: hg19_refgenome/chr21.fa
+vcffile: chr22.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_22.fa reffile: hg19_refgenome/chr22.fa
+vcffile: chrX.bcf ancestralfile:  hg19_ancestral/homo_sapiens_ancestor_X.fa reffile:  hg19_refgenome/chrX.fa
+
+> Callability file: strickmask.bed
+> Writing output to: outgroup.txt
+----------------------------------------
 ```
 
-Something to note is that if you use an outgroup vcffile (like 1000 genomes) and an ingroup vcf file from a different dataset (like SGDP) there is an edge case which could occur. There could be recurrent mutations where every individual in 1000 genome has the derived variant and one individual in SGDP where the derived variant has mutated back to the ancestral allele. This means that this position will not be present in the outgroup file. However if a recurrent mutation occurs it will look like multiple individuals in the ingroup file have the mutation. This does not happen often but just in case you can create the outgroup file and adding the sites which are fixed derived in all individuals using the reference genome:
+Here it is important to check that hmmix matches up the reference, ancestral and vcffiles correctly e.g. chr1.bcf should fit with hg19_ancestral/homo_sapiens_ancestor_1.fa and hg19_refgenome/chr1.fa for instance. If you see an issue here its better to give the files as commaseparated values.
 
-```bash
-# Recommended usage (if you want to remove sites which are fixed derived in your outgroup/ingroup)
-> hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa -refgenome=*fa
+```note
+hmmix create_outgroup -ind=individuals.json -vcf=chr1.bcf,chr2.bcf,chr3.bcf,chr4.bcf,chr5.bcf,chr6.bcf,chr7.bcf,chr8.bcf,chr9.bcf,chr10.bcf,chr11.bcf,chr12.bcf,chr13.bcf,chr14.bcf,chr15.bcf,chr16.bcf,chr17.bcf,chr18.bcf,chr19.bcf,chr20.bcf,chr21.bcf,chr22.bcf,chrX.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_1.fa,hg19_ancestral/homo_sapiens_ancestor_2.fa,hg19_ancestral/homo_sapiens_ancestor_3.fa,hg19_ancestral/homo_sapiens_ancestor_4.fa,hg19_ancestral/homo_sapiens_ancestor_5.fa,hg19_ancestral/homo_sapiens_ancestor_6.fa,hg19_ancestral/homo_sapiens_ancestor_7.fa,hg19_ancestral/homo_sapiens_ancestor_8.fa,hg19_ancestral/homo_sapiens_ancestor_9.fa,hg19_ancestral/homo_sapiens_ancestor_10.fa,hg19_ancestral/homo_sapiens_ancestor_11.fa,hg19_ancestral/homo_sapiens_ancestor_12.fa,hg19_ancestral/homo_sapiens_ancestor_13.fa,hg19_ancestral/homo_sapiens_ancestor_14.fa,hg19_ancestral/homo_sapiens_ancestor_15.fa,hg19_ancestral/homo_sapiens_ancestor_16.fa,hg19_ancestral/homo_sapiens_ancestor_17.fa,hg19_ancestral/homo_sapiens_ancestor_18.fa,hg19_ancestral/homo_sapiens_ancestor_19.fa,hg19_ancestral/homo_sapiens_ancestor_20.fa,hg19_ancestral/homo_sapiens_ancestor_21.fa,hg19_ancestral/homo_sapiens_ancestor_22.fa,hg19_ancestral/homo_sapiens_ancestor_X.fa -refgenome=hg19_refgenome/chr1.fa,hg19_refgenome/chr2.fa,hg19_refgenome/chr3.fa,hg19_refgenome/chr4.fa,hg19_refgenome/chr5.fa,hg19_refgenome/chr6.fa,hg19_refgenome/chr7.fa,hg19_refgenome/chr8.fa,hg19_refgenome/chr9.fa,hg19_refgenome/chr10.fa,hg19_refgenome/chr11.fa,hg19_refgenome/chr12.fa,hg19_refgenome/chr13.fa,hg19_refgenome/chr14.fa,hg19_refgenome/chr15.fa,hg19_refgenome/chr16.fa,hg19_refgenome/chr17.fa,hg19_refgenome/chr18.fa,hg19_refgenome/chr19.fa,hg19_refgenome/chr20.fa,hg19_refgenome/chr21.fa,hg19_refgenome/chr22.fa,hg19_refgenome/chrX.fa
 ```
 
 ---
 
 ### Estimating mutation rate across genome
 
 We can use the number of variants in the outgroup to estimate the substitution rate as a proxy for mutation rate.
@@ -405,54 +416,55 @@
 ---
 
 ### Find a set of variants which are not derived in the outgroup
 
 Keep variants that are not found to be derived in the outgroup for each individual in ingroup. You can also speficy a single individual or a comma separated list of individuals.
 
 ```note
-(took 20 min) > hmmix create_ingroup  -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa
+(took 20 min) > hmmix create_ingroup  -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa
 ----------------------------------------
 > Ingroup individuals: 2
 > Using vcf and ancestral files
-vcffile: chr1.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_1.fa
-vcffile: chr2.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_2.fa
-vcffile: chr3.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_3.fa
-vcffile: chr4.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_4.fa
-vcffile: chr5.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_5.fa
-vcffile: chr6.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_6.fa
-vcffile: chr7.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_7.fa
-vcffile: chr8.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_8.fa
-vcffile: chr9.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_9.fa
-vcffile: chr10.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_10.fa
-vcffile: chr11.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_11.fa
-vcffile: chr12.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_12.fa
-vcffile: chr13.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_13.fa
-vcffile: chr14.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_14.fa
-vcffile: chr15.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_15.fa
-vcffile: chr16.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_16.fa
-vcffile: chr17.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_17.fa
-vcffile: chr18.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_18.fa
-vcffile: chr19.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_19.fa
-vcffile: chr20.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_20.fa
-vcffile: chr21.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_21.fa
-vcffile: chr22.bcf ancestralfile: homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_22.fa
+vcffile: chr1.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_1.fa
+vcffile: chr2.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_2.fa
+vcffile: chr3.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_3.fa
+vcffile: chr4.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_4.fa
+vcffile: chr5.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_5.fa
+vcffile: chr6.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_6.fa
+vcffile: chr7.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_7.fa
+vcffile: chr8.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_8.fa
+vcffile: chr9.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_9.fa
+vcffile: chr10.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_10.fa
+vcffile: chr11.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_11.fa
+vcffile: chr12.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_12.fa
+vcffile: chr13.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_13.fa
+vcffile: chr14.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_14.fa
+vcffile: chr15.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_15.fa
+vcffile: chr16.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_16.fa
+vcffile: chr17.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_17.fa
+vcffile: chr18.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_18.fa
+vcffile: chr19.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_19.fa
+vcffile: chr20.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_20.fa
+vcffile: chr21.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_21.fa
+vcffile: chr22.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_22.fa
+vcffile: chrX.bcf ancestralfile: hg19_ancestral/homo_sapiens_ancestor_X.fa
 
 > Using outgroup variants from: outgroup.txt 
 > Callability file: strickmask.bed 
 > Writing output to file with prefix: obs.<individual>.txt
 
 ----------------------------------------
 Running command:
 bcftools view -m2 -M2 -v snps -s HG00096 -T strickmask.bed chr1.bcf | vcftools --vcf - --exclude-positions outgroup.txt --recode --stdout 
 ...
 bcftools view -m2 -M2 -v snps -s HG00097 -T strickmask.bed chr22.bcf | vcftools --vcf - --exclude-positions outgroup.txt --recode --stdout 
 
 
 # Different way to define which individuals are in the ingroup
-(took 20 min) > hmmix create_ingroup  -ind=HG00096,HG00097 -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=homo_sapiens_ancestor_GRCh37_e71/homo_sapiens_ancestor_*.fa
+(took 20 min) > hmmix create_ingroup  -ind=HG00096,HG00097 -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa
 ```
 
 ---
 
 ### Training
 
 Now for training the HMM parameters and decoding
@@ -461,160 +473,160 @@
 (took 2 min) > hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.json 
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.98, 0.02]
 > transitions = [[1.0, 0.0], [0.02, 0.98]]
 > emissions = [0.04, 0.4]
 > chromosomes to use: All
-> number of windows: 2877010 . Number of snps =  129734
+> number of windows: 3032224 . Number of snps =  129803
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output is trained.HG00096.json
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 iteration  loglikelihood  start1  start2  emis1   emis2   trans1_1  trans2_2
-0          -492287.8643   0.98    0.02    0.04    0.4     0.9999    0.98
-1          -488898.6051   0.961   0.039   0.0483  0.3913  0.9994    0.986
-2          -488754.2455   0.958   0.042   0.0481  0.3911  0.9993    0.9835
+0          -495665.7379   0.98    0.02    0.04    0.4     0.9999    0.98
+1          -493092.9242   0.964   0.036   0.0459  0.3894  0.9995    0.9859
+2          -492917.6235   0.959   0.041   0.0455  0.3847  0.9993    0.9834
 ...
-19         -488641.0769   0.954   0.046   0.047   0.3862  0.9989    0.9771
-20         -488641.0755   0.954   0.046   0.047   0.3862  0.9989    0.9771
-21         -488641.0748   0.954   0.046   0.047   0.3862  0.9989    0.9771
+20         -492775.4072   0.954   0.046   0.0442  0.3725  0.9989    0.9768
+21         -492775.4058   0.954   0.046   0.0442  0.3725  0.9989    0.9768
+22         -492775.4049   0.954   0.046   0.0442  0.3725  0.9989    0.9768
 ```
 
 ---
 
 ### Decoding
 
 ```note
 (took 30 sec) > hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json 
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.954, 0.046]
 > transitions = [[0.999, 0.001], [0.023, 0.977]]
-> emissions = [0.047, 0.386]
+> emissions = [0.044, 0.372]
 > chromosomes to use: All
-> number of windows: 2877010 . Number of snps =  129734
+> number of windows: 3032224 . Number of snps =  129803
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 chrom  start    end      length   state    mean_prob  snps
-1      0        2988000  2988000  Human    0.98484    91
-1      2988000  2997000  9000     Archaic  0.71819    6
-1      2997000  3425000  428000   Human    0.98944    30
-1      3425000  3452000  27000    Archaic  0.95652    22
-1      3452000  4302000  850000   Human    0.98203    36
-1      4302000  4361000  59000    Archaic  0.84636    20
-1      4361000  4500000  139000   Human    0.97136    4
-1      4500000  4510000  10000    Archaic  0.84457    7
+1      0        2988000  2988000  Human    0.98429    91
+1      2988000  2997000  9000     Archaic  0.76217    6
+1      2997000  3425000  428000   Human    0.98776    30
+1      3425000  3452000  27000    Archaic  0.95816    22
+1      3452000  4302000  850000   Human    0.97917    36
+1      4302000  4361000  59000    Archaic  0.867      20
+1      4361000  4500000  139000   Human    0.96854    4
+1      4500000  4510000  10000    Archaic  0.8552     7
 ```
 
 You can also save to an output file with the command:
 
 ```note
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json -out=HG00096.decoded
 ```
 
 This will create a file named HG00096.decoded.diploid.txt because the default option is treating the data as diploid (more on haploid decoding in next chapter)
 
 ---
 
 ### Training and decoding with phased data
 
-It is also possible to tell the model that the data is phased with the -haploid parameter. For that we first need to train the parameters for haploid data and then decode. Training the model on phased data is done like this - and we also remember to change the name of the parameter file to include phased so future versions of ourselves don't forget. Another thing to note is that the number of snps is bigger than before 135411 vs 129734. This is because the program is counting snps on both haplotypes and homozygotes will be counted twice!
+It is also possible to tell the model that the data is phased with the -haploid parameter. For that we first need to train the parameters for haploid data and then decode. Training the model on phased data is done like this - and we also remember to change the name of the parameter file to include phased so future versions of ourselves don't forget. Another thing to note is that the number of snps is bigger than before 135483 vs 129803. This is because the program is counting snps on both haplotypes and homozygotes will be counted twice!
 
 ```note
 (took 4 min) > hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.phased.json -haploid
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.98, 0.02]
 > transitions = [[1.0, 0.0], [0.02, 0.98]]
 > emissions = [0.04, 0.4]
 > chromosomes to use: All
-> number of windows: 5754020 . Number of snps =  135411
+> number of windows: 6064448 . Number of snps =  135483
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output is trained.HG00096.phased.json
 > Window size is 1000 bp
 > Haploid True
 ----------------------------------------
 iteration  loglikelihood  start1  start2  emis1   emis2   trans1_1  trans2_2
-0          -597750.7043   0.98    0.02    0.04    0.4     0.9999    0.98
-1          -585028.8828   0.983   0.017   0.0261  0.4026  0.9998    0.9853
-2          -584447.5809   0.979   0.021   0.0252  0.373   0.9996    0.9826
+0          -605433.1928   0.98    0.02    0.04    0.4     0.9999    0.98
+1          -589492.2      0.985   0.015   0.0248  0.3999  0.9998    0.9852
+2          -588823.124    0.98    0.02    0.0238  0.3671  0.9996    0.9825
 ...
-19         -584131.0153   0.972   0.028   0.0241  0.3367  0.9993    0.9758
-20         -584131.0138   0.972   0.028   0.0241  0.3367  0.9993    0.9758
-21         -584131.013    0.972   0.028   0.0241  0.3366  0.9993    0.9758
+20         -588456.6027   0.973   0.027   0.0228  0.3267  0.9993    0.9755
+21         -588456.6015   0.973   0.027   0.0228  0.3266  0.9993    0.9755
+22         -588456.6009   0.973   0.027   0.0228  0.3266  0.9993    0.9755
 ```
 
-Below I am only showing the first archaic segments on chromosome 1 for each haplotype (note you have to scroll down after chrom 22 before the new haplotype begins). The seem to fall more or less in the same places as when we used diploid data.
+Below I am only showing the first archaic segments on chromosome 1 for each haplotype (note you have to scroll down after chrom X before the new haplotype begins). The seem to fall more or less in the same places as when we used diploid data.
 
 ```note
 (took 30 sec) > hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.phased.json -haploid
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
-> starting_probabilities = [0.972, 0.028]
+> starting_probabilities = [0.973, 0.027]
 > transitions = [[0.999, 0.001], [0.024, 0.976]]
-> emissions = [0.024, 0.337]
+> emissions = [0.023, 0.327]
 > chromosomes to use: All
-> number of windows: 5754020 . Number of snps =  135411
+> number of windows: 6064448 . Number of snps =  135483
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid True
 ----------------------------------------
 hap1
 chrom  start    end      length  state    mean_prob  snps
-1      2162000  2185000  23000   Archaic  0.61054    6
-1      3425000  3452000  27000   Archaic  0.96595    22
+1      2156000  2185000  29000   Archaic  0.64711    6
+1      3425000  3452000  27000   Archaic  0.96701    22
 
 ...
 hap2
-1      2780000  2803000  23000   Archaic  0.61948    7
-1      4302000  4337000  35000   Archaic  0.94008    13
-1      4500000  4511000  11000   Archaic  0.87592    7
-1      4989000  5000000  11000   Archaic  0.579      4
+1      2780000  2803000  23000   Archaic  0.68285    7
+1      4302000  4337000  35000   Archaic  0.94244    13
+1      4500000  4511000  11000   Archaic  0.87938    7
+1      4989000  5001000  12000   Archaic  0.61874    5
 ```
 
 You can also save to an output file with the command:
 
 ```note
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.phased.json -haploid -out=HG00096.decoded
 ```
 
 This will create two files named HG00096.decoded.hap1.txt and HG00096.decoded.hap2.txt
 
 ---
 
 ### Annotate with known admixing population
 
-Even though this method does not use archaic reference genomes for finding segments you can still use them to annotate your segments. 
+Even though this method does not use archaic reference genomes for finding segments you can still use them to annotate your segments.
 I have uploaded a VCF file containing 4 high coverage archaic genomes (3 Neanderthals and 1 Denisovan) here:
 
-https://zenodo.org/records/7246376 (hg19 - the one I use in this example)
+<https://zenodo.org/records/7246376> (hg19 - the one I use in this example)
 
-https://zenodo.org/records/10806726 (hg38)
+<https://zenodo.org/records/10806726> (hg38)
 
 If you have a vcf from the population that admixed in VCF/BCF format you can write this:
 
 ```note
 > hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json -admixpop=archaicvar/*bcf
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.954, 0.046]
 > transitions = [[0.999, 0.001], [0.023, 0.977]]
-> emissions = [0.047, 0.386]
+> emissions = [0.044, 0.372]
 > chromosomes to use: All
-> number of windows: 2877010 . Number of snps =  129734
+> number of windows: 3032224 . Number of snps =  129803
 > total callability: 0.72
 > average mutation rate per bin: 1.0
 > Output prefix is /dev/stdout
 > Window size is 1000 bp
 > Haploid False
 ----------------------------------------
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_9.bcf
@@ -638,22 +650,22 @@
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_5.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_8.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_11.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_12.bcf
 bcftools view -a -R obs.HG00096.txttemp archaicvar/highcov_ind_13.bcf
 
 chrom  start     end       length  state    mean_prob  snps  admixpopvariants  AltaiNeandertal  Vindija33.19  Denisova  Chagyrskaya-Phalanx
-1      2988000   2997000   9000    Archaic  0.71819    6     4                 4                4             1         4
-1      3425000   3452000   27000   Archaic  0.95652    22    17                17               15            3         17
-1      4302000   4361000   59000   Archaic  0.84636    20    12                11               12            11        11
-1      4500000   4510000   10000   Archaic  0.84457    7     5                 4                5             4         5
-1      5339000   5347000   8000    Archaic  0.58914    4     3                 2                3             0         3
-1      9322000   9355000   33000   Archaic  0.84751    9     0                 0                0             0         0
-1      12599000  12654000  55000   Archaic  0.9142     18    11                4                11            0         10
-
+1      2988000   2997000   9000    Archaic  0.76217    6     4                 4                4             1         4
+1      3425000   3452000   27000   Archaic  0.95816    22    17                17               15            3         17
+1      4302000   4361000   59000   Archaic  0.867      20    12                11               12            11        11
+1      4500000   4510000   10000   Archaic  0.8552     7     5                 4                5             4         5
+1      5306000   5319000   13000   Archaic  0.55584    4     1                 1                1             0         1
+1      5338000   5348000   10000   Archaic  0.65033    5     3                 2                3             0         3
+1      9321000   9355000   34000   Archaic  0.86414    9     0                 0                0             0         0
+1      12599000  12655000  56000   Archaic  0.91159    18    11                4                11            0         10
 ```
 
 For the first segment there are 6 derived snps. Of these snps 4 are shared with Altai,Vindija, Denisova and Chagyrskaya. Only 1 is shared with Denisova so this segment likeli introgressed from Neanderthals
 
 ---
 
 ### Run in python
@@ -710,9 +722,7 @@
 
 ```
 
 And that is it! Now you have run the model and gotten a set of parameters that you can interpret biologically (see my paper) and you have a list of segments that belong to the human and Archaic state.
 
 If you have any questions about the use of the scripts, if you find errors or if you have feedback you can contact my here (make an issue) or write to:
 lauritsskov2@gmail.com
-
-
```

### Comparing `hmmix-0.7.0/src/main.py` & `hmmix-0.7.1/src/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from hmm_functions import TrainModel, DecodeModel, write_HMM_to_file, read_HMM_parameters_from_file, Write_Decoded_output, inhomogeneous
 from bcf_vcf import make_out_group, make_ingroup_obs
 from make_test_data import create_test_data
 from make_mutationrate import make_mutation_rate
 from helper_functions import Load_observations_weights_mutrates, handle_individuals_input, handle_infiles, combined_files
 
 
-VERSION = '0.7.0'
+VERSION = '0.7.1'
 
 
 def print_script_usage():
     toprint = f'''
 Script for identifying introgressed archaic segments (version: {VERSION})
 
 > Turorial:
@@ -73,15 +73,15 @@
 
 > inhomogeneous                
     -obs                [required] file with observation data
     -chrom              Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3 (default is use all chromosomes)
     -weights            file with callability (defaults to all positions being called)
     -mutrates           file with mutation rates (default is mutation rate is uniform)
     -param              markov parameters file (default is human/neanderthal like parameters)
-    -out                outputfile prefix <out>.hap1.txt and <out>.hap2.txt if -haploid option is used or <out>.diploid.txt (default is stdout)
+    -out                outputfile prefix <out>.hap1_sim(0-n).txt and <out>.hap2_sim(0-n).txt if -haploid option is used or <out>.diploid_(0-n).txt (default is stdout)
     -window_size        size of bins (default is 1000 bp)
     -haploid            Change from using diploid data to haploid data (default is diploid)
     -samples            Number of simulated paths for the inhomogeneous markov chain (default is 100)
     -admixpop           Annotate using vcffile with admixing population (default is none)
     -extrainfo          Add variant position for each SNP (default is off)
     '''
 
@@ -273,15 +273,15 @@
         for vcffile, ancestralfile, reffile in zip(vcffiles, ancestralfiles, refgenomefiles):
             print('vcffile:',vcffile, 'ancestralfile:',ancestralfile, 'reffile:', reffile)
         print()    
         print('> Callability file:',  args.weights)
         print(f'> Writing output to:', args.out)
         print('-' * 40)
 
-
+        
         make_out_group(outgroup_individuals, args.weights, vcffiles, args.out, ancestralfiles, refgenomefiles)
 
 
 
 
     # Create ingroup observations
     # ------------------------------------------------------------------------------------------------------------
```

### Comparing `hmmix-0.7.0/src/make_mutationrate.py` & `hmmix-0.7.1/src/make_mutationrate.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.7.0/src/make_test_data.py` & `hmmix-0.7.1/src/make_test_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,19 +45,14 @@
             
             # Use prior dist if starting window
             if index == 0:
                 current_state = np.random.choice(state_values, p=hmm_parameters.starting_probabilities)
             else:
                 current_state = np.random.choice(state_values, p=hmm_parameters.transitions[prevstate] )
 
-            # if 300 < index < 400:
-            #     current_state = 1
-            # else:
-            #     current_state = 0
-
             n_mutations = np.random.poisson(lam=hmm_parameters.emissions[current_state]) 
             for mutation in [int(x) for x in np.random.uniform(low=index*window_size, high=index*window_size + window_size, size=n_mutations)]: 
                 ancestral_base = np.random.choice(bases, p=base_composition)
                 derived_base = np.random.choice(bases, p=mutation_matrix[ancestral_base])
                 observations_for_obsfile.append(f'{chrom}\t{mutation}\t{ancestral_base}\t{ancestral_base + derived_base}') 
                 obs_counter[chrom][index*window_size] += 1
                 variants_dict[chrom][index*window_size].append(str(mutation))
```

### Comparing `hmmix-0.7.0/test/test.py` & `hmmix-0.7.1/test/test.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.7.0/test/test_main.py` & `hmmix-0.7.1/test/test_main.py`

 * *Files identical despite different names*

