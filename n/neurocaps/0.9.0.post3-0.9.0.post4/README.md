# Comparing `tmp/neurocaps-0.9.0.post3.tar.gz` & `tmp/neurocaps-0.9.0.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurocaps-0.9.0.post3.tar", last modified: Tue May 14 20:16:39 2024, max compression
+gzip compressed data, was "neurocaps-0.9.0.post4.tar", last modified: Sat May 18 21:41:13 2024, max compression
```

## Comparing `neurocaps-0.9.0.post3.tar` & `neurocaps-0.9.0.post4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1077 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/LICENSE.md
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    15137 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/PKG-INFO
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    14179 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/README.md
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       78 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/__init__.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps/_utils/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      352 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/_utils/__init__.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps/_utils/_cap_internals/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       87 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/_utils/_cap_internals/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2492 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/_utils/_cap_internals/_capgetter.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      179 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2825 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/_utils/_check_confound_names.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps/_utils/_timeseriesextractor_internals/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      178 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     5250 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     7927 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2637 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps/analysis/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      137 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/analysis/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    57051 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/analysis/cap.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     4716 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/analysis/merge.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1564 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/analysis/standardize.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps/extraction/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       86 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/extraction/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    29643 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/neurocaps/extraction/timeseriesextractor.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps.egg-info/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    15137 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps.egg-info/PKG-INFO
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1061 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps.egg-info/SOURCES.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)        1 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps.egg-info/dependency_links.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      121 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps.egg-info/requires.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       10 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/neurocaps.egg-info/top_level.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1324 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/pyproject.toml
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       38 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/setup.cfg
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-14 20:16:39.000000 neurocaps-0.9.0.post3/tests/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     6365 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/tests/test_CAP.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     3685 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/tests/test_TimeseriesExtractor.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1045 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/tests/test_TimeseriesExtractor_additional.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1906 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/tests/test_merge_dicts.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      678 2024-05-14 20:15:21.000000 neurocaps-0.9.0.post3/tests/test_standardize.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-18 21:41:13.000000 neurocaps-0.9.0.post4/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1077 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/LICENSE.md
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    15139 2024-05-18 21:41:13.000000 neurocaps-0.9.0.post4/PKG-INFO
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    14181 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/README.md
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-18 21:41:11.000000 neurocaps-0.9.0.post4/neurocaps/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       78 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/__init__.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-18 21:41:11.000000 neurocaps-0.9.0.post4/neurocaps/_utils/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      352 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/_utils/__init__.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-18 21:41:11.000000 neurocaps-0.9.0.post4/neurocaps/_utils/_cap_internals/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       87 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/_utils/_cap_internals/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2492 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/_utils/_cap_internals/_capgetter.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      179 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2825 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/_utils/_check_confound_names.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-18 21:41:12.000000 neurocaps-0.9.0.post4/neurocaps/_utils/_timeseriesextractor_internals/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      178 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     5578 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     8043 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2637 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-18 21:41:12.000000 neurocaps-0.9.0.post4/neurocaps/analysis/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      137 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/analysis/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    57051 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/analysis/cap.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     4716 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/analysis/merge.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1564 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/analysis/standardize.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-18 21:41:12.000000 neurocaps-0.9.0.post4/neurocaps/extraction/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       86 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/extraction/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    29824 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/extraction/timeseriesextractor.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-18 21:41:11.000000 neurocaps-0.9.0.post4/neurocaps.egg-info/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    15139 2024-05-18 21:41:11.000000 neurocaps-0.9.0.post4/neurocaps.egg-info/PKG-INFO
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1061 2024-05-18 21:41:11.000000 neurocaps-0.9.0.post4/neurocaps.egg-info/SOURCES.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)        1 2024-05-18 21:41:11.000000 neurocaps-0.9.0.post4/neurocaps.egg-info/dependency_links.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      121 2024-05-18 21:41:11.000000 neurocaps-0.9.0.post4/neurocaps.egg-info/requires.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       10 2024-05-18 21:41:11.000000 neurocaps-0.9.0.post4/neurocaps.egg-info/top_level.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1324 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/pyproject.toml
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       38 2024-05-18 21:41:13.000000 neurocaps-0.9.0.post4/setup.cfg
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-18 21:41:13.000000 neurocaps-0.9.0.post4/tests/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     6365 2024-05-18 21:40:20.000000 neurocaps-0.9.0.post4/tests/test_CAP.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     3685 2024-05-18 21:40:20.000000 neurocaps-0.9.0.post4/tests/test_TimeseriesExtractor.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1053 2024-05-18 21:40:20.000000 neurocaps-0.9.0.post4/tests/test_TimeseriesExtractor_additional.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1906 2024-05-18 21:40:20.000000 neurocaps-0.9.0.post4/tests/test_merge_dicts.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      678 2024-05-18 21:40:20.000000 neurocaps-0.9.0.post4/tests/test_standardize.py
```

### Comparing `neurocaps-0.9.0.post3/LICENSE.md` & `neurocaps-0.9.0.post4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post3/PKG-INFO` & `neurocaps-0.9.0.post4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.0.post3
+Version: 0.9.0.post4
 Summary: Co-activation patterns Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -62,15 +62,15 @@
 pip install -e .
 
 ```
 
 # Usage
 **This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
 
-**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes has a left and right version**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
+**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes has a left and right version**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm: 1}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
 
 If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. 
 
 Custom Key Structure:
 - maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
 - nodes:  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
 Each label should match the parcellation index it represents. For example, if the parcellation label "0" corresponds to the left hemisphere 
@@ -125,15 +125,15 @@
              "rot_z","rot_z_derivative1"]
 
 """If use_confounds is True but no confound_names provided, there are hardcoded 
 confound names that will extract the data from the confound files outputted by fMRIPrep
 `n_acompcor_separate` will use the first 'n' components derived from the separate 
 white-matter (WM) and cerebrospinal fluid (CSF). To use the acompcor components from the 
 combined mask, list them in the `confound_names` parameter"""
-parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
+parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm": 2}}
 
 extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
                                  use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01, 
                                  confound_names=confounds, n_acompcor_separate=6)
 
 bids_dir = "/path/to/bids/dir"
 
@@ -166,15 +166,15 @@
 ```
 **Graph Outputs:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
 
 ```python
 
-# Get CAP metrics; zero indicates the absence of a CAP
+# Get CAP metrics
 outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
                                          return_df=True, output_dir=output_dir,
                                          metrics=["temporal fraction", "persistence"],
                                          continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
 
 print(outputs["temporal fraction"])
 ```
