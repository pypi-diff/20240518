# Comparing `tmp/pydra_freesurfer-0.0.9.tar.gz` & `tmp/pydra_freesurfer-0.1.1.tar.gz`

## Comparing `pydra_freesurfer-0.0.9.tar` & `pydra_freesurfer-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,438 @@
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/.editorconfig
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/.github/dependabot.yaml
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/.github/workflows/docs.yaml
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/.github/workflows/test.yaml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/docs/api.rst
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/docs/conf.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/docs/index.rst
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/__init__.py
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/gtmseg.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/mri_convert.py
--rw-r--r--   0        0        0     8401 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/mri_surf2surf.py
--rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/mri_vol2vol.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/mris_anatomical_stats.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/mris_ca_label.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/mris_ca_train.py
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/mris_expand.py
--rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/mris_preproc.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/specs.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/tkregister2.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/recon_all/__init__.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/recon_all/base_recon_all.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/recon_all/long_recon_all.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/recon_all/recon_all.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/recon_all/specs.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/recon_all/tests/test_base_recon_all.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/recon_all/tests/test_long_recon_all.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/recon_all/tests/test_recon_all.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/recon_all/tests/test_specs.py
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/LICENSE
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/README.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/hatch.toml
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 pydra_freesurfer-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/.coveragerc
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/.editorconfig
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/.flake8
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/codecov.yml
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/report_progress.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/.github/dependabot.yaml
+-rw-r--r--   0        0        0    15855 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/.github/workflows/ci-cd.yaml
+-rw-r--r--   0        0        0     7414 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/docs/source/api.rst
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/docs/source/conf.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/docs/source/index.rst
+-rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/generate
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/requirements.txt
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/package.yaml
+-rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/add_x_form_to_header.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/add_x_form_to_header_callables.py
+-rw-r--r--   0        0        0    13500 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/aparc_2_aseg.yaml
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/aparc_2_aseg_callables.py
+-rw-r--r--   0        0        0     6578 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/apas_2_aseg.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/apas_2_aseg_callables.py
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/apply_mask.yaml
+-rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/apply_mask_callables.py
+-rw-r--r--   0        0        0    10237 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/apply_vol_transform.yaml
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/apply_vol_transform_callables.py
+-rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/bb_register.yaml
+-rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/bb_register_callables.py
+-rw-r--r--   0        0        0     8918 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/binarize.yaml
+-rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/binarize_callables.py
+-rw-r--r--   0        0        0     8825 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/ca_label.yaml
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/ca_label_callables.py
+-rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/ca_normalize.yaml
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/ca_normalize_callables.py
+-rw-r--r--   0        0        0     8257 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/ca_register.yaml
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/ca_register_callables.py
+-rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/check_talairach_alignment.yaml
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/check_talairach_alignment_callables.py
+-rw-r--r--   0        0        0     8583 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/concatenate.yaml
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/concatenate_callables.py
+-rw-r--r--   0        0        0    12363 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/concatenate_lta.yaml
+-rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/concatenate_lta_callables.py
+-rw-r--r--   0        0        0     9649 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/contrast.yaml
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/contrast_callables.py
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/curvature.yaml
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/curvature_callables.py
+-rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/curvature_stats.yaml
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/curvature_stats_callables.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/dicom_convert.yaml
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/dicom_convert_callables.py
+-rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/edit_w_mwith_aseg.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/edit_w_mwith_aseg_callables.py
+-rw-r--r--   0        0        0     7854 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/em_register.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/em_register_callables.py
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/euler_number.yaml
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/euler_number_callables.py
+-rw-r--r--   0        0        0     6020 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/extract_main_component.yaml
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/extract_main_component_callables.py
+-rw-r--r--   0        0        0     7145 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/fit_ms_params.yaml
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/fit_ms_params_callables.py
+-rw-r--r--   0        0        0     8934 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/fix_topology.yaml
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/fix_topology_callables.py
+-rw-r--r--   0        0        0     9782 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/fuse_segmentations.yaml
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/fuse_segmentations_callables.py
+-rw-r--r--   0        0        0    13257 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/glm_fit.yaml
+-rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/glm_fit_callables.py
+-rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/gtm_seg.yaml
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/gtm_seg_callables.py
+-rw-r--r--   0        0        0    20547 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/gtmpvc.yaml
+-rw-r--r--   0        0        0     6778 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/gtmpvc_callables.py
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/image_info.yaml
+-rw-r--r--   0        0        0     8066 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/image_info_callables.py
+-rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/jacobian.yaml
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/jacobian_callables.py
+-rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/label_2_annot.yaml
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/label_2_annot_callables.py
+-rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/label_2_label.yaml
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/label_2_label_callables.py
+-rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/label_2_vol.yaml
+-rw-r--r--   0        0        0     4065 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/label_2_vol_callables.py
+-rw-r--r--   0        0        0    13705 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/logan_ref.yaml
+-rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/logan_ref_callables.py
+-rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/lta_convert.yaml
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/lta_convert_callables.py
+-rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/make_average_subject.yaml
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/make_average_subject_callables.py
+-rw-r--r--   0        0        0    10736 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/make_surfaces.yaml
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/make_surfaces_callables.py
+-rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mni_bias_correction.yaml
+-rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mni_bias_correction_callables.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mp_rto_mni305.yaml
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mp_rto_mni305_callables.py
+-rw-r--r--   0        0        0     9889 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mr_is_ca_label.yaml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mr_is_ca_label_callables.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mr_is_calc.yaml
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mr_is_calc_callables.py
+-rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mr_is_combine.yaml
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mr_is_combine_callables.py
+-rw-r--r--   0        0        0     7060 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mr_is_convert.yaml
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mr_is_convert_callables.py
+-rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mr_is_expand.yaml
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mr_is_expand_callables.py
+-rw-r--r--   0        0        0     6819 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mr_is_inflate.yaml
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mr_is_inflate_callables.py
+-rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mri_convert.yaml
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mri_convert_callables.py
+-rw-r--r--   0        0        0    16880 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mri_coreg.yaml
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mri_coreg_callables.py
+-rw-r--r--   0        0        0     7433 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mri_fill.yaml
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mri_fill_callables.py
+-rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mri_marching_cubes.yaml
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mri_marching_cubes_callables.py
+-rw-r--r--   0        0        0     7839 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mri_pretess.yaml
+-rw-r--r--   0        0        0     6067 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mri_pretess_callables.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mri_tessellate.yaml
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mri_tessellate_callables.py
+-rw-r--r--   0        0        0     9244 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mris_preproc.yaml
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mris_preproc_callables.py
+-rw-r--r--   0        0        0    10100 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mris_preproc_recon_all.yaml
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mris_preproc_recon_all_callables.py
+-rw-r--r--   0        0        0    13617 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mrtm.yaml
+-rw-r--r--   0        0        0    13700 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mrtm2.yaml
+-rw-r--r--   0        0        0     8279 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mrtm2_callables.py
+-rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/mrtm_callables.py
+-rw-r--r--   0        0        0     9415 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/ms__lda.yaml
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/ms__lda_callables.py
+-rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/normalize.yaml
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/normalize_callables.py
+-rw-r--r--   0        0        0    10999 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/one_sample_t_test.yaml
+-rw-r--r--   0        0        0     8288 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/one_sample_t_test_callables.py
+-rw-r--r--   0        0        0     8263 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/paint.yaml
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/paint_callables.py
+-rw-r--r--   0        0        0    14908 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/parcellation_stats.yaml
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/parcellation_stats_callables.py
+-rw-r--r--   0        0        0     6926 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/parse_dicom_dir.yaml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/parse_dicom_dir_callables.py
+-rw-r--r--   0        0        0    25646 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/recon_all.yaml
+-rw-r--r--   0        0        0     9446 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/recon_all_callables.py
+-rw-r--r--   0        0        0     9041 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/register.yaml
+-rw-r--r--   0        0        0     8121 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/register_av_ito_talairach.yaml
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/register_av_ito_talairach_callables.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/register_callables.py
+-rw-r--r--   0        0        0     7455 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/relabel_hypointensities.yaml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/relabel_hypointensities_callables.py
+-rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/remove_intersection.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/remove_intersection_callables.py
+-rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/remove_neck.yaml
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/remove_neck_callables.py
+-rw-r--r--   0        0        0     6928 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/resample.yaml
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/resample_callables.py
+-rw-r--r--   0        0        0    11654 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/robust_register.yaml
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/robust_register_callables.py
+-rw-r--r--   0        0        0    17211 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/robust_template.yaml
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/robust_template_callables.py
+-rw-r--r--   0        0        0    12896 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/sample_to_surface.yaml
+-rw-r--r--   0        0        0     5856 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/sample_to_surface_callables.py
+-rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/seg_stats.yaml
+-rw-r--r--   0        0        0     5080 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/seg_stats_callables.py
+-rw-r--r--   0        0        0    20531 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/seg_stats_recon_all.yaml
+-rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/seg_stats_recon_all_callables.py
+-rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/segment_cc.yaml
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/segment_cc_callables.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/segment_wm.yaml
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/segment_wm_callables.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/smooth.yaml
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/smooth_callables.py
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/smooth_tessellation.yaml
+-rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/smooth_tessellation_callables.py
+-rw-r--r--   0        0        0     6569 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/sphere.yaml
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/sphere_callables.py
+-rw-r--r--   0        0        0     9521 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/spherical_average.yaml
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/spherical_average_callables.py
+-rw-r--r--   0        0        0     8966 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/surface_2_vol_transform.yaml
+-rw-r--r--   0        0        0     6307 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/surface_2_vol_transform_callables.py
+-rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/surface_smooth.yaml
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/surface_smooth_callables.py
+-rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/surface_snapshots.yaml
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/surface_snapshots_callables.py
+-rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/surface_transform.yaml
+-rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/surface_transform_callables.py
+-rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/synthesize_flash.yaml
+-rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/synthesize_flash_callables.py
+-rw-r--r--   0        0        0     6997 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/talairach_avi.yaml
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/talairach_avi_callables.py
+-rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/talairach_qc.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/talairach_qc_callables.py
+-rw-r--r--   0        0        0    11604 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/tkregister_2.yaml
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/tkregister_2_callables.py
+-rw-r--r--   0        0        0     8411 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/unpack_sdicom_dir.yaml
+-rw-r--r--   0        0        0     5870 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/unpack_sdicom_dir_callables.py
+-rw-r--r--   0        0        0    10317 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/volume_mask.yaml
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/volume_mask_callables.py
+-rw-r--r--   0        0        0     7889 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/watershed_skull_strip.yaml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/nipype-auto-conv/specs/interfaces/watershed_skull_strip_callables.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/_version.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/latest.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/__init__.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/_post_release.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/longitudinal/__init__.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/longitudinal/fuse_segmentations.py
+-rw-r--r--   0        0        0     5838 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/longitudinal/robust_template.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/longitudinal/tests/conftest.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/longitudinal/tests/test_fusesegmentations.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/longitudinal/tests/test_robusttemplate.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/__init__.py
+-rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/binarize.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/concatenate.py
+-rw-r--r--   0        0        0    13592 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/glm_fit.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/label_2_annot.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/label_2_label.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/label_2_vol.py
+-rw-r--r--   0        0        0     5592 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/mris_preproc.py
+-rw-r--r--   0        0        0     6925 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/mris_preproc_recon_all.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/ms__lda.py
+-rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/one_sample_t_test.py
+-rw-r--r--   0        0        0     9920 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/seg_stats.py
+-rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/seg_stats_recon_all.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/spherical_average.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/tests/conftest.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/tests/test_binarize.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/tests/test_concatenate.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/tests/test_glmfit.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/tests/test_label2annot.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/tests/test_label2label.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/tests/test_label2vol.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/tests/test_mrispreproc.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/tests/test_mrispreprocreconall.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/tests/test_ms_lda.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/tests/test_onesamplettest.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/tests/test_segstats.py
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/tests/test_segstatsreconall.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/model/tests/test_sphericalaverage.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/petsurfer/__init__.py
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/petsurfer/gtm_seg.py
+-rw-r--r--   0        0        0    16115 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/petsurfer/gtmpvc.py
+-rw-r--r--   0        0        0    13769 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/petsurfer/logan_ref.py
+-rw-r--r--   0        0        0    13722 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/petsurfer/mrtm.py
+-rw-r--r--   0        0        0    13751 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/petsurfer/mrtm2.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/petsurfer/tests/conftest.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/petsurfer/tests/test_gtmpvc.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/petsurfer/tests/test_gtmseg.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/petsurfer/tests/test_loganref.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/petsurfer/tests/test_mrtm.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/petsurfer/tests/test_mrtm2.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/__init__.py
+-rw-r--r--   0        0        0     8652 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/apply_vol_transform.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/bb_register.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/ca_label.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/ca_normalize.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/ca_register.py
+-rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/concatenate_lta.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/dicom_convert.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/edit_w_mwith_aseg.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/fit_ms_params.py
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/mni_bias_correction.py
+-rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/mr_is_ca_label.py
+-rw-r--r--   0        0        0    15120 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/mri_convert.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/normalize.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/parse_dicom_dir.py
+-rw-r--r--   0        0        0    14416 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/recon_all.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/resample.py
+-rw-r--r--   0        0        0     7672 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/robust_register.py
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/segment_cc.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/segment_wm.py
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/smooth.py
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/synthesize_flash.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/unpack_sdicom_dir.py
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/watershed_skull_strip.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/conftest.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_applyvoltransform.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_bbregister.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_calabel.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_canormalize.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_caregister.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_concatenatelta.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_dicomconvert.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_editwmwithaseg.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_fitmsparams.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_mnibiascorrection.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_mriconvert.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_mriscalabel.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_normalize.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_parsedicomdir.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_reconall.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_resample.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_robustregister.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_segmentcc.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_segmentwm.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_smooth.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_synthesizeflash.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_unpacksdicomdir.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/tests/test_watershedskullstrip.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/registration/__init__.py
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/registration/em_register.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/registration/mp_rto_mni305.py
+-rw-r--r--   0        0        0     8348 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/registration/mri_coreg.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/registration/paint.py
+-rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/registration/register.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/registration/register_av_ito_talairach.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/registration/tests/conftest.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/registration/tests/test_emregister.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/registration/tests/test_mprtomni305.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/registration/tests/test_mricoreg.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/registration/tests/test_paint.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/registration/tests/test_register.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/registration/tests/test_registeravitotalairach.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/__init__.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/add_x_form_to_header.py
+-rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/aparc_2_aseg.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/apas_2_aseg.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/apply_mask.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/check_talairach_alignment.py
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/contrast.py
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/curvature.py
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/curvature_stats.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/euler_number.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/extract_main_component.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/fix_topology.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/image_info.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/jacobian.py
+-rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/lta_convert.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/make_average_subject.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/make_surfaces.py
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/mr_is_calc.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/mr_is_combine.py
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/mr_is_convert.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/mr_is_expand.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/mr_is_inflate.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/mri_fill.py
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/mri_marching_cubes.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/mri_pretess.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/mri_tessellate.py
+-rw-r--r--   0        0        0     6731 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/parcellation_stats.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/relabel_hypointensities.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/remove_intersection.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/remove_neck.py
+-rw-r--r--   0        0        0     8862 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/sample_to_surface.py
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/smooth_tessellation.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/sphere.py
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/surface_2_vol_transform.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/surface_smooth.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/surface_snapshots.py
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/surface_transform.py
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/talairach_avi.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/talairach_qc.py
+-rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tkregister_2.py
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/volume_mask.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/conftest.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_addxformtoheader.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_aparc2aseg.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_apas2aseg.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_applymask.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_checktalairachalignment.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_contrast.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_curvature.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_curvaturestats.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_eulernumber.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_extractmaincomponent.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_fixtopology.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_imageinfo.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_jacobian.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_ltaconvert.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_makeaveragesubject.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_makesurfaces.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_mrifill.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_mrimarchingcubes.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_mripretess.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_mriscalc.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_mriscombine.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_mrisconvert.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_mrisexpand.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_mrisinflate.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_mritessellate.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_parcellationstats.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_relabelhypointensities.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_removeintersection.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_removeneck.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_sampletosurface.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_smoothtessellation.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_sphere.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_surface2voltransform.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_surfacesmooth.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_surfacesnapshots.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_surfacetransform.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_talairachavi.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_talairachqc.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_tkregister2.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/tests/test_volumemask.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/__init__.py
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/gtmseg.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/specs.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/tkregister2.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mri/__init__.py
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mri/aparc2aseg.py
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mri/binarize.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mri/convert.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mri/coreg.py
+-rw-r--r--   0        0        0     5970 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mri/label2vol.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mri/robust_register.py
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mri/robust_template.py
+-rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mri/surf2surf.py
+-rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mri/vol2vol.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mris/__init__.py
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mris/anatomical_stats.py
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mris/ca_label.py
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mris/ca_train.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mris/expand.py
+-rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mris/preproc.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/recon_all/__init__.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/recon_all/base_recon_all.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/recon_all/long_recon_all.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/recon_all/recon_all.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/recon_all/specs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/recon_all/tests/__init__.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/recon_all/tests/test_base_recon_all.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/recon_all/tests/test_long_recon_all.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/recon_all/tests/test_recon_all.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/recon_all/tests/test_specs.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/related-packages/conftest.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/related-packages/fileformats/LICENSE
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/related-packages/fileformats/README.rst
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/related-packages/fileformats/pyproject.toml
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/related-packages/fileformats/fileformats/medimage_freesurfer/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/related-packages/fileformats-extras/LICENSE
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/related-packages/fileformats-extras/README.rst
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/related-packages/fileformats-extras/pyproject.toml
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/related-packages/fileformats-extras/fileformats/extras/medimage_freesurfer/__init__.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/related-packages/fileformats-extras/fileformats/extras/medimage_freesurfer/tests/test_generate_sample_data.py
+-rwxr-xr-x   0        0        0     2272 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/tools/increment_tool_version.py
+-rwxr-xr-x   0        0        0     1396 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/tools/rename_template.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/tools/requirements.txt
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/LICENSE
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/NOTICE
+-rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/README.md
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    23091 2020-02-02 00:00:00.000000 pydra_freesurfer-0.1.1/PKG-INFO
```

### Comparing `pydra_freesurfer-0.0.9/docs/conf.py` & `pydra_freesurfer-0.1.1/docs/source/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # Configuration file for the Sphinx documentation builder.
 #
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
-from sphinx_pyproject import SphinxConfig
-
-config = SphinxConfig(globalns=globals())
+from pydra.tasks.freesurfer import __version__  # noqa
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
-project = config.name
-author = 'The Aramis Lab'
-copyright = f'2022-2023, {author}'
-release = config.version
+project = "pydra-freesurfer"
+author = "Pydra Developers"
+copyright = f"2022-2023, {author}"
+release = __version__
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
-extensions = ['sphinx.ext.autosummary', 'sphinx.ext.napoleon']
-templates_path = ['_templates']
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+extensions = ["sphinx.ext.autosummary", "sphinx.ext.napoleon"]
+templates_path = ["_templates"]
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
-html_theme = 'pydata_sphinx_theme'
+html_theme = "pydata_sphinx_theme"
```

### Comparing `pydra_freesurfer-0.0.9/docs/index.rst` & `pydra_freesurfer-0.1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/__init__.py` & `pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,37 @@
 """Pydra tasks for FreeSurfer.
 
-Core interfaces can be imported directly from the package namespace.
+1. Recon-All
 
->>> from pydra.tasks.freesurfer import MRIConvert
+The main task definition for recon-all can be imported directly from the root package.
 
-Some modules such as :mod:`recon_all` provide additional interfaces for advanced
-use cases. Those interfaces have to be imported from their corresponding subpackage.
+>>> from pydra.tasks.freesurfer.v7_4 import ReconAll
 
->>> from pydra.tasks.freesurfer.recon_all import BaseReconAll, LongReconAll
+Additional task definitions are available under the :mod:`recon_all` namespace
+for more advanced use cases.
 
-.. automodule:: pydra.tasks.freesurfer.gtmseg
-.. automodule:: pydra.tasks.freesurfer.mri_convert
-.. automodule:: pydra.tasks.freesurfer.mri_surf2surf
-.. automodule:: pydra.tasks.freesurfer.mri_vol2vol
-.. automodule:: pydra.tasks.freesurfer.mris_anatomical_stats
-.. automodule:: pydra.tasks.freesurfer.mris_ca_label
-.. automodule:: pydra.tasks.freesurfer.mris_ca_train
-.. automodule:: pydra.tasks.freesurfer.mris_expand
-.. automodule:: pydra.tasks.freesurfer.mris_preproc
-.. automodule:: pydra.tasks.freesurfer.recon_all
-.. automodule:: pydra.tasks.freesurfer.tkregister2
+>>> from pydra.tasks.freesurfer.v7_4.recon_all import BaseReconAll, LongReconAll
+
+2. Volume Utilities
+
+Task definitions for volume processing utilities are available under the :mod:`mri` namespace.
+
+>>> from pydra.tasks.freesurfer.v7_4 import mri
+
+3. Surface Utilities
+
+Task definitions for surface processing utilities are available under the :mod:`mris` namespace.
+
+>>> from pydra.tasks.freesurfer.v7_4 import mris
+
+.. automodule:: pydra.tasks.freesurfer.v7_4.gtmseg
+.. automodule:: pydra.tasks.freesurfer.v7_4.mri
+.. automodule:: pydra.tasks.freesurfer.v7_4.mris
+.. automodule:: pydra.tasks.freesurfer.v7_4.recon_all
+.. automodule:: pydra.tasks.freesurfer.v7_4.tkregister2
 """