@@ -190,15 +190,15 @@
 | 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
 | 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
 | 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
 | 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
 
 ```python
 # If you experience coverage issues, usually smoothing helps to mitigate these issues
-cap_analysis.caps2surf(fwhm=1)
+cap_analysis.caps2surf(fwhm=2)
 ```
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
 
 # Testing 
 This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
 
 Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
```

### Comparing `neurocaps-0.9.0.post3/README.md` & `neurocaps-0.9.0.post4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 pip install -e .
 
 ```
 
 # Usage
 **This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
 
-**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes has a left and right version**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
+**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes has a left and right version**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm: 1}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
 
 If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. 
 
 Custom Key Structure:
 - maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
 - nodes:  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
 Each label should match the parcellation index it represents. For example, if the parcellation label "0" corresponds to the left hemisphere 
@@ -95,15 +95,15 @@
              "rot_z","rot_z_derivative1"]
 
 """If use_confounds is True but no confound_names provided, there are hardcoded 
 confound names that will extract the data from the confound files outputted by fMRIPrep
 `n_acompcor_separate` will use the first 'n' components derived from the separate 
 white-matter (WM) and cerebrospinal fluid (CSF). To use the acompcor components from the 
 combined mask, list them in the `confound_names` parameter"""
-parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
+parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm": 2}}
 
 extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
                                  use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01, 
                                  confound_names=confounds, n_acompcor_separate=6)
 
 bids_dir = "/path/to/bids/dir"
 
@@ -136,15 +136,15 @@
 ```
 **Graph Outputs:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
 
 ```python
 
-# Get CAP metrics; zero indicates the absence of a CAP
+# Get CAP metrics
 outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
                                          return_df=True, output_dir=output_dir,
                                          metrics=["temporal fraction", "persistence"],
                                          continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
 
 print(outputs["temporal fraction"])
 ```
@@ -160,15 +160,15 @@
 | 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
 | 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
 | 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
 | 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
 
 ```python
 # If you experience coverage issues, usually smoothing helps to mitigate these issues
-cap_analysis.caps2surf(fwhm=1)
+cap_analysis.caps2surf(fwhm=2)
 ```
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
 
 # Testing 
 This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
 
 Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
```

### Comparing `neurocaps-0.9.0.post3/neurocaps/_utils/_cap_internals/_capgetter.py` & `neurocaps-0.9.0.post4/neurocaps/_utils/_cap_internals/_capgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post3/neurocaps/_utils/_check_confound_names.py` & `neurocaps-0.9.0.post4/neurocaps/_utils/_check_confound_names.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post3/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py` & `neurocaps-0.9.0.post4/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from nilearn import datasets
 import warnings, re, os
 
 def _check_parcel_approach(parcel_approach, call = "TimeseriesExtractor"):