+
 from .gtmseg import GTMSeg
-from .mri_convert import MRIConvert
-from .mri_surf2surf import MRISurf2Surf
-from .mri_vol2vol import MRIVol2Vol
-from .mris_anatomical_stats import MRISAnatomicalStats
-from .mris_ca_label import MRISCALabel
-from .mris_ca_train import MRISCATrain
-from .mris_expand import MRISExpand
-from .mris_preproc import MRISPreproc
 from .recon_all import ReconAll
 from .tkregister2 import TkRegister2
 
-__all__ = [
-    "GTMSeg",
-    "MRIConvert",
-    "MRISurf2Surf",
-    "MRIVol2Vol",
-    "MRISAnatomicalStats",
-    "MRISCALabel",
-    "MRISCATrain",
-    "MRISExpand",
-    "MRISPreproc",
-    "ReconAll",
-    "TkRegister2",
-]
+__all__ = ["GTMSeg", "ReconAll", "TkRegister2"]
```

### Comparing `pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/gtmseg.py` & `pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/gtmseg.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,155 +3,143 @@
 ======
 
 Examples
 --------
 >>> task = GTMSeg(subject_id="subject", generate_segmentation=True)
 >>> task.cmdline
 'gtmseg --s subject --o gtmseg.mgz --xcerseg'
+
 >>> task = GTMSeg(
 ...     subject_id="subject",
 ...     keep_hypointensities=True,
 ...     subsegment_white_matter=True,
-...     output_volume_file="gtmseg.wmseg.hypo.mgz",
+...     output_volume="gtmseg.wmseg.hypo.mgz",
 ...     upsampling_factor=1,
-...     use_existing_segmentation=True,
+...     generate_segmentation=False,
 ... )
 >>> task.cmdline
 'gtmseg --s subject --o gtmseg.wmseg.hypo.mgz --no-xcerseg --usf 1 --keep-hypo --subsegwm'
+
 >>> task = GTMSeg(
 ...     subject_id="subject",
-...     output_volume_file="gtmseg+myseg.mgz",
-...     segmentation_file="apas+head+myseg.mgz",
+...     output_volume="gtmseg+myseg.mgz",
+...     head_segmentation="apas+head+myseg.mgz",
 ...     colortable="myseg.colortable.txt",
 ... )
 >>> task.cmdline
 'gtmseg --s subject --o gtmseg+myseg.mgz --head apas+head+myseg.mgz --ctab myseg.colortable.txt'
 """
-import attrs
 
-import pydra
+__all__ = ["GTMSeg"]
 
-from . import specs
+from os import PathLike
 
-__all__ = ["GTMSeg"]
+from attrs import NOTHING, define, field
+
+from pydra.engine.specs import ShellSpec, SpecInfo
+from pydra.engine.task import ShellCommandTask
+from pydra.tasks.freesurfer.v7_4 import specs
 
 
-@attrs.define(slots=False, kw_only=True)
-class GTMSegSpec(pydra.specs.ShellSpec):
-    """Specifications for FreeSurfer's gtmseg."""
+@define(kw_only=True)
+class GTMSegSpec(ShellSpec):
+    """Specifications for gtmseg."""
 