-    valid_parcel_dict = {"Schaefer": {"n_rois" : 400, "yeo_networks": 7},
+    valid_parcel_dict = {"Schaefer": {"n_rois" : 400, "yeo_networks": 7, "resolution_mm": 1},
                          "AAL": {"version": "SPM12"},
                          "Custom": {"maps": "/location/to/parcellation.nii.gz",
                                     "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
                                     "regions": {"Vis" : {"lh": [0,1],
                                                           "rh": [3,4]},
                                                  "Hippocampus": {"lh": [2],
                                                                  "rh": [5]}}}}
@@ -24,17 +24,21 @@
         if "n_rois" not in parcel_approach["Schaefer"].keys():
             warnings.warn("'n_rois' not specified in `parcel_approach`. Defaulting to 400 ROIs.")
             parcel_approach["Schaefer"].update({"n_rois": 400})
 
         if "yeo_networks" not in parcel_approach["Schaefer"].keys():
             warnings.warn("'yeo_networks' not specified in `parcel_approach`. Defaulting to 7 networks.")
             parcel_approach["Schaefer"].update({"yeo_networks": 7})
+        
+        if "resolution_mm" not in parcel_approach["Schaefer"].keys():
+            warnings.warn("'resolution_mm' not specified in `parcel_approach`. Defaulting to 1mm.")
+            parcel_approach["Schaefer"].update({"resolution_mm": 1})
 
         # Get atlas
-        fetched_schaefer = datasets.fetch_atlas_schaefer_2018(n_rois=parcel_approach["Schaefer"]["n_rois"], yeo_networks=parcel_approach["Schaefer"]["yeo_networks"])
+        fetched_schaefer = datasets.fetch_atlas_schaefer_2018(n_rois=parcel_approach["Schaefer"]["n_rois"], yeo_networks=parcel_approach["Schaefer"]["yeo_networks"], resolution_mm=parcel_approach["Schaefer"]["resolution_mm"])
         parcel_approach["Schaefer"].update({"maps": fetched_schaefer.maps})
         parcel_approach["Schaefer"].update({"nodes": [label.decode().split("7Networks_")[-1]  for label in fetched_schaefer.labels]})
         # Get node networks
         parcel_approach["Schaefer"].update({"regions": list(dict.fromkeys([re.split("LH_|RH_", node)[-1].split("_")[0] for node in parcel_approach["Schaefer"]["nodes"]]))})
 
     if "AAL" in parcel_approach.keys():
         if "version" not in parcel_approach["AAL"].keys():
```

### Comparing `neurocaps-0.9.0.post3/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py` & `neurocaps-0.9.0.post4/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,25 +78,27 @@
                 mask_img=mask_file[0],
                 labels_img=parcel_approach[list(parcel_approach.keys())[0]]["maps"], 
                 resampling_target='data',
                 standardize=signal_clean_info["standardize"],
                 detrend=signal_clean_info["detrend"],
                 low_pass=signal_clean_info["low_pass"],
                 high_pass=signal_clean_info["high_pass"],
-                t_r=tr
+                t_r=tr,
+                smoothing_fwhm=signal_clean_info["fwhm"]
             )
         else:
             masker = NiftiLabelsMasker(
                 labels_img=parcel_approach[list(parcel_approach.keys())[0]]["maps"], 
                 resampling_target='data',
                 standardize=signal_clean_info["standardize"],
                 detrend=signal_clean_info["detrend"],
                 low_pass=signal_clean_info["low_pass"],
                 high_pass=signal_clean_info["high_pass"],
-                t_r=tr
+                t_r=tr,
+                smoothing_fwhm=signal_clean_info["fwhm"]
             )
         # Load and discard volumes if needed
         nifti_img = load_img(nifti_file[0])
         if signal_clean_info["dummy_scans"]: 
             nifti_img = index_img(nifti_img, slice(signal_clean_info["dummy_scans"], None))
             if signal_clean_info["use_confounds"]: 
                 confounds.drop(list(range(0,signal_clean_info["dummy_scans"])),axis=0,inplace=True)