-    subject_id: str = attrs.field(
+    subject_id: str = field(
         metadata={
-            "help_string": "subject to analyze",
+            "help_string": "subject identifier",
             "mandatory": True,
             "argstr": "--s",
         }
     )
 
-    output_volume_file: str = attrs.field(
+    output_volume: str = field(
         default="gtmseg.mgz",
         metadata={
-            "help_string": "output volume file relative to the subject's mri directory",
+            "help_string": "output volume relative to the subject's mri directory",
             "argstr": "--o",
         },
     )
 
-    generate_segmentation: bool = attrs.field(
-        metadata={
-            "help_string": "generate segmentation using xcerebralseg",
-            "mandatory": True,
-            "argstr": "--xcerseg",
-            "xor": {"use_existing_segmentation", "segmentation_file"},
-        }
-    )
-
-    use_existing_segmentation: bool = attrs.field(
+    generate_segmentation: bool = field(
         metadata={
-            "help_string": "use existing segmentation",
+            "help_string": "generate or use subject's head segmentation",
             "mandatory": True,
-            "argstr": "--no-xcerseg",
-            "xor": {"generate_segmentation", "segmentation_file"},
+            "formatter": lambda generate_segmentation: (
+                ""
+                if generate_segmentation is NOTHING
+                else "--xcerseg" if generate_segmentation else "--no-xcerseg"
+            ),
+            "xor": {"head_segmentation"},
         }
     )
 
-    segmentation_file: str = attrs.field(
+    head_segmentation: PathLike = field(
         metadata={
-            "help_string": "use custom segmentation",
+            "help_string": "custom head segmentation",
             "mandatory": True,
             "argstr": "--head",
-            "xor": {"generate_segmentation", "use_existing_segmentation"},
+            "xor": {"generate_segmentation"},
         }
     )
 
-    no_pons_segmentation: bool = attrs.field(
+    no_pons_segmentation: bool = field(
         metadata={
             "help_string": "exclude pons from segmentation",
             "argstr": "--no-pons",
             "requires": {"generate_segmentation"},
         }
     )
 
-    no_vermis_segmentation: bool = attrs.field(
+    no_vermis_segmentation: bool = field(
         metadata={
             "help_string": "exclude vermis from segmentation",
             "argstr": "--no-vermis",
             "requires": {"generate_segmentation"},
         }
     )
 
-    colortable: str = attrs.field(
-        metadata={
-            "help_string": "use custom colortable",
-            "argstr": "--ctab",
-        }
+    colortable: str = field(
+        metadata={"help_string": "use custom colortable", "argstr": "--ctab"}
     )
 
-    upsampling_factor: int = attrs.field(
-        metadata={
-            "help_string": "upsampling factor (defaults to 2)",
-            "argstr": "--usf",
-        }
+    upsampling_factor: int = field(
+        metadata={"help_string": "upsampling factor (defaults to 2)", "argstr": "--usf"}
     )
 
-    output_upsampling_factor: int = attrs.field(
+    output_upsampling_factor: int = field(
         metadata={
             "help_string": "output upsampling factor (if different from upsampling factor)",
             "argstr": "--output-usf",
         }
     )
 
-    keep_hypointensities: bool = attrs.field(
+    keep_hypointensities: bool = field(
         metadata={
             "help_string": "do not relabel hypointensities as white matter",
             "argstr": "--keep-hypo",
         }
     )
 
-    keep_corpus_callosum: bool = attrs.field(
+    keep_corpus_callosum: bool = field(
         metadata={
             "help_string": "do not relabel corpus callosum as white matter",
             "argstr": "--keep-cc",
         }
     )
 
-    subsegment_white_matter: bool = attrs.field(
+    subsegment_white_matter: bool = field(
         metadata={
             "help_string": "subsegment white matter into lobes",
             "argstr": "--subsegwm",
         }
     )
 
 
-class GTMSeg(pydra.ShellCommandTask):
-    """Task generator for FreeSurfer's gtmseg."""
+class GTMSeg(ShellCommandTask):
+    """Task definition for gtmseg."""
 
-    input_spec = pydra.specs.SpecInfo(
-        name="GTMSegInput",
-        bases=(GTMSegSpec, specs.SubjectsDirSpec),
-    )
+    executable = "gtmseg"
 
-    output_spec = pydra.specs.SpecInfo(
-        name="GTMSegOutput",
-        bases=(specs.SubjectsDirOutSpec,),
-    )
+    input_spec = SpecInfo(name="Output", bases=(GTMSegSpec, specs.SubjectsDirSpec))
 
-    executable = "gtmseg"
+    output_spec = SpecInfo(name="Input", bases=(specs.SubjectsDirOutSpec,))
```

### Comparing `pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/mri_convert.py` & `pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mri/convert.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,63 @@
 """
-MRIConvert
-==========
+Convert
+=======
 
 General purpose utility for converting between different file formats.
 
 Examples
 --------
 
 Convert volume data to float:
 
->>> task = MRIConvert(
-...     input_volume_file="orig.nii.gz",
-...     output_volume_file="float.nii.gz",
-...     output_data_type="float",
-... )
+>>> task = Convert(input_volume="orig.nii.gz", output_volume="float.nii.gz", output_datatype="float")
 >>> task.cmdline
 'mri_convert -odt float orig.nii.gz float.nii.gz'
 """
 
-import attrs
+__all__ = ["Convert"]
 
-import pydra
+from os import PathLike
 
-__all__ = ["MRIConvert"]
+from attrs import define, field
 
+from pydra.engine.specs import ShellSpec, SpecInfo
+from pydra.engine.task import ShellCommandTask
 
-@attrs.define(slots=False, kw_only=True)
-class MRIConvertSpec(pydra.specs.ShellSpec):
+
+@define(kw_only=True)
+class ConvertSpec(ShellSpec):
     """Specifications for mri_convert."""
 
-    input_volume_file: str = attrs.field(
+    input_volume: PathLike = field(
         metadata={
             "help_string": "input volume",
             "mandatory": True,
             "argstr": "",
             "position": -2,
         }
     )
 
-    output_volume_file: str = attrs.field(
+    output_volume: str = field(
         metadata={
             "help_string": "output volume",
             "argstr": "",
             "position": -1,
-            "output_file_template": "{input_volume}_converted.nii.gz",
+            "output_file_template": "{input_volume}_convert.nii.gz",
         }
     )
 
-    output_data_type: str = attrs.field(
+    output_datatype: str = field(
         metadata={
-            "help_string": "output data type",
+            "help_string": "output datatype",
             "argstr": "-odt",
+            "allowed_values": {"uchar", "short", "int", "float", "rgb"},
         }
     )
 
 
-class MRIConvert(pydra.ShellCommandTask):
-    """Task for mri_convert."""
+class Convert(ShellCommandTask):
+    """Task definition for mri_convert."""
 
-    input_spec = pydra.specs.SpecInfo(
-        name="MRIConvertInput",
-        bases=(MRIConvertSpec, pydra.specs.ShellSpec),
-    )
+    input_spec = SpecInfo(name="ConvertInput", bases=(ConvertSpec,))
 
     executable = "mri_convert"
```

### Comparing `pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/mri_surf2surf.py` & `pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mri/surf2surf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,262 +1,263 @@
 """
-MRISurf2Surf
+parcellation_tableSurf2Surf
 ============
 
 Resamples data from one surface onto another. If both the source and
 target subjects are the same, this is just a format conversion.
 
 Examples
 --------
 1. Resample a subject's thickness of the left cortical hemisphere on to a 7th order
 icosahedron and save in analyze4d format:
 
->>> task = MRISurf2Surf(
+>>> task = Surf2Surf(
 ...     hemisphere="lh",
 ...     source_subject_id="bert",
-...     source_surface_file="thickness",
+...     source_surface="thickness",
 ...     source_format="curv",
 ...     target_subject_id="ico",
 ...     target_icosahedron_order=7,
-...     target_surface_file="bert-thickness-lh.img",
+...     target_surface="bert-thickness-lh.img",
 ...     target_format="analyze4d",
 ... )
 >>> task.cmdline
 'mri_surf2surf --srcsubject bert --sval thickness --sfmt curv --trgsubject ico --trgicoorder 7 \
 --tval bert-thickness-lh.img --tfmt analyze4d --hemi lh'
 
 2. Resample data on the icosahedron to the right hemisphere of subject bert:
 
->>> task = MRISurf2Surf(
+>>> task = Surf2Surf(
 ...     hemisphere="rh",
 ...     source_subject_id="ico",
-...     source_surface_file="icodata-rh.mgh",
+...     source_surface="icodata-rh.mgh",
 ...     target_subject_id="bert",
-...     target_surface_file="bert-ico-rh.mgh",
+...     target_surface="bert-ico-rh.mgh",
 ... )
 >>> task.cmdline
 'mri_surf2surf --srcsubject ico --sval icodata-rh.mgh --trgsubject bert --tval bert-ico-rh.mgh --hemi rh'
 
 3. Convert the surface coordinates of the lh.white of a subject to a (talairach) average:
 
->>> task = MRISurf2Surf(
+>>> task = Surf2Surf(
 ...     source_subject_id="yoursubject",
-...     use_vertex_coordinates_in_talairach_from_surface="white",
+...     use_vertex_coordinates_in_talairach="white",
 ...     target_subject_id="youraveragesubject",
-...     target_surface_file="lh.white.yoursubject",
-...     save_target_with_vertex_coordinates_from_file="$SUBJECTS_DIR/fsaverage/mri/orig.mgz",
+...     target_surface="lh.white.yoursubject",
+...     save_vertex_coordinates_from_file="$SUBJECTS_DIR/fsaverage/mri/orig.mgz",
 ... )
 >>> task.cmdline
 'mri_surf2surf --srcsubject yoursubject --sval-tal-xyz white --trgsubject youraveragesubject \
 --tval lh.white.yoursubject --tval-xyz $SUBJECTS_DIR/fsaverage/mri/orig.mgz'
 
 4. Convert the surface coordinates of the lh.white of a subject to the subject's functional space:
 
->>> task = MRISurf2Surf(
+>>> task = Surf2Surf(
 ...     registration_file="register.lta",
 ...     hemisphere="lh",
-...     use_vertex_coordinates_from_surface="white",
-...     save_target_with_vertex_coordinates_from_file="template.nii.gz",
-...     target_surface_file="./lh.white.func",
+...     use_vertex_coordinates_in_surface="white",
+...     save_vertex_coordinates_from_file="template.nii.gz",
+...     target_surface="./lh.white.func",
 ...     source_subject_id="yoursubject",
 ... )
 >>> task.cmdline
 'mri_surf2surf --srcsubject yoursubject --sval-xyz white --reg register.lta --tval ./lh.white.func \
 --tval-xyz template.nii.gz --hemi lh'
 
 
 5. Extract surface normals of the white surface and save in a volume-encoded file:
 
->>> task = MRISurf2Surf(
+>>> task = Surf2Surf(
 ...     source_subject_id="yoursubject",
 ...     hemisphere="lh",
-...     use_vertex_normal_coordinates_from_surface="white",
-...     target_surface_file="lh.white.norm.mgh",
+...     use_vertex_normal_coordinates="white",
+...     target_surface="lh.white.norm.mgh",
 ... )
 >>> task.cmdline
 'mri_surf2surf --srcsubject yoursubject --sval-nxyz white --tval lh.white.norm.mgh --hemi lh'
 
 6. Convert the annotation for one subject to the surface of another:
 
->>> task = MRISurf2Surf(
+>>> task = Surf2Surf(
 ...     source_subject_id="subj1",
 ...     target_subject_id="subj2",
 ...     hemisphere="lh",
 ...     source_annotation_file="$SUBJECTS_DIR/subj1/label/lh.aparc.annot",
 ...     target_annotation_file="$SUBJECTS_DIR/subj2/label/lh.subj1.aparc.annot",
 ... )
 >>> task.cmdline
 'mri_surf2surf --srcsubject subj1 --sval-annot $SUBJECTS_DIR/subj1/label/lh.aparc.annot --trgsubject subj2 \
 --tval $SUBJECTS_DIR/subj2/label/lh.subj1.aparc.annot --hemi lh'
 
 
 """
-import attrs
 
-import pydra
+__all__ = ["Surf2Surf"]
 
-from . import specs
 
-__all__ = ["MRISurf2Surf"]
+from attrs import define, field
 
+from pydra.engine.specs import ShellSpec, SpecInfo
+from pydra.engine.task import ShellCommandTask
+from pydra.tasks.freesurfer.v7_4 import specs
 
-@attrs.define(slots=False, kw_only=True)
-class MRISurf2SurfSpec(pydra.specs.ShellSpec):
+
+@define(kw_only=True)
+class Surf2SurfSpec(ShellSpec):
     """Specifications for mri_surf2surf."""
 
-    source_subject_id: str = attrs.field(
+    source_subject_id: str = field(
         metadata={
             "help_string": "source subject identifier within FreeSurfer's subjects directory",
             "argstr": "--srcsubject",
         }
     )
 
-    source_surface_file: str = attrs.field(
+    source_surface: str = field(
         metadata={
             "help_string": "source surface file",
             "argstr": "--sval",
         }
     )
 
-    use_vertex_coordinates_from_surface: str = attrs.field(
+    use_vertex_coordinates_in_surface: str = field(
         metadata={
             "help_string": "extract coordinates for each vertex of the surface",
             "argstr": "--sval-xyz",
             "xor": {
-                "use_vertex_coordinates_in_talairach_from_surface",
-                "use_vertex_area_from_surface",
-                "use_vertex_normal_coordinates_from_surface",
+                "use_vertex_coordinates_in_talairach",
+                "use_vertex_area",
+                "use_vertex_normal_coordinates",
             },
         }
     )
 
-    use_vertex_coordinates_in_talairach_from_surface: str = attrs.field(
+    use_vertex_coordinates_in_talairach: str = field(
         metadata={
-            "help_string": "extract coordinates and transform them to Talairach for each vertex of the surface",
+            "help_string": "extract coordinates for each vertex and transform them to Talairach",
             "argstr": "--sval-tal-xyz",
             "xor": {
-                "use_vertex_coordinates_from_surface",
-                "use_vertex_area_from_surface",
-                "use_vertex_normal_coordinates_from_surface",
+                "use_vertex_coordinates_in_surface",
+                "use_vertex_area",
+                "use_vertex_normal_coordinates",
             },
         }
     )
 
-    use_vertex_area_from_surface: str = attrs.field(
+    use_vertex_area: str = field(
         metadata={
             "help_string": "extract surface area for each vertex of the surface",
             "argstr": "--sval-area",
             "xor": {
-                "use_vertex_coordinates_from_surface",
-                "use_vertex_coordinates_in_talairach_from_surface",
-                "use_vertex_normal_coordinates_from_surface",
+                "use_vertex_coordinates_in_surface",
+                "use_vertex_coordinates_in_talairach",
+                "use_vertex_normal_coordinates",
             },
         }
     )
 
-    use_vertex_normal_coordinates_from_surface: str = attrs.field(
+    use_vertex_normal_coordinates: str = field(
         metadata={
             "help_string": "extract surface normal coordinates for each vertex of the surface",
             "argstr": "--sval-nxyz",
             "xor": {
-                "use_vertex_coordinates_from_surface",
-                "use_vertex_coordinates_in_talairach_from_surface",
-                "use_vertex_area_from_surface",
+                "use_vertex_coordinates_in_surface",
+                "use_vertex_coordinates_in_talairach",
+                "use_vertex_area",
             },
         }
     )
 
-    source_annotation_file: str = attrs.field(
+    source_annotation_file: str = field(
         metadata={
             "help_string": "source annotation file",
             "argstr": "--sval-annot",
             "requires": {"target_annotation_file"},
         }
     )
 
-    source_format: str = attrs.field(
+    source_format: str = field(
         metadata={
             "help_string": "source format type string",
             "argstr": "--sfmt",
         }
     )
 
-    source_icosahedron_order: int = attrs.field(
+    source_icosahedron_order: int = field(
         metadata={
             "help_string": "source icosahedron order number",
             "argstr": "--srcicoorder",
         }
     )
 
-    registration_file: str = attrs.field(
+    registration_file: str = field(
         metadata={
             "help_string": "apply registration to vertex coordinates",
             "argstr": "--reg",
-            "requires": {"use_vertex_coordinates_from_surface"},
+            "requires": {"use_vertex_coordinates_in_surface"},
             "xor": {"inverse_registration_file"},
         }
     )
 
-    inverse_registration_file: str = attrs.field(
+    inverse_registration_file: str = field(
         metadata={
             "help_string": "apply inverse registration to vertex coordinates",
             "argstr": "--reg-inv",
-            "requires": {"use_vertex_coordinates_from_surface"},
+            "requires": {"use_vertex_coordinates_in_surface"},
             "xor": {"registration_file"},
         }
     )
 
-    target_subject_id: str = attrs.field(
+    target_subject_id: str = field(
         metadata={
             "help_string": "target subject identifier within FreeSurfer's subjects directory",
             "argstr": "--trgsubject",
         }
     )
 
-    target_icosahedron_order: int = attrs.field(
+    target_icosahedron_order: int = field(
         metadata={
             "help_string": "target icosahedron order number",
             "argstr": "--trgicoorder",
         }
     )
 
-    target_surface_file: str = attrs.field(
+    target_surface: str = field(
         metadata={
             "help_string": "target surface file",
             "argstr": "--tval",
             "xor": {"target_annotation_file"},
         }
     )
 
-    save_target_with_vertex_coordinates_from_file: str = attrs.field(
+    save_vertex_coordinates_from_file: str = field(
         metadata={
             "help_string": "save target surface with different vertex coordinates",
             "argstr": "--tval-xyz",
-            "requires": {"target_surface_file"},
+            "requires": {"target_surface"},
         }
     )
 
-    target_annotation_file: str = attrs.field(
+    target_annotation_file: str = field(
         metadata={
             "help_string": "target annotation file",
             "argstr": "--tval",
-            "xor": {"target_surface_file"},
+            "xor": {"target_surface"},
         }
     )
 
-    target_format: str = attrs.field(
+    target_format: str = field(
         metadata={
             "help_string": "target format type string",
             "argstr": "--tfmt",
         }
     )
 
 
-class MRISurf2Surf(pydra.ShellCommandTask):
-    """Task for mri_surf2surf."""
+class Surf2Surf(ShellCommandTask):
+    """Task definition for mri_surf2surf."""
 
-    input_spec = pydra.specs.SpecInfo(
-        name="MRISurf2SurfInput",
-        bases=(MRISurf2SurfSpec, specs.HemisphereSpec, specs.SubjectsDirSpec),
+    input_spec = SpecInfo(
+        name="Input", bases=(Surf2SurfSpec, specs.HemisphereSpec, specs.SubjectsDirSpec)
     )
 
     executable = "mri_surf2surf"
```

### Comparing `pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/mris_anatomical_stats.py` & `pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mris/anatomical_stats.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,124 @@
 """
-MRISAnatomicalStats
-===================
+AnatomicalStats
+===============
 
 Computes a number of anatomical properties.
 
 Examples
 --------
 
->>> task = MRISAnatomicalStats(
-...     subject_id="subjid",
-...     hemisphere="lh",
-...     annotation_file="subjid/label/lh.aparc.annot",
-...     format_stdout_as_table=True,
-... )
->>> task.cmdline
-'mris_anatomical_stats -a subjid/label/lh.aparc.annot -b subjid lh white'
-
->>> task = MRISAnatomicalStats(
-...     subject_id="subjid",
-...     hemisphere="lh",
-...     label_file="lh.cortex.label",
-...     format_stdout_as_table=True,
-... )
->>> task.cmdline
-'mris_anatomical_stats -l lh.cortex.label -b subjid lh white'
+>>> task = AnatomicalStats(subject_id="subjid", hemisphere="lh", annotation_file="lh.aparc.annot")
+>>> task.cmdline    # doctest: +ELLIPSIS
+'mris_anatomical_stats -a lh.aparc.annot -f ...lh.white.stats -log ...lh.white.log subjid lh white'
+
+>>> task = AnatomicalStats(subject_id="subjid", hemisphere="lh", label_file="lh.cortex.label")
+>>> task.cmdline    # doctest: +ELLIPSIS
+'mris_anatomical_stats -l lh.cortex.label -f ...lh.white.stats -log ...lh.white.log subjid lh white'
 """
 
-import attrs
+__all__ = ["AnatomicalStats"]
 
-import pydra
+from os import PathLike
 
-from . import specs
+from attrs import define, field
 
-__all__ = ["MRISAnatomicalStats"]
+from pydra.engine.specs import ShellSpec, SpecInfo
+from pydra.engine.task import ShellCommandTask
+from pydra.tasks.freesurfer.v7_4 import specs
 
 
-@attrs.define(slots=False, kw_only=True)
-class MRISAnatomicalStatsSpec(pydra.specs.ShellSpec):
+@define(slots=False, kw_only=True)
+class AnatomicalStatsSpec(ShellSpec):
     """Specifications for mris_anatomical_stats."""
 
-    subject_id: str = attrs.field(
+    subject_id: str = field(
         metadata={
-            "help_string": "subject to process",
+            "help_string": "subject identifier",
             "mandatory": True,
             "argstr": "",
             "position": -3,
         }
     )
 
-    hemisphere: str = attrs.field(
+    hemisphere: str = field(
         metadata={
-            "help_string": "left or right hemisphere",
+            "help_string": "process left or right hemisphere",
             "mandatory": True,
             "argstr": "",
             "position": -2,
             "allowed_values": {"lh", "rh"},
         }
     )
 
-    surface_name: str = attrs.field(
+    surface_name: str = field(
         default="white",
-        metadata={
-            "help_string": "surface name",
-            "argstr": "",
-            "position": -1,
-        },
+        metadata={"help_string": "surface name", "argstr": "", "position": -1},
     )
 
-    label_file: str = attrs.field(
+    label_file: PathLike = field(
         metadata={
-            "help_string": "restrict computation to the specified label",
+            "help_string": "restrict computation to each label in this file",
             "argstr": "-l",
         }
     )
 
-    annotation_file: str = attrs.field(
+    annotation_file: PathLike = field(
         metadata={
             "help_string": "compute statistics for each annotation in this file",
             "argstr": "-a",
         }
     )
 
-    format_stdout_as_table: bool = attrs.field(
+    output_stats_file: str = field(
         metadata={
-            "help_string": "write to stdout in table format",
-            "argstr": "-b",
+            "help_string": "output stats file in table format",
+            "argstr": "-f",
+            "output_file_template": "{hemisphere}.{surface_name}.stats",
         }
     )
 
-    output_table_file = attrs.field(
+    output_log_file: str = field(
         metadata={
-            "help_string": "write table output to this file",
-            "argstr": "-f",
+            "help_string": "output stats file in log format",
+            "argstr": "-log",
+            "output_file_template": "{hemisphere}.{surface_name}.log",
         }
     )
 
-    output_stats_file = attrs.field(
+    output_colortable_file: PathLike = field(
         metadata={
-            "help_string": "write stats output to this file",
-            "argstr": "-log",
+            "help_string": "write colortable for annotations",
+            "argstr": "-c",
+            "requires": {"annotation_file"},
         }
     )
 
-    subjects_dir: str = attrs.field(
+    no_global_stats: bool = field(
         metadata={
-            "help_string": "subjects directory",
-            "argstr": "-sdir",
+            "help_string": "do not write global stats",
+            "argstr": "-noglobal",
+            "requires": {"output_stats_file"},
         }
     )
 
-
-class MRISAnatomicalStats(pydra.engine.ShellCommandTask):
-    """Task for mris_annatomical_stats."""
-
-    input_spec = pydra.specs.SpecInfo(
-        name="MRISAnnatomicalStatsInput",
-        bases=(MRISAnatomicalStatsSpec,),
+    no_header: bool = field(
+        metadata={
+            "help_string": "do not write a header",
+            "argstr": "-noheader",
+            "requires": {"output_log_file"},
+        }
     )
 
-    output_spec = pydra.specs.SpecInfo(
-        name="MRISAnnatomicalStatsOutput",
-        bases=(specs.SubjectsDirOutSpec,),
+    subjects_dir: str = field(
+        metadata={"help_string": "subjects directory", "argstr": "-sdir"}
     )
 
+
+class AnatomicalStats(ShellCommandTask):
+    """Task definition for mris_anatomical_stats."""
+
     executable = "mris_anatomical_stats"
+
+    input_spec = SpecInfo(name="Input", bases=(AnatomicalStatsSpec,))
+
+    output_spec = SpecInfo(name="Output", bases=(specs.SubjectsDirOutSpec,))
```

### Comparing `pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/mris_ca_label.py` & `pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mris/ca_label.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,127 @@
 """
-MRISCALabel
-===========
+CALabel
+=======
 
 Assign an anatomical label to each cortical surface vertex.
 
 Examples
 --------
 
->>> task = MRISCALabel(
+>>> task = CALabel(
 ...     subject_id="my_subject",
 ...     hemisphere="lh",
-...     canonical_surface_file="sphere.reg",
-...     surface_atlas_file="lh.rahul.gcs",
-...     original_surface_file="white",
+...     canonical_surface="sphere.reg",
+...     surface_atlas="lh.rahul.gcs",
+...     original_surface="white",
 ...     no_covariance=True,
-...     parcellation_table_file="colortable.txt",
+...     parcellation_table="colortable.txt",
+...     atlas_name="rahul",
 ... )
 >>> task.cmdline  # doctest: +ELLIPSIS
 'mris_ca_label -orig white -novar -t colortable.txt \
-my_subject lh sphere.reg lh.rahul.gcs ...lh.aparc.annot'
+my_subject lh sphere.reg lh.rahul.gcs ...lh.rahul.annot'
 """
 
-import attrs
+__all__ = ["CALabel"]
 
-import pydra
+from os import PathLike
 
-from . import specs
+from attrs import define, field
 
-__all__ = ["MRISCALabel"]
+from pydra.engine.specs import ShellSpec, SpecInfo
+from pydra.engine.task import ShellCommandTask
+from pydra.tasks.freesurfer.v7_4 import specs
 
 
-@attrs.define(slots=False, kw_only=True)
-class MRISCALabelSpec(pydra.specs.ShellSpec):
+@define(slots=False, kw_only=True)
+class CALabelSpec(ShellSpec):
     """Specifications for mris_ca_label."""
 
-    subject_id: str = attrs.field(
+    subject_id: str = field(
         metadata={
             "help_string": "subject to process",
             "mandatory": True,
             "argstr": "",
             "position": -5,
         }
     )
 
-    hemisphere: str = attrs.field(
+    hemisphere: str = field(
         metadata={
-            "help_string": "left or right hemisphere",
+            "help_string": "process left or right hemisphere",
             "mandatory": True,
             "argstr": "",
             "position": -4,
             "allowed_values": {"lh", "rh"},
         }
     )
 
-    canonical_surface_file: str = attrs.field(
+    canonical_surface: PathLike = field(
         metadata={
             "help_string": "canonical surface file",
             "mandatory": True,
             "argstr": "",
             "position": -3,
         }
     )
 
-    surface_atlas_file: str = attrs.field(
+    surface_atlas: PathLike = field(
         metadata={
             "help_string": "surface atlas file",
             "mandatory": True,
             "argstr": "",
             "position": -2,
         }
     )
 
-    output_annotation_file: str = attrs.field(
+    atlas_name: str = field(default="atlas", metadata={"help_string": "atlas name"})
+
+    output_annotation_file: str = field(
         metadata={
             "help_string": "output surface annotation file",
             "argstr": "",
             "position": -1,
-            "output_file_template": "{hemisphere}.aparc.annot",
+            "output_file_template": "{hemisphere}.{atlas_name}.annot",
         }
     )
 
-    subjects_dir: str = attrs.field(
+    subjects_dir: str = field(
+        metadata={"help_string": "subjects directory", "argstr": "-sdir"}
+    )
+
+    aseg_volume: PathLike = field(
         metadata={
-            "help_string": "subjects directory",
-            "argstr": "-sdir",
+            "help_string": "use aseg volume to correct midline",
+            "argstr": "-aseg",
         }
     )
 
-    original_surface_file: str = attrs.field(
+    original_surface: str = field(
         default="smoothwm",
-        metadata={
-            "help_string": "original surface file",
-            "argstr": "-orig",
-        },
+        metadata={"help_string": "original surface", "argstr": "-orig"},
     )
 
-    no_covariance: bool = attrs.field(
+    no_covariance: bool = field(
         metadata={
             "help_string": "set covariance matrices to identity",
             "argstr": "-novar",
         }
     )
 
-    parcellation_table_file: str = attrs.field(
-        metadata={
-            "help_string": "parcellation table file",
-            "argstr": "-t",
-        }
+    parcellation_table: PathLike = field(
+        metadata={"help_string": "parcellation table", "argstr": "-t"}
     )
 
-
-class MRISCALabel(pydra.ShellCommandTask):
-    """Task for mris_ca_label."""
-
-    input_spec = pydra.specs.SpecInfo(
-        name="MRISCALabelInput",
-        bases=(MRISCALabelSpec,),
+    cortex_label_file: PathLike = field(
+        metadata={"help_string": "cortex label file", "argstr": "-l"}
     )
 
-    output_spec = pydra.specs.SpecInfo(
-        name="MRISCALabelOuput",
-        bases=(specs.SubjectsDirOutSpec,),
-    )
+
+class CALabel(ShellCommandTask):
+    """Task definition for mris_ca_label."""
 
     executable = "mris_ca_label"
+
+    input_spec = SpecInfo(name="Input", bases=(CALabelSpec,))
+
+    output_spec = SpecInfo(name="Output", bases=(specs.SubjectsDirOutSpec,))
```

### Comparing `pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/mris_ca_train.py` & `pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mris/ca_train.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,124 +1,111 @@
 """
-MRISCATrain
-===========
+CATrain
+=======
 
 Examples
 --------
 
->>> task = MRISCATrain(
+>>> task = CATrain(
 ...     hemisphere="lh",
-...     canonical_surface_file="sphere.reg",
+...     canonical_surface="sphere.reg",
 ...     annotation_file="my_manual_labeling",
 ...     subject_ids=["subj1", "subj2"],
-...     parcellation_table_file="colortable.txt",
+...     parcellation_table="colortable.txt",
 ... )
 >>> task.cmdline  # doctest: +ELLIPSIS
 'mris_ca_train -orig smoothwm -t colortable.txt -n 2 \
 lh sphere.reg my_manual_labeling subj1 subj2 ...lh.my_atlas.gcs'
 """
 
-import typing as ty
+__all__ = ["CATrain"]
 
-import attrs
+from os import PathLike
+from typing import Sequence
 
-import pydra
+from attrs import define, field
 
-from . import specs
+from pydra.engine.specs import ShellSpec, SpecInfo
+from pydra.engine.task import ShellCommandTask
+from pydra.tasks.freesurfer.v7_4 import specs
 
-__all__ = ["MRISCATrain"]
 
-
-@attrs.define(slots=False, kw_only=True)
-class MRISCATrainSpec(pydra.specs.ShellSpec):
+@define(slots=False, kw_only=True)
+class CATrainSpec(ShellSpec):
     """Specifications for mris_ca_train."""
 
-    hemisphere: str = attrs.field(
+    hemisphere: str = field(
         metadata={
-            "help_string": "left or right hemisphere",
+            "help_string": "process left or right hemisphere",
             "mandatory": True,
             "argstr": "",
             "position": -5,
             "allowed_values": {"lh", "rh"},
         }
     )
 
-    canonical_surface_file: str = attrs.field(
+    canonical_surface: PathLike = field(
         metadata={
-            "help_string": "canonical surface file",
+            "help_string": "canonical surface",
             "mandatory": True,
             "argstr": "",
             "position": -4,
         }
     )
 
-    annotation_file: str = attrs.field(
+    annotation_file: PathLike = field(
         metadata={
-            "help_string": "per-subject annotation file",
+            "help_string": "annotation file",
             "mandatory": True,
             "argstr": "",
             "position": -3,
         }
     )
 
-    subject_ids: ty.Iterable[str] = attrs.field(
+    subject_ids: Sequence[str] = field(
         metadata={
-            "help_string": "subject to process",
+            "help_string": "subject identifiers",
             "mandatory": True,
             "argstr": "...",
             "position": -2,
         }
     )
 
-    output_surface_atlas_file: str = attrs.field(
+    output_surface_atlas: str = field(
         metadata={
             "help_string": "output surface atlas file",
             "argstr": "",
             "position": -1,
             "output_file_template": "{hemisphere}.my_atlas.gcs",
         }
     )
 
-    subjects_dir: str = attrs.field(
-        metadata={
-            "help_string": "subjects directory",
-            "argstr": "-sdir",
-        }
+    subjects_dir: str = field(
+        metadata={"help_string": "subjects directory", "argstr": "-sdir"}
     )
 
-    original_surface_file: str = attrs.field(
+    original_surface: str = field(
         default="smoothwm",
-        metadata={
-            "help_string": "original surface file",
-            "argstr": "-orig",
-        },
+        metadata={"help_string": "original surface", "argstr": "-orig"},
     )
 
-    parcellation_table_file: str = attrs.field(
-        metadata={
-            "help_string": "parcellation table file",
-            "argstr": "-t",
-        }
+    parcellation_table: str = field(
+        metadata={"help_string": "parcellation table", "argstr": "-t"}
     )
 
-    number_of_subjects: int = attrs.field(
+    num_subjects: int = field(
         metadata={
             "help_string": "number of input subjects to process",
             "formatter": lambda subject_ids: f"-n {len(subject_ids)}",
+            "readonly": True,
         }
     )
 
 
-class MRISCATrain(pydra.ShellCommandTask):
-    """Task for mris_ca_train."""
+class CATrain(ShellCommandTask):
+    """Task definition for mris_ca_train."""
 
-    input_spec = pydra.specs.SpecInfo(
-        name="MRISCATrainInput",
-        bases=(MRISCATrainSpec,),
-    )
+    executable = "mris_ca_train"
 
-    output_spec = pydra.specs.SpecInfo(
-        name="MRISCATrainOuput",
-        bases=(specs.SubjectsDirOutSpec,),
-    )
+    input_spec = SpecInfo(name="Input", bases=(CATrainSpec,))
 
-    executable = "mris_ca_train"
+    output_spec = SpecInfo(name="Output", bases=(specs.SubjectsDirOutSpec,))
```

### Comparing `pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/mris_expand.py` & `pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/utils/surface_transform.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,109 +1,130 @@
-"""
-MRISExpand
-==========
-
-Expand a surface outwards by a specified amount
-while maintaining smoothness and self-intersection constraints.
-
-Examples
---------
-
-1. Expand by cortical thickness:
-
->>> task = MRISExpand(
-...     input_surface_file="lh.white",
-...     fraction_of_cortical_thickness=0.5,
-... )
->>> task.cmdline    # doctest: +ELLIPSIS
-'mris_expand -thickness lh.white 0.5 ...lh_expanded.white'
-
-2. Expand by distance from label:
-
->>> task = MRISExpand(
-...     input_surface_file="lh.white",
-...     distance=0.5,
-...     output_surface_file="lh.graymid",
-...     label="labelfile",
-... )
->>> task.cmdline
-'mris_expand -label labelfile lh.white 0.5 lh.graymid'
-"""
-
-import attrs
-
-import pydra
-
-__all__ = ["MRISExpand"]
-
-
-@attrs.define(slots=False, kw_only=True)
-class MIRSExpandSpec(pydra.specs.ShellSpec):
-    """Specifications for mris_expand."""
-
-    input_surface_file: str = attrs.field(
-        metadata={
-            "help_string": "input surface",
+from fileformats.generic import Directory, File
+import logging
+from pathlib import Path
+from pydra.engine import ShellCommandTask, specs
+import typing as ty
+
+
+logger = logging.getLogger(__name__)
+
+
+input_fields = [
+    (
+        "source_file",
+        File,
+        {
+            "help_string": "surface file with source values",
+            "argstr": "--sval {source_file}",
             "mandatory": True,
-            "argstr": "",
-            "position": -3,
-        }
-    )
-
-    distance: float = attrs.field(
-        metadata={
-            "help_string": "distance in millimeters",
+            "xor": ["source_annot_file"],
+        },
+    ),
+    (
+        "source_annot_file",
+        File,
+        {
+            "help_string": "surface annotation file",
+            "argstr": "--sval-annot {source_annot_file}",
             "mandatory": True,
-            "argstr": "",
-            "position": -2,
-            "xor": {"fraction_of_cortical_thickness"},
-        }
-    )
-
-    fraction_of_cortical_thickness: float = attrs.field(
-        metadata={
-            "help_string": "fraction of cortical thickness",
+            "xor": ["source_file"],
+        },
+    ),
+    (
+        "source_subject",
+        ty.Any,
+        {
+            "help_string": "subject id for source surface",
+            "argstr": "--srcsubject {source_subject}",
             "mandatory": True,
-            "argstr": "",
-            "position": -2,
-            "xor": {"distance"},
-        }
-    )
-
-    output_surface_file: str = attrs.field(
-        metadata={
-            "help_string": "output surface",
-            "argstr": "",
-            "position": -1,
-            "output_file_template": "{input_surface_file}_expanded",
-        }
-    )
-
-    distance_is_fraction_of_cortical_thickness: bool = attrs.field(
-        metadata={
-            "help_string": "treat distance as fraction of cortical thickness",
-            "formatter": (
-                lambda fraction_of_cortical_thickness, distance_is_fraction_of_cortical_thickness: "-thickness"
-                if fraction_of_cortical_thickness
-                or distance_is_fraction_of_cortical_thickness
-                else ""
-            ),
-        }
-    )
-
-    label: str = attrs.field(
-        metadata={
-            "help_string": "input labels",
-            "argstr": "-label",
-        }
-    )
-
-
-class MRISExpand(pydra.ShellCommandTask):
-    """Task for mris_expand."""
-
-    input_spec = pydra.specs.SpecInfo(
-        name="MRISExpandInput",
-        bases=(MIRSExpandSpec, pydra.specs.ShellSpec),
-    )
-
-    executable = "mris_expand"
+        },
+    ),
+    (
+        "hemi",
+        ty.Any,
+        {
+            "help_string": "hemisphere to transform",
+            "argstr": "--hemi {hemi}",
+            "mandatory": True,
+        },
+    ),
+    (
+        "target_subject",
+        ty.Any,
+        {
+            "help_string": "subject id of target surface",
+            "argstr": "--trgsubject {target_subject}",
+            "mandatory": True,
+        },
+    ),
+    (
+        "target_ico_order",
+        ty.Any,
+        {
+            "help_string": "order of the icosahedron if target_subject is 'ico'",
+            "argstr": "--trgicoorder {target_ico_order}",
+        },
+    ),
+    (
+        "source_type",
+        ty.Any,
+        {
+            "help_string": "source file format",
+            "argstr": "--sfmt {source_type}",
+            "requires": ["source_file"],
+        },
+    ),
+    (
+        "target_type",
+        ty.Any,
+        {"help_string": "output format", "argstr": "--tfmt {target_type}"},
+    ),
+    (
+        "reshape",
+        bool,
+        {
+            "help_string": "reshape output surface to conform with Nifti",
+            "argstr": "--reshape",
+        },
+    ),
+    (
+        "reshape_factor",
+        int,
+        {
+            "help_string": "number of slices in reshaped image",
+            "argstr": "--reshape-factor",
+        },
+    ),
+    (
+        "out_file",
+        Path,
+        {
+            "help_string": "surface file to write",
+            "argstr": "--tval {out_file}",
+            "output_file_template": "out_file",
+        },
+    ),
+    ("subjects_dir", Directory, {"help_string": "subjects directory"}),
+]
+SurfaceTransform_input_spec = specs.SpecInfo(
+    name="Input", fields=input_fields, bases=(specs.ShellSpec,)
+)
+
+output_fields = []
+SurfaceTransform_output_spec = specs.SpecInfo(
+    name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
+)
+
+
+class SurfaceTransform(ShellCommandTask):
+    """
+    Examples
+    -------
+
+    >>> from fileformats.generic import Directory, File
+    >>> from pydra.tasks.freesurfer.auto.utils.surface_transform import SurfaceTransform
+
+    """
+
+    input_spec = SurfaceTransform_input_spec
+    output_spec = SurfaceTransform_output_spec
+    executable = "mri_surf2surf"
```

### Comparing `pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/mris_preproc.py` & `pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/mris/preproc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,193 +1,183 @@
 """
-MRISPreproc
-===========
+Preproc
+=======
 
 Script to prepare surface-based data for high-level analysis
 by resampling surface or volume source data to a common subject (usually an average subject)
 and then concatenating them into one file which can then be used by a number of programs (eg, mri_glmfit).
 
 Examples
 --------
 
 >>> source_subject_ids = [f"abc{s:02d}-anat" for s in range(1, 5)]
 
 1. Resample abcXX-anat/surf/lh.thickness onto fsaverage:
 
->>> task = MRISPreproc(
+>>> task = Preproc(
 ...     source_subject_ids=source_subject_ids,
 ...     target_subject_id="fsaverage",
 ...     hemisphere="lh",
 ...     measure="thickness",
-...     output_surface_file="abc-lh-thickness.mgh",
+...     output_surface="abc-lh-thickness.mgh",
 ... )
 >>> task.cmdline
 'mris_preproc --out abc-lh-thickness.mgh --target fsaverage --hemi lh --meas thickness \
 --s abc01-anat --s abc02-anat --s abc03-anat --s abc04-anat'
 
 2. Same as above but using a fsgd file (which would have the abcXXs as Inputs):
 
->>> task = MRISPreproc(
+>>> task = Preproc(
 ...     fsgd_file="abc.fsgd",
 ...     target_subject_id="fsaverage",
 ...     hemisphere="lh",
 ...     measure="thickness",
-...     output_surface_file="abc-lh-thickness.mgh",
+...     output_surface="abc-lh-thickness.mgh",
 ... )
 >>> task.cmdline
 'mris_preproc --out abc-lh-thickness.mgh --target fsaverage --hemi lh --meas thickness --fsgd abc.fsgd'
 
 3. Same as #1 with additional smoothing by 5mm:
 
->>> task = MRISPreproc(
+>>> task = Preproc(
 ...     source_subject_ids=source_subject_ids,
 ...     target_subject_id="fsaverage",
 ...     hemisphere="lh",
 ...     measure="thickness",
-...     output_surface_file="abc-lh-thickness.sm5.mgh",
+...     output_surface="abc-lh-thickness.sm5.mgh",
 ...     target_smoothing=5,
 ... )
 >>> task.cmdline
 'mris_preproc --out abc-lh-thickness.sm5.mgh --target fsaverage --hemi lh --meas thickness \
 --s abc01-anat --s abc02-anat --s abc03-anat --s abc04-anat --fwhm 5'
 
 4. Same as #1 but using full paths.
 
->>> task = MRISPreproc(
+>>> task = Preproc(
 ...     target_subject_id="fsaverage",
 ...     hemisphere="lh",
-...     output_surface_file="abc-lh-thickness.mgh",
+...     output_surface="abc-lh-thickness.mgh",
 ...     fsgd_file="abc.fsgd",
 ...     source_format="curv",
-...     input_surface_measures=[f"abc{s:02d}-anat/surf/lh.thickness" for s in range(1, 5)],
+...     input_surface_paths=[f"abc{s:02d}-anat/surf/lh.thickness" for s in range(1, 5)],
 ... )
 >>> task.cmdline
 'mris_preproc --out abc-lh-thickness.mgh --target fsaverage --hemi lh --fsgd abc.fsgd \
 --isp abc01-anat/surf/lh.thickness --isp abc02-anat/surf/lh.thickness --isp abc03-anat/surf/lh.thickness \
 --isp abc04-anat/surf/lh.thickness --srcfmt curv'
 
 5. Same as #2 but computes paired differences.
 
->>> task = MRISPreproc(
+>>> task = Preproc(
 ...     fsgd_file="abc.fsgd",
 ...     target_subject_id="fsaverage",
 ...     hemisphere="lh",
 ...     measure="thickness",
-...     output_surface_file="abc-lh-thickness-pdiff.mgh",
+...     output_surface="abc-lh-thickness-pdiff.mgh",
 ...     compute_paired_differences=True,
 ... )
 >>> task.cmdline
 'mris_preproc --out abc-lh-thickness-pdiff.mgh --target fsaverage --hemi lh --meas thickness --fsgd abc.fsgd \
 --paired-diff'
 """
 
-import typing as ty
+__all__ = ["Preproc"]
 
-import attrs
+from os import PathLike
+from typing import Sequence
 
-import pydra
+from attrs import define, field
 
-from . import specs
+from pydra.engine.specs import ShellSpec, SpecInfo
+from pydra.engine.task import ShellCommandTask
+from pydra.tasks.freesurfer.v7_4 import specs
 
-__all__ = ["MRISPreproc"]
 
-
-@attrs.define(slots=False, kw_only=True)
-class MRISPreprocSpec(pydra.specs.ShellSpec):
-
-    output_surface_file: str = attrs.field(
+@define(kw_only=True)
+class PreprocSpec(ShellSpec):
+    output_surface: str = field(
         metadata={
-            "help_string": "output file",
+            "help_string": "output surface",
             "argstr": "--out",
-            "requires": {"target_subject_id", "hemisphere"},
             "output_file_template": "{target_subject_id}_{hemisphere}.mgz",
         }
     )
 
-    target_subject_id: str = attrs.field(
+    target_subject_id: str = field(
         metadata={
             "help_string": "subject identifier to use as common space",
             "mandatory": True,
             "argstr": "--target",
         }
     )
 
-    hemisphere: str = attrs.field(
+    hemisphere: str = field(
         metadata={
-            "help_string": "left or right hemisphere",
+            "help_string": "process left or right hemisphere",
             "mandatory": True,
             "argstr": "--hemi",
             "allowed_values": {"lh", "rh"},
         }
     )
 
-    measure: str = attrs.field(
-        metadata={
-            "help_string": "use source subject's measure as input",
-            "argstr": "--meas",
-        }
+    measure: str = field(
+        metadata={"help_string": "use measure as input", "argstr": "--meas"}
     )
 
-    source_subject_ids: ty.Iterable[str] = attrs.field(
+    source_subject_ids: Sequence[str] = field(
         metadata={
             "help_string": "source subjects used as input",
             "argstr": "--s ...",
             "requires": {"measure"},
             "xor": {"fsdg_file"},
         }
     )
 
-    fsgd_file: str = attrs.field(
+    fsgd_file: PathLike = field(
         metadata={
             "help_string": "fsgd file containing the source subjects",
             "argstr": "--fsgd",
             "xor": {"source_subject_ids"},
         }
     )
 
-    input_surface_measures: ty.Iterable[str] = attrs.field(
+    input_surface_paths: Sequence[PathLike] = field(
         metadata={
             "help_string": "paths to input surface measure files",
             "argstr": "--isp ...",
             "requires": {"fsgd_file"},
         }
     )
 
-    source_format: str = attrs.field(
+    source_format: str = field(
         metadata={
             "help_string": "source format of input surface measure files",
             "argstr": "--srcfmt",
-            "requires": {"input_surface_measures"},
+            "requires": {"input_surface_paths"},
         }
     )
 
-    target_smoothing: float = attrs.field(
-        metadata={
-            "help_string": "smooth target surface by X mm",
-            "argstr": "--fwhm",
-        }
+    target_smoothing: float = field(
+        metadata={"help_string": "smooth target surface by X mm", "argstr": "--fwhm"}
     )
 
-    source_smoothing: float = attrs.field(
+    source_smoothing: float = field(
         metadata={
             "help_string": "smooth source surface by X mm",
             "argstr": "--fwhm-src",
         }
     )
 
-    compute_paired_differences: bool = attrs.field(
+    compute_paired_differences: bool = field(
         metadata={
             "help_string": "compute paired differences",
             "argstr": "--paired-diff",
         }
     )
 
 
-class MRISPreproc(pydra.ShellCommandTask):
-    """Task for mris_preproc."""
-
-    input_spec = pydra.specs.SpecInfo(
-        name="MRISPreprocInput",
-        bases=(MRISPreprocSpec, specs.SubjectsDirSpec),
-    )
+class Preproc(ShellCommandTask):
+    """Task definition for mris_preproc."""
 
     executable = "mris_preproc"
+
+    input_spec = SpecInfo(name="Input", bases=(PreprocSpec, specs.SubjectsDirSpec))
```

### Comparing `pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/specs.py` & `pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/specs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,46 @@
+from __future__ import annotations
+
 import os
-import typing as ty
 
 import attrs
 
 import pydra
 
 __all__ = ["SubjectsDirSpec", "SubjectsDirOutSpec", "HemisphereSpec"]
 
 
 @attrs.define(slots=False, kw_only=True)
 class SubjectsDirSpec(pydra.specs.ShellSpec):
-
     subjects_dir: os.PathLike = attrs.field(
         metadata={
             "help_string": "subjects directory processed by FreeSurfer",
             "argstr": "--sd {subjects_dir}",
         }
     )
 
 
 @attrs.define(slots=False, kw_only=True)
 class SubjectsDirOutSpec(pydra.specs.ShellOutSpec):
     @staticmethod
-    def get_subjects_dir(subjects_dir: ty.Optional[str]) -> str:
+    def get_subjects_dir(subjects_dir: str | None) -> str:
         return os.fspath(subjects_dir or os.getenv("SUBJECTS_DIR"))
 
     subjects_dir: str = attrs.field(
         metadata={
             "help_string": "subjects directory processed by FreeSurfer",
             "callable": get_subjects_dir,
         }
     )
 
 
 @attrs.define(slots=False, kw_only=True)
 class HemisphereSpec(pydra.specs.ShellSpec):
+    """Specifications for hemisphere parameter."""
 
     hemisphere: str = attrs.field(
         metadata={
-            "help_string": "restrict processing to left or right hemisphere",
-            "argstr": "--hemi {hemisphere}",
+            "help_string": "process left or right hemisphere",
+            "argstr": "--hemi",
             "allowed_values": ["lh", "rh"],
         }
     )
```

### Comparing `pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/recon_all/recon_all.py` & `pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/auto/preprocess/dicom_convert.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,81 +1,90 @@
-"""Cross-sectional processing using FreeSurfer's recon-all."""
-
-import os
+from fileformats.generic import Directory, File
+import logging
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
-import attrs
-
-import pydra
-
-from . import specs
 
-__all__ = ["ReconAll"]
+logger = logging.getLogger(__name__)
 
 
-@attrs.define(slots=False, kw_only=True)
-class ReconAllSpec(pydra.specs.ShellSpec):
-    subject_id: str = attrs.field(
-        metadata={
-            "help_string": "subject identifier",
+input_fields = [
+    (
+        "dicom_dir",
+        Directory,
+        {
+            "help_string": "dicom directory from which to convert dicom files",
             "mandatory": True,
-            "argstr": "-subjid",
-        }
-    )
-
-    t1_volume_file: os.PathLike = attrs.field(
-        metadata={
-            "help_string": "input T1 volume",
-            "argstr": "-i",
-            "xor": ["t1_volume_files"],
-        }
-    )
-
-    t1_volume_files: ty.Iterable[os.PathLike] = attrs.field(
-        metadata={
-            "help_string": "input T1 volumes",
-            "argstr": "-i...",
-            "xor": ["t1_volume_file"],
-        }
-    )
-
-    t2_volume_file: os.PathLike = attrs.field(
-        metadata={
-            "help_string": "input T2 volume",
-            "argstr": "-t2",
-        }
-    )
-
-    flair_volume_file: os.PathLike = attrs.field(
-        metadata={
-            "help_string": "input FLAIR volume",
-            "argstr": "-flair",
-        }
-    )
-
-
-@attrs.define(slots=False, kw_only=True)
-class ReconAllOutSpec(pydra.specs.ShellOutSpec):
-    @staticmethod
-    def get_subject_id(subject_id: str) -> str:
-        return subject_id
-
-    subject_id: str = attrs.field(
-        metadata={
-            "help_string": "subject identifier where outputs are written",
-            "callable": get_subject_id,
-        }
-    )
-
-
-class ReconAll(pydra.ShellCommandTask):
-    input_spec = pydra.specs.SpecInfo(
-        name="ReconAllInput",
-        bases=(ReconAllSpec, specs.ReconAllBaseSpec),
-    )
-
-    output_spec = pydra.specs.SpecInfo(
-        name="ReconAllOutput",
-        bases=(ReconAllOutSpec, specs.ReconAllBaseOutSpec),
-    )
-
-    executable = "recon-all"
+        },
+    ),
+    (
+        "base_output_dir",
+        Directory,
+        {
+            "help_string": "directory in which subject directories are created",
+            "mandatory": True,
+        },
+    ),
+    (
+        "subject_dir_template",
+        str,
+        "S.%04d",
+        {"help_string": "template for subject directory name"},
+    ),
+    (
+        "subject_id",
+        ty.Any,
+        {"help_string": "subject identifier to insert into template"},
+    ),
+    ("file_mapping", list, {"help_string": "defines the output fields of interface"}),
+    (
+        "out_type",
+        ty.Any,
+        "niigz",
+        {"help_string": "defines the type of output file produced"},
+    ),
+    (
+        "dicom_info",
+        File,
+        {"help_string": "File containing summary information from mri_parse_sdcmdir"},
+    ),
+    (
+        "seq_list",
+        list,
+        {
+            "help_string": "list of pulse sequence names to be converted.",
+            "requires": ["dicom_info"],
+        },
+    ),
+    (
+        "ignore_single_slice",
+        bool,
+        {
+            "help_string": "ignore volumes containing a single slice",
+            "requires": ["dicom_info"],
+        },
+    ),
+    ("subjects_dir", Directory, {"help_string": "subjects directory"}),
+]
+DICOMConvert_input_spec = specs.SpecInfo(
+    name="Input", fields=input_fields, bases=(specs.ShellSpec,)
+)
+
+output_fields = []
+DICOMConvert_output_spec = specs.SpecInfo(
+    name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
+)
+
+
+class DICOMConvert(ShellCommandTask):
+    """
+    Examples
+    -------
+
+    >>> from fileformats.generic import Directory, File
+    >>> from pydra.tasks.freesurfer.auto.preprocess.dicom_convert import DICOMConvert
+
+    """
+
+    input_spec = DICOMConvert_input_spec
+    output_spec = DICOMConvert_output_spec
+    executable = "mri_convert"
```

### Comparing `pydra_freesurfer-0.0.9/pydra/tasks/freesurfer/recon_all/specs.py` & `pydra_freesurfer-0.1.1/pydra/tasks/freesurfer/v7_4/recon_all/specs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-import os
-import typing as ty
-
-import attrs
+__all__ = ["ReconAllBaseSpec", "ReconAllBaseOutSpec"]
 
-import pydra
+from os import PathLike
+from typing import List
 
-from ..specs import SubjectsDirOutSpec as ReconAllBaseOutSpec
+from attrs import define, field
 
-__all__ = ["ReconAllBaseSpec", "ReconAllBaseOutSpec"]
+from pydra.engine.specs import ShellSpec
+from pydra.tasks.freesurfer.v7_4.specs import SubjectsDirOutSpec
 
 # FIXME: Change to ty.Tuple[float, float, float] once Pydra supports it, if ever.
-SeedPoint = ty.List[float]
+SeedPoint = List[float]
+
 
+@define(slots=False, kw_only=True)
+class ReconAllBaseSpec(ShellSpec):
+    """Base specifications for recon-all."""
 
-@attrs.define(slots=False, kw_only=True)
-class ReconAllBaseSpec(pydra.specs.ShellSpec):
-    directive: str = attrs.field(
+    directive: str = field(
         default="all",
         metadata={
             "help_string": "process directive",
             "argstr": "-{directive}",
             "allowed_values": {
                 # All steps.
                 "all",
@@ -35,111 +36,90 @@
                 "autorecon2-pial",
                 # Steps 24 to 31.
                 "autorecon3",
             },
         },
     )
 
-    custom_brain_mask_file: os.PathLike = attrs.field(
-        metadata={
-            "help_string": "use a custom brain mask",
-            "argstr": "-xmask",
-        },
+    custom_brain_mask: PathLike = field(
+        metadata={"help_string": "custom brain mask", "argstr": "-xmask"}
     )
 
-    hemisphere: str = attrs.field(
+    hemisphere: str = field(
         metadata={
             "help_string": "restrict processing to this hemisphere",
-            "argstr": "-hemi {hemisphere}",
+            "argstr": "-hemi",
             "allowed_values": ["lh", "rh"],
-        },
+            "xor": {"parallel"},
+        }
     )
 
-    pons_seed_point: SeedPoint = attrs.field(
-        metadata={
-            "help_string": "col, row, slice of seed point for pons",
-            "argstr": "-pons-crs",
-        }
+    pons_seed_point: SeedPoint = field(
+        metadata={"help_string": "seed point for pons", "argstr": "-pons-crs"}
     )
 
-    corpus_callosum_seed_point: SeedPoint = attrs.field(
-        metadata={
-            "help_string": "col, row, slice of seed point for corpus callosum",
-            "argstr": "-cc-crs",
-        }
+    corpus_callosum_seed_point: SeedPoint = field(
+        metadata={"help_string": "seed point for corpus callosum", "argstr": "-cc-crs"}
     )
 
-    left_hemisphere_seed_point: SeedPoint = attrs.field(
-        metadata={
-            "help_string": "col, row, slice of seed point for left hemisphere",
-            "argstr": "-lh-crs",
-        }
+    left_hemisphere_seed_point: SeedPoint = field(
+        metadata={"help_string": "seed point for left hemisphere", "argstr": "-lh-crs"}
     )
 
-    right_hemisphere_seed_point: SeedPoint = attrs.field(
-        metadata={
-            "help_string": "col, row, slice of seed point for right hemisphere",
-            "argstr": "-rh-crs",
-        }
+    right_hemisphere_seed_point: SeedPoint = field(
+        metadata={"help_string": "seed point for right hemisphere", "argstr": "-rh-crs"}
     )
 
-    custom_talairach_atlas_file: os.PathLike = attrs.field(
+    custom_talairach_atlas: PathLike = field(
         metadata={
             "help_string": "use a custom talairach atlas",
             "argstr": "-custom-tal-atlas",
         }
     )
 
-    deface: bool = attrs.field(
-        metadata={
-            "help_string": "deface subject",
-            "argstr": "-deface",
-        }
+    deface: bool = field(
+        metadata={"help_string": "deface subject", "argstr": "-deface"}
     )
 
-    no_subcortical_segmentation: bool = attrs.field(
+    no_subcortical_segmentation: bool = field(
         metadata={
             "help_string": "skip subcortical segmentation steps",
             "argstr": "-nosubcortseg",
         }
     )
 
-    conform_width_to_256: bool = attrs.field(
+    conform_width_to_256: bool = field(
         metadata={
-            "help_string": (
-                "conform image dimensions to 256 when running mri_convert",
-            ),
+            "help_string": "conform image dimensions to 256 when running mri_convert",
             "argstr": "-cw256",
         }
     )
 
-    cache_files_for_qdec: bool = attrs.field(
+    cache_files_for_qdec: bool = field(
         metadata={
-            "help_string": (
-                "accelerate analysis of group data "
-                "by pre-computing files required for the Qdec utility"
-            ),
+            "help_string": "accelerate analysis of group data by pre-computing files required for the Qdec utility",
             "argstr": "-qcache",
         }
     )
 
-    parallel: bool = attrs.field(
+    parallel: bool = field(
         metadata={
             "help_string": "process both hemispheres in parallel",
             "argstr": "-parallel",
             "xor": ["hemisphere"],
-        },
+        }
     )
 
-    threads: int = attrs.field(
-        metadata={
-            "help_string": "set number of threads to use",
-            "argstr": "-threads {threads}",
-        },
+    num_threads: int = field(
+        metadata={"help_string": "set number of threads to use", "argstr": "-threads"}
     )
 
-    subjects_dir: os.PathLike = attrs.field(
+    subjects_dir: PathLike = field(
         metadata={
             "help_string": "subjects directory processed by FreeSurfer",
-            "argstr": "-sd {subjects_dir}",
-        },
+            "argstr": "-sd",
+        }
     )
+
+
+class ReconAllBaseOutSpec(SubjectsDirOutSpec):
+    """Base output specifications for recon-all."""
```

### Comparing `pydra_freesurfer-0.0.9/.gitignore` & `pydra_freesurfer-0.1.1/.gitignore`

 * *Files 20% similar despite different names*

```diff
@@ -78,40 +78,16 @@
 # Jupyter Notebook
 .ipynb_checkpoints
 
 # IPython
 profile_default/
 ipython_config.py
 
-# pyenv
-#   For a library or package, you might want to ignore these files since the code is
-#   intended to run in multiple environments; otherwise, check them in:
-# .python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# poetry
-#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
-#   This is especially recommended for binary packages to ensure reproducibility, and is more
-#   commonly ignored for libraries.
-#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
-#poetry.lock
-
-# pdm
-#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
-#pdm.lock
-#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
-#   in version control.
-#   https://pdm.fming.dev/#use-with-ide
-.pdm.toml
+# Hatch
+.hatch/
 
 # PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
 __pypackages__/
 
 # Celery stuff
 celerybeat-schedule
 celerybeat.pid
@@ -142,26 +118,43 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
+# Pycharm
+.idea
+
+# Vim
+.*.sw[op]
+
+# VS Code
+.vscode
+
+# Mac garbarge
+.DS_store
+
 # pytype static type analyzer
 .pytype/
 
 # Cython debug symbols
 cython_debug/
 
 # Makefile stamp files
 *.stamp
 
 # JetBrains
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
+
 .fleet/
-.idea/
 
 # macOS
 .DS_Store
+
+# Generated files
+/pydra/tasks/freesurfer/_version.py
+/related-packages/fileformats/fileformats/medimage_freesurfer/_version.py
+/related-packages/fileformats-extras/fileformats/extras/medimage_freesurfer/_version.py
```

### Comparing `pydra_freesurfer-0.0.9/LICENSE` & `pydra_freesurfer-0.1.1/LICENSE`

 * *Files identical despite different names*