```

### Comparing `neurocaps-0.9.0.post3/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py` & `neurocaps-0.9.0.post4/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post3/neurocaps/analysis/cap.py` & `neurocaps-0.9.0.post4/neurocaps/analysis/cap.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post3/neurocaps/analysis/merge.py` & `neurocaps-0.9.0.post4/neurocaps/analysis/merge.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post3/neurocaps/analysis/standardize.py` & `neurocaps-0.9.0.post4/neurocaps/analysis/standardize.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post3/neurocaps/extraction/timeseriesextractor.py` & `neurocaps-0.9.0.post4/neurocaps/extraction/timeseriesextractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json, os, re, sys, warnings
 from typing import Union
 from .._utils import _TimeseriesExtractorGetter, _check_confound_names, _check_parcel_approach, _extract_timeseries
 
 class TimeseriesExtractor(_TimeseriesExtractorGetter):
     def __init__(self, space: str="MNI152NLin2009cAsym", standardize: Union[bool,str]="zscore_sample", detrend: bool=False , low_pass: float=None, high_pass: float=None, 
-                 parcel_approach : dict={"Schaefer": {"n_rois": 400, "yeo_networks": 7}}, use_confounds: bool=True, confound_names: list[str]=None, fd_threshold: float=None,
+                 parcel_approach : dict={"Schaefer": {"n_rois": 400, "yeo_networks": 7, "resolution_mm": 1}}, use_confounds: bool=True, confound_names: list[str]=None, fwhm: float=None, fd_threshold: float=None,
                  n_acompcor_separate: int=None, dummy_scans: int=None):
         """Timeseries Extractor Class
         
         Initializes a TimeseriesExtractor to prepare for Co-activation Patterns (CAPs) analysis.
 
         Parameters
         ----------
@@ -18,25 +18,27 @@
             Determines whether to standardize the timeseries. Refer to Nilearn's NiftiLabelsMasker for available options. 
         detrend : bool, default=True
             Detrends timeseries during extraction.
         low_pass : bool, default=None
             Signals above cutoff frequency will be filtered out.
         high_pass : float, default=None
             Signals below cutoff frequency will be filtered out.
-        parcel_approach : dict, default={"Schaefer": {"n_rois": 400, "yeo_networks": 7}}
+        parcel_approach : dict, default={"Schaefer": {"n_rois": 400, "yeo_networks": 7, "resolution_mm": 1}}
             Approach to use to parcellate bold images. Should be in the form of a nested dictionary where the first key is the atlas.
-            Currently only "Schaefer" and "AAL" is supported. For the sub-dictionary for "Schaefer", available options includes "n_rois" and "yeo_networks".
+            Currently only "Schaefer", "AAL", and "Custom" is supported. For the sub-dictionary for "Schaefer", available options includes "n_rois", "yeo_networks", and "resolution_mm".
             Please refer to the documentation for Nilearn's `datasets.fetch_atlas_schaefer_2018` for valid inputs. For the subdictionary for "AAL" only "version"
             is an option. Please refer to the documentation for Nilearn's `datasets.fetch_atlas_aal` for valid inputs. As of version 0.8.9, you can replace "Schaefer"
             and "AAL" with "Custom". At minimum, if "Custom" is specified, a subkey, called "maps" specifying the directory location of the parcellation as a Nifti (e.g .nii or .nii.gz)
             - {"Custom": {"maps": "/location/to/parcellation.nii.gz"}}.
         use_confounds : bool, default=True
             To use confounds when extracting timeseries.
         confound_names : List[str], default=None
             Names of confounds to use in confound files. If None, default confounds are used.
+        fwhm : float, default=None
+            Parameter for spatial smoothing.
         fd_threshold : float, default=None
             Threshold criteria to remove volume after nuisance regression and timeseries extraction. For this to work, a column named "framewise_displacement" must be
             in the confounds dataframe and `use_confounds` must be true. Additionally, 'framewise_displacemnt' does not need to be specified in the `confound_names` for this to work.
         n_acompcor_separate : int, default = None
             The number of seperate acompcor components derived from the white-matter (WM) and cerebrospinal (CSF) masks to use. For instance if '5' is assigned to this parameter
             then the first five components derived from the WM mask and the first five components derived from the CSF mask will be used, resulting in ten acompcor components being
             used. If this parameter is not none any acompcor components listed in the confound names will be disregarded in order to locate the first 'n' components derived from the 
@@ -70,15 +72,15 @@
                              "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
                              "regions": {"Vis" : {"lh": [0,1],
                                                   "rh": [3,4]},
                                          "Hippocampus": {"lh": [2],
                                                          "rh": [5]}}}}
         """
         self._space = space
-        self._signal_clean_info = {"standardize": standardize, "detrend": detrend, "low_pass": low_pass, "high_pass": high_pass, 
+        self._signal_clean_info = {"standardize": standardize, "detrend": detrend, "low_pass": low_pass, "high_pass": high_pass, "fwhm": fwhm, 
                                    "dummy_scans": dummy_scans, "use_confounds": use_confounds,  "n_acompcor_separate": n_acompcor_separate,
                                    "fd_threshold": None}   
 
         # Check parcel_apprach
         self._parcel_approach = _check_parcel_approach(parcel_approach=parcel_approach)
 
         if self._signal_clean_info["use_confounds"]:
```

### Comparing `neurocaps-0.9.0.post3/neurocaps.egg-info/PKG-INFO` & `neurocaps-0.9.0.post4/neurocaps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.0.post3
+Version: 0.9.0.post4
 Summary: Co-activation patterns Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -62,15 +62,15 @@
 pip install -e .
 
 ```
 
 # Usage
 **This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
 
-**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes has a left and right version**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
+**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes has a left and right version**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm: 1}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
 
 If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. 
 
 Custom Key Structure:
 - maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
 - nodes:  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
 Each label should match the parcellation index it represents. For example, if the parcellation label "0" corresponds to the left hemisphere 
@@ -125,15 +125,15 @@
              "rot_z","rot_z_derivative1"]
 
 """If use_confounds is True but no confound_names provided, there are hardcoded 
 confound names that will extract the data from the confound files outputted by fMRIPrep
 `n_acompcor_separate` will use the first 'n' components derived from the separate 
 white-matter (WM) and cerebrospinal fluid (CSF). To use the acompcor components from the 
 combined mask, list them in the `confound_names` parameter"""
-parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
+parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm": 2}}
 
 extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
                                  use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01, 
                                  confound_names=confounds, n_acompcor_separate=6)
 
 bids_dir = "/path/to/bids/dir"
 
@@ -166,15 +166,15 @@
 ```
 **Graph Outputs:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
 
 ```python
 
-# Get CAP metrics; zero indicates the absence of a CAP
+# Get CAP metrics
 outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
                                          return_df=True, output_dir=output_dir,
                                          metrics=["temporal fraction", "persistence"],
                                          continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
 
 print(outputs["temporal fraction"])
 ```
@@ -190,15 +190,15 @@
 | 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
 | 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
 | 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
 | 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
 
 ```python
 # If you experience coverage issues, usually smoothing helps to mitigate these issues
-cap_analysis.caps2surf(fwhm=1)
+cap_analysis.caps2surf(fwhm=2)
 ```
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
 
 # Testing 
 This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
 
 Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
```

### Comparing `neurocaps-0.9.0.post3/neurocaps.egg-info/SOURCES.txt` & `neurocaps-0.9.0.post4/neurocaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post3/pyproject.toml` & `neurocaps-0.9.0.post4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neurocaps"
-version = "0.9.0post3"
+version = "0.9.0post4"
 authors = [{name = "Donisha Smith", email = "donishasmith@outlook.com"}]
 description = "Co-activation patterns Python package"
 readme = "README.md"
 requires-python = ">=3.9.0"
 keywords = ["python", "Co-Activation Patterns", "CAPs", "neuroimaging", "fmri", "dfc", "dynamic functional connectivity", "fMRIPrep"]
 classifiers = [
     "Intended Audience :: Education",
```

### Comparing `neurocaps-0.9.0.post3/tests/test_CAP.py` & `neurocaps-0.9.0.post4/tests/test_CAP.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post3/tests/test_TimeseriesExtractor.py` & `neurocaps-0.9.0.post4/tests/test_TimeseriesExtractor.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post3/tests/test_TimeseriesExtractor_additional.py` & `neurocaps-0.9.0.post4/tests/test_TimeseriesExtractor_additional.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
     confounds=["Cosine*", "aComp*", "Rot*"]
 
     parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
 
     extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
                                     use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01,
-                                    confound_names=confounds)
+                                    confound_names=confounds, fwhm=2)
 
     bids_dir = os.path.join(dir, "ds000031_R1.0.4_ses001-022/ds000031_R1.0.4")
 
     pipeline_name = "fmriprep_1.0.0/fmriprep"
     extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name, tr=1.2)
     
     print(extractor.subject_timeseries, flush=True)
```

### Comparing `neurocaps-0.9.0.post3/tests/test_merge_dicts.py` & `neurocaps-0.9.0.post4/tests/test_merge_dicts.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post3/tests/test_standardize.py` & `neurocaps-0.9.0.post4/tests/test_standardize.py`

 * *Files identical despite different names*

