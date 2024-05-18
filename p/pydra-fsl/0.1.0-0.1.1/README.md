# Comparing `tmp/pydra_fsl-0.1.0.tar.gz` & `tmp/pydra_fsl-0.1.1.tar.gz`

## Comparing `pydra_fsl-0.1.0.tar` & `pydra_fsl-0.1.1.tar`

### file list

```diff
@@ -1,505 +1,523 @@
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/.coveragerc
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/.editorconfig
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/.flake8
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/.gitattributes
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/codecov.yml
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/report_progress.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/.github/dependabot.yaml
--rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/.github/workflows/ci-cd.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/docs/Makefile
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/docs/make.bat
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/docs/source/api.rst
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/docs/source/conf.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/docs/source/index.rst
--rwxr-xr-x   0        0        0     2504 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/generate
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/requirements.txt
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/accuracy_tester.yaml
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/accuracy_tester_callables.py
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_mask.yaml
--rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_mask_callables.py
--rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_topup.yaml
--rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_topup_callables.py
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_warp.yaml
--rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_warp_callables.py
--rw-r--r--   0        0        0    10616 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_xfm.yaml
--rw-r--r--   0        0        0    10391 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_xfm_callables.py
--rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/ar1_image.yaml
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/ar1_image_callables.py
--rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/av_scale.yaml
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/av_scale_callables.py
--rw-r--r--   0        0        0     8472 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/b0_calc.yaml
--rw-r--r--   0        0        0     9973 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/b0_calc_callables.py
--rw-r--r--   0        0        0    11124 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/bedpostx5.yaml
--rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/bedpostx5_callables.py
--rw-r--r--   0        0        0     9719 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/bet.yaml
--rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/bet_callables.py
--rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/binary_maths.yaml
--rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/binary_maths_callables.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/change_data_type.yaml
--rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/change_data_type_callables.py
--rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/classifier.yaml
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/classifier_callables.py
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/cleaner.yaml
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/cleaner_callables.py
--rw-r--r--   0        0        0     9715 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/cluster.yaml
--rw-r--r--   0        0        0    10818 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/cluster_callables.py
--rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/complex.yaml
--rw-r--r--   0        0        0    13119 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/complex_callables.py
--rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/contrast_mgr.yaml
--rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/contrast_mgr_callables.py
--rw-r--r--   0        0        0    12669 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/convert_warp.yaml
--rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/convert_warp_callables.py
--rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/convert_xfm.yaml
--rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/convert_xfm_callables.py
--rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/copy_geom.yaml
--rw-r--r--   0        0        0     9975 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/copy_geom_callables.py
--rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/dilate_image.yaml
--rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/dilate_image_callables.py
--rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/distance_map.yaml
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/distance_map_callables.py
--rw-r--r--   0        0        0     8990 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/dti_fit.yaml
--rw-r--r--   0        0        0    11404 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/dti_fit_callables.py
--rw-r--r--   0        0        0     9704 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/dual_regression.yaml
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/dual_regression_callables.py
--rw-r--r--   0        0        0    22074 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/eddy.yaml
--rw-r--r--   0        0        0     7201 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/eddy_callables.py
--rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/eddy_correct.yaml
--rw-r--r--   0        0        0     9990 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/eddy_correct_callables.py
--rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/eddy_quad.yaml
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/eddy_quad_callables.py
--rw-r--r--   0        0        0     8763 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/epi_de_warp.yaml
--rw-r--r--   0        0        0    11970 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/epi_de_warp_callables.py
--rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/epi_reg.yaml
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/epi_reg_callables.py
--rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/erode_image.yaml
--rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/erode_image_callables.py
--rw-r--r--   0        0        0     7287 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/extract_roi.yaml
--rw-r--r--   0        0        0     9601 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/extract_roi_callables.py
--rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/fast.yaml
--rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/fast_callables.py
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/feat.yaml
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/feat_callables.py
--rw-r--r--   0        0        0     4295 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/feat_model.yaml
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/feat_model_callables.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/feature_extractor.yaml
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/feature_extractor_callables.py
--rw-r--r--   0        0        0     7938 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/filmgls.yaml
--rw-r--r--   0        0        0    16816 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/filmgls_callables.py
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/filter_regressor.yaml
--rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/filter_regressor_callables.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/find_the_biggest.yaml
--rw-r--r--   0        0        0     9186 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/find_the_biggest_callables.py
--rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/first.yaml
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/first_callables.py
--rw-r--r--   0        0        0    11007 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/flameo.yaml
--rw-r--r--   0        0        0     5492 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/flameo_callables.py
--rw-r--r--   0        0        0    13543 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/flirt.yaml
--rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/flirt_callables.py
--rw-r--r--   0        0        0    14632 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/fnirt.yaml
--rw-r--r--   0        0        0    12257 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/fnirt_callables.py
--rw-r--r--   0        0        0    19493 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/fugue.yaml
--rw-r--r--   0        0        0    10616 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/fugue_callables.py
--rw-r--r--   0        0        0    12021 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/glm.yaml
--rw-r--r--   0        0        0    13720 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/glm_callables.py
--rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/ica__aroma.yaml
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/ica__aroma_callables.py
--rw-r--r--   0        0        0     7122 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/image_maths.yaml
--rw-r--r--   0        0        0     9279 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/image_maths_callables.py
--rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/image_meants.yaml
--rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/image_meants_callables.py
--rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/image_stats.yaml
--rw-r--r--   0        0        0     9977 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/image_stats_callables.py
--rw-r--r--   0        0        0    10143 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/inv_warp.yaml
--rw-r--r--   0        0        0     9982 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/inv_warp_callables.py
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/isotropic_smooth.yaml
--rw-r--r--   0        0        0     9165 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/isotropic_smooth_callables.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/l2_model.yaml
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/l2_model_callables.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/level_1_design.yaml
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/level_1_design_callables.py
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/make_dyadic_vectors.yaml
--rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/make_dyadic_vectors_callables.py
--rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/maths_command.yaml
--rw-r--r--   0        0        0     9162 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/maths_command_callables.py
--rw-r--r--   0        0        0     6764 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/max_image.yaml
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/max_image_callables.py
--rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/maxn_image.yaml
--rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/maxn_image_callables.py
--rw-r--r--   0        0        0     9212 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/mcflirt.yaml
--rw-r--r--   0        0        0    14141 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/mcflirt_callables.py
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/mean_image.yaml
--rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/mean_image_callables.py
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/median_image.yaml
--rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/median_image_callables.py
--rw-r--r--   0        0        0    14386 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/melodic.yaml
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/melodic_callables.py
--rw-r--r--   0        0        0     7556 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/merge.yaml
--rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/merge_callables.py
--rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/min_image.yaml
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/min_image_callables.py
--rw-r--r--   0        0        0     7841 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/motion_outliers.yaml
--rw-r--r--   0        0        0    10417 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/motion_outliers_callables.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/multi_image_maths.yaml
--rw-r--r--   0        0        0     9165 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/multi_image_maths_callables.py
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/multiple_regress_design.yaml
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/multiple_regress_design_callables.py
--rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/overlay.yaml
--rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/overlay_callables.py
--rw-r--r--   0        0        0     6939 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/percentile_image.yaml
--rw-r--r--   0        0        0     9165 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/percentile_image_callables.py
--rw-r--r--   0        0        0     5211 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/plot_motion_params.yaml
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/plot_motion_params_callables.py
--rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/plot_time_series.yaml
--rw-r--r--   0        0        0     9252 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/plot_time_series_callables.py
--rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/power_spectrum.yaml
--rw-r--r--   0        0        0     9443 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/power_spectrum_callables.py
--rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/prelude.yaml
--rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/prelude_callables.py
--rw-r--r--   0        0        0     7813 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/prepare_fieldmap.yaml
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/prepare_fieldmap_callables.py
--rw-r--r--   0        0        0    15857 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/prob_track_x.yaml
--rw-r--r--   0        0        0    16132 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/prob_track_x2.yaml
--rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/prob_track_x2_callables.py
--rw-r--r--   0        0        0    12168 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/prob_track_x_callables.py
--rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/proj_thresh.yaml
--rw-r--r--   0        0        0     9000 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/proj_thresh_callables.py
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/randomise.yaml
--rw-r--r--   0        0        0    11553 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/randomise_callables.py
--rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/reorient_2_std.yaml
--rw-r--r--   0        0        0     9196 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/reorient_2_std_callables.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/robust_fov.yaml
--rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/robust_fov_callables.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/sig_loss.yaml
--rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/sig_loss_callables.py
--rw-r--r--   0        0        0     5915 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/slice.yaml
--rw-r--r--   0        0        0     7880 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/slice_callables.py
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/slice_timer.yaml
--rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/slice_timer_callables.py
--rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/slicer.yaml
--rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/slicer_callables.py
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/smm.yaml
--rw-r--r--   0        0        0     9795 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/smm_callables.py
--rw-r--r--   0        0        0    11555 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/smooth.yaml
--rw-r--r--   0        0        0     9983 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/smooth_callables.py
--rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/smooth_estimate.yaml
--rw-r--r--   0        0        0    10367 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/smooth_estimate_callables.py
--rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/spatial_filter.yaml
--rw-r--r--   0        0        0     9163 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/spatial_filter_callables.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/split.yaml
--rw-r--r--   0        0        0     5276 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/split_callables.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/std_image.yaml
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/std_image_callables.py
--rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/susan.yaml
--rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/susan_callables.py
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/swap_dimensions.yaml
--rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/swap_dimensions_callables.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/temporal_filter.yaml
--rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/temporal_filter_callables.py
--rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/text_2_vest.yaml
--rw-r--r--   0        0        0     9976 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/text_2_vest_callables.py
--rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/threshold.yaml
--rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/threshold_callables.py
--rw-r--r--   0        0        0    12627 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/topup.yaml
--rw-r--r--   0        0        0    16840 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/topup_callables.py
--rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/tract_skeleton.yaml
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/tract_skeleton_callables.py
--rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/training.yaml
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/training_callables.py
--rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/training_set_creator.yaml
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/training_set_creator_callables.py
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/unary_maths.yaml
--rw-r--r--   0        0        0     9506 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/unary_maths_callables.py
--rw-r--r--   0        0        0     9481 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/vec_reg.yaml
--rw-r--r--   0        0        0     9298 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/vec_reg_callables.py
--rw-r--r--   0        0        0     6409 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/vest_2_text.yaml
--rw-r--r--   0        0        0     9976 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/vest_2_text_callables.py
--rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_points.yaml
--rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_points_callables.py
--rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_points_from_std.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_points_from_std_callables.py
--rw-r--r--   0        0        0     8617 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_points_to_std.yaml
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_points_to_std_callables.py
--rw-r--r--   0        0        0    13194 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_utils.yaml
--rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_utils_callables.py
--rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/x_fibres_5.yaml
--rw-r--r--   0        0        0    12428 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/nipype-auto-conv/specs/x_fibres_5_callables.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/_version.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/latest.py
--rw-r--r--   0        0        0     5666 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/__init__.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/_version.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/accuracy_tester.py
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/apply_mask.py
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/apply_topup.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/apply_warp.py
--rw-r--r--   0        0        0     8880 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/apply_xfm.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/ar1_image.py
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/av_scale.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/b0_calc.py
--rw-r--r--   0        0        0     7416 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/bedpostx5.py
--rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/bet.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/binary_maths.py
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/change_data_type.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/classifier.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/cleaner.py
--rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/cluster.py
--rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/complex.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/contrast_mgr.py
--rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/convert_warp.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/convert_xfm.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/copy_geom.py
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/dilate_image.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/distance_map.py
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/dti_fit.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/dual_regression.py
--rw-r--r--   0        0        0    16415 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/eddy.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/eddy_correct.py
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/eddy_quad.py
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/epi_de_warp.py
--rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/epi_reg.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/erode_image.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/extract_roi.py
--rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/fast.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/feat.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/feat_model.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/feature_extractor.py
--rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/filmgls.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/filter_regressor.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/find_the_biggest.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/first.py
--rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/flameo.py
--rw-r--r--   0        0        0     9715 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/flirt.py
--rw-r--r--   0        0        0    11246 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/fnirt.py
--rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/fugue.py
--rw-r--r--   0        0        0     6778 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/glm.py
--rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/ica__aroma.py
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/image_maths.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/image_meants.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/image_stats.py
--rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/inv_warp.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/isotropic_smooth.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/l2_model.py
--rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/level_1_design.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/make_dyadic_vectors.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/maths_command.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/max_image.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/maxn_image.py
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/mcflirt.py
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/mean_image.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/median_image.py
--rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/melodic.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/merge.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/min_image.py
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/motion_outliers.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/multi_image_maths.py
--rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/multiple_regress_design.py
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/overlay.py
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/percentile_image.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/plot_motion_params.py
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/plot_time_series.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/power_spectrum.py
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/prelude.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/prepare_fieldmap.py
--rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/prob_track_x.py
--rw-r--r--   0        0        0    14397 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/prob_track_x2.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/proj_thresh.py
--rw-r--r--   0        0        0     6789 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/randomise.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/reorient_2_std.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/robust_fov.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/sig_loss.py
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/slice.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/slice_timer.py
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/slicer.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/smm.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/smooth.py
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/smooth_estimate.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/spatial_filter.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/split.py
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/std_image.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/susan.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/swap_dimensions.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/temporal_filter.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/text_2_vest.py
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/threshold.py
--rw-r--r--   0        0        0     7952 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/topup.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tract_skeleton.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/training.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/training_set_creator.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/unary_maths.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/vec_reg.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/vest_2_text.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/warp_points.py
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/warp_points_from_std.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/warp_points_to_std.py
--rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/warp_utils.py
--rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/x_fibres_5.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/conftest.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_accuracytester.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_applymask.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_applytopup.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_applywarp.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_applyxfm.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_ar1image.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_avscale.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_b0calc.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_bedpostx5.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_bet.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_binarymaths.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_changedatatype.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_classifier.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_cleaner.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_cluster.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_complex.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_contrastmgr.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_convertwarp.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_convertxfm.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_copygeom.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_dilateimage.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_distancemap.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_dtifit.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_dualregression.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_eddy.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_eddycorrect.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_eddyquad.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_epidewarp.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_epireg.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_erodeimage.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_extractroi.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_fast.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_feat.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_featmodel.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_featureextractor.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_filmgls.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_filterregressor.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_findthebiggest.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_first.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_flameo.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_flirt.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_fnirt.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_fugue.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_glm.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_ica_aroma.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_imagemaths.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_imagemeants.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_imagestats.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_invwarp.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_isotropicsmooth.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_l2model.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_level1design.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_makedyadicvectors.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_mathscommand.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_maximage.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_maxnimage.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_mcflirt.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_meanimage.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_medianimage.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_melodic.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_merge.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_minimage.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_motionoutliers.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_multiimagemaths.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_multipleregressdesign.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_overlay.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_percentileimage.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_plotmotionparams.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_plottimeseries.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_powerspectrum.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_prelude.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_preparefieldmap.py
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_probtrackx.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_probtrackx2.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_projthresh.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_randomise.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_reorient2std.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_robustfov.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_sigloss.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_slice.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_slicer.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_slicetimer.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_smm.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_smooth.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_smoothestimate.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_spatialfilter.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_split.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_stdimage.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_susan.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_swapdimensions.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_temporalfilter.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_text2vest.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_threshold.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_topup.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_tractskeleton.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_training.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_trainingsetcreator.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_unarymaths.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_vecreg.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_vest2text.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_warppoints.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_warppointsfromstd.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_warppointstostd.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_warputils.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_xfibres5.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/__init__.py
--rw-r--r--   0        0        0     5677 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fast.py
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/maths.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/susan.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/bet/__init__.py
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/bet/bet.py
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/bet/robustfov.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/eddy/__init__.py
--rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/eddy/applytopup.py
--rw-r--r--   0        0        0    12618 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/eddy/eddy.py
--rw-r--r--   0        0        0     7250 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/eddy/topup.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/__init__.py
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/convertxfm.py
--rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/flirt.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/img2imgcoord.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/img2stdcoord.py
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/specs.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/std2imgcoord.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/__init__.py
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/applywarp.py
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/convertwarp.py
--rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/fnirt.py
--rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/fnirtfileutils.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/invwarp.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/specs.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fugue/__init__.py
--rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fugue/fugue.py
--rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fugue/prelude.py
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fugue/prepare_fieldmap.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fugue/sigloss.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/__init__.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/chfiletype.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/fft.py
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/info.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/interleave.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/merge.py
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/orient.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/reorient2std.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/roi.py
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/selectvols.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/smoothfill.py
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/split.py
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/swapdim.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/related-packages/conftest.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/related-packages/fileformats/LICENSE
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/related-packages/fileformats/README.rst
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/related-packages/fileformats/pyproject.toml
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/related-packages/fileformats/fileformats/medimage_fsl/__init__.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/related-packages/fileformats-extras/LICENSE
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/related-packages/fileformats-extras/README.rst
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/related-packages/fileformats-extras/pyproject.toml
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/related-packages/fileformats-extras/fileformats/extras/medimage_fsl/__init__.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/related-packages/fileformats-extras/fileformats/extras/medimage_fsl/tests/test_generate_sample_data.py
--rwxr-xr-x   0        0        0     2272 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/tools/increment_tool_version.py
--rwxr-xr-x   0        0        0     1368 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/tools/rename_template.py
--rwxr-xr-x   0        0        0      802 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/tools/report_progress.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/tools/requirements.txt
--rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/LICENSE
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/NOTICE
--rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/README.md
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    23882 2020-02-02 00:00:00.000000 pydra_fsl-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/.coveragerc
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/.editorconfig
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/.flake8
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/.gitattributes
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/codecov.yml
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/report_progress.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/.github/dependabot.yaml
+-rw-r--r--   0        0        0    16182 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/.github/workflows/ci-cd.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/docs/source/api.rst
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/docs/source/conf.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/docs/source/index.rst
+-rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/generate
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/requirements.txt
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/package.yaml
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/accuracy_tester.yaml
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/accuracy_tester_callables.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/apply_mask.yaml
+-rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/apply_mask_callables.py
+-rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/apply_topup.yaml
+-rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/apply_topup_callables.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/apply_warp.yaml
+-rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/apply_warp_callables.py
+-rw-r--r--   0        0        0    10616 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/apply_xfm.yaml
+-rw-r--r--   0        0        0    10391 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/apply_xfm_callables.py
+-rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/ar1_image.yaml
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/ar1_image_callables.py
+-rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/av_scale.yaml
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/av_scale_callables.py
+-rw-r--r--   0        0        0     8472 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/b0_calc.yaml
+-rw-r--r--   0        0        0     9973 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/b0_calc_callables.py
+-rw-r--r--   0        0        0    11124 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/bedpostx5.yaml
+-rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/bedpostx5_callables.py
+-rw-r--r--   0        0        0     9719 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/bet.yaml
+-rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/bet_callables.py
+-rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/binary_maths.yaml
+-rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/binary_maths_callables.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/change_data_type.yaml
+-rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/change_data_type_callables.py
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/classifier.yaml
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/classifier_callables.py
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/cleaner.yaml
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/cleaner_callables.py
+-rw-r--r--   0        0        0     9715 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/cluster.yaml
+-rw-r--r--   0        0        0    10818 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/cluster_callables.py
+-rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/complex.yaml
+-rw-r--r--   0        0        0    13119 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/complex_callables.py
+-rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/contrast_mgr.yaml
+-rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/contrast_mgr_callables.py
+-rw-r--r--   0        0        0    12669 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/convert_warp.yaml
+-rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/convert_warp_callables.py
+-rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/convert_xfm.yaml
+-rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/convert_xfm_callables.py
+-rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/copy_geom.yaml
+-rw-r--r--   0        0        0     9975 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/copy_geom_callables.py
+-rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/dilate_image.yaml
+-rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/dilate_image_callables.py
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/distance_map.yaml
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/distance_map_callables.py
+-rw-r--r--   0        0        0     8990 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/dti_fit.yaml
+-rw-r--r--   0        0        0    11404 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/dti_fit_callables.py
+-rw-r--r--   0        0        0     9704 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/dual_regression.yaml
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/dual_regression_callables.py
+-rw-r--r--   0        0        0    22074 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/eddy.yaml
+-rw-r--r--   0        0        0     7201 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/eddy_callables.py
+-rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/eddy_correct.yaml
+-rw-r--r--   0        0        0     9990 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/eddy_correct_callables.py
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/eddy_quad.yaml
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/eddy_quad_callables.py
+-rw-r--r--   0        0        0     8763 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/epi_de_warp.yaml
+-rw-r--r--   0        0        0    11970 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/epi_de_warp_callables.py
+-rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/epi_reg.yaml
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/epi_reg_callables.py
+-rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/erode_image.yaml
+-rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/erode_image_callables.py
+-rw-r--r--   0        0        0     7287 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/extract_roi.yaml
+-rw-r--r--   0        0        0     9601 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/extract_roi_callables.py
+-rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/fast.yaml
+-rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/fast_callables.py
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/feat.yaml
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/feat_callables.py
+-rw-r--r--   0        0        0     4295 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/feat_model.yaml
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/feat_model_callables.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/feature_extractor.yaml
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/feature_extractor_callables.py
+-rw-r--r--   0        0        0     7938 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/filmgls.yaml
+-rw-r--r--   0        0        0    16816 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/filmgls_callables.py
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/filter_regressor.yaml
+-rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/filter_regressor_callables.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/find_the_biggest.yaml
+-rw-r--r--   0        0        0     9186 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/find_the_biggest_callables.py
+-rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/first.yaml
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/first_callables.py
+-rw-r--r--   0        0        0    11007 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/flameo.yaml
+-rw-r--r--   0        0        0     5492 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/flameo_callables.py
+-rw-r--r--   0        0        0    13543 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/flirt.yaml
+-rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/flirt_callables.py
+-rw-r--r--   0        0        0    14632 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/fnirt.yaml
+-rw-r--r--   0        0        0    12257 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/fnirt_callables.py
+-rw-r--r--   0        0        0    19493 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/fugue.yaml
+-rw-r--r--   0        0        0    10616 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/fugue_callables.py
+-rw-r--r--   0        0        0    12021 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/glm.yaml
+-rw-r--r--   0        0        0    13720 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/glm_callables.py
+-rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/ica__aroma.yaml
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/ica__aroma_callables.py
+-rw-r--r--   0        0        0     7122 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/image_maths.yaml
+-rw-r--r--   0        0        0     9279 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/image_maths_callables.py
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/image_meants.yaml
+-rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/image_meants_callables.py
+-rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/image_stats.yaml
+-rw-r--r--   0        0        0     9977 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/image_stats_callables.py
+-rw-r--r--   0        0        0    10143 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/inv_warp.yaml
+-rw-r--r--   0        0        0     9982 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/inv_warp_callables.py
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/isotropic_smooth.yaml
+-rw-r--r--   0        0        0     9165 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/isotropic_smooth_callables.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/l2_model.yaml
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/l2_model_callables.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/level_1_design.yaml
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/level_1_design_callables.py
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/make_dyadic_vectors.yaml
+-rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/make_dyadic_vectors_callables.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/maths_command.yaml
+-rw-r--r--   0        0        0     9162 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/maths_command_callables.py
+-rw-r--r--   0        0        0     6764 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/max_image.yaml
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/max_image_callables.py
+-rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/maxn_image.yaml
+-rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/maxn_image_callables.py
+-rw-r--r--   0        0        0     9212 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/mcflirt.yaml
+-rw-r--r--   0        0        0    14141 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/mcflirt_callables.py
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/mean_image.yaml
+-rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/mean_image_callables.py
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/median_image.yaml
+-rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/median_image_callables.py
+-rw-r--r--   0        0        0    14386 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/melodic.yaml
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/melodic_callables.py
+-rw-r--r--   0        0        0     7556 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/merge.yaml
+-rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/merge_callables.py
+-rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/min_image.yaml
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/min_image_callables.py
+-rw-r--r--   0        0        0     7841 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/motion_outliers.yaml
+-rw-r--r--   0        0        0    10417 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/motion_outliers_callables.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/multi_image_maths.yaml
+-rw-r--r--   0        0        0     9165 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/multi_image_maths_callables.py
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/multiple_regress_design.yaml
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/multiple_regress_design_callables.py
+-rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/overlay.yaml
+-rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/overlay_callables.py
+-rw-r--r--   0        0        0     6939 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/percentile_image.yaml
+-rw-r--r--   0        0        0     9165 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/percentile_image_callables.py
+-rw-r--r--   0        0        0     5211 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/plot_motion_params.yaml
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/plot_motion_params_callables.py
+-rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/plot_time_series.yaml
+-rw-r--r--   0        0        0     9252 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/plot_time_series_callables.py
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/power_spectrum.yaml
+-rw-r--r--   0        0        0     9443 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/power_spectrum_callables.py
+-rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/prelude.yaml
+-rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/prelude_callables.py
+-rw-r--r--   0        0        0     7813 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/prepare_fieldmap.yaml
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/prepare_fieldmap_callables.py
+-rw-r--r--   0        0        0    15857 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/prob_track_x.yaml
+-rw-r--r--   0        0        0    16132 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/prob_track_x2.yaml
+-rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/prob_track_x2_callables.py
+-rw-r--r--   0        0        0    12168 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/prob_track_x_callables.py
+-rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/proj_thresh.yaml
+-rw-r--r--   0        0        0     9000 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/proj_thresh_callables.py
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/randomise.yaml
+-rw-r--r--   0        0        0    11553 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/randomise_callables.py
+-rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/reorient_2_std.yaml
+-rw-r--r--   0        0        0     9196 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/reorient_2_std_callables.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/robust_fov.yaml
+-rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/robust_fov_callables.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/sig_loss.yaml
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/sig_loss_callables.py
+-rw-r--r--   0        0        0     5915 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/slice.yaml
+-rw-r--r--   0        0        0     7880 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/slice_callables.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/slice_timer.yaml
+-rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/slice_timer_callables.py
+-rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/slicer.yaml
+-rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/slicer_callables.py
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/smm.yaml
+-rw-r--r--   0        0        0     9795 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/smm_callables.py
+-rw-r--r--   0        0        0    11555 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/smooth.yaml
+-rw-r--r--   0        0        0     9983 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/smooth_callables.py
+-rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/smooth_estimate.yaml
+-rw-r--r--   0        0        0    10367 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/smooth_estimate_callables.py
+-rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/spatial_filter.yaml
+-rw-r--r--   0        0        0     9163 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/spatial_filter_callables.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/split.yaml
+-rw-r--r--   0        0        0     5276 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/split_callables.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/std_image.yaml
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/std_image_callables.py
+-rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/susan.yaml
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/susan_callables.py
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/swap_dimensions.yaml
+-rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/swap_dimensions_callables.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/temporal_filter.yaml
+-rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/temporal_filter_callables.py
+-rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/text_2_vest.yaml
+-rw-r--r--   0        0        0     9976 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/text_2_vest_callables.py
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/threshold.yaml
+-rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/threshold_callables.py
+-rw-r--r--   0        0        0    12627 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/topup.yaml
+-rw-r--r--   0        0        0    16840 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/topup_callables.py
+-rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/tract_skeleton.yaml
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/tract_skeleton_callables.py
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/training.yaml
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/training_callables.py
+-rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/training_set_creator.yaml
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/training_set_creator_callables.py
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/unary_maths.yaml
+-rw-r--r--   0        0        0     9506 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/unary_maths_callables.py
+-rw-r--r--   0        0        0     9481 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/vec_reg.yaml
+-rw-r--r--   0        0        0     9298 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/vec_reg_callables.py
+-rw-r--r--   0        0        0     6409 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/vest_2_text.yaml
+-rw-r--r--   0        0        0     9976 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/vest_2_text_callables.py
+-rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/warp_points.yaml
+-rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/warp_points_callables.py
+-rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/warp_points_from_std.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/warp_points_from_std_callables.py
+-rw-r--r--   0        0        0     8617 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/warp_points_to_std.yaml
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/warp_points_to_std_callables.py
+-rw-r--r--   0        0        0    13194 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/warp_utils.yaml
+-rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/warp_utils_callables.py
+-rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/x_fibres_5.yaml
+-rw-r--r--   0        0        0    12428 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/x_fibres_5_callables.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/_version.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/latest.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/__init__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/_post_release.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/aroma/__init__.py
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/aroma/ica__aroma.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/aroma/tests/conftest.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/aroma/tests/test_ica_aroma.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/__init__.py
+-rw-r--r--   0        0        0     7155 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/bedpostx5.py
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/distance_map.py
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/dti_fit.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/find_the_biggest.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/make_dyadic_vectors.py
+-rw-r--r--   0        0        0    11008 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/prob_track_x.py
+-rw-r--r--   0        0        0    14410 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/prob_track_x2.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/proj_thresh.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tract_skeleton.py
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/vec_reg.py
+-rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/x_fibres_5.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tests/conftest.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tests/test_bedpostx5.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tests/test_distancemap.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tests/test_dtifit.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tests/test_findthebiggest.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tests/test_makedyadicvectors.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tests/test_probtrackx.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tests/test_probtrackx2.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tests/test_projthresh.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tests/test_tractskeleton.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tests/test_vecreg.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tests/test_xfibres5.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/__init__.py
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/apply_topup.py
+-rw-r--r--   0        0        0    16244 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/eddy.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/eddy_correct.py
+-rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/eddy_quad.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/epi_de_warp.py
+-rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/epi_reg.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/prepare_fieldmap.py
+-rw-r--r--   0        0        0     7965 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/topup.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/tests/conftest.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/tests/test_applytopup.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/tests/test_eddy.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/tests/test_eddycorrect.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/tests/test_eddyquad.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/tests/test_epidewarp.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/tests/test_epireg.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/tests/test_preparefieldmap.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/tests/test_topup.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/__init__.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/accuracy_tester.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/classifier.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/cleaner.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/feature_extractor.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/training.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/training_set_creator.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/tests/conftest.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/tests/test_accuracytester.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/tests/test_classifier.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/tests/test_cleaner.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/tests/test_featureextractor.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/tests/test_training.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/tests/test_trainingsetcreator.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/__init__.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/apply_mask.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/ar1_image.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/binary_maths.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/change_data_type.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/dilate_image.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/erode_image.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/isotropic_smooth.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/maths_command.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/max_image.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/maxn_image.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/mean_image.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/median_image.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/min_image.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/multi_image_maths.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/percentile_image.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/spatial_filter.py
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/std_image.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/temporal_filter.py
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/threshold.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/unary_maths.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/conftest.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_applymask.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_ar1image.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_binarymaths.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_changedatatype.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_dilateimage.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_erodeimage.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_isotropicsmooth.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_mathscommand.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_maximage.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_maxnimage.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_meanimage.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_medianimage.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_minimage.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_multiimagemaths.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_percentileimage.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_spatialfilter.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_stdimage.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_temporalfilter.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_threshold.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_unarymaths.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/__init__.py
+-rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/cluster.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/contrast_mgr.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/dual_regression.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/feat.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/feat_model.py
+-rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/filmgls.py
+-rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/flameo.py
+-rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/glm.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/l2_model.py
+-rw-r--r--   0        0        0    12167 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/level_1_design.py
+-rw-r--r--   0        0        0     9958 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/melodic.py
+-rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/multiple_regress_design.py
+-rw-r--r--   0        0        0     6794 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/randomise.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/smm.py
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/smooth_estimate.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/conftest.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_cluster.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_contrastmgr.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_dualregression.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_feat.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_featmodel.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_filmgls.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_flameo.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_glm.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_l2model.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_level1design.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_melodic.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_multipleregressdesign.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_randomise.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_smm.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_smoothestimate.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/possum/__init__.py
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/possum/b0_calc.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/possum/tests/conftest.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/possum/tests/test_b0calc.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/__init__.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/apply_warp.py
+-rw-r--r--   0        0        0     8912 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/apply_xfm.py
+-rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/bet.py
+-rw-r--r--   0        0        0     5580 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/fast.py
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/first.py
+-rw-r--r--   0        0        0     9735 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/flirt.py
+-rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/fnirt.py
+-rw-r--r--   0        0        0     8778 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/fugue.py
+-rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/mcflirt.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/prelude.py
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/slice_timer.py
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/susan.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/conftest.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/test_applywarp.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/test_applyxfm.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/test_bet.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/test_fast.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/test_first.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/test_flirt.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/test_fnirt.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/test_fugue.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/test_mcflirt.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/test_prelude.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/test_slicetimer.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/test_susan.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/__init__.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/av_scale.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/complex.py
+-rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/convert_warp.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/convert_xfm.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/copy_geom.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/extract_roi.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/filter_regressor.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/image_maths.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/image_meants.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/image_stats.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/inv_warp.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/merge.py
+-rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/motion_outliers.py
+-rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/overlay.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/plot_motion_params.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/plot_time_series.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/power_spectrum.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/reorient_2_std.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/robust_fov.py
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/sig_loss.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/slice.py
+-rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/slicer.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/smooth.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/split.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/swap_dimensions.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/text_2_vest.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/vest_2_text.py
+-rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/warp_points.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/warp_points_from_std.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/warp_points_to_std.py
+-rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/warp_utils.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/conftest.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_avscale.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_complex.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_convertwarp.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_convertxfm.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_copygeom.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_extractroi.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_filterregressor.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_imagemaths.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_imagemeants.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_imagestats.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_invwarp.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_merge.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_motionoutliers.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_overlay.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_plotmotionparams.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_plottimeseries.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_powerspectrum.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_reorient2std.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_robustfov.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_sigloss.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_slice.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_slicer.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_smooth.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_split.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_swapdimensions.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_text2vest.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_vest2text.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_warppoints.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_warppointsfromstd.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_warppointstostd.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_warputils.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/__init__.py
+-rw-r--r--   0        0        0     5677 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fast.py
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/maths.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/susan.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/bet/__init__.py
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/bet/bet.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/bet/robustfov.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/eddy/__init__.py
+-rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/eddy/applytopup.py
+-rw-r--r--   0        0        0    12618 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/eddy/eddy.py
+-rw-r--r--   0        0        0     7250 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/eddy/topup.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/flirt/__init__.py
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/flirt/convertxfm.py
+-rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/flirt/flirt.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/flirt/img2imgcoord.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/flirt/img2stdcoord.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/flirt/specs.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/flirt/std2imgcoord.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fnirt/__init__.py
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fnirt/applywarp.py
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fnirt/convertwarp.py
+-rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fnirt/fnirt.py
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fnirt/fnirtfileutils.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fnirt/invwarp.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fnirt/specs.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fugue/__init__.py
+-rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fugue/fugue.py
+-rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fugue/prelude.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fugue/prepare_fieldmap.py
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fugue/sigloss.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/__init__.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/chfiletype.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/fft.py
+-rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/info.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/interleave.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/merge.py
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/orient.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/reorient2std.py
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/roi.py
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/selectvols.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/smoothfill.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/split.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/swapdim.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/related-packages/conftest.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/related-packages/fileformats/LICENSE
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/related-packages/fileformats/README.rst
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/related-packages/fileformats/pyproject.toml
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/related-packages/fileformats/fileformats/medimage_fsl/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/related-packages/fileformats-extras/LICENSE
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/related-packages/fileformats-extras/README.rst
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/related-packages/fileformats-extras/pyproject.toml
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/related-packages/fileformats-extras/fileformats/extras/medimage_fsl/__init__.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/related-packages/fileformats-extras/fileformats/extras/medimage_fsl/tests/test_generate_sample_data.py
+-rwxr-xr-x   0        0        0     2272 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/tools/increment_tool_version.py
+-rwxr-xr-x   0        0        0     1368 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/tools/rename_template.py
+-rwxr-xr-x   0        0        0      802 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/tools/report_progress.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/tools/requirements.txt
+-rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/LICENSE
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/NOTICE
+-rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/README.md
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    23882 2020-02-02 00:00:00.000000 pydra_fsl-0.1.1/PKG-INFO
```

### Comparing `pydra_fsl-0.1.0/report_progress.py` & `pydra_fsl-0.1.1/report_progress.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/.github/workflows/ci-cd.yaml` & `pydra_fsl-0.1.1/.github/workflows/ci-cd.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # For deployment, it will be necessary to create a PyPI API token and store it as a secret
 # https://docs.github.com/en/actions/reference/encrypted-secrets
 
 name: CI/CD
 
 on:
   push:
-    branches: [ master, develop ]
+    branches: [ main, develop ]
   pull_request:
-    branches: [ master, develop ]
+    branches: [ main, develop ]
   release:
     types: [published]
   repository_dispatch:
     types: [create-post-release]
 
 env:
   FSL_VERSION: 6.0.7.9
@@ -332,15 +332,15 @@
     - name: Install task package to calculate post-release tag
       run: |
         pip install "./related-packages/fileformats" "./related-packages/fileformats-extras" ".[test]"
 
     - name: Generate post-release tag based on Nipype and Nipype2Pydra versions
       id: post_release_tag
       run: |
-        POST=$(python -c "from pydra.tasks.fsl.auto._version import *; print(post_release)")
+        POST=$(python -c "from pydra.tasks.fsl.auto._post_release import *; print(post_release)")
         echo "TAG=${{ steps.latest_tag.outputs.TAG }}post${POST}" >> $GITHUB_OUTPUT
 
     - name: Add auto directory to git repo
       if: github.event_name == 'release' || github.event_name == 'repository_dispatch'
       run: |
         git add pydra/tasks/fsl/auto
         git commit -am"added auto-generated version to make new tag for package version"
```

### Comparing `pydra_fsl-0.1.0/docs/Makefile` & `pydra_fsl-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/docs/make.bat` & `pydra_fsl-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/docs/source/conf.py` & `pydra_fsl-0.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/docs/source/index.rst` & `pydra_fsl-0.1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/accuracy_tester.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/accuracy_tester.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/accuracy_tester_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/accuracy_tester_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_mask.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/apply_mask.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_mask_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/apply_mask_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_topup.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/apply_topup.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_topup_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/apply_topup_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_warp.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/apply_warp.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_warp_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/apply_warp_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_xfm.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/apply_xfm.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/apply_xfm_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/apply_xfm_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/ar1_image.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/ar1_image.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/ar1_image_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/ar1_image_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/av_scale.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/av_scale.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/av_scale_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/av_scale_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/b0_calc.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/b0_calc.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/b0_calc_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/b0_calc_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/bedpostx5.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/bedpostx5.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/bedpostx5_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/bedpostx5_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/bet.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/bet.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/bet_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/bet_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/binary_maths.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/binary_maths.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/binary_maths_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/binary_maths_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/change_data_type.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/change_data_type.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/change_data_type_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/change_data_type_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/classifier.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/classifier.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/classifier_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/classifier_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/cleaner.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/cleaner.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/cleaner_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/cleaner_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/cluster.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/cluster.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/cluster_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/cluster_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/complex.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/complex.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/complex_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/complex_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/contrast_mgr.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/contrast_mgr.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/contrast_mgr_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/contrast_mgr_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/convert_warp.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/convert_warp.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/convert_warp_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/convert_warp_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/convert_xfm.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/convert_xfm.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/convert_xfm_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/convert_xfm_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/copy_geom.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/copy_geom.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/copy_geom_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/copy_geom_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/dilate_image.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/dilate_image.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/dilate_image_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/dilate_image_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/distance_map.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/distance_map.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/distance_map_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/distance_map_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/dti_fit.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/dti_fit.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/dti_fit_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/dti_fit_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/dual_regression.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/dual_regression.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/dual_regression_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/dual_regression_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/eddy.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/eddy.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/eddy_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/eddy_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/eddy_correct.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/eddy_correct.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/eddy_correct_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/eddy_correct_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/eddy_quad.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/eddy_quad.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/eddy_quad_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/eddy_quad_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/epi_de_warp.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/epi_de_warp.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/epi_de_warp_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/epi_de_warp_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/epi_reg.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/epi_reg.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/epi_reg_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/epi_reg_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/erode_image.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/erode_image.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/erode_image_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/erode_image_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/extract_roi.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/extract_roi.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/extract_roi_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/extract_roi_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/fast.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/fast.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/fast_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/fast_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/feat.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/feat.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/feat_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/feat_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/feat_model.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/feat_model.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/feat_model_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/feat_model_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/feature_extractor.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/feature_extractor.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/feature_extractor_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/feature_extractor_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/filmgls.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/filmgls.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/filmgls_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/filmgls_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/filter_regressor.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/filter_regressor.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/filter_regressor_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/filter_regressor_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/find_the_biggest.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/find_the_biggest.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/find_the_biggest_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/find_the_biggest_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/first.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/first.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/first_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/first_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/flameo.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/flameo.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/flameo_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/flameo_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/flirt.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/flirt.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/flirt_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/flirt_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/fnirt.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/fnirt.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/fnirt_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/fnirt_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/fugue.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/fugue.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/fugue_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/fugue_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/glm.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/glm.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/glm_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/glm_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/ica__aroma.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/ica__aroma.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/ica__aroma_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/ica__aroma_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/image_maths.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/image_maths.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/image_maths_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/image_maths_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/image_meants.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/image_meants.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/image_meants_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/image_meants_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/image_stats.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/image_stats.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/image_stats_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/image_stats_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/inv_warp.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/inv_warp.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/inv_warp_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/inv_warp_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/isotropic_smooth.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/isotropic_smooth.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/isotropic_smooth_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/isotropic_smooth_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/l2_model.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/l2_model.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/l2_model_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/l2_model_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/level_1_design.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/level_1_design.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/level_1_design_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/level_1_design_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/make_dyadic_vectors.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/make_dyadic_vectors.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/make_dyadic_vectors_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/make_dyadic_vectors_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/maths_command.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/maths_command.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/maths_command_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/maths_command_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/max_image.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/max_image.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/max_image_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/max_image_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/maxn_image.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/maxn_image.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/maxn_image_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/maxn_image_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/mcflirt.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/mcflirt.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/mcflirt_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/mcflirt_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/mean_image.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/mean_image.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/mean_image_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/mean_image_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/median_image.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/median_image.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/median_image_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/median_image_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/melodic.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/melodic.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/melodic_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/melodic_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/merge.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/merge.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/merge_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/merge_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/min_image.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/min_image.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/min_image_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/min_image_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/motion_outliers.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/motion_outliers.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/motion_outliers_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/motion_outliers_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/multi_image_maths.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/multi_image_maths.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/multi_image_maths_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/multi_image_maths_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/multiple_regress_design.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/multiple_regress_design.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/multiple_regress_design_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/multiple_regress_design_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/overlay.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/overlay.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/overlay_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/overlay_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/percentile_image.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/percentile_image.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/percentile_image_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/percentile_image_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/plot_motion_params.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/plot_motion_params.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/plot_motion_params_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/plot_motion_params_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/plot_time_series.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/plot_time_series.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/plot_time_series_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/plot_time_series_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/power_spectrum.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/power_spectrum.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/power_spectrum_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/power_spectrum_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/prelude.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/prelude.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/prelude_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/prelude_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/prepare_fieldmap.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/prepare_fieldmap.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/prepare_fieldmap_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/prepare_fieldmap_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/prob_track_x.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/prob_track_x.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/prob_track_x2.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/prob_track_x2.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/prob_track_x2_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/prob_track_x2_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/prob_track_x_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/prob_track_x_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/proj_thresh.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/proj_thresh.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/proj_thresh_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/proj_thresh_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/randomise.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/randomise.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/randomise_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/randomise_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/reorient_2_std.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/reorient_2_std.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/reorient_2_std_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/reorient_2_std_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/robust_fov.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/robust_fov.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/robust_fov_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/robust_fov_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/sig_loss.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/sig_loss.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/sig_loss_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/sig_loss_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/slice.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/slice.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/slice_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/slice_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/slice_timer.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/slice_timer.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/slice_timer_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/slice_timer_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/slicer.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/slicer.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/slicer_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/slicer_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/smm.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/smm.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/smm_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/smm_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/smooth.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/smooth.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/smooth_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/smooth_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/smooth_estimate.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/smooth_estimate.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/smooth_estimate_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/smooth_estimate_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/spatial_filter.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/spatial_filter.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/spatial_filter_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/spatial_filter_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/split.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/split.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/split_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/split_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/std_image.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/std_image.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/std_image_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/std_image_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/susan.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/susan.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/susan_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/susan_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/swap_dimensions.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/swap_dimensions.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/swap_dimensions_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/swap_dimensions_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/temporal_filter.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/temporal_filter.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/temporal_filter_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/temporal_filter_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/text_2_vest.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/text_2_vest.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/text_2_vest_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/text_2_vest_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/threshold.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/threshold.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/threshold_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/threshold_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/topup.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/topup.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/topup_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/topup_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/tract_skeleton.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/tract_skeleton.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/tract_skeleton_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/tract_skeleton_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/training.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/training.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/training_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/training_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/training_set_creator.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/training_set_creator.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/training_set_creator_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/training_set_creator_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/unary_maths.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/unary_maths.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/unary_maths_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/unary_maths_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/vec_reg.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/vec_reg.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/vec_reg_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/vec_reg_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/vest_2_text.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/vest_2_text.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/vest_2_text_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/vest_2_text_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_points.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/warp_points.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_points_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/warp_points_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_points_from_std.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/warp_points_from_std.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_points_from_std_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/warp_points_from_std_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_points_to_std.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/warp_points_to_std.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_points_to_std_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/warp_points_to_std_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_utils.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/warp_utils.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/warp_utils_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/warp_utils_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/x_fibres_5.yaml` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/x_fibres_5.yaml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/nipype-auto-conv/specs/x_fibres_5_callables.py` & `pydra_fsl-0.1.1/nipype-auto-conv/specs/interfaces/x_fibres_5_callables.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/__init__.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/__init__.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/accuracy_tester.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/accuracy_tester.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-from fileformats.generic.directory import Directory
-from fileformats.generic.file import File
+from fileformats.generic import Directory, File
 from fileformats.medimage_fsl import MelodicIca
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "mel_icas",
         ty.List[MelodicIca],
         {
             "help_string": "Melodic output directories",
             "argstr": "{mel_icas}",
@@ -58,17 +61,16 @@
 
 
 class AccuracyTester(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.directory import Directory
-    >>> from fileformats.generic.file import File
+    >>> from fileformats.generic import Directory, File
     >>> from fileformats.medimage_fsl import MelodicIca
-    >>> from pydra.tasks.fsl.auto.accuracy_tester import AccuracyTester
+    >>> from pydra.tasks.fsl.auto.fix.accuracy_tester import AccuracyTester
 
     """
 
     input_spec = AccuracyTester_input_spec
     output_spec = AccuracyTester_output_spec
     executable = "fix -C"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/apply_mask.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/percentile_image.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,55 @@
-from fileformats.medimage.contents.imaging.derivatives import Mask
-from fileformats.medimage.nifti import NiftiGz
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
-        "mask_file",
-        NiftiGz[Mask],
+        "dimension",
+        ty.Any,
+        "T",
         {
-            "help_string": "binary image defining mask space",
-            "argstr": "-mas {mask_file}",
-            "mandatory": True,
+            "help_string": "dimension to percentile across",
+            "argstr": "-{dimension}perc",
             "position": 4,
         },
     ),
     (
+        "perc",
+        ty.Any,
+        {
+            "help_string": "nth percentile (0-100) of FULL RANGE across dimension",
+            "argstr": "{perc}",
+            "position": 5,
+        },
+    ),
+    (
         "in_file",
-        NiftiGz,
+        Nifti1,
         {
             "help_string": "image to operate on",
             "argstr": "{in_file}",
             "mandatory": True,
             "position": 2,
         },
     ),
     (
         "out_file",
         Path,
         {
             "help_string": "image to write",
             "argstr": "{out_file}",
             "position": -2,
-            "output_file_template": "out_file.nii.gz",
+            "output_file_template": "out_file",
         },
     ),
     (
         "internal_datatype",
         ty.Any,
         {
             "help_string": "datatype to use for calculations (default is float)",
@@ -60,31 +72,36 @@
         {
             "help_string": "change NaNs to zeros before doing anything",
             "argstr": "-nan",
             "position": 3,
         },
     ),
 ]
-ApplyMask_input_spec = specs.SpecInfo(
+PercentileImage_input_spec = specs.SpecInfo(
     name="Input", fields=input_fields, bases=(specs.ShellSpec,)
 )
 
 output_fields = []
-ApplyMask_output_spec = specs.SpecInfo(
+PercentileImage_output_spec = specs.SpecInfo(
     name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
 )
 
 
-class ApplyMask(ShellCommandTask):
+class PercentileImage(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.medimage.contents.imaging.derivatives import Mask
-    >>> from fileformats.medimage.nifti import NiftiGz
-    >>> from pydra.tasks.fsl.auto.apply_mask import ApplyMask
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.maths.percentile_image import PercentileImage
+
+    >>> task = PercentileImage()
+    >>> task.inputs.in_file = Nifti1.mock("functional.nii"  # doctest: +SKIP)
+    >>> task.cmdline
+    'fslmaths functional.nii -Tperc 90 functional_perc.nii'
+
 
     """
 
-    input_spec = ApplyMask_input_spec
-    output_spec = ApplyMask_output_spec
+    input_spec = PercentileImage_input_spec
+    output_spec = PercentileImage_output_spec
     executable = "fslmaths"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/apply_topup.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/apply_topup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-from fileformats.medimage.nifti import Nifti1
-from fileformats.medimage.nifti import NiftiGz
+from fileformats.medimage import Nifti1, NiftiGz
 from fileformats.text import TextFile
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_files",
         ty.List[Nifti1],
         {
             "help_string": "name of file with images",
             "argstr": "--imain={in_files}",
@@ -93,18 +96,17 @@
 
 
 class ApplyTOPUP(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from fileformats.medimage.nifti import NiftiGz
+    >>> from fileformats.medimage import Nifti1, NiftiGz
     >>> from fileformats.text import TextFile
-    >>> from pydra.tasks.fsl.auto.apply_topup import ApplyTOPUP
+    >>> from pydra.tasks.fsl.auto.epi.apply_topup import ApplyTOPUP
 
     >>> task = ApplyTOPUP()
     >>> task.inputs.in_files = [Nifti1.mock("epi.nii"), Nifti1.mock("epi_rev.nii")]
     >>> task.inputs.encoding_file = TextFile.mock("topup_encoding.txt")
     >>> task.inputs.in_topup_fieldcoef = NiftiGz.mock("topup_fieldcoef.nii.gz")
     >>> task.inputs.in_topup_movpar = TextFile.mock("topup_movpar.txt")
     >>> task.cmdline
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/apply_warp.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/apply_warp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.medimage.nifti import NiftiGz
+from fileformats.medimage import NiftiGz
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         NiftiGz,
         {
             "help_string": "image to be warped",
             "argstr": "--in={in_file}",
@@ -128,15 +132,15 @@
 
 
 class ApplyWarp(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.medimage.nifti import NiftiGz
-    >>> from pydra.tasks.fsl.auto.apply_warp import ApplyWarp
+    >>> from fileformats.medimage import NiftiGz
+    >>> from pydra.tasks.fsl.auto.preprocess.apply_warp import ApplyWarp
 
     """
 
     input_spec = ApplyWarp_input_spec
     output_spec = ApplyWarp_output_spec
     executable = "applywarp"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/apply_xfm.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/apply_xfm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "apply_xfm",
         bool,
         True,
         {
             "help_string": "apply transformation supplied by in_matrix_file or uses_qform to use the affine matrix stored in the reference header",
@@ -348,15 +352,15 @@
 
 
 class ApplyXFM(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.apply_xfm import ApplyXFM
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.preprocess.apply_xfm import ApplyXFM
 
     """
 
     input_spec = ApplyXFM_input_spec
     output_spec = ApplyXFM_output_spec
     executable = "flirt"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/ar1_image.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/unary_maths.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
-        "dimension",
+        "operation",
         ty.Any,
-        "T",
         {
-            "help_string": "dimension to find AR(1) coefficientacross",
-            "argstr": "-{dimension}ar1",
+            "help_string": "operation to perform",
+            "argstr": "-{operation}",
+            "mandatory": True,
             "position": 4,
         },
     ),
     (
         "in_file",
         File,
         {
@@ -59,30 +63,30 @@
         {
             "help_string": "change NaNs to zeros before doing anything",
             "argstr": "-nan",
             "position": 3,
         },
     ),
 ]
-AR1Image_input_spec = specs.SpecInfo(
+UnaryMaths_input_spec = specs.SpecInfo(
     name="Input", fields=input_fields, bases=(specs.ShellSpec,)
 )
 
 output_fields = []
-AR1Image_output_spec = specs.SpecInfo(
+UnaryMaths_output_spec = specs.SpecInfo(
     name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
 )
 
 
-class AR1Image(ShellCommandTask):
+class UnaryMaths(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.ar1_image import AR1Image
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.maths.unary_maths import UnaryMaths
 
     """
 
-    input_spec = AR1Image_input_spec
-    output_spec = AR1Image_output_spec
+    input_spec = UnaryMaths_input_spec
+    output_spec = UnaryMaths_output_spec
     executable = "fslmaths"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/av_scale.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/av_scale.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from fileformats.generic.file import File
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from fileformats.generic import File
+import logging
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
 
 
 def average_scaling_callable(output_dir, inputs, stdout, stderr):
     outputs = _list_outputs(
         output_dir=output_dir, inputs=inputs, stdout=stdout, stderr=stderr
     )
     return outputs["average_scaling"]
@@ -82,15 +85,15 @@
 
 
 class AvScale(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.av_scale import AvScale
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.utils.av_scale import AvScale
 
     """
 
     input_spec = AvScale_input_spec
     output_spec = AvScale_output_spec
     executable = "avscale"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/b0_calc.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/possum/b0_calc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.medimage.nifti import Nifti1
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         Nifti1,
         {
             "help_string": "filename of input image (usually a tissue/air segmentation)",
             "argstr": "-i {in_file}",
@@ -142,16 +146,16 @@
 
 
 class B0Calc(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.b0_calc import B0Calc
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.possum.b0_calc import B0Calc
 
     >>> task = B0Calc()
     >>> task.inputs.in_file = Nifti1.mock("tissue+air_map.nii")
     >>> task.inputs.z_b0 = 3.0
     >>> task.cmdline
     'b0calc -i tissue+air_map.nii -o tissue+air_map_b0field.nii.gz --chi0=4.000000e-07 -d -9.450000e-06 --extendboundary=1.00 --b0x=0.00 --gx=0.0000 --b0y=0.00 --gy=0.0000 --b0=3.00 --gz=0.0000'
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/bedpostx5.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/bedpostx5.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from fileformats.generic.directory import Directory
-from fileformats.generic.file import File
-from fileformats.medimage.diffusion import Bval
-from fileformats.medimage.diffusion import Bvec
-from fileformats.medimage.nifti import Nifti1
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from fileformats.generic import Directory, File
+from fileformats.medimage import Bval, Bvec, Nifti1
+import logging
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "dwi",
         Nifti1,
         {"help_string": "diffusion weighted image data file", "mandatory": True},
     ),
     ("mask", Nifti1, {"help_string": "bet binary mask file", "mandatory": True}),
@@ -229,20 +230,17 @@
 
 
 class BEDPOSTX5(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.directory import Directory
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.diffusion import Bval
-    >>> from fileformats.medimage.diffusion import Bvec
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.bedpostx5 import BEDPOSTX5
+    >>> from fileformats.generic import Directory, File
+    >>> from fileformats.medimage import Bval, Bvec, Nifti1
+    >>> from pydra.tasks.fsl.auto.dti.bedpostx5 import BEDPOSTX5
 
     >>> task = BEDPOSTX5()
     >>> task.inputs.dwi = Nifti1.mock("diffusion.nii")
     >>> task.inputs.mask = Nifti1.mock("mask.nii")
     >>> task.inputs.bvecs = Bvec.mock("bvecs")
     >>> task.inputs.bvals = Bval.mock("bvals")
     >>> task.inputs.logdir = Directory.mock()
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/bet.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/bet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "in_file",
         Nifti1,
         {
             "help_string": "input file to skull strip",
@@ -241,17 +245,17 @@
 
 
 class BET(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.bet import BET
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.preprocess.bet import BET
 
     >>> task = BET()
     >>> task.inputs.in_file = Nifti1.mock("structural.nii")
     >>> task.inputs.out_file = "brain_anat.nii"
     >>> task.inputs.frac = 0.7
     >>> task.inputs.t2_guided = File.mock()
     >>> task.cmdline
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/binary_maths.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/binary_maths.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "operation",
         ty.Any,
         {
             "help_string": "operation to perform",
             "argstr": "-{operation}",
@@ -96,15 +100,15 @@
 
 
 class BinaryMaths(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.binary_maths import BinaryMaths
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.maths.binary_maths import BinaryMaths
 
     """
 
     input_spec = BinaryMaths_input_spec
     output_spec = BinaryMaths_output_spec
     executable = "fslmaths"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/change_data_type.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/smm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,68 @@
-from fileformats.generic.file import File
-from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
-import typing as ty
+from fileformats.generic import File
+import logging
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
-        "output_datatype",
-        ty.Any,
+        "spatial_data_file",
+        File,
         {
-            "help_string": "output data type",
-            "argstr": "-odt {output_datatype}",
+            "help_string": "statistics spatial map",
+            "argstr": '--sdf="{spatial_data_file}"',
+            "copyfile": False,
             "mandatory": True,
-            "position": -1,
+            "position": 0,
         },
     ),
     (
-        "in_file",
+        "mask",
         File,
         {
-            "help_string": "image to operate on",
-            "argstr": "{in_file}",
+            "help_string": "mask file",
+            "argstr": '--mask="{mask}"',
+            "copyfile": False,
             "mandatory": True,
-            "position": 2,
-        },
-    ),
-    (
-        "out_file",
-        Path,
-        {
-            "help_string": "image to write",
-            "argstr": "{out_file}",
-            "position": -2,
-            "output_file_template": "out_file",
-        },
-    ),
-    (
-        "internal_datatype",
-        ty.Any,
-        {
-            "help_string": "datatype to use for calculations (default is float)",
-            "argstr": "-dt {internal_datatype}",
             "position": 1,
         },
     ),
     (
-        "nan2zeros",
+        "no_deactivation_class",
         bool,
         {
-            "help_string": "change NaNs to zeros before doing anything",
-            "argstr": "-nan",
-            "position": 3,
+            "help_string": "enforces no deactivation class",
+            "argstr": "--zfstatmode",
+            "position": 2,
         },
     ),
 ]
-ChangeDataType_input_spec = specs.SpecInfo(
+SMM_input_spec = specs.SpecInfo(
     name="Input", fields=input_fields, bases=(specs.ShellSpec,)
 )
 
-output_fields = []
-ChangeDataType_output_spec = specs.SpecInfo(
+output_fields = [
+    ("null_p_map", File, {}),
+    ("activation_p_map", File, {}),
+    ("deactivation_p_map", File, {}),
+]
+SMM_output_spec = specs.SpecInfo(
     name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
 )
 
 
-class ChangeDataType(ShellCommandTask):
+class SMM(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.change_data_type import ChangeDataType
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.model.smm import SMM
 
     """
 
-    input_spec = ChangeDataType_input_spec
-    output_spec = ChangeDataType_output_spec
-    executable = "fslmaths"
+    input_spec = SMM_input_spec
+    output_spec = SMM_output_spec
+    executable = "mm --ld=logdir"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/classifier.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/classifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-from fileformats.generic.directory import Directory
-from fileformats.generic.file import File
+from fileformats.generic import Directory, File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "mel_ica",
         Directory,
         {
             "help_string": "Melodic output directory or directories",
@@ -63,16 +66,15 @@
 
 
 class Classifier(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.directory import Directory
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.classifier import Classifier
+    >>> from fileformats.generic import Directory, File
+    >>> from pydra.tasks.fsl.auto.fix.classifier import Classifier
 
     """
 
     input_spec = Classifier_input_spec
     output_spec = Classifier_output_spec
     executable = "fix -c"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/cleaner.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/cleaner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-from fileformats.generic.file import File
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from fileformats.generic import File
+import logging
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "artifacts_list_file",
         File,
         {
             "help_string": "Text file listing which ICs are artifacts; can be the output from classification or can be created manually",
@@ -82,15 +86,15 @@
 
 
 class Cleaner(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.cleaner import Cleaner
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.fix.cleaner import Cleaner
 
     """
 
     input_spec = Cleaner_input_spec
     output_spec = Cleaner_output_spec
     executable = "fix -a"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/cluster.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import NiftiGz
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from fileformats.generic import File
+from fileformats.medimage import NiftiGz
+import logging
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         NiftiGz,
         {"help_string": "input volume", "argstr": "--in={in_file}", "mandatory": True},
     ),
     (
@@ -211,17 +215,17 @@
 
 
 class Cluster(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import NiftiGz
-    >>> from pydra.tasks.fsl.auto.cluster import Cluster
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import NiftiGz
+    >>> from pydra.tasks.fsl.auto.model.cluster import Cluster
 
     >>> task = Cluster()
     >>> task.inputs.in_file = NiftiGz.mock("zstat1.nii.gz")
     >>> task.inputs.threshold = 2.3
     >>> task.inputs.out_localmax_txt_file = "stats.txt"
     >>> task.inputs.cope_file = File.mock()
     >>> task.inputs.use_mm = True
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/complex.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/complex.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "complex_in_file",
         File,
         {"help_string": "", "argstr": "{complex_in_file}", "position": 2},
     ),
@@ -251,15 +255,15 @@
 
 
 class Complex(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.complex import Complex
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.utils.complex import Complex
 
     """
 
     input_spec = Complex_input_spec
     output_spec = Complex_output_spec
     executable = "fslcomplex"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/contrast_mgr.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/contrast_mgr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-from fileformats.generic.file import File
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from fileformats.generic import File
+import logging
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "tcon_file",
         File,
         {
             "help_string": "contrast file containing T-contrasts",
             "argstr": "{tcon_file}",
@@ -102,15 +106,15 @@
 
 
 class ContrastMgr(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.contrast_mgr import ContrastMgr
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.model.contrast_mgr import ContrastMgr
 
     """
 
     input_spec = ContrastMgr_input_spec
     output_spec = ContrastMgr_output_spec
     executable = "contrast_mgr"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/convert_warp.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/convert_warp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "reference",
         Nifti1,
         {
             "help_string": "Name of a file in target space of the full transform.",
             "argstr": "--ref={reference}",
@@ -155,17 +159,17 @@
 
 
 class ConvertWarp(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.convert_warp import ConvertWarp
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.utils.convert_warp import ConvertWarp
 
     >>> task = ConvertWarp()
     >>> task.inputs.reference = Nifti1.mock("T1.nii")
     >>> task.inputs.premat = File.mock()
     >>> task.inputs.warp1 = Nifti1.mock("warpfield.nii")
     >>> task.inputs.midmat = File.mock()
     >>> task.inputs.warp2 = File.mock()
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/convert_xfm.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/convert_xfm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-from fileformats.datascience.data import TextMatrix
-from fileformats.generic.file import File
+from fileformats.datascience import TextMatrix
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "in_file",
         TextMatrix,
         {
             "help_string": "input transformation matrix",
@@ -78,17 +82,17 @@
 
 
 class ConvertXFM(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.datascience.data import TextMatrix
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.convert_xfm import ConvertXFM
+    >>> from fileformats.datascience import TextMatrix
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.utils.convert_xfm import ConvertXFM
 
     >>> task = ConvertXFM()
     >>> task.inputs.in_file = TextMatrix.mock("flirt.mat")
     >>> task.inputs.in_file2 = File.mock()
     >>> task.inputs.invert_xfm = True
     >>> task.inputs.out_file = "flirt_inv.mat"
     >>> task.cmdline
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/copy_geom.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/copy_geom.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "in_file",
         File,
         {
             "help_string": "source image",
@@ -46,15 +50,15 @@
 
 
 class CopyGeom(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.copy_geom import CopyGeom
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.utils.copy_geom import CopyGeom
 
     """
 
     input_spec = CopyGeom_input_spec
     output_spec = CopyGeom_output_spec
     executable = "fslcpgeom"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/dilate_image.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/dilate_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "operation",
         ty.Any,
         {
             "help_string": "filtering operation to perform in dilation",
             "argstr": "-dil{operation}",
@@ -103,15 +107,15 @@
 
 
 class DilateImage(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.dilate_image import DilateImage
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.maths.dilate_image import DilateImage
 
     """
 
     input_spec = DilateImage_input_spec
     output_spec = DilateImage_output_spec
     executable = "fslmaths"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/distance_map.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/distance_map.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         File,
         {
             "help_string": "image to calculate distance values for",
             "argstr": "--in={in_file}",
@@ -52,15 +56,15 @@
 
 
 class DistanceMap(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.distance_map import DistanceMap
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.dti.distance_map import DistanceMap
 
     """
 
     input_spec = DistanceMap_input_spec
     output_spec = DistanceMap_output_spec
     executable = "distancemap"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/dti_fit.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/dti_fit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from fileformats.generic.file import File
-from fileformats.medimage.diffusion import Bval
-from fileformats.medimage.diffusion import Bvec
-from fileformats.medimage.nifti import Nifti1
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from fileformats.generic import File
+from fileformats.medimage import Bval, Bvec, Nifti1
+import logging
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "dwi",
         Nifti1,
         {
             "help_string": "diffusion weighted image data file",
@@ -117,19 +119,17 @@
 
 
 class DTIFit(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.diffusion import Bval
-    >>> from fileformats.medimage.diffusion import Bvec
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.dti_fit import DTIFit
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Bval, Bvec, Nifti1
+    >>> from pydra.tasks.fsl.auto.dti.dti_fit import DTIFit
 
     >>> task = DTIFit()
     >>> task.inputs.dwi = Nifti1.mock("diffusion.nii")
     >>> task.inputs.base_name = "TP"
     >>> task.inputs.mask = Nifti1.mock("mask.nii")
     >>> task.inputs.bvecs = Bvec.mock("bvecs")
     >>> task.inputs.bvals = Bval.mock("bvals")
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/dual_regression.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/dual_regression.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_files",
         ty.List[Nifti1],
         {
             "help_string": "List all subjects' preprocessed, standard-space 4D datasets",
             "argstr": "{in_files}",
@@ -97,17 +101,17 @@
 
 
 class DualRegression(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.dual_regression import DualRegression
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.model.dual_regression import DualRegression
 
     >>> task = DualRegression()
     >>> task.inputs.in_files = [Nifti1.mock("functional.nii"), Nifti1.mock("functional2.nii"), Nifti1.mock("functional3.nii")]
     >>> task.inputs.group_IC_maps_4D = Nifti1.mock("allFA.nii")
     >>> task.inputs.des_norm = False
     >>> task.inputs.one_sample_group_mean = True
     >>> task.inputs.design_file = File.mock()
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/eddy.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/eddy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.diffusion import Bval
-from fileformats.medimage.diffusion import Bvec
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Bval, Bvec, Nifti1
 from fileformats.text import TextFile
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+import logging
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         Nifti1,
         {
             "help_string": "File containing all the images to estimate distortions for",
             "argstr": "--imain={in_file}",
@@ -467,20 +469,18 @@
 
 
 class Eddy(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.diffusion import Bval
-    >>> from fileformats.medimage.diffusion import Bvec
-    >>> from fileformats.medimage.nifti import Nifti1
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Bval, Bvec, Nifti1
     >>> from fileformats.text import TextFile
-    >>> from pydra.tasks.fsl.auto.eddy import Eddy
+    >>> from pydra.tasks.fsl.auto.epi.eddy import Eddy
 
     >>> task = Eddy()
     >>> task.inputs.in_file = Nifti1.mock("epi.nii")
     >>> task.inputs.in_mask = File.mock()
     >>> task.inputs.in_index = TextFile.mock("epi_index.txt")
     >>> task.inputs.in_acqp = File.mock()
     >>> task.inputs.in_bvec = Bvec.mock()
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/eddy_correct.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/eddy_correct.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "in_file",
         Nifti1,
         {
             "help_string": "4D input file",
@@ -48,17 +52,17 @@
 
 
 class EddyCorrect(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.eddy_correct import EddyCorrect
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.epi.eddy_correct import EddyCorrect
 
     >>> task = EddyCorrect()
     >>> task.inputs.in_file = Nifti1.mock("diffusion.nii")
     >>> task.inputs.out_file = "diffusion_edc.nii"
     >>> task.inputs.ref_num = 0
     >>> task.cmdline
     'eddy_correct diffusion.nii diffusion_edc.nii 0'
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/eddy_quad.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/eddy_quad.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.diffusion import Bval
-from fileformats.medimage.diffusion import Bvec
+from fileformats.generic import File
+from fileformats.medimage import Bval, Bvec
 from fileformats.text import TextFile
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+import logging
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "base_name",
         str,
         "eddy_corrected",
         {
             "help_string": "Basename (including path) for EDDY output files, i.e., corrected images and QC files",
@@ -146,19 +149,18 @@
 
 
 class EddyQuad(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.diffusion import Bval
-    >>> from fileformats.medimage.diffusion import Bvec
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Bval, Bvec
     >>> from fileformats.text import TextFile
-    >>> from pydra.tasks.fsl.auto.eddy_quad import EddyQuad
+    >>> from pydra.tasks.fsl.auto.epi.eddy_quad import EddyQuad
 
     >>> task = EddyQuad()
     >>> task.inputs.idx_file = File.mock()
     >>> task.inputs.param_file = TextFile.mock("epi_acqp.txt")
     >>> task.inputs.mask_file = File.mock()
     >>> task.inputs.bval_file = Bval.mock()
     >>> task.inputs.bvec_file = Bvec.mock()
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/epi_de_warp.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/epi_de_warp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "mag_file",
         Nifti1,
         {
             "help_string": "Magnitude file",
             "argstr": "--mag {mag_file}",
@@ -90,17 +94,17 @@
 
 
 class EPIDeWarp(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.epi_de_warp import EPIDeWarp
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.epi.epi_de_warp import EPIDeWarp
 
     >>> task = EPIDeWarp()
     >>> task.inputs.mag_file = Nifti1.mock("magnitude.nii")
     >>> task.inputs.dph_file = Nifti1.mock("phase.nii")
     >>> task.inputs.exf_file = File.mock()
     >>> task.inputs.epi_file = Nifti1.mock("functional.nii")
     >>> task.cmdline
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/epi_reg.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/epi_reg.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "epi",
         Nifti1,
         {
             "help_string": "EPI image",
             "argstr": "--epi={epi}",
@@ -150,17 +154,17 @@
 
 
 class EpiReg(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.epi_reg import EpiReg
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.epi.epi_reg import EpiReg
 
     >>> task = EpiReg()
     >>> task.inputs.epi = Nifti1.mock("epi.nii")
     >>> task.inputs.t1_head = Nifti1.mock("T1.nii")
     >>> task.inputs.t1_brain = Nifti1.mock("T1_brain.nii")
     >>> task.inputs.out_base = "epi2struct"
     >>> task.inputs.fmap = Nifti1.mock("fieldmap_phase_fslprepared.nii")
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/erode_image.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/erode_image.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "minimum_filter",
         bool,
         False,
         {
             "help_string": "if true, minimum filter rather than erosion by zeroing-out",
@@ -103,15 +107,15 @@
 
 
 class ErodeImage(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.erode_image import ErodeImage
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.maths.erode_image import ErodeImage
 
     """
 
     input_spec = ErodeImage_input_spec
     output_spec = ErodeImage_output_spec
     executable = "fslmaths"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/extract_roi.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/extract_roi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "in_file",
         File,
         {
             "help_string": "input file",
@@ -63,16 +67,16 @@
 
 
 class ExtractROI(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.extract_roi import ExtractROI
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.utils.extract_roi import ExtractROI
 
     >>> task = ExtractROI()
     >>> task.inputs.in_file = File.mock(anatfile)
     >>> task.inputs.roi_file = "bar.nii"
     >>> task.inputs.t_min = 0
     >>> task.inputs.t_size = 1
     >>> task.cmdline
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/fast.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/fast.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_files",
         ty.List[Nifti1],
         {
             "help_string": "image, or multi-channel set of images, to be segmented",
             "argstr": "{in_files}",
@@ -178,17 +182,17 @@
 
 
 class FAST(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.fast import FAST
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.preprocess.fast import FAST
 
     >>> task = FAST()
     >>> task.inputs.in_files = [Nifti1.mock("s"), Nifti1.mock("t"), Nifti1.mock("r"), Nifti1.mock("u"), Nifti1.mock("c"), Nifti1.mock("t"), Nifti1.mock("u"), Nifti1.mock("r"), Nifti1.mock("a"), Nifti1.mock("l"), Nifti1.mock("."), Nifti1.mock("n"), Nifti1.mock("i"), Nifti1.mock("i")]
     >>> task.inputs.out_basename = "fast_"
     >>> task.inputs.init_transform = File.mock()
     >>> task.inputs.manual_seg = File.mock()
     >>> task.cmdline
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/feat.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/power_spectrum.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,54 @@
-from fileformats.generic.directory import Directory
-from fileformats.generic.file import File
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from fileformats.generic import File
+import logging
+from pathlib import Path
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
-        "fsf_file",
+        "in_file",
         File,
         {
-            "help_string": "File specifying the feat design spec file",
-            "argstr": "{fsf_file}",
+            "help_string": "input 4D file to estimate the power spectrum",
+            "argstr": "{in_file}",
             "mandatory": True,
             "position": 0,
         },
-    )
+    ),
+    (
+        "out_file",
+        Path,
+        {
+            "help_string": "name of output 4D file for power spectrum",
+            "argstr": "{out_file}",
+            "position": 1,
+            "output_file_template": "out_file",
+        },
+    ),
 ]
-FEAT_input_spec = specs.SpecInfo(
+PowerSpectrum_input_spec = specs.SpecInfo(
     name="Input", fields=input_fields, bases=(specs.ShellSpec,)
 )
 
-output_fields = [("feat_dir", Directory, {})]
-FEAT_output_spec = specs.SpecInfo(
+output_fields = []
+PowerSpectrum_output_spec = specs.SpecInfo(
     name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
 )
 
 
-class FEAT(ShellCommandTask):
+class PowerSpectrum(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.directory import Directory
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.feat import FEAT
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.utils.power_spectrum import PowerSpectrum
 
     """
 
-    input_spec = FEAT_input_spec
-    output_spec = FEAT_output_spec
-    executable = "feat"
+    input_spec = PowerSpectrum_input_spec
+    output_spec = PowerSpectrum_output_spec
+    executable = "fslpspec"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/feat_model.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/feat_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-from fileformats.generic.file import File
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from fileformats.generic import File
+import logging
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "fsf_file",
         File,
         {
             "help_string": "File specifying the feat design spec file",
             "argstr": "{fsf_file}",
@@ -56,15 +60,15 @@
 
 
 class FEATModel(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.feat_model import FEATModel
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.model.feat_model import FEATModel
 
     """
 
     input_spec = FEATModel_input_spec
     output_spec = FEATModel_output_spec
     executable = "feat_model"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/feature_extractor.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/feature_extractor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from fileformats.generic.directory import Directory
+from fileformats.generic import Directory
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "mel_ica",
         Path,
         {
             "help_string": "Melodic output directory or directories",
@@ -28,15 +32,15 @@
 
 
 class FeatureExtractor(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.directory import Directory
-    >>> from pydra.tasks.fsl.auto.feature_extractor import FeatureExtractor
+    >>> from fileformats.generic import Directory
+    >>> from pydra.tasks.fsl.auto.fix.feature_extractor import FeatureExtractor
 
     """
 
     input_spec = FeatureExtractor_input_spec
     output_spec = FeatureExtractor_output_spec
     executable = "fix -f"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/filmgls.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/filmgls.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-from fileformats.generic.directory import Directory
-from fileformats.generic.file import File
+from fileformats.generic import Directory, File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         File,
         {
             "help_string": "input data file",
             "argstr": "{in_file}",
@@ -186,16 +189,15 @@
 
 
 class FILMGLS(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.directory import Directory
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.filmgls import FILMGLS
+    >>> from fileformats.generic import Directory, File
+    >>> from pydra.tasks.fsl.auto.model.filmgls import FILMGLS
 
     """
 
     input_spec = FILMGLS_input_spec
     output_spec = FILMGLS_output_spec
     executable = "film_gls"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/filter_regressor.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/filter_regressor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "in_file",
         File,
         {
             "help_string": "input file name (4D image)",
@@ -82,15 +86,15 @@
 
 
 class FilterRegressor(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.filter_regressor import FilterRegressor
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.utils.filter_regressor import FilterRegressor
 
     """
 
     input_spec = FilterRegressor_input_spec
     output_spec = FilterRegressor_output_spec
     executable = "fsl_regfilt"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/find_the_biggest.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/slice.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,59 @@
-from fileformats.generic.file import File
-from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
-        "in_files",
-        ty.List[File],
+        "in_file",
+        Nifti1,
         {
-            "help_string": "a list of input volumes or a singleMatrixFile",
-            "argstr": "{in_files}",
+            "help_string": "input filename",
+            "argstr": "{in_file}",
+            "copyfile": False,
             "mandatory": True,
             "position": 0,
         },
     ),
     (
-        "out_file",
-        Path,
-        {
-            "help_string": "file with the resulting segmentation",
-            "argstr": "{out_file}",
-            "position": 2,
-            "output_file_template": '"biggestSegmentation"',
-        },
+        "out_base_name",
+        str,
+        {"help_string": "outputs prefix", "argstr": "{out_base_name}", "position": 1},
     ),
 ]
-FindTheBiggest_input_spec = specs.SpecInfo(
+Slice_input_spec = specs.SpecInfo(
     name="Input", fields=input_fields, bases=(specs.ShellSpec,)
 )
 
-output_fields = []
-FindTheBiggest_output_spec = specs.SpecInfo(
+output_fields = [("out_files", ty.List[File], {})]
+Slice_output_spec = specs.SpecInfo(
     name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
 )
 
 
-class FindTheBiggest(ShellCommandTask):
+class Slice(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.find_the_biggest import FindTheBiggest
-
-    >>> task = FindTheBiggest()
-    >>> task.inputs.in_files = ldir
-    >>> task.inputs.out_file = "biggestSegmentation"
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.utils.slice import Slice
+
+    >>> task = Slice()
+    >>> task.inputs.in_file = Nifti1.mock("functional.nii")
+    >>> task.inputs.out_base_name = "sl"
     >>> task.cmdline
-    'find_the_biggest seeds_to_M1.nii seeds_to_M2.nii biggestSegmentation'
+    'fslslice functional.nii sl'
 
 
     """
 
-    input_spec = FindTheBiggest_input_spec
-    output_spec = FindTheBiggest_output_spec
-    executable = "find_the_biggest"
+    input_spec = Slice_input_spec
+    output_spec = Slice_output_spec
+    executable = "fslslice"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/first.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/first.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-from fileformats.generic.file import File
-from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from fileformats.generic import File
 import logging
+from pathlib import Path
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         File,
         {
             "help_string": "input data file",
             "argstr": "-i {in_file}",
@@ -122,15 +125,15 @@
 
 
 class FIRST(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.first import FIRST
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.preprocess.first import FIRST
 
     """
 
     input_spec = FIRST_input_spec
     output_spec = FIRST_output_spec
     executable = "run_first_all"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/flameo.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/flameo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from fileformats.datascience.data import TextMatrix
-from fileformats.generic.directory import Directory
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
-from fileformats.medimage.nifti import NiftiGz
+from fileformats.datascience import TextMatrix
+from fileformats.generic import Directory, File
+from fileformats.medimage import Nifti1, NiftiGz
 from fileformats.medimage_fsl import Con
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+import logging
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "cope_file",
         NiftiGz,
         {
             "help_string": "cope regressor data file",
             "argstr": "--copefile={cope_file}",
@@ -183,21 +185,19 @@
 
 
 class FLAMEO(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.datascience.data import TextMatrix
-    >>> from fileformats.generic.directory import Directory
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from fileformats.medimage.nifti import NiftiGz
+    >>> from fileformats.datascience import TextMatrix
+    >>> from fileformats.generic import Directory, File
+    >>> from fileformats.medimage import Nifti1, NiftiGz
     >>> from fileformats.medimage_fsl import Con
-    >>> from pydra.tasks.fsl.auto.flameo import FLAMEO
+    >>> from pydra.tasks.fsl.auto.model.flameo import FLAMEO
 
     >>> task = FLAMEO()
     >>> task.inputs.cope_file = NiftiGz.mock("cope.nii.gz")
     >>> task.inputs.var_cope_file = NiftiGz.mock("varcope.nii.gz")
     >>> task.inputs.dof_var_cope_file = File.mock()
     >>> task.inputs.mask_file = Nifti1.mock("mask.nii")
     >>> task.inputs.design_file = TextMatrix.mock("design.mat")
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/flirt.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/flirt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         Nifti1,
         {
             "help_string": "input file",
             "argstr": "-in {in_file}",
@@ -348,17 +352,17 @@
 
 
 class FLIRT(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.flirt import FLIRT
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.preprocess.flirt import FLIRT
 
     >>> task = FLIRT()
     >>> task.inputs.in_file = Nifti1.mock("structural.nii")
     >>> task.inputs.reference = Nifti1.mock("mni.nii")
     >>> task.inputs.in_matrix_file = File.mock()
     >>> task.inputs.cost_func = "mutualinfo"
     >>> task.inputs.bins = 640
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/fnirt.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/fnirt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "ref_file",
         File,
         {
             "help_string": "name of reference image",
             "argstr": "--ref={ref_file}",
@@ -378,16 +382,16 @@
 
 
 class FNIRT(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.fnirt import FNIRT
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.preprocess.fnirt import FNIRT
 
     >>> task = FNIRT()
     >>> task.inputs.ref_file = File.mock()
     >>> task.inputs.in_file = File.mock()
     >>> task.inputs.affine_file = File.mock()
     >>> task.inputs.inwarp_file = File.mock()
     >>> task.inputs.refmask_file = File.mock()
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/fugue.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/fugue.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         Nifti1,
         {"help_string": "filename of input volume", "argstr": "--in={in_file}"},
     ),
     (
@@ -264,17 +268,17 @@
 
 
 class FUGUE(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.fugue import FUGUE
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.preprocess.fugue import FUGUE
 
     >>> task = FUGUE()
     >>> task.inputs.in_file = Nifti1.mock("epi.nii")
     >>> task.inputs.shift_in_file = Nifti1.mock("vsm.nii"  # Previously computed with fugue as well)
     >>> task.inputs.phasemap_in_file = Nifti1.mock()
     >>> task.inputs.fmap_in_file = File.mock()
     >>> task.inputs.unwarp_direction = "y"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/glm.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/glm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         Nifti1,
         {
             "help_string": "input file name (text matrix or 3D/4D image file)",
             "argstr": "-i {in_file}",
@@ -238,17 +242,17 @@
 
 
 class GLM(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.glm import GLM
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.model.glm import GLM
 
     >>> task = GLM()
     >>> task.inputs.in_file = Nifti1.mock("functional.nii")
     >>> task.inputs.design = Nifti1.mock("maps.nii")
     >>> task.inputs.contrasts = File.mock()
     >>> task.inputs.mask = File.mock()
     >>> task.cmdline
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/ica__aroma.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/aroma/ica__aroma.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from fileformats.datascience.data import TextMatrix
-from fileformats.generic.directory import Directory
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
-from fileformats.medimage.nifti import NiftiGz
+from fileformats.datascience import TextMatrix
+from fileformats.generic import Directory, File
+from fileformats.medimage import Nifti1, NiftiGz
 from fileformats.text import TextFile
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "feat_dir",
         Directory,
         {
             "help_string": "If a feat directory exists and temporal filtering has not been run yet, ICA_AROMA can use the files in this directory.",
             "argstr": "-feat {feat_dir}",
@@ -139,21 +141,19 @@
 
 
 class ICA_AROMA(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.datascience.data import TextMatrix
-    >>> from fileformats.generic.directory import Directory
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from fileformats.medimage.nifti import NiftiGz
+    >>> from fileformats.datascience import TextMatrix
+    >>> from fileformats.generic import Directory, File
+    >>> from fileformats.medimage import Nifti1, NiftiGz
     >>> from fileformats.text import TextFile
-    >>> from pydra.tasks.fsl.auto.ica__aroma import ICA_AROMA
+    >>> from pydra.tasks.fsl.auto.aroma.ica__aroma import ICA_AROMA
 
     >>> task = ICA_AROMA()
     >>> task.inputs.feat_dir = Directory.mock()
     >>> task.inputs.in_file = Nifti1.mock("functional.nii")
     >>> task.inputs.out_dir = "ICA_testout"
     >>> task.inputs.mask = NiftiGz.mock("mask.nii.gz")
     >>> task.inputs.melodic_dir = Directory.mock()
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/image_maths.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/image_maths.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         File,
         {"help_string": "", "argstr": "{in_file}", "mandatory": True, "position": 1},
     ),
     ("in_file2", File, {"help_string": "", "argstr": "{in_file2}", "position": 3}),
@@ -60,16 +64,16 @@
 
 
 class ImageMaths(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.image_maths import ImageMaths
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.utils.image_maths import ImageMaths
 
     >>> task = ImageMaths()
     >>> task.inputs.in_file = File.mock(anatfile)
     >>> task.inputs.in_file2 = File.mock()
     >>> task.inputs.mask_file = File.mock()
     >>> task.inputs.out_file = "foo_maths.nii"
     >>> task.inputs.op_string = "-add 5"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/image_meants.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/image_meants.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "in_file",
         File,
         {
             "help_string": "input file for computing the average timeseries",
@@ -90,15 +94,15 @@
 
 
 class ImageMeants(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.image_meants import ImageMeants
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.utils.image_meants import ImageMeants
 
     """
 
     input_spec = ImageMeants_input_spec
     output_spec = ImageMeants_output_spec
     executable = "fslmeants"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/image_stats.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/image_stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-from fileformats.generic.file import File
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from fileformats.generic import File
+import logging
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
 
+logger = logging.getLogger(__name__)
+
+
 def out_stat_callable(output_dir, inputs, stdout, stderr):
     outputs = _list_outputs(
         output_dir=output_dir, inputs=inputs, stdout=stdout, stderr=stderr
     )
     return outputs["out_stat"]
 
 
@@ -73,16 +76,16 @@
 
 
 class ImageStats(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.image_stats import ImageStats
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.utils.image_stats import ImageStats
 
     >>> task = ImageStats()
     >>> task.inputs.in_file = File.mock(funcfile)
     >>> task.inputs.op_string = "-M"
     >>> task.inputs.mask_file = File.mock()
     >>> task.inputs.index_mask_file = File.mock()
     >>> task.cmdline
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/inv_warp.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/inv_warp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from fileformats.medimage.nifti import Nifti1
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "warp",
         Nifti1,
         {
             "help_string": "Name of file containing warp-coefficients/fields. This would typically be the output from the --cout switch of fnirt (but can also use fields, like the output from --fout).",
@@ -98,16 +102,16 @@
 
 
 class InvWarp(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.inv_warp import InvWarp
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.utils.inv_warp import InvWarp
 
     >>> task = InvWarp()
     >>> task.inputs.warp = Nifti1.mock("struct2mni.nii")
     >>> task.inputs.reference = Nifti1.mock("anatomical.nii")
     >>> task.cmdline
     'invwarp --out=struct2mni_inverse.nii.gz --ref=anatomical.nii --warp=struct2mni.nii'
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/isotropic_smooth.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/isotropic_smooth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "fwhm",
         float,
         {
             "help_string": "fwhm of smoothing kernel [mm]",
             "argstr": "-s {fwhm:.5}",
@@ -86,15 +90,15 @@
 
 
 class IsotropicSmooth(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.isotropic_smooth import IsotropicSmooth
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.maths.isotropic_smooth import IsotropicSmooth
 
     """
 
     input_spec = IsotropicSmooth_input_spec
     output_spec = IsotropicSmooth_output_spec
     executable = "fslmaths"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/l2_model.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/l2_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from fileformats.generic.file import File
-from logging import getLogger
-import attrs
+from fileformats.generic import File
 import logging
 import os
 import pydra.mark
 import typing as ty
 
 
-logger = getLogger(__name__)
+logger = logging.getLogger(__name__)
 
 
 @pydra.mark.task
 @pydra.mark.annotate(
     {"return": {"design_mat": File, "design_con": File, "design_grp": File}}
 )
 def L2Model(num_copes: ty.Any) -> ty.Tuple[File, File, File]:
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.l2_model import L2Model
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.model.l2_model import L2Model
 
     """
     cwd = os.getcwd()
     mat_txt = [
         "/NumWaves   1",
         "/NumPoints  {:d}".format(num_copes),
         "/PPheights  1",
@@ -61,14 +59,15 @@
     txt = {"design.mat": mat_txt, "design.con": con_txt, "design.grp": grp_txt}
 
     # write design files
     for i, name in enumerate(["design.mat", "design.con", "design.grp"]):
         f = open(os.path.join(cwd, name), "wt")
         f.write(txt[name])
         f.close()
+
     outputs = _outputs().get()
     for field in list(outputs.keys()):
         outputs[field] = os.path.join(os.getcwd(), field.replace("_", "."))
 
     return design_mat, design_con, design_grp
 
 
@@ -78,13 +77,7 @@
 def _outputs():
     """Returns a bunch containing output fields for the class"""
     outputs = None
     if self.output_spec:
         outputs = {}
 
     return outputs
-
-
-# Functions defined locally in the original module
-
-
-# Functions defined in neighbouring modules that have been included inline instead of imported
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/level_1_design.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/level_1_design.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-from fileformats.generic.file import File
-from logging import getLogger
-from nibabel import load
-from pkg_resources import resource_filename as pkgrf
-from pydra.engine.specs import MultiOutputType
-from string import Template
 import attrs
+from fileformats.generic import File
 import logging
+from nibabel import load
 import numpy as np
 import os
+from pydra.engine.specs import MultiOutputType
 import pydra.mark
+from string import Template
 import typing as ty
 
 
-logger = getLogger(__name__)
+logger = logging.getLogger(__name__)
 
 
 @pydra.mark.task
 @pydra.mark.annotate(
     {
         "return": {
             "fsf_files": ty.List[File],
@@ -32,17 +30,17 @@
     model_serial_correlations: bool,
     contrasts: list,
 ) -> ty.Tuple[ty.List[File], ty.Union[list, object, MultiOutputType]]:
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
+    >>> from fileformats.generic import File
     >>> from pydra.engine.specs import MultiOutputType
-    >>> from pydra.tasks.fsl.auto.level_1_design import Level1Design
+    >>> from pydra.tasks.fsl.auto.model.level_1_design import Level1Design
 
     """
     cwd = os.getcwd()
     fsf_header = load_template("feat_header_l1.tcl")
     fsf_postscript = load_template("feat_nongui.tcl")
 
     prewhiten = 0
@@ -92,14 +90,15 @@
         )
         fsf_txt += cond_txt
         fsf_txt += fsf_postscript.substitute(overwrite=1)
 
         f = open(os.path.join(cwd, "run%d.fsf" % i), "w")
         f.write(fsf_txt)
         f.close()
+
     outputs = {}
     cwd = os.getcwd()
     fsf_files = []
     ev_files = []
     basis_key = list(bases.keys())[0]
     ev_parameters = dict(bases[basis_key])
     for runno, runinfo in enumerate(_format_session_info(session_info)):
@@ -333,18 +332,14 @@
     """Returns functional files in the order of runs"""
     func_files = []
     for i, info in enumerate(session_info):
         func_files.insert(i, info["scans"])
     return func_files
 
 
-# Functions defined locally in the original module
-
-
-# Original source at L2550 of <nipype-install>/interfaces/fsl/model.py
 def load_template(name):
     """Load a template from the model_templates directory
 
     Parameters
     ----------
     name : str
         The name of the file to load
@@ -357,12 +352,8 @@
     from pkg_resources import resource_filename as pkgrf
 
     full_fname = pkgrf(
         "nipype", os.path.join("interfaces", "fsl", "model_templates", name)
     )
     with open(full_fname) as template_file:
         template = Template(template_file.read())
-
     return template
-
-
-# Functions defined in neighbouring modules that have been included inline instead of imported
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/make_dyadic_vectors.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/make_dyadic_vectors.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-from fileformats.generic.file import File
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from fileformats.generic import File
+import logging
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "theta_vol",
         File,
         {"help_string": "", "argstr": "{theta_vol}", "mandatory": True, "position": 0},
     ),
@@ -36,15 +40,15 @@
 
 
 class MakeDyadicVectors(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.make_dyadic_vectors import MakeDyadicVectors
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.dti.make_dyadic_vectors import MakeDyadicVectors
 
     """
 
     input_spec = MakeDyadicVectors_input_spec
     output_spec = MakeDyadicVectors_output_spec
     executable = "make_dyadic_vectors"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/maths_command.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/maths_command.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         File,
         {
             "help_string": "image to operate on",
             "argstr": "{in_file}",
@@ -64,15 +68,15 @@
 
 
 class MathsCommand(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.maths_command import MathsCommand
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.maths.maths_command import MathsCommand
 
     """
 
     input_spec = MathsCommand_input_spec
     output_spec = MathsCommand_output_spec
     executable = "fslmaths"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/max_image.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/max_image.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.medimage.nifti import Nifti1
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "dimension",
         ty.Any,
         "T",
         {
             "help_string": "dimension to max across",
@@ -74,16 +78,16 @@
 
 
 class MaxImage(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.max_image import MaxImage
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.maths.max_image import MaxImage
 
     >>> task = MaxImage()
     >>> task.inputs.in_file = Nifti1.mock("functional.nii"  # doctest: +SKIP)
     >>> task.cmdline
     'fslmaths functional.nii -Tmax functional_max.nii'
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/maxn_image.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/min_image.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "dimension",
         ty.Any,
         "T",
         {
-            "help_string": "dimension to index max across",
-            "argstr": "-{dimension}maxn",
+            "help_string": "dimension to min across",
+            "argstr": "-{dimension}min",
             "position": 4,
         },
     ),
     (
         "in_file",
         File,
         {
@@ -59,30 +63,30 @@
         {
             "help_string": "change NaNs to zeros before doing anything",
             "argstr": "-nan",
             "position": 3,
         },
     ),
 ]
-MaxnImage_input_spec = specs.SpecInfo(
+MinImage_input_spec = specs.SpecInfo(
     name="Input", fields=input_fields, bases=(specs.ShellSpec,)
 )
 
 output_fields = []
-MaxnImage_output_spec = specs.SpecInfo(
+MinImage_output_spec = specs.SpecInfo(
     name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
 )
 
 
-class MaxnImage(ShellCommandTask):
+class MinImage(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.maxn_image import MaxnImage
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.maths.min_image import MinImage
 
     """
 
-    input_spec = MaxnImage_input_spec
-    output_spec = MaxnImage_output_spec
+    input_spec = MinImage_input_spec
+    output_spec = MinImage_output_spec
     executable = "fslmaths"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/mcflirt.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/mcflirt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         Nifti1,
         {
             "help_string": "timeseries to motion-correct",
             "argstr": "-in {in_file}",
@@ -159,17 +163,17 @@
 
 
 class MCFLIRT(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.mcflirt import MCFLIRT
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.preprocess.mcflirt import MCFLIRT
 
     >>> task = MCFLIRT()
     >>> task.inputs.in_file = Nifti1.mock("functional.nii")
     >>> task.inputs.out_file = "moco.nii"
     >>> task.inputs.cost = "mutualinfo"
     >>> task.inputs.init = File.mock()
     >>> task.inputs.ref_file = File.mock()
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/mean_image.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/std_image.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "dimension",
         ty.Any,
         "T",
         {
-            "help_string": "dimension to mean across",
-            "argstr": "-{dimension}mean",
+            "help_string": "dimension to standard deviate across",
+            "argstr": "-{dimension}std",
             "position": 4,
         },
     ),
     (
         "in_file",
         File,
         {
@@ -59,30 +63,30 @@
         {
             "help_string": "change NaNs to zeros before doing anything",
             "argstr": "-nan",
             "position": 3,
         },
     ),
 ]
-MeanImage_input_spec = specs.SpecInfo(
+StdImage_input_spec = specs.SpecInfo(
     name="Input", fields=input_fields, bases=(specs.ShellSpec,)
 )
 
 output_fields = []
-MeanImage_output_spec = specs.SpecInfo(
+StdImage_output_spec = specs.SpecInfo(
     name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
 )
 
 
-class MeanImage(ShellCommandTask):
+class StdImage(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.mean_image import MeanImage
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.maths.std_image import StdImage
 
     """
 
-    input_spec = MeanImage_input_spec
-    output_spec = MeanImage_output_spec
+    input_spec = StdImage_input_spec
+    output_spec = StdImage_output_spec
     executable = "fslmaths"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/median_image.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/median_image.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "dimension",
         ty.Any,
         "T",
         {
             "help_string": "dimension to median across",
@@ -74,15 +78,15 @@
 
 
 class MedianImage(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.median_image import MedianImage
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.maths.median_image import MedianImage
 
     """
 
     input_spec = MedianImage_input_spec
     output_spec = MedianImage_output_spec
     executable = "fslmaths"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/melodic.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/melodic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-from fileformats.datascience.data import TextMatrix
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.datascience import TextMatrix
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
 from fileformats.medimage_fsl import Con
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_files",
         ty.List[Nifti1],
         {
             "help_string": "input file names (either single file name or a list)",
             "argstr": "-i {in_files}",
@@ -320,19 +324,19 @@
 
 
 class MELODIC(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.datascience.data import TextMatrix
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
+    >>> from fileformats.datascience import TextMatrix
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
     >>> from fileformats.medimage_fsl import Con
-    >>> from pydra.tasks.fsl.auto.melodic import MELODIC
+    >>> from pydra.tasks.fsl.auto.model.melodic import MELODIC
 
     >>> task = MELODIC()
     >>> task.inputs.in_files = [Nifti1.mock("functional.nii"), Nifti1.mock("functional2.nii"), Nifti1.mock("functional3.nii")]
     >>> task.inputs.out_dir = "groupICA.out"
     >>> task.inputs.mask = File.mock()
     >>> task.inputs.no_bet = True
     >>> task.inputs.bg_threshold = 10
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/merge.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/merge.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.medimage.nifti import Nifti1
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_files",
         ty.List[Nifti1],
         {"help_string": "", "argstr": "{in_files}", "mandatory": True, "position": 2},
     ),
     (
@@ -51,16 +55,16 @@
 
 
 class Merge(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.merge import Merge
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.utils.merge import Merge
 
     >>> task = Merge()
     >>> task.inputs.in_files = [Nifti1.mock("functional2.nii"), Nifti1.mock("functional3.nii")]
     >>> task.inputs.dimension = "t"
     >>> task.inputs.tr = 2.25
     >>> task.cmdline
     'fslmerge -tr functional2_merged.nii.gz functional2.nii functional3.nii 2.25'
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/min_image.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/maxn_image.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "dimension",
         ty.Any,
         "T",
         {
-            "help_string": "dimension to min across",
-            "argstr": "-{dimension}min",
+            "help_string": "dimension to index max across",
+            "argstr": "-{dimension}maxn",
             "position": 4,
         },
     ),
     (
         "in_file",
         File,
         {
@@ -59,30 +63,30 @@
         {
             "help_string": "change NaNs to zeros before doing anything",
             "argstr": "-nan",
             "position": 3,
         },
     ),
 ]
-MinImage_input_spec = specs.SpecInfo(
+MaxnImage_input_spec = specs.SpecInfo(
     name="Input", fields=input_fields, bases=(specs.ShellSpec,)
 )
 
 output_fields = []
-MinImage_output_spec = specs.SpecInfo(
+MaxnImage_output_spec = specs.SpecInfo(
     name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
 )
 
 
-class MinImage(ShellCommandTask):
+class MaxnImage(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.min_image import MinImage
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.maths.maxn_image import MaxnImage
 
     """
 
-    input_spec = MinImage_input_spec
-    output_spec = MinImage_output_spec
+    input_spec = MaxnImage_input_spec
+    output_spec = MaxnImage_output_spec
     executable = "fslmaths"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/motion_outliers.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/motion_outliers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         Nifti1,
         {
             "help_string": "unfiltered 4D image",
             "argstr": "-i {in_file}",
@@ -91,17 +95,17 @@
 
 
 class MotionOutliers(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.motion_outliers import MotionOutliers
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.utils.motion_outliers import MotionOutliers
 
     >>> task = MotionOutliers()
     >>> task.inputs.in_file = Nifti1.mock("epi.nii")
     >>> task.inputs.mask = File.mock()
     >>> task.cmdline
     'fsl_motion_outliers -i epi.nii -o epi_outliers.txt -p epi_metrics.png -s epi_metrics.txt'
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/multi_image_maths.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/multi_image_maths.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.medimage.nifti import Nifti1
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "op_string",
         ty.Any,
         {
             "help_string": "python formatted string of operations to perform",
             "argstr": "{op_string}",
@@ -79,16 +83,16 @@
 
 
 class MultiImageMaths(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.multi_image_maths import MultiImageMaths
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.maths.multi_image_maths import MultiImageMaths
 
     >>> task = MultiImageMaths()
     >>> task.inputs.op_string = "-add %s -mul -1 -div %s"
     >>> task.inputs.operand_files = [Nifti1.mock("functional2.nii"), Nifti1.mock("functional3.nii")]
     >>> task.inputs.in_file = Nifti1.mock("functional.nii")
     >>> task.inputs.out_file = "functional4.nii"
     >>> task.cmdline
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/multiple_regress_design.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/multiple_regress_design.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from fileformats.generic.file import File
-from logging import getLogger
 import attrs
+from fileformats.generic import File
 import logging
 import numpy as np
 import os
 import pydra.mark
 import typing as ty
 
 
-logger = getLogger(__name__)
+logger = logging.getLogger(__name__)
 
 
 @pydra.mark.task
 @pydra.mark.annotate(
     {
         "return": {
             "design_mat": File,
@@ -25,16 +24,16 @@
 def MultipleRegressDesign(
     contrasts: list, regressors: dict, groups: list
 ) -> ty.Tuple[File, File, File, File]:
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.multiple_regress_design import MultipleRegressDesign
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.model.multiple_regress_design import MultipleRegressDesign
 
     """
     cwd = os.getcwd()
     regs = sorted(regressors.keys())
     nwaves = len(regs)
     npoints = len(regressors[regs[0]])
     ntcons = sum([1 for con in contrasts if con[1] == "T"])
@@ -114,14 +113,15 @@
     for key, val in list(txt.items()):
         if ("fts" in key) and (nfcons == 0):
             continue
         filename = key.replace("_", ".")
         f = open(os.path.join(cwd, filename), "wt")
         f.write(val)
         f.close()
+
     outputs = _outputs().get()
     nfcons = sum([1 for con in contrasts if con[1] == "F"])
     for field in list(outputs.keys()):
         if ("fts" in field) and (nfcons == 0):
             continue
         outputs[field] = os.path.join(os.getcwd(), field.replace("_", "."))
 
@@ -134,13 +134,7 @@
 def _outputs():
     """Returns a bunch containing output fields for the class"""
     outputs = None
     if self.output_spec:
         outputs = {}
 
     return outputs
-
-
-# Functions defined locally in the original module
-
-
-# Functions defined in neighbouring modules that have been included inline instead of imported
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/overlay.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/overlay.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "transparency",
         bool,
         True,
         {
             "help_string": "make overlay colors semi-transparent",
@@ -148,15 +152,15 @@
 
 
 class Overlay(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.overlay import Overlay
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.utils.overlay import Overlay
 
     """
 
     input_spec = Overlay_input_spec
     output_spec = Overlay_output_spec
     executable = "overlay"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/percentile_image.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/apply_mask.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,46 @@
-from fileformats.medimage.nifti import Nifti1
+from fileformats.medimage import Mask, NiftiGz
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
-        "dimension",
-        ty.Any,
-        "T",
+        "mask_file",
+        NiftiGz[Mask],
         {
-            "help_string": "dimension to percentile across",
-            "argstr": "-{dimension}perc",
+            "help_string": "binary image defining mask space",
+            "argstr": "-mas {mask_file}",
+            "mandatory": True,
             "position": 4,
         },
     ),
     (
-        "perc",
-        ty.Any,
-        {
-            "help_string": "nth percentile (0-100) of FULL RANGE across dimension",
-            "argstr": "{perc}",
-            "position": 5,
-        },
-    ),
-    (
         "in_file",
-        Nifti1,
+        NiftiGz,
         {
             "help_string": "image to operate on",
             "argstr": "{in_file}",
             "mandatory": True,
             "position": 2,
         },
     ),
     (
         "out_file",
         Path,
         {
             "help_string": "image to write",
             "argstr": "{out_file}",
             "position": -2,
-            "output_file_template": "out_file",
+            "output_file_template": "out_file.nii.gz",
         },
     ),
     (
         "internal_datatype",
         ty.Any,
         {
             "help_string": "datatype to use for calculations (default is float)",
@@ -68,36 +63,30 @@
         {
             "help_string": "change NaNs to zeros before doing anything",
             "argstr": "-nan",
             "position": 3,
         },
     ),
 ]
-PercentileImage_input_spec = specs.SpecInfo(
+ApplyMask_input_spec = specs.SpecInfo(
     name="Input", fields=input_fields, bases=(specs.ShellSpec,)
 )
 
 output_fields = []
-PercentileImage_output_spec = specs.SpecInfo(
+ApplyMask_output_spec = specs.SpecInfo(
     name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
 )
 
 
-class PercentileImage(ShellCommandTask):
+class ApplyMask(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.percentile_image import PercentileImage
-
-    >>> task = PercentileImage()
-    >>> task.inputs.in_file = Nifti1.mock("functional.nii"  # doctest: +SKIP)
-    >>> task.cmdline
-    'fslmaths functional.nii -Tperc 90 functional_perc.nii'
-
+    >>> from fileformats.medimage import Mask, NiftiGz
+    >>> from pydra.tasks.fsl.auto.maths.apply_mask import ApplyMask
 
     """
 
-    input_spec = PercentileImage_input_spec
-    output_spec = PercentileImage_output_spec
+    input_spec = ApplyMask_input_spec
+    output_spec = ApplyMask_output_spec
     executable = "fslmaths"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/plot_motion_params.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/plot_motion_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         ty.Any,
         {
             "help_string": "file with motion parameters",
             "argstr": "{in_file}",
@@ -57,14 +61,14 @@
 
 
 class PlotMotionParams(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from pydra.tasks.fsl.auto.plot_motion_params import PlotMotionParams
+    >>> from pydra.tasks.fsl.auto.utils.plot_motion_params import PlotMotionParams
 
     """
 
     input_spec = PlotMotionParams_input_spec
     output_spec = PlotMotionParams_output_spec
     executable = "fsl_tsplot"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/plot_time_series.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/plot_time_series.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         ty.Any,
         {
             "help_string": "file or list of files with columns of timecourse information",
             "argstr": "{in_file}",
@@ -128,15 +132,15 @@
 
 
 class PlotTimeSeries(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.plot_time_series import PlotTimeSeries
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.utils.plot_time_series import PlotTimeSeries
 
     """
 
     input_spec = PlotTimeSeries_input_spec
     output_spec = PlotTimeSeries_output_spec
     executable = "fsl_tsplot"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/power_spectrum.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/split.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,59 @@
-from fileformats.generic.file import File
-from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from fileformats.generic import File
+import logging
+from pydra.engine import ShellCommandTask, specs
+import typing as ty
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "in_file",
         File,
         {
-            "help_string": "input 4D file to estimate the power spectrum",
+            "help_string": "input filename",
             "argstr": "{in_file}",
             "mandatory": True,
             "position": 0,
         },
     ),
     (
-        "out_file",
-        Path,
+        "out_base_name",
+        str,
+        {"help_string": "outputs prefix", "argstr": "{out_base_name}", "position": 1},
+    ),
+    (
+        "dimension",
+        ty.Any,
         {
-            "help_string": "name of output 4D file for power spectrum",
-            "argstr": "{out_file}",
-            "position": 1,
-            "output_file_template": "out_file",
+            "help_string": "dimension along which the file will be split",
+            "argstr": "-{dimension}",
+            "mandatory": True,
+            "position": 2,
         },
     ),
 ]
-PowerSpectrum_input_spec = specs.SpecInfo(
+Split_input_spec = specs.SpecInfo(
     name="Input", fields=input_fields, bases=(specs.ShellSpec,)
 )
 
-output_fields = []
-PowerSpectrum_output_spec = specs.SpecInfo(
+output_fields = [("out_files", ty.List[File], {})]
+Split_output_spec = specs.SpecInfo(
     name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
 )
 
 
-class PowerSpectrum(ShellCommandTask):
+class Split(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.power_spectrum import PowerSpectrum
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.utils.split import Split
 
     """
 
-    input_spec = PowerSpectrum_input_spec
-    output_spec = PowerSpectrum_output_spec
-    executable = "fslpspec"
+    input_spec = Split_input_spec
+    output_spec = Split_output_spec
+    executable = "fslsplit"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/prelude.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/prelude.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "complex_phase_file",
         File,
         {
             "help_string": "complex phase input volume",
@@ -153,15 +157,15 @@
 
 
 class PRELUDE(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.prelude import PRELUDE
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.preprocess.prelude import PRELUDE
 
     """
 
     input_spec = PRELUDE_input_spec
     output_spec = PRELUDE_output_spec
     executable = "prelude"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/prepare_fieldmap.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/prepare_fieldmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "scanner",
         ty.Any,
         "SIEMENS",
         {"help_string": "must be SIEMENS", "argstr": "{scanner}", "position": 1},
     ),
@@ -75,17 +79,17 @@
 
 
 class PrepareFieldmap(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.prepare_fieldmap import PrepareFieldmap
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.epi.prepare_fieldmap import PrepareFieldmap
 
     >>> task = PrepareFieldmap()
     >>> task.inputs.in_phase = Nifti1.mock("phase.nii")
     >>> task.inputs.in_magnitude = Nifti1.mock("magnitude.nii")
     >>> task.cmdline
     'fsl_prepare_fieldmap SIEMENS phase.nii magnitude.nii .../phase_fslprepared.nii.gz 2.460000'
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/prob_track_x.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/prob_track_x.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-from fileformats.datascience.data import TextMatrix
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.datascience import TextMatrix
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "mode",
         ty.Any,
         {
             "help_string": "options: simple (single seed voxel), seedmask (mask of seed voxels), twomask_symm (two bet binary masks)",
             "argstr": "--mode={mode}",
@@ -301,18 +305,18 @@
 
 
 class ProbTrackX(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.datascience.data import TextMatrix
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.prob_track_x import ProbTrackX
+    >>> from fileformats.datascience import TextMatrix
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.dti.prob_track_x import ProbTrackX
 
     >>> task = ProbTrackX()
     >>> task.inputs.mode = "seedmask"
     >>> task.inputs.mask2 = File.mock()
     >>> task.inputs.mesh = File.mock()
     >>> task.inputs.thsamples = [Nifti1.mock("m"), Nifti1.mock("e"), Nifti1.mock("r"), Nifti1.mock("g"), Nifti1.mock("e"), Nifti1.mock("d"), Nifti1.mock("_"), Nifti1.mock("t"), Nifti1.mock("h"), Nifti1.mock("s"), Nifti1.mock("a"), Nifti1.mock("m"), Nifti1.mock("p"), Nifti1.mock("l"), Nifti1.mock("e"), Nifti1.mock("s"), Nifti1.mock("."), Nifti1.mock("n"), Nifti1.mock("i"), Nifti1.mock("i")]
     >>> task.inputs.phsamples = [Nifti1.mock("m"), Nifti1.mock("e"), Nifti1.mock("r"), Nifti1.mock("g"), Nifti1.mock("e"), Nifti1.mock("d"), Nifti1.mock("_"), Nifti1.mock("p"), Nifti1.mock("h"), Nifti1.mock("s"), Nifti1.mock("a"), Nifti1.mock("m"), Nifti1.mock("p"), Nifti1.mock("l"), Nifti1.mock("e"), Nifti1.mock("s"), Nifti1.mock("."), Nifti1.mock("n"), Nifti1.mock("i"), Nifti1.mock("i")]
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/prob_track_x2.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/prob_track_x2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import NiftiGz
+from fileformats.generic import File
+from fileformats.medimage import NiftiGz
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "simple",
         bool,
         {
             "help_string": "rack from a list of voxels (seed must be a ASCII list of coordinates)",
             "argstr": "--simple",
@@ -428,17 +432,17 @@
 
 
 class ProbTrackX2(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import NiftiGz
-    >>> from pydra.tasks.fsl.auto.prob_track_x2 import ProbTrackX2
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import NiftiGz
+    >>> from pydra.tasks.fsl.auto.dti.prob_track_x2 import ProbTrackX2
 
     >>> task = ProbTrackX2()
     >>> task.inputs.fopd = File.mock()
     >>> task.inputs.target2 = File.mock()
     >>> task.inputs.target3 = File.mock()
     >>> task.inputs.lrtarget3 = File.mock()
     >>> task.inputs.colmask4 = File.mock()
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/proj_thresh.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/proj_thresh.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-from fileformats.generic.file import File
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from fileformats.generic import File
+import logging
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_files",
         ty.List[File],
         {
             "help_string": "a list of input volumes",
             "argstr": "{in_files}",
@@ -42,16 +46,16 @@
 
 
 class ProjThresh(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.proj_thresh import ProjThresh
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.dti.proj_thresh import ProjThresh
 
     >>> task = ProjThresh()
     >>> task.inputs.in_files = ldir
     >>> task.inputs.threshold = 3
     >>> task.cmdline
     'proj_thresh seeds_to_M1.nii seeds_to_M2.nii 3'
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/randomise.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/randomise.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-from fileformats.datascience.data import TextMatrix
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.datascience import TextMatrix
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
 from fileformats.medimage_fsl import Con
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+import logging
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         Nifti1,
         {
             "help_string": "4D input file",
             "argstr": "-i {in_file}",
@@ -234,19 +238,19 @@
 
 
 class Randomise(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.datascience.data import TextMatrix
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
+    >>> from fileformats.datascience import TextMatrix
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
     >>> from fileformats.medimage_fsl import Con
-    >>> from pydra.tasks.fsl.auto.randomise import Randomise
+    >>> from pydra.tasks.fsl.auto.model.randomise import Randomise
 
     >>> task = Randomise()
     >>> task.inputs.in_file = Nifti1.mock("allFA.nii")
     >>> task.inputs.design_mat = TextMatrix.mock("design.mat")
     >>> task.inputs.tcon = Con.mock("design.con")
     >>> task.inputs.fcon = File.mock()
     >>> task.inputs.mask = Nifti1.mock("mask.nii")
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/reorient_2_std.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/reorient_2_std.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     ("in_file", File, {"help_string": "", "argstr": "{in_file}", "mandatory": True}),
     (
         "out_file",
         Path,
         {"help_string": "", "argstr": "{out_file}", "output_file_template": "out_file"},
@@ -22,15 +26,15 @@
 
 
 class Reorient2Std(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.reorient_2_std import Reorient2Std
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.utils.reorient_2_std import Reorient2Std
 
     """
 
     input_spec = Reorient2Std_input_spec
     output_spec = Reorient2Std_output_spec
     executable = "fslreorient2std"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/robust_fov.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/robust_fov.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "in_file",
         File,
         {
             "help_string": "input filename",
@@ -52,15 +56,15 @@
 
 
 class RobustFOV(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.robust_fov import RobustFOV
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.utils.robust_fov import RobustFOV
 
     """
 
     input_spec = RobustFOV_input_spec
     output_spec = RobustFOV_output_spec
     executable = "robustfov"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/sig_loss.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/sig_loss.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         File,
         {
             "help_string": "b0 fieldmap file",
             "argstr": "-i {in_file}",
@@ -46,15 +50,15 @@
 
 
 class SigLoss(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.sig_loss import SigLoss
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.utils.sig_loss import SigLoss
 
     """
 
     input_spec = SigLoss_input_spec
     output_spec = SigLoss_output_spec
     executable = "sigloss"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/slice.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/feat.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,43 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
-import typing as ty
+from fileformats.generic import Directory, File
+import logging
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
-        "in_file",
-        Nifti1,
+        "fsf_file",
+        File,
         {
-            "help_string": "input filename",
-            "argstr": "{in_file}",
-            "copyfile": False,
+            "help_string": "File specifying the feat design spec file",
+            "argstr": "{fsf_file}",
             "mandatory": True,
             "position": 0,
         },
-    ),
-    (
-        "out_base_name",
-        str,
-        {"help_string": "outputs prefix", "argstr": "{out_base_name}", "position": 1},
-    ),
+    )
 ]
-Slice_input_spec = specs.SpecInfo(
+FEAT_input_spec = specs.SpecInfo(
     name="Input", fields=input_fields, bases=(specs.ShellSpec,)
 )
 
-output_fields = [("out_files", ty.List[File], {})]
-Slice_output_spec = specs.SpecInfo(
+output_fields = [("feat_dir", Directory, {})]
+FEAT_output_spec = specs.SpecInfo(
     name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
 )
 
 
-class Slice(ShellCommandTask):
+class FEAT(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.slice import Slice
-
-    >>> task = Slice()
-    >>> task.inputs.in_file = Nifti1.mock("functional.nii")
-    >>> task.inputs.out_base_name = "sl"
-    >>> task.cmdline
-    'fslslice functional.nii sl'
-
+    >>> from fileformats.generic import Directory, File
+    >>> from pydra.tasks.fsl.auto.model.feat import FEAT
 
     """
 
-    input_spec = Slice_input_spec
-    output_spec = Slice_output_spec
-    executable = "fslslice"
+    input_spec = FEAT_input_spec
+    output_spec = FEAT_output_spec
+    executable = "feat"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/slice_timer.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/slice_timer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         File,
         {
             "help_string": "filename of input timeseries",
             "argstr": "--in={in_file}",
@@ -84,15 +88,15 @@
 
 
 class SliceTimer(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.slice_timer import SliceTimer
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.preprocess.slice_timer import SliceTimer
 
     """
 
     input_spec = SliceTimer_input_spec
     output_spec = SliceTimer_output_spec
     executable = "slicetimer"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/slicer.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/slicer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         File,
         {
             "help_string": "input volume",
             "argstr": "{in_file}",
@@ -169,15 +173,15 @@
 
 
 class Slicer(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.slicer import Slicer
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.utils.slicer import Slicer
 
     """
 
     input_spec = Slicer_input_spec
     output_spec = Slicer_output_spec
     executable = "slicer"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/smm.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/ar1_image.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,92 @@
-from fileformats.generic.file import File
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from fileformats.generic import File
+import logging
+from pathlib import Path
+from pydra.engine import ShellCommandTask, specs
+import typing as ty
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
-        "spatial_data_file",
-        File,
+        "dimension",
+        ty.Any,
+        "T",
         {
-            "help_string": "statistics spatial map",
-            "argstr": '--sdf="{spatial_data_file}"',
-            "copyfile": False,
-            "mandatory": True,
-            "position": 0,
+            "help_string": "dimension to find AR(1) coefficientacross",
+            "argstr": "-{dimension}ar1",
+            "position": 4,
         },
     ),
     (
-        "mask",
+        "in_file",
         File,
         {
-            "help_string": "mask file",
-            "argstr": '--mask="{mask}"',
-            "copyfile": False,
+            "help_string": "image to operate on",
+            "argstr": "{in_file}",
             "mandatory": True,
+            "position": 2,
+        },
+    ),
+    (
+        "out_file",
+        Path,
+        {
+            "help_string": "image to write",
+            "argstr": "{out_file}",
+            "position": -2,
+            "output_file_template": "out_file",
+        },
+    ),
+    (
+        "internal_datatype",
+        ty.Any,
+        {
+            "help_string": "datatype to use for calculations (default is float)",
+            "argstr": "-dt {internal_datatype}",
             "position": 1,
         },
     ),
     (
-        "no_deactivation_class",
+        "output_datatype",
+        ty.Any,
+        {
+            "help_string": "datatype to use for output (default uses input type)",
+            "argstr": "-odt {output_datatype}",
+            "position": -1,
+        },
+    ),
+    (
+        "nan2zeros",
         bool,
         {
-            "help_string": "enforces no deactivation class",
-            "argstr": "--zfstatmode",
-            "position": 2,
+            "help_string": "change NaNs to zeros before doing anything",
+            "argstr": "-nan",
+            "position": 3,
         },
     ),
 ]
-SMM_input_spec = specs.SpecInfo(
+AR1Image_input_spec = specs.SpecInfo(
     name="Input", fields=input_fields, bases=(specs.ShellSpec,)
 )
 
-output_fields = [
-    ("null_p_map", File, {}),
-    ("activation_p_map", File, {}),
-    ("deactivation_p_map", File, {}),
-]
-SMM_output_spec = specs.SpecInfo(
+output_fields = []
+AR1Image_output_spec = specs.SpecInfo(
     name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
 )
 
 
-class SMM(ShellCommandTask):
+class AR1Image(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.smm import SMM
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.maths.ar1_image import AR1Image
 
     """
 
-    input_spec = SMM_input_spec
-    output_spec = SMM_output_spec
-    executable = "mm --ld=logdir"
+    input_spec = AR1Image_input_spec
+    output_spec = AR1Image_output_spec
+    executable = "fslmaths"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/smooth.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/smooth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from fileformats.medimage.nifti import Nifti1
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "in_file",
         Nifti1,
         {"help_string": "", "argstr": "{in_file}", "mandatory": True, "position": 0},
     ),
@@ -53,16 +57,16 @@
 
 
 class Smooth(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.smooth import Smooth
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.utils.smooth import Smooth
 
     >>> task = Smooth()
     >>> task.inputs.in_file = Nifti1.mock("functional2.nii")
     >>> task.inputs.sigma = 8.0
     >>> task.cmdline
     'fslmaths functional2.nii -kernel gauss 8.000 -fmean functional2_smooth.nii.gz'
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/smooth_estimate.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/smooth_estimate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
-from fileformats.medimage.nifti import NiftiGz
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from fileformats.generic import File
+from fileformats.medimage import Nifti1, NiftiGz
+import logging
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
 
 
 def dlh_callable(output_dir, inputs, stdout, stderr):
     outputs = _list_outputs(
         output_dir=output_dir, inputs=inputs, stdout=stdout, stderr=stderr
     )
     return outputs["dlh"]
@@ -98,18 +100,17 @@
 
 
 class SmoothEstimate(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from fileformats.medimage.nifti import NiftiGz
-    >>> from pydra.tasks.fsl.auto.smooth_estimate import SmoothEstimate
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1, NiftiGz
+    >>> from pydra.tasks.fsl.auto.model.smooth_estimate import SmoothEstimate
 
     >>> task = SmoothEstimate()
     >>> task.inputs.mask_file = Nifti1.mock("mask.nii")
     >>> task.inputs.residual_fit_file = File.mock()
     >>> task.inputs.zstat_file = NiftiGz.mock("zstat1.nii.gz")
     >>> task.cmdline
     'smoothest --mask=mask.nii --zstat=zstat1.nii.gz'
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/spatial_filter.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/spatial_filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "operation",
         ty.Any,
         {
             "help_string": "operation to filter with",
             "argstr": "-f{operation}",
@@ -103,15 +107,15 @@
 
 
 class SpatialFilter(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.spatial_filter import SpatialFilter
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.maths.spatial_filter import SpatialFilter
 
     """
 
     input_spec = SpatialFilter_input_spec
     output_spec = SpatialFilter_output_spec
     executable = "fslmaths"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/split.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/vest_2_text.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,64 @@
-from fileformats.generic.file import File
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
-import typing as ty
+from fileformats.datascience import TextMatrix
+from fileformats.generic import File
+import logging
+from pathlib import Path
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "in_file",
-        File,
+        TextMatrix,
         {
-            "help_string": "input filename",
+            "help_string": "matrix data stored in the format used by FSL tools",
             "argstr": "{in_file}",
             "mandatory": True,
             "position": 0,
         },
     ),
     (
-        "out_base_name",
-        str,
-        {"help_string": "outputs prefix", "argstr": "{out_base_name}", "position": 1},
-    ),
-    (
-        "dimension",
-        ty.Any,
+        "out_file",
+        Path,
+        "design.txt",
         {
-            "help_string": "dimension along which the file will be split",
-            "argstr": "-{dimension}",
-            "mandatory": True,
-            "position": 2,
+            "help_string": "file name to store text output from matrix",
+            "argstr": "{out_file}",
+            "position": 1,
         },
     ),
 ]
-Split_input_spec = specs.SpecInfo(
+Vest2Text_input_spec = specs.SpecInfo(
     name="Input", fields=input_fields, bases=(specs.ShellSpec,)
 )
 
-output_fields = [("out_files", ty.List[File], {})]
-Split_output_spec = specs.SpecInfo(
+output_fields = [
+    ("out_file", File, {"help_string": "plain text representation of FSL matrix"})
+]
+Vest2Text_output_spec = specs.SpecInfo(
     name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
 )
 
 
-class Split(ShellCommandTask):
+class Vest2Text(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.split import Split
+    >>> from fileformats.datascience import TextMatrix
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.utils.vest_2_text import Vest2Text
+
+    >>> task = Vest2Text()
+    >>> task.inputs.in_file = TextMatrix.mock("design.mat")
+    >>> task.cmdline
+    'Vest2Text design.mat design.txt'
+
 
     """
 
-    input_spec = Split_input_spec
-    output_spec = Split_output_spec
-    executable = "fslsplit"
+    input_spec = Vest2Text_input_spec
+    output_spec = Vest2Text_output_spec
+    executable = "Vest2Text"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/std_image.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/mean_image.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "dimension",
         ty.Any,
         "T",
         {
-            "help_string": "dimension to standard deviate across",
-            "argstr": "-{dimension}std",
+            "help_string": "dimension to mean across",
+            "argstr": "-{dimension}mean",
             "position": 4,
         },
     ),
     (
         "in_file",
         File,
         {
@@ -59,30 +63,30 @@
         {
             "help_string": "change NaNs to zeros before doing anything",
             "argstr": "-nan",
             "position": 3,
         },
     ),
 ]
-StdImage_input_spec = specs.SpecInfo(
+MeanImage_input_spec = specs.SpecInfo(
     name="Input", fields=input_fields, bases=(specs.ShellSpec,)
 )
 
 output_fields = []
-StdImage_output_spec = specs.SpecInfo(
+MeanImage_output_spec = specs.SpecInfo(
     name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
 )
 
 
-class StdImage(ShellCommandTask):
+class MeanImage(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.std_image import StdImage
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.maths.mean_image import MeanImage
 
     """
 
-    input_spec = StdImage_input_spec
-    output_spec = StdImage_output_spec
+    input_spec = MeanImage_input_spec
+    output_spec = MeanImage_output_spec
     executable = "fslmaths"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/susan.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/susan.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         File,
         {
             "help_string": "filename of input timeseries",
             "argstr": "{in_file}",
@@ -82,15 +86,15 @@
 
 
 class SUSAN(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.susan import SUSAN
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.preprocess.susan import SUSAN
 
     """
 
     input_spec = SUSAN_input_spec
     output_spec = SUSAN_output_spec
     executable = "susan"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/swap_dimensions.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/swap_dimensions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         File,
         {
             "help_string": "input image",
             "argstr": "{in_file}",
@@ -45,15 +49,15 @@
 
 
 class SwapDimensions(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.swap_dimensions import SwapDimensions
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.utils.swap_dimensions import SwapDimensions
 
     """
 
     input_spec = SwapDimensions_input_spec
     output_spec = SwapDimensions_output_spec
     executable = "fslswapdim"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/temporal_filter.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/temporal_filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "lowpass_sigma",
         float,
         -1,
         {
             "help_string": "lowpass filter sigma (in volumes)",
@@ -84,15 +88,15 @@
 
 
 class TemporalFilter(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.temporal_filter import TemporalFilter
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.maths.temporal_filter import TemporalFilter
 
     """
 
     input_spec = TemporalFilter_input_spec
     output_spec = TemporalFilter_output_spec
     executable = "fslmaths"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/text_2_vest.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/text_2_vest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-from fileformats.datascience.data import TextMatrix
+from fileformats.datascience import TextMatrix
 from fileformats.text import TextFile
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "in_file",
         TextFile,
         {
             "help_string": "plain text file representing your design, contrast, or f-test matrix",
@@ -43,17 +47,17 @@
 
 
 class Text2Vest(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.datascience.data import TextMatrix
+    >>> from fileformats.datascience import TextMatrix
     >>> from fileformats.text import TextFile
-    >>> from pydra.tasks.fsl.auto.text_2_vest import Text2Vest
+    >>> from pydra.tasks.fsl.auto.utils.text_2_vest import Text2Vest
 
     >>> task = Text2Vest()
     >>> task.inputs.in_file = TextFile.mock("design.txt")
     >>> task.inputs.out_file = "design.mat"
     >>> task.cmdline
     'Text2Vest design.txt design.mat'
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/threshold.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/threshold.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "thresh",
         float,
         {
             "help_string": "threshold value",
             "argstr": "{thresh}",
@@ -93,15 +97,15 @@
 
 
 class Threshold(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.threshold import Threshold
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.maths.threshold import Threshold
 
     """
 
     input_spec = Threshold_input_spec
     output_spec = Threshold_output_spec
     executable = "fslmaths"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/topup.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/topup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
 from fileformats.text import TextFile
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         Nifti1,
         {
             "help_string": "name of 4D file with images",
             "argstr": "--imain={in_file}",
@@ -247,18 +251,18 @@
 
 
 class TOPUP(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
     >>> from fileformats.text import TextFile
-    >>> from pydra.tasks.fsl.auto.topup import TOPUP
+    >>> from pydra.tasks.fsl.auto.epi.topup import TOPUP
 
     >>> task = TOPUP()
     >>> task.inputs.in_file = Nifti1.mock("b0_b0rev.nii")
     >>> task.inputs.encoding_file = TextFile.mock("topup_encoding.txt")
     >>> task.cmdline
     'topup --config=b02b0.cnf --datain=topup_encoding.txt --imain=b0_b0rev.nii --out=b0_b0rev_base --iout=b0_b0rev_corrected.nii.gz --fout=b0_b0rev_field.nii.gz --jacout=jac --logout=b0_b0rev_topup.log --rbmout=xfm --dfout=warpfield'
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tract_skeleton.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tract_skeleton.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         File,
         {
             "help_string": "input image (typically mean FA volume)",
             "argstr": "-i {in_file}",
@@ -81,15 +85,15 @@
 
 
 class TractSkeleton(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.tract_skeleton import TractSkeleton
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.dti.tract_skeleton import TractSkeleton
 
     """
 
     input_spec = TractSkeleton_input_spec
     output_spec = TractSkeleton_output_spec
     executable = "tbss_skeleton"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/training.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/training.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-from fileformats.generic.file import File
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from fileformats.generic import File
+import logging
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "mel_icas",
         ty.List[File],
         {
             "help_string": "Melodic output directories",
             "argstr": "{mel_icas}",
@@ -44,15 +48,15 @@
 
 
 class Training(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.training import Training
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.fix.training import Training
 
     """
 
     input_spec = Training_input_spec
     output_spec = Training_output_spec
     executable = "fix -t"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/training_set_creator.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/training_set_creator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-from fileformats.generic.directory import Directory
-from logging import getLogger
-import attrs
+from fileformats.generic import Directory
 import logging
 import os
 import pydra.mark
 import typing as ty
 
 
-logger = getLogger(__name__)
+logger = logging.getLogger(__name__)
 
 
 @pydra.mark.task
 @pydra.mark.annotate({"return": {"mel_icas_out": ty.List[Directory]}})
 def TrainingSetCreator(mel_icas_in: ty.List[Directory]) -> ty.List[Directory]:
     """
     Examples
     -------
 
-    >>> from fileformats.generic.directory import Directory
-    >>> from pydra.tasks.fsl.auto.training_set_creator import TrainingSetCreator
+    >>> from fileformats.generic import Directory
+    >>> from pydra.tasks.fsl.auto.fix.training_set_creator import TrainingSetCreator
 
     """
     mel_icas = []
     for item in mel_icas_in:
         if os.path.exists(os.path.join(item, "hand_labels_noise.txt")):
             mel_icas.append(item)
 
     if len(mel_icas) == 0:
         raise Exception(
             "%s did not find any hand_labels_noise.txt files in the following directories: %s"
             % (self.__class__.__name__, mel_icas)
         )
+
     mel_icas = []
     for item in mel_icas_in:
         if os.path.exists(os.path.join(item, "hand_labels_noise.txt")):
             mel_icas.append(item)
     outputs = _outputs().get()
     mel_icas_out = mel_icas
 
@@ -47,13 +46,7 @@
 def _outputs():
     """Returns a bunch containing output fields for the class"""
     outputs = None
     if self.output_spec:
         outputs = {}
 
     return outputs
-
-
-# Functions defined locally in the original module
-
-
-# Functions defined in neighbouring modules that have been included inline instead of imported
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/unary_maths.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/change_data_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
-        "operation",
+        "output_datatype",
         ty.Any,
         {
-            "help_string": "operation to perform",
-            "argstr": "-{operation}",
+            "help_string": "output data type",
+            "argstr": "-odt {output_datatype}",
             "mandatory": True,
-            "position": 4,
+            "position": -1,
         },
     ),
     (
         "in_file",
         File,
         {
             "help_string": "image to operate on",
@@ -41,48 +45,39 @@
         {
             "help_string": "datatype to use for calculations (default is float)",
             "argstr": "-dt {internal_datatype}",
             "position": 1,
         },
     ),
     (
-        "output_datatype",
-        ty.Any,
-        {
-            "help_string": "datatype to use for output (default uses input type)",
-            "argstr": "-odt {output_datatype}",
-            "position": -1,
-        },
-    ),
-    (
         "nan2zeros",
         bool,
         {
             "help_string": "change NaNs to zeros before doing anything",
             "argstr": "-nan",
             "position": 3,
         },
     ),
 ]
-UnaryMaths_input_spec = specs.SpecInfo(
+ChangeDataType_input_spec = specs.SpecInfo(
     name="Input", fields=input_fields, bases=(specs.ShellSpec,)
 )
 
 output_fields = []
-UnaryMaths_output_spec = specs.SpecInfo(
+ChangeDataType_output_spec = specs.SpecInfo(
     name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
 )
 
 
-class UnaryMaths(ShellCommandTask):
+class ChangeDataType(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.unary_maths import UnaryMaths
+    >>> from fileformats.generic import File
+    >>> from pydra.tasks.fsl.auto.maths.change_data_type import ChangeDataType
 
     """
 
-    input_spec = UnaryMaths_input_spec
-    output_spec = UnaryMaths_output_spec
+    input_spec = ChangeDataType_input_spec
+    output_spec = ChangeDataType_output_spec
     executable = "fslmaths"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/vec_reg.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/vec_reg.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-from fileformats.datascience.data import TextMatrix
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.datascience import TextMatrix
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         Nifti1,
         {
             "help_string": "filename for input vector or tensor field",
             "argstr": "-i {in_file}",
@@ -95,18 +99,18 @@
 
 
 class VecReg(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.datascience.data import TextMatrix
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.vec_reg import VecReg
+    >>> from fileformats.datascience import TextMatrix
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.dti.vec_reg import VecReg
 
     >>> task = VecReg()
     >>> task.inputs.in_file = Nifti1.mock("diffusion.nii")
     >>> task.inputs.out_file = "diffusion_vreg.nii"
     >>> task.inputs.ref_vol = Nifti1.mock("mni.nii")
     >>> task.inputs.affine_mat = TextMatrix.mock("trans.mat")
     >>> task.inputs.warp_field = File.mock()
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/vest_2_text.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/warp_points.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,117 @@
-from fileformats.datascience.data import TextMatrix
-from fileformats.generic.file import File
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+from fileformats.text import TextFile
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
-        "in_file",
-        TextMatrix,
+        "src_file",
+        Nifti1,
+        {
+            "help_string": "filename of source image",
+            "argstr": "-src {src_file}",
+            "mandatory": True,
+        },
+    ),
+    (
+        "dest_file",
+        Nifti1,
         {
-            "help_string": "matrix data stored in the format used by FSL tools",
-            "argstr": "{in_file}",
+            "help_string": "filename of destination image",
+            "argstr": "-dest {dest_file}",
             "mandatory": True,
-            "position": 0,
         },
     ),
     (
+        "in_coords",
+        TextFile,
+        {
+            "help_string": "filename of file containing coordinates",
+            "argstr": "{in_coords}",
+            "mandatory": True,
+            "position": -1,
+        },
+    ),
+    (
+        "xfm_file",
+        File,
+        {
+            "help_string": "filename of affine transform (e.g. source2dest.mat)",
+            "argstr": "-xfm {xfm_file}",
+            "xor": ["warp_file"],
+        },
+    ),
+    (
+        "warp_file",
+        Nifti1,
+        {
+            "help_string": "filename of warpfield (e.g. intermediate2dest_warp.nii.gz)",
+            "argstr": "-warp {warp_file}",
+            "xor": ["xfm_file"],
+        },
+    ),
+    (
+        "coord_vox",
+        bool,
+        {
+            "help_string": "all coordinates in voxels - default",
+            "argstr": "-vox",
+            "xor": ["coord_mm"],
+        },
+    ),
+    (
+        "coord_mm",
+        bool,
+        {"help_string": "all coordinates in mm", "argstr": "-mm", "xor": ["coord_vox"]},
+    ),
+    (
         "out_file",
         Path,
-        "design.txt",
         {
-            "help_string": "file name to store text output from matrix",
-            "argstr": "{out_file}",
-            "position": 1,
+            "help_string": "output file name",
+            "output_file_template": "{in_coords}_warped",
         },
     ),
 ]
-Vest2Text_input_spec = specs.SpecInfo(
+WarpPoints_input_spec = specs.SpecInfo(
     name="Input", fields=input_fields, bases=(specs.ShellSpec,)
 )
 
-output_fields = [
-    ("out_file", File, {"help_string": "plain text representation of FSL matrix"})
-]
-Vest2Text_output_spec = specs.SpecInfo(
+output_fields = []
+WarpPoints_output_spec = specs.SpecInfo(
     name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
 )
 
 
-class Vest2Text(ShellCommandTask):
+class WarpPoints(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.datascience.data import TextMatrix
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.vest_2_text import Vest2Text
-
-    >>> task = Vest2Text()
-    >>> task.inputs.in_file = TextMatrix.mock("design.mat")
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
+    >>> from fileformats.text import TextFile
+    >>> from pydra.tasks.fsl.auto.utils.warp_points import WarpPoints
+
+    >>> task = WarpPoints()
+    >>> task.inputs.src_file = Nifti1.mock("epi.nii")
+    >>> task.inputs.dest_file = Nifti1.mock("T1.nii")
+    >>> task.inputs.in_coords = TextFile.mock("surf.txt")
+    >>> task.inputs.xfm_file = File.mock()
+    >>> task.inputs.warp_file = Nifti1.mock("warpfield.nii")
+    >>> task.inputs.coord_mm = True
     >>> task.cmdline
-    'Vest2Text design.mat design.txt'
+    'img2imgcoord -mm -dest T1.nii -src epi.nii -warp warpfield.nii surf.txt'
 
 
     """
 
-    input_spec = Vest2Text_input_spec
-    output_spec = Vest2Text_output_spec
-    executable = "Vest2Text"
+    input_spec = WarpPoints_input_spec
+    output_spec = WarpPoints_output_spec
+    executable = "img2imgcoord"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/warp_points.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/warp_points_to_std.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,46 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
 from fileformats.text import TextFile
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
-        "src_file",
+        "img_file",
         Nifti1,
         {
-            "help_string": "filename of source image",
-            "argstr": "-src {src_file}",
+            "help_string": "filename of input image",
+            "argstr": "-img {img_file}",
             "mandatory": True,
         },
     ),
     (
-        "dest_file",
+        "std_file",
         Nifti1,
         {
             "help_string": "filename of destination image",
-            "argstr": "-dest {dest_file}",
+            "argstr": "-std {std_file}",
             "mandatory": True,
         },
     ),
     (
+        "premat_file",
+        File,
+        {
+            "help_string": "filename of pre-warp affine transform (e.g. example_func2highres.mat)",
+            "argstr": "-premat {premat_file}",
+        },
+    ),
+    (
         "in_coords",
         TextFile,
         {
             "help_string": "filename of file containing coordinates",
             "argstr": "{in_coords}",
             "mandatory": True,
             "position": -1,
@@ -71,43 +83,44 @@
         Path,
         {
             "help_string": "output file name",
             "output_file_template": "{in_coords}_warped",
         },
     ),
 ]
-WarpPoints_input_spec = specs.SpecInfo(
+WarpPointsToStd_input_spec = specs.SpecInfo(
     name="Input", fields=input_fields, bases=(specs.ShellSpec,)
 )
 
 output_fields = []
-WarpPoints_output_spec = specs.SpecInfo(
+WarpPointsToStd_output_spec = specs.SpecInfo(
     name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
 )
 
 
-class WarpPoints(ShellCommandTask):
+class WarpPointsToStd(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
     >>> from fileformats.text import TextFile
-    >>> from pydra.tasks.fsl.auto.warp_points import WarpPoints
+    >>> from pydra.tasks.fsl.auto.utils.warp_points_to_std import WarpPointsToStd
 
-    >>> task = WarpPoints()
-    >>> task.inputs.src_file = Nifti1.mock("epi.nii")
-    >>> task.inputs.dest_file = Nifti1.mock("T1.nii")
+    >>> task = WarpPointsToStd()
+    >>> task.inputs.img_file = Nifti1.mock("T1.nii")
+    >>> task.inputs.std_file = Nifti1.mock("mni.nii")
+    >>> task.inputs.premat_file = File.mock()
     >>> task.inputs.in_coords = TextFile.mock("surf.txt")
     >>> task.inputs.xfm_file = File.mock()
     >>> task.inputs.warp_file = Nifti1.mock("warpfield.nii")
     >>> task.inputs.coord_mm = True
     >>> task.cmdline
-    'img2imgcoord -mm -dest T1.nii -src epi.nii -warp warpfield.nii surf.txt'
+    'img2stdcoord -mm -img T1.nii -std mni.nii -warp warpfield.nii surf.txt'
 
 
     """
 
-    input_spec = WarpPoints_input_spec
-    output_spec = WarpPoints_output_spec
-    executable = "img2imgcoord"
+    input_spec = WarpPointsToStd_input_spec
+    output_spec = WarpPointsToStd_output_spec
+    executable = "img2stdcoord"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/warp_points_from_std.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/warp_points_from_std.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
 from fileformats.text import TextFile
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+import logging
+from pydra.engine import ShellCommandTask, specs
+
+
+logger = logging.getLogger(__name__)
+
 
 input_fields = [
     (
         "img_file",
         Nifti1,
         {
             "help_string": "filename of a destination image",
@@ -85,18 +89,18 @@
 
 
 class WarpPointsFromStd(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
     >>> from fileformats.text import TextFile
-    >>> from pydra.tasks.fsl.auto.warp_points_from_std import WarpPointsFromStd
+    >>> from pydra.tasks.fsl.auto.utils.warp_points_from_std import WarpPointsFromStd
 
     >>> task = WarpPointsFromStd()
     >>> task.inputs.img_file = Nifti1.mock("T1.nii")
     >>> task.inputs.std_file = Nifti1.mock("mni.nii")
     >>> task.inputs.in_coords = TextFile.mock("surf.txt")
     >>> task.inputs.xfm_file = File.mock()
     >>> task.inputs.warp_file = Nifti1.mock("warpfield.nii")
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/warp_points_to_std.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/roi.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
-from fileformats.text import TextFile
-from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
-
-input_fields = [
-    (
-        "img_file",
-        Nifti1,
-        {
-            "help_string": "filename of input image",
-            "argstr": "-img {img_file}",
-            "mandatory": True,
-        },
-    ),
-    (
-        "std_file",
-        Nifti1,
-        {
-            "help_string": "filename of destination image",
-            "argstr": "-std {std_file}",
-            "mandatory": True,
-        },
-    ),
-    (
-        "premat_file",
-        File,
-        {
-            "help_string": "filename of pre-warp affine transform (e.g. example_func2highres.mat)",
-            "argstr": "-premat {premat_file}",
-        },
-    ),
-    (
-        "in_coords",
-        TextFile,
-        {
-            "help_string": "filename of file containing coordinates",
-            "argstr": "{in_coords}",
-            "mandatory": True,
-            "position": -1,
-        },
-    ),
-    (
-        "xfm_file",
-        File,
-        {
-            "help_string": "filename of affine transform (e.g. source2dest.mat)",
-            "argstr": "-xfm {xfm_file}",
-            "xor": ["warp_file"],
-        },
-    ),
-    (
-        "warp_file",
-        Nifti1,
-        {
-            "help_string": "filename of warpfield (e.g. intermediate2dest_warp.nii.gz)",
-            "argstr": "-warp {warp_file}",
-            "xor": ["xfm_file"],
-        },
-    ),
-    (
-        "coord_vox",
-        bool,
-        {
-            "help_string": "all coordinates in voxels - default",
-            "argstr": "-vox",
-            "xor": ["coord_mm"],
-        },
-    ),
-    (
-        "coord_mm",
-        bool,
-        {"help_string": "all coordinates in mm", "argstr": "-mm", "xor": ["coord_vox"]},
-    ),
-    (
-        "out_file",
-        Path,
-        {
-            "help_string": "output file name",
-            "output_file_template": "{in_coords}_warped",
-        },
-    ),
-]
-WarpPointsToStd_input_spec = specs.SpecInfo(
-    name="Input", fields=input_fields, bases=(specs.ShellSpec,)
-)
-
-output_fields = []
-WarpPointsToStd_output_spec = specs.SpecInfo(
-    name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
-)
-
-
-class WarpPointsToStd(ShellCommandTask):
-    """
-    Examples
-    -------
-
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from fileformats.text import TextFile
-    >>> from pydra.tasks.fsl.auto.warp_points_to_std import WarpPointsToStd
-
-    >>> task = WarpPointsToStd()
-    >>> task.inputs.img_file = Nifti1.mock("T1.nii")
-    >>> task.inputs.std_file = Nifti1.mock("mni.nii")
-    >>> task.inputs.premat_file = File.mock()
-    >>> task.inputs.in_coords = TextFile.mock("surf.txt")
-    >>> task.inputs.xfm_file = File.mock()
-    >>> task.inputs.warp_file = Nifti1.mock("warpfield.nii")
-    >>> task.inputs.coord_mm = True
-    >>> task.cmdline
-    'img2stdcoord -mm -img T1.nii -std mni.nii -warp warpfield.nii surf.txt'
-
-
-    """
-
-    input_spec = WarpPointsToStd_input_spec
-    output_spec = WarpPointsToStd_output_spec
-    executable = "img2stdcoord"
+"""
+ROI (Region-Of-Interest)
+========================
+
+Manual cropping to a region-of-interest for structural brain images.
+
+Examples
+--------
+
+Extract a 16-voxel cube starting at position (10, 20, 30):
+
+>>> task = ROI(
+...     input_image="image.nii",
+...     x_min=10,
+...     x_size=16,
+...     y_min=20,
+...     y_size=16,
+...     z_min=30,
+...     z_size=16,
+... )
+>>> task.cmdline    # doctest: +ELLIPSIS
+'fslroi image.nii ...image_roi.nii 10 16 20 16 30 16 ...'
+
+Extract a temporal window starting at 5 onwards:
+
+>>> task = ROI(input_image="input.nii", output_image="output.nii", t_min=5)
+>>> task.cmdline
+'fslroi input.nii output.nii 5 -1'
+"""
+
+__all__ = ["ROI"]
+
+from os import PathLike
+
+from attrs import define, field
+from pydra.engine.specs import ShellSpec, SpecInfo
+from pydra.engine.task import ShellCommandTask
+
+
+@define(kw_only=True)
+class ROISpec(ShellSpec):
+    """Specifications for fslroi."""
+
+    _requires = {"x_min", "y_min", "z_min"}
+
+    input_image: PathLike = field(
+        metadata={"help_string": "input image", "mandatory": True, "argstr": ""}
+    )
+
+    output_image: str = field(
+        metadata={
+            "help_string": "output image",
+            "argstr": "",
+            "output_file_template": "{input_image}_roi",
+        }
+    )
+
+    x_min: int = field(
+        metadata={
+            "help_string": "start of ROI in x (0-based indexing)",
+            "argstr": "",
+            "requires": _requires,
+        }
+    )
+
+    x_size: int = field(
+        metadata={
+            "help_string": "size of ROI in x (-1 for maximum)",
+            "argstr": "",
+            "requires": {"x_min"},
+        }
+    )
+
+    y_min: int = field(
+        metadata={
+            "help_string": "start of ROI in y (0-based indexing)",
+            "argstr": "",
+            "requires": _requires,
+        }
+    )
+
+    y_size: int = field(
+        metadata={
+            "help_string": "size of ROI in y (-1 for maximum)",
+            "argstr": "",
+            "requires": {"y_min"},
+        }
+    )
+
+    z_min: int = field(
+        metadata={
+            "help_string": "start of ROI in z (0-based indexing)",
+            "argstr": "",
+            "requires": _requires,
+        }
+    )
+
+    z_size: int = field(
+        metadata={
+            "help_string": "size of ROI in z (-1 for maximum)",
+            "argstr": "",
+            "requires": {"z_min"},
+        }
+    )
+
+    t_min: int = field(
+        default=0,
+        metadata={"help_string": "start of ROI in t (0-based indexing)", "argstr": ""},
+    )
+
+    t_size: int = field(
+        default=-1,
+        metadata={"help_string": "size of ROI in t (-1 for maximum)", "argstr": ""},
+    )
+
+
+class ROI(ShellCommandTask):
+    """Task definition for fslroi."""
+
+    executable = "fslroi"
+
+    input_spec = SpecInfo(name="Input", bases=(ROISpec,))
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/warp_utils.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/warp_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from pathlib import Path
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "in_file",
         Nifti1,
         {
             "help_string": "Name of file containing warp-coefficients/fields. This would typically be the output from the --cout switch of fnirt (but can also use fields, like the output from --fout).",
             "argstr": "--in={in_file}",
@@ -108,17 +112,17 @@
 
 
 class WarpUtils(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.file import File
-    >>> from fileformats.medimage.nifti import Nifti1
-    >>> from pydra.tasks.fsl.auto.warp_utils import WarpUtils
+    >>> from fileformats.generic import File
+    >>> from fileformats.medimage import Nifti1
+    >>> from pydra.tasks.fsl.auto.utils.warp_utils import WarpUtils
 
     >>> task = WarpUtils()
     >>> task.inputs.in_file = Nifti1.mock("warpfield.nii")
     >>> task.inputs.reference = Nifti1.mock("T1.nii")
     >>> task.inputs.out_format = "spline"
     >>> task.inputs.warp_resolution = (10,10,10)
     >>> task.cmdline
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/x_fibres_5.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/x_fibres_5.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-from fileformats.generic.directory import Directory
-from fileformats.generic.file import File
-from pydra.engine import ShellCommandTask
-from pydra.engine import specs
+from fileformats.generic import Directory, File
+import logging
+from pydra.engine import ShellCommandTask, specs
 import typing as ty
 
+
+logger = logging.getLogger(__name__)
+
+
 input_fields = [
     (
         "gradnonlin",
         File,
         {
             "help_string": "gradient file corresponding to slice",
             "argstr": "--gradnonlin={gradnonlin}",
@@ -239,16 +242,15 @@
 
 
 class XFibres5(ShellCommandTask):
     """
     Examples
     -------
 
-    >>> from fileformats.generic.directory import Directory
-    >>> from fileformats.generic.file import File
-    >>> from pydra.tasks.fsl.auto.x_fibres_5 import XFibres5
+    >>> from fileformats.generic import Directory, File
+    >>> from pydra.tasks.fsl.auto.dti.x_fibres_5 import XFibres5
 
     """
 
     input_spec = XFibres5_input_spec
     output_spec = XFibres5_output_spec
     executable = "xfibres"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/conftest.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/aroma/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_accuracytester.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/fix/tests/test_accuracytester.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-from fileformats.generic.directory import Directory
-from fileformats.generic.file import File
+from fileformats.generic import File
 from fileformats.medimage_fsl import MelodicIca
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.accuracy_tester import AccuracyTester
+from pydra.tasks.fsl.auto.fix.accuracy_tester import AccuracyTester
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_accuracytester_1():
     task = AccuracyTester()
     task.inputs.mel_icas = [MelodicIca.sample(seed=0)]
     task.inputs.trained_wts_file = File.sample(seed=1)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_applymask.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_slice.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,27 @@
-from fileformats.medimage.contents.imaging.derivatives import Mask
-from fileformats.medimage.nifti import NiftiGz
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.apply_mask import ApplyMask
+from pydra.tasks.fsl.auto.utils.slice import Slice
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
+@pytest.mark.xfail
+def test_slice_1():
+    task = Slice()
+    task.inputs.in_file = Nifti1.sample(seed=0)
+    print(f"CMDLINE: {task.cmdline}\n\n")
+    res = task(plugin=PassAfterTimeoutWorker)
+    print("RESULT: ", res)
+
+
 @pytest.mark.xfail
-def test_applymask_1():
-    task = ApplyMask()
-    task.inputs.mask_file = Mask__NiftiGz.sample(seed=0)
-    task.inputs.in_file = NiftiGz.sample(seed=1)
+def test_slice_2():
+    task = Slice()
+    task.inputs.in_file = Nifti1.sample(seed=0)
+    task.inputs.out_base_name = "sl"
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_applytopup.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/tests/test_applytopup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-from fileformats.medimage.nifti import Nifti1
-from fileformats.medimage.nifti import NiftiGz
+from fileformats.medimage import Nifti1, NiftiGz
 from fileformats.text import TextFile
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.apply_topup import ApplyTOPUP
+from pydra.tasks.fsl.auto.epi.apply_topup import ApplyTOPUP
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_applytopup_1():
     task = ApplyTOPUP()
     task.inputs.in_files = [Nifti1.sample(seed=0)]
     task.inputs.encoding_file = TextFile.sample(seed=1)
     task.inputs.in_topup_fieldcoef = NiftiGz.sample(seed=3)
     task.inputs.in_topup_movpar = TextFile.sample(seed=4)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_applyxfm.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/test_applyxfm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.apply_xfm import ApplyXFM
+from pydra.tasks.fsl.auto.preprocess.apply_xfm import ApplyXFM
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_applyxfm_1():
     task = ApplyXFM()
     task.inputs.apply_xfm = True
     task.inputs.in_file = File.sample(seed=1)
     task.inputs.reference = File.sample(seed=2)
     task.inputs.in_matrix_file = File.sample(seed=6)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_b0calc.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/test_mcflirt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.b0_calc import B0Calc
+from pydra.tasks.fsl.auto.preprocess.mcflirt import MCFLIRT
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_b0calc_1():
-    task = B0Calc()
+def test_mcflirt_1():
+    task = MCFLIRT()
     task.inputs.in_file = Nifti1.sample(seed=0)
-    task.inputs.x_grad = 0.0
-    task.inputs.y_grad = 0.0
-    task.inputs.z_grad = 0.0
-    task.inputs.x_b0 = 0.0
-    task.inputs.y_b0 = 0.0
-    task.inputs.z_b0 = 1.0
-    task.inputs.delta = -9.45e-06
-    task.inputs.chi_air = 4e-07
-    task.inputs.compute_xyz = False
-    task.inputs.extendboundary = 1.0
-    task.inputs.directconv = False
+    task.inputs.init = File.sample(seed=10)
+    task.inputs.ref_file = File.sample(seed=19)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
 
 
 @pytest.mark.xfail
-def test_b0calc_2():
-    task = B0Calc()
+def test_mcflirt_2():
+    task = MCFLIRT()
     task.inputs.in_file = Nifti1.sample(seed=0)
-    task.inputs.z_b0 = 3.0
+    task.inputs.out_file = "moco.nii"
+    task.inputs.cost = "mutualinfo"
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_bedpostx5.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tests/test_bedpostx5.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from fileformats.generic.directory import Directory
-from fileformats.generic.file import File
-from fileformats.medimage.diffusion import Bval
-from fileformats.medimage.diffusion import Bvec
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import Directory, File
+from fileformats.medimage import Bval, Bvec, Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.bedpostx5 import BEDPOSTX5
+from pydra.tasks.fsl.auto.dti.bedpostx5 import BEDPOSTX5
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_bedpostx5_1():
     task = BEDPOSTX5()
     task.inputs.dwi = Nifti1.sample(seed=0)
     task.inputs.mask = Nifti1.sample(seed=1)
     task.inputs.bvecs = Bvec.sample(seed=2)
     task.inputs.bvals = Bval.sample(seed=3)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_bet.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_invwarp.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.bet import BET
+from pydra.tasks.fsl.auto.utils.inv_warp import InvWarp
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_bet_1():
-    task = BET()
-    task.inputs.in_file = Nifti1.sample(seed=0)
-    task.inputs.t2_guided = File.sample(seed=16)
+def test_invwarp_1():
+    task = InvWarp()
+    task.inputs.warp = Nifti1.sample(seed=0)
+    task.inputs.reference = Nifti1.sample(seed=1)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
 
 
 @pytest.mark.xfail
-def test_bet_2():
-    task = BET()
-    task.inputs.in_file = Nifti1.sample(seed=0)
-    task.inputs.out_file = "brain_anat.nii"
-    task.inputs.frac = 0.7
+def test_invwarp_2():
+    task = InvWarp()
+    task.inputs.warp = Nifti1.sample(seed=0)
+    task.inputs.reference = Nifti1.sample(seed=1)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_cleaner.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_spatialfilter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.cleaner import Cleaner
+from pydra.tasks.fsl.auto.maths.spatial_filter import SpatialFilter
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_cleaner_1():
-    task = Cleaner()
-    task.inputs.artifacts_list_file = File.sample(seed=0)
-    task.inputs.highpass = 100
-    task.inputs.confound_file = File.sample(seed=4)
-    task.inputs.confound_file_1 = File.sample(seed=5)
-    task.inputs.confound_file_2 = File.sample(seed=6)
+def test_spatialfilter_1():
+    task = SpatialFilter()
+    task.inputs.kernel_file = File.sample(seed=3)
+    task.inputs.in_file = File.sample(seed=4)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_cluster.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import NiftiGz
+from fileformats.generic import File
+from fileformats.medimage import NiftiGz
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.cluster import Cluster
+from pydra.tasks.fsl.auto.model.cluster import Cluster
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_cluster_1():
     task = Cluster()
     task.inputs.in_file = NiftiGz.sample(seed=0)
     task.inputs.cope_file = File.sample(seed=12)
     task.inputs.fractional = False
     task.inputs.use_mm = False
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_complex.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_convertwarp.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,35 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.complex import Complex
+from pydra.tasks.fsl.auto.utils.convert_warp import ConvertWarp
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
+@pytest.mark.xfail
+def test_convertwarp_1():
+    task = ConvertWarp()
+    task.inputs.reference = Nifti1.sample(seed=0)
+    task.inputs.premat = File.sample(seed=2)
+    task.inputs.warp1 = Nifti1.sample(seed=3)
+    task.inputs.midmat = File.sample(seed=4)
+    task.inputs.warp2 = File.sample(seed=5)
+    task.inputs.postmat = File.sample(seed=6)
+    task.inputs.shift_in_file = File.sample(seed=7)
+    print(f"CMDLINE: {task.cmdline}\n\n")
+    res = task(plugin=PassAfterTimeoutWorker)
+    print("RESULT: ", res)
+
+
 @pytest.mark.xfail
-def test_complex_1():
-    task = Complex()
-    task.inputs.complex_in_file = File.sample(seed=0)
-    task.inputs.complex_in_file2 = File.sample(seed=1)
-    task.inputs.real_in_file = File.sample(seed=2)
-    task.inputs.imaginary_in_file = File.sample(seed=3)
-    task.inputs.magnitude_in_file = File.sample(seed=4)
-    task.inputs.phase_in_file = File.sample(seed=5)
+def test_convertwarp_2():
+    task = ConvertWarp()
+    task.inputs.reference = Nifti1.sample(seed=0)
+    task.inputs.warp1 = Nifti1.sample(seed=3)
+    task.inputs.relwarp = True
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_contrastmgr.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_complex.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.contrast_mgr import ContrastMgr
+from pydra.tasks.fsl.auto.utils.complex import Complex
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_contrastmgr_1():
-    task = ContrastMgr()
-    task.inputs.tcon_file = File.sample(seed=0)
-    task.inputs.fcon_file = File.sample(seed=1)
-    task.inputs.param_estimates = [File.sample(seed=2)]
-    task.inputs.corrections = File.sample(seed=3)
-    task.inputs.dof_file = File.sample(seed=4)
-    task.inputs.sigmasquareds = File.sample(seed=5)
+def test_complex_1():
+    task = Complex()
+    task.inputs.complex_in_file = File.sample(seed=0)
+    task.inputs.complex_in_file2 = File.sample(seed=1)
+    task.inputs.real_in_file = File.sample(seed=2)
+    task.inputs.imaginary_in_file = File.sample(seed=3)
+    task.inputs.magnitude_in_file = File.sample(seed=4)
+    task.inputs.phase_in_file = File.sample(seed=5)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_convertwarp.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tests/test_xfibres5.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,28 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import Directory, File
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.convert_warp import ConvertWarp
+from pydra.tasks.fsl.auto.dti.x_fibres_5 import XFibres5
 import pytest
 
 
-@pytest.mark.xfail
-def test_convertwarp_1():
-    task = ConvertWarp()
-    task.inputs.reference = Nifti1.sample(seed=0)
-    task.inputs.premat = File.sample(seed=2)
-    task.inputs.warp1 = Nifti1.sample(seed=3)
-    task.inputs.midmat = File.sample(seed=4)
-    task.inputs.warp2 = File.sample(seed=5)
-    task.inputs.postmat = File.sample(seed=6)
-    task.inputs.shift_in_file = File.sample(seed=7)
-    print(f"CMDLINE: {task.cmdline}\n\n")
-    res = task(plugin=PassAfterTimeoutWorker)
-    print("RESULT: ", res)
+logger = logging.getLogger(__name__)
 
 
 @pytest.mark.xfail
-def test_convertwarp_2():
-    task = ConvertWarp()
-    task.inputs.reference = Nifti1.sample(seed=0)
-    task.inputs.warp1 = Nifti1.sample(seed=3)
-    task.inputs.relwarp = True
+def test_xfibres5_1():
+    task = XFibres5()
+    task.inputs.gradnonlin = File.sample(seed=0)
+    task.inputs.dwi = File.sample(seed=1)
+    task.inputs.mask = File.sample(seed=2)
+    task.inputs.bvecs = File.sample(seed=3)
+    task.inputs.bvals = File.sample(seed=4)
+    task.inputs.logdir = Directory.sample(seed=5)
+    task.inputs.n_jumps = 5000
+    task.inputs.burn_in = 0
+    task.inputs.burn_in_no_ard = 0
+    task.inputs.sample_every = 1
+    task.inputs.update_proposal_every = 40
+    task.inputs.force_dir = True
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_convertxfm.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_warputils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,30 @@
-from fileformats.datascience.data import TextMatrix
-from fileformats.generic.file import File
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.convert_xfm import ConvertXFM
+from pydra.tasks.fsl.auto.utils.warp_utils import WarpUtils
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_convertxfm_1():
-    task = ConvertXFM()
-    task.inputs.in_file = TextMatrix.sample(seed=0)
-    task.inputs.in_file2 = File.sample(seed=1)
+def test_warputils_1():
+    task = WarpUtils()
+    task.inputs.in_file = Nifti1.sample(seed=0)
+    task.inputs.reference = Nifti1.sample(seed=1)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
 
 
 @pytest.mark.xfail
-def test_convertxfm_2():
-    task = ConvertXFM()
-    task.inputs.in_file = TextMatrix.sample(seed=0)
-    task.inputs.invert_xfm = True
-    task.inputs.out_file = "flirt_inv.mat"
+def test_warputils_2():
+    task = WarpUtils()
+    task.inputs.in_file = Nifti1.sample(seed=0)
+    task.inputs.reference = Nifti1.sample(seed=1)
+    task.inputs.out_format = "spline"
+    task.inputs.warp_resolution = (10, 10, 10)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_dtifit.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/tests/test_preparefieldmap.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,30 @@
-from fileformats.generic.file import File
-from fileformats.medimage.diffusion import Bval
-from fileformats.medimage.diffusion import Bvec
-from fileformats.medimage.nifti import Nifti1
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.dti_fit import DTIFit
+from pydra.tasks.fsl.auto.epi.prepare_fieldmap import PrepareFieldmap
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_dtifit_1():
-    task = DTIFit()
-    task.inputs.dwi = Nifti1.sample(seed=0)
-    task.inputs.base_name = "dtifit_"
-    task.inputs.mask = Nifti1.sample(seed=2)
-    task.inputs.bvecs = Bvec.sample(seed=3)
-    task.inputs.bvals = Bval.sample(seed=4)
-    task.inputs.cni = File.sample(seed=13)
-    task.inputs.gradnonlin = File.sample(seed=15)
+def test_preparefieldmap_1():
+    task = PrepareFieldmap()
+    task.inputs.scanner = "SIEMENS"
+    task.inputs.in_phase = Nifti1.sample(seed=1)
+    task.inputs.in_magnitude = Nifti1.sample(seed=2)
+    task.inputs.nocheck = False
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
 
 
 @pytest.mark.xfail
-def test_dtifit_2():
-    task = DTIFit()
-    task.inputs.dwi = Nifti1.sample(seed=0)
-    task.inputs.base_name = "TP"
-    task.inputs.mask = Nifti1.sample(seed=2)
-    task.inputs.bvecs = Bvec.sample(seed=3)
-    task.inputs.bvals = Bval.sample(seed=4)
+def test_preparefieldmap_2():
+    task = PrepareFieldmap()
+    task.inputs.in_phase = Nifti1.sample(seed=1)
+    task.inputs.in_magnitude = Nifti1.sample(seed=2)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_dualregression.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_dualregression.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.dual_regression import DualRegression
+from pydra.tasks.fsl.auto.model.dual_regression import DualRegression
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_dualregression_1():
     task = DualRegression()
     task.inputs.in_files = [Nifti1.sample(seed=0)]
     task.inputs.group_IC_maps_4D = Nifti1.sample(seed=1)
     task.inputs.des_norm = True
     task.inputs.design_file = File.sample(seed=4)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_eddy.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/tests/test_eddy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from fileformats.generic.file import File
-from fileformats.medimage.diffusion import Bval
-from fileformats.medimage.diffusion import Bvec
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Bval, Bvec, Nifti1
 from fileformats.text import TextFile
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.eddy import Eddy
+from pydra.tasks.fsl.auto.epi.eddy import Eddy
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_eddy_1():
     task = Eddy()
     task.inputs.in_file = Nifti1.sample(seed=0)
     task.inputs.in_mask = File.sample(seed=1)
     task.inputs.in_index = TextFile.sample(seed=2)
     task.inputs.in_acqp = File.sample(seed=3)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_eddycorrect.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/tests/test_eddycorrect.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.eddy_correct import EddyCorrect
+from pydra.tasks.fsl.auto.epi.eddy_correct import EddyCorrect
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_eddycorrect_1():
     task = EddyCorrect()
     task.inputs.in_file = Nifti1.sample(seed=0)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_eddyquad.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_glm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-from fileformats.generic.file import File
-from fileformats.medimage.diffusion import Bval
-from fileformats.medimage.diffusion import Bvec
-from fileformats.text import TextFile
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.eddy_quad import EddyQuad
+from pydra.tasks.fsl.auto.model.glm import GLM
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_eddyquad_1():
-    task = EddyQuad()
-    task.inputs.base_name = "eddy_corrected"
-    task.inputs.idx_file = File.sample(seed=1)
-    task.inputs.param_file = TextFile.sample(seed=2)
-    task.inputs.mask_file = File.sample(seed=3)
-    task.inputs.bval_file = Bval.sample(seed=4)
-    task.inputs.bvec_file = Bvec.sample(seed=5)
-    task.inputs.field = File.sample(seed=7)
-    task.inputs.slice_spec = File.sample(seed=8)
+def test_glm_1():
+    task = GLM()
+    task.inputs.in_file = Nifti1.sample(seed=0)
+    task.inputs.design = Nifti1.sample(seed=2)
+    task.inputs.contrasts = File.sample(seed=3)
+    task.inputs.mask = File.sample(seed=4)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
 
 
 @pytest.mark.xfail
-def test_eddyquad_2():
-    task = EddyQuad()
-    task.inputs.param_file = TextFile.sample(seed=2)
-    task.inputs.output_dir = "eddy_corrected.qc"
+def test_glm_2():
+    task = GLM()
+    task.inputs.in_file = Nifti1.sample(seed=0)
+    task.inputs.design = Nifti1.sample(seed=2)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_epidewarp.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/tests/test_epidewarp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.epi_de_warp import EPIDeWarp
+from pydra.tasks.fsl.auto.epi.epi_de_warp import EPIDeWarp
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_epidewarp_1():
     task = EPIDeWarp()
     task.inputs.mag_file = Nifti1.sample(seed=0)
     task.inputs.dph_file = Nifti1.sample(seed=1)
     task.inputs.exf_file = File.sample(seed=2)
     task.inputs.epi_file = Nifti1.sample(seed=3)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_epireg.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/tests/test_epireg.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.epi_reg import EpiReg
+from pydra.tasks.fsl.auto.epi.epi_reg import EpiReg
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_epireg_1():
     task = EpiReg()
     task.inputs.epi = Nifti1.sample(seed=0)
     task.inputs.t1_head = Nifti1.sample(seed=1)
     task.inputs.t1_brain = Nifti1.sample(seed=2)
     task.inputs.out_base = "epi2struct"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_extractroi.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tests/test_projthresh.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.extract_roi import ExtractROI
+from pydra.tasks.fsl.auto.dti.proj_thresh import ProjThresh
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_extractroi_1():
-    task = ExtractROI()
-    task.inputs.in_file = File.sample(seed=0)
+def test_projthresh_1():
+    task = ProjThresh()
+    task.inputs.in_files = [File.sample(seed=0)]
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
 
 
 @pytest.mark.xfail
-def test_extractroi_2():
-    task = ExtractROI()
-    task.inputs.in_file = File.sample(seed=0)
-    task.inputs.roi_file = "bar.nii"
-    task.inputs.t_min = 0
-    task.inputs.t_size = 1
+def test_projthresh_2():
+    task = ProjThresh()
+    task.inputs.in_files = [File.sample(seed=0)]
+    task.inputs.threshold = 3
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_fast.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_text2vest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.text import TextFile
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.fast import FAST
+from pydra.tasks.fsl.auto.utils.text_2_vest import Text2Vest
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_fast_1():
-    task = FAST()
-    task.inputs.in_files = [Nifti1.sample(seed=0)]
-    task.inputs.init_transform = File.sample(seed=10)
-    task.inputs.other_priors = [File.sample(seed=11)]
-    task.inputs.manual_seg = File.sample(seed=20)
+def test_text2vest_1():
+    task = Text2Vest()
+    task.inputs.in_file = TextFile.sample(seed=0)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
 
 
 @pytest.mark.xfail
-def test_fast_2():
-    task = FAST()
-    task.inputs.in_files = [Nifti1.sample(seed=0)]
-    task.inputs.out_basename = "fast_"
+def test_text2vest_2():
+    task = Text2Vest()
+    task.inputs.in_file = TextFile.sample(seed=0)
+    task.inputs.out_file = "design.mat"
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_filmgls.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_motionoutliers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,28 @@
-from fileformats.generic.directory import Directory
-from fileformats.generic.file import File
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.filmgls import FILMGLS
+from pydra.tasks.fsl.auto.utils.motion_outliers import MotionOutliers
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
+@pytest.mark.xfail
+def test_motionoutliers_1():
+    task = MotionOutliers()
+    task.inputs.in_file = Nifti1.sample(seed=0)
+    task.inputs.mask = File.sample(seed=2)
+    print(f"CMDLINE: {task.cmdline}\n\n")
+    res = task(plugin=PassAfterTimeoutWorker)
+    print("RESULT: ", res)
+
+
 @pytest.mark.xfail
-def test_filmgls_1():
-    task = FILMGLS()
-    task.inputs.in_file = File.sample(seed=0)
-    task.inputs.design_file = File.sample(seed=1)
-    task.inputs.threshold = 1000.0
-    task.inputs.results_dir = "results"
+def test_motionoutliers_2():
+    task = MotionOutliers()
+    task.inputs.in_file = Nifti1.sample(seed=0)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_filterregressor.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_filterregressor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.filter_regressor import FilterRegressor
+from pydra.tasks.fsl.auto.utils.filter_regressor import FilterRegressor
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_filterregressor_1():
     task = FilterRegressor()
     task.inputs.in_file = File.sample(seed=0)
     task.inputs.design_file = File.sample(seed=2)
     task.inputs.mask = File.sample(seed=5)
     print(f"CMDLINE: {task.cmdline}\n\n")
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_findthebiggest.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tests/test_findthebiggest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.find_the_biggest import FindTheBiggest
+from pydra.tasks.fsl.auto.dti.find_the_biggest import FindTheBiggest
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_findthebiggest_1():
     task = FindTheBiggest()
     task.inputs.in_files = [File.sample(seed=0)]
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_flameo.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_flameo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from fileformats.datascience.data import TextMatrix
-from fileformats.generic.directory import Directory
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
-from fileformats.medimage.nifti import NiftiGz
+from fileformats.datascience import TextMatrix
+from fileformats.generic import Directory, File
+from fileformats.medimage import Nifti1, NiftiGz
 from fileformats.medimage_fsl import Con
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.flameo import FLAMEO
+from pydra.tasks.fsl.auto.model.flameo import FLAMEO
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_flameo_1():
     task = FLAMEO()
     task.inputs.cope_file = NiftiGz.sample(seed=0)
     task.inputs.var_cope_file = NiftiGz.sample(seed=1)
     task.inputs.dof_var_cope_file = File.sample(seed=2)
     task.inputs.mask_file = Nifti1.sample(seed=3)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_flirt.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_melodic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,49 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.datascience import TextMatrix
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+from fileformats.medimage_fsl import Con
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.flirt import FLIRT
+from pydra.tasks.fsl.auto.model.melodic import MELODIC
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_flirt_1():
-    task = FLIRT()
-    task.inputs.in_file = Nifti1.sample(seed=0)
-    task.inputs.reference = Nifti1.sample(seed=1)
-    task.inputs.in_matrix_file = File.sample(seed=5)
-    task.inputs.schedule = File.sample(seed=29)
-    task.inputs.ref_weight = File.sample(seed=30)
-    task.inputs.in_weight = File.sample(seed=31)
-    task.inputs.wm_seg = File.sample(seed=38)
-    task.inputs.wmcoords = File.sample(seed=39)
-    task.inputs.wmnorms = File.sample(seed=40)
-    task.inputs.fieldmap = File.sample(seed=41)
-    task.inputs.fieldmapmask = File.sample(seed=42)
+def test_melodic_1():
+    task = MELODIC()
+    task.inputs.in_files = [Nifti1.sample(seed=0)]
+    task.inputs.mask = File.sample(seed=2)
+    task.inputs.ICs = File.sample(seed=27)
+    task.inputs.mix = File.sample(seed=28)
+    task.inputs.smode = File.sample(seed=29)
+    task.inputs.bg_image = File.sample(seed=32)
+    task.inputs.t_des = TextMatrix.sample(seed=35)
+    task.inputs.t_con = Con.sample(seed=36)
+    task.inputs.s_des = TextMatrix.sample(seed=37)
+    task.inputs.s_con = Con.sample(seed=38)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
 
 
 @pytest.mark.xfail
-def test_flirt_2():
-    task = FLIRT()
-    task.inputs.in_file = Nifti1.sample(seed=0)
-    task.inputs.reference = Nifti1.sample(seed=1)
-    task.inputs.cost_func = "mutualinfo"
-    task.inputs.bins = 640
+def test_melodic_2():
+    task = MELODIC()
+    task.inputs.in_files = [Nifti1.sample(seed=0)]
+    task.inputs.out_dir = "groupICA.out"
+    task.inputs.no_bet = True
+    task.inputs.bg_threshold = 10
+    task.inputs.approach = "tica"
+    task.inputs.mm_thresh = 0.5
+    task.inputs.tr_sec = 1.5
+    task.inputs.t_des = TextMatrix.sample(seed=35)
+    task.inputs.t_con = Con.sample(seed=36)
+    task.inputs.s_des = TextMatrix.sample(seed=37)
+    task.inputs.s_con = Con.sample(seed=38)
+    task.inputs.out_stats = True
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_fnirt.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/test_fnirt.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.fnirt import FNIRT
+from pydra.tasks.fsl.auto.preprocess.fnirt import FNIRT
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_fnirt_1():
     task = FNIRT()
     task.inputs.ref_file = File.sample(seed=0)
     task.inputs.in_file = File.sample(seed=1)
     task.inputs.affine_file = File.sample(seed=2)
     task.inputs.inwarp_file = File.sample(seed=3)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_fugue.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/test_fugue.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.fugue import FUGUE
+from pydra.tasks.fsl.auto.preprocess.fugue import FUGUE
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_fugue_1():
     task = FUGUE()
     task.inputs.in_file = Nifti1.sample(seed=0)
     task.inputs.shift_in_file = Nifti1.sample(seed=1)
     task.inputs.phasemap_in_file = Nifti1.sample(seed=2)
     task.inputs.fmap_in_file = File.sample(seed=3)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_glm.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/test_flirt.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,40 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.glm import GLM
+from pydra.tasks.fsl.auto.preprocess.flirt import FLIRT
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_glm_1():
-    task = GLM()
+def test_flirt_1():
+    task = FLIRT()
     task.inputs.in_file = Nifti1.sample(seed=0)
-    task.inputs.design = Nifti1.sample(seed=2)
-    task.inputs.contrasts = File.sample(seed=3)
-    task.inputs.mask = File.sample(seed=4)
+    task.inputs.reference = Nifti1.sample(seed=1)
+    task.inputs.in_matrix_file = File.sample(seed=5)
+    task.inputs.schedule = File.sample(seed=29)
+    task.inputs.ref_weight = File.sample(seed=30)
+    task.inputs.in_weight = File.sample(seed=31)
+    task.inputs.wm_seg = File.sample(seed=38)
+    task.inputs.wmcoords = File.sample(seed=39)
+    task.inputs.wmnorms = File.sample(seed=40)
+    task.inputs.fieldmap = File.sample(seed=41)
+    task.inputs.fieldmapmask = File.sample(seed=42)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
 
 
 @pytest.mark.xfail
-def test_glm_2():
-    task = GLM()
+def test_flirt_2():
+    task = FLIRT()
     task.inputs.in_file = Nifti1.sample(seed=0)
-    task.inputs.design = Nifti1.sample(seed=2)
+    task.inputs.reference = Nifti1.sample(seed=1)
+    task.inputs.cost_func = "mutualinfo"
+    task.inputs.bins = 640
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_ica_aroma.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_warppointstostd.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-from fileformats.datascience.data import TextMatrix
-from fileformats.generic.directory import Directory
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
-from fileformats.medimage.nifti import NiftiGz
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
 from fileformats.text import TextFile
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.ica__aroma import ICA_AROMA
+from pydra.tasks.fsl.auto.utils.warp_points_to_std import WarpPointsToStd
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_ica_aroma_1():
-    task = ICA_AROMA()
-    task.inputs.feat_dir = Directory.sample(seed=0)
-    task.inputs.in_file = Nifti1.sample(seed=1)
-    task.inputs.mask = NiftiGz.sample(seed=3)
-    task.inputs.melodic_dir = Directory.sample(seed=6)
-    task.inputs.mat_file = TextMatrix.sample(seed=7)
-    task.inputs.fnirt_warp_file = Nifti1.sample(seed=8)
-    task.inputs.motion_parameters = TextFile.sample(seed=9)
+def test_warppointstostd_1():
+    task = WarpPointsToStd()
+    task.inputs.img_file = Nifti1.sample(seed=0)
+    task.inputs.std_file = Nifti1.sample(seed=1)
+    task.inputs.premat_file = File.sample(seed=2)
+    task.inputs.in_coords = TextFile.sample(seed=3)
+    task.inputs.xfm_file = File.sample(seed=4)
+    task.inputs.warp_file = Nifti1.sample(seed=5)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
 
 
 @pytest.mark.xfail
-def test_ica_aroma_2():
-    task = ICA_AROMA()
-    task.inputs.in_file = Nifti1.sample(seed=1)
-    task.inputs.out_dir = "ICA_testout"
-    task.inputs.mask = NiftiGz.sample(seed=3)
-    task.inputs.mat_file = TextMatrix.sample(seed=7)
-    task.inputs.fnirt_warp_file = Nifti1.sample(seed=8)
-    task.inputs.motion_parameters = TextFile.sample(seed=9)
-    task.inputs.denoise_type = "both"
+def test_warppointstostd_2():
+    task = WarpPointsToStd()
+    task.inputs.img_file = Nifti1.sample(seed=0)
+    task.inputs.std_file = Nifti1.sample(seed=1)
+    task.inputs.in_coords = TextFile.sample(seed=3)
+    task.inputs.warp_file = Nifti1.sample(seed=5)
+    task.inputs.coord_mm = True
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_imagemaths.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_imagemaths.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.image_maths import ImageMaths
+from pydra.tasks.fsl.auto.utils.image_maths import ImageMaths
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_imagemaths_1():
     task = ImageMaths()
     task.inputs.in_file = File.sample(seed=0)
     task.inputs.in_file2 = File.sample(seed=1)
     task.inputs.mask_file = File.sample(seed=2)
     print(f"CMDLINE: {task.cmdline}\n\n")
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_imagestats.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/test_bet.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.image_stats import ImageStats
+from pydra.tasks.fsl.auto.preprocess.bet import BET
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_imagestats_1():
-    task = ImageStats()
-    task.inputs.in_file = File.sample(seed=1)
-    task.inputs.mask_file = File.sample(seed=3)
-    task.inputs.index_mask_file = File.sample(seed=4)
+def test_bet_1():
+    task = BET()
+    task.inputs.in_file = Nifti1.sample(seed=0)
+    task.inputs.t2_guided = File.sample(seed=16)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
 
 
 @pytest.mark.xfail
-def test_imagestats_2():
-    task = ImageStats()
-    task.inputs.in_file = File.sample(seed=1)
-    task.inputs.op_string = "-M"
+def test_bet_2():
+    task = BET()
+    task.inputs.in_file = Nifti1.sample(seed=0)
+    task.inputs.out_file = "brain_anat.nii"
+    task.inputs.frac = 0.7
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_makedyadicvectors.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/test_first.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.make_dyadic_vectors import MakeDyadicVectors
+from pydra.tasks.fsl.auto.preprocess.first import FIRST
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_makedyadicvectors_1():
-    task = MakeDyadicVectors()
-    task.inputs.theta_vol = File.sample(seed=0)
-    task.inputs.phi_vol = File.sample(seed=1)
-    task.inputs.mask = File.sample(seed=2)
-    task.inputs.output = File.sample(seed=3)
+def test_first_1():
+    task = FIRST()
+    task.inputs.in_file = File.sample(seed=0)
+    task.inputs.method = "auto"
+    task.inputs.affine_file = File.sample(seed=8)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_maximage.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_percentileimage.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-from fileformats.medimage.nifti import Nifti1
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.max_image import MaxImage
+from pydra.tasks.fsl.auto.maths.percentile_image import PercentileImage
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_maximage_1():
-    task = MaxImage()
+def test_percentileimage_1():
+    task = PercentileImage()
     task.inputs.dimension = "T"
-    task.inputs.in_file = Nifti1.sample(seed=1)
+    task.inputs.in_file = Nifti1.sample(seed=2)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
 
 
 @pytest.mark.xfail
-def test_maximage_2():
-    task = MaxImage()
-    task.inputs.in_file = Nifti1.sample(seed=1)
+def test_percentileimage_2():
+    task = PercentileImage()
+    task.inputs.in_file = Nifti1.sample(seed=2)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_mcflirt.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_slicer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,21 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.mcflirt import MCFLIRT
+from pydra.tasks.fsl.auto.utils.slicer import Slicer
 import pytest
 
 
-@pytest.mark.xfail
-def test_mcflirt_1():
-    task = MCFLIRT()
-    task.inputs.in_file = Nifti1.sample(seed=0)
-    task.inputs.init = File.sample(seed=10)
-    task.inputs.ref_file = File.sample(seed=19)
-    print(f"CMDLINE: {task.cmdline}\n\n")
-    res = task(plugin=PassAfterTimeoutWorker)
-    print("RESULT: ", res)
+logger = logging.getLogger(__name__)
 
 
 @pytest.mark.xfail
-def test_mcflirt_2():
-    task = MCFLIRT()
-    task.inputs.in_file = Nifti1.sample(seed=0)
-    task.inputs.out_file = "moco.nii"
-    task.inputs.cost = "mutualinfo"
+def test_slicer_1():
+    task = Slicer()
+    task.inputs.in_file = File.sample(seed=0)
+    task.inputs.image_edges = File.sample(seed=1)
+    task.inputs.label_slices = True
+    task.inputs.colour_map = File.sample(seed=3)
+    task.inputs.show_orientation = True
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_melodic.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tests/test_probtrackx.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,58 @@
-from fileformats.datascience.data import TextMatrix
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
-from fileformats.medimage_fsl import Con
+from fileformats.datascience import TextMatrix
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.melodic import MELODIC
+from pydra.tasks.fsl.auto.dti.prob_track_x import ProbTrackX
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_melodic_1():
-    task = MELODIC()
-    task.inputs.in_files = [Nifti1.sample(seed=0)]
-    task.inputs.mask = File.sample(seed=2)
-    task.inputs.ICs = File.sample(seed=27)
-    task.inputs.mix = File.sample(seed=28)
-    task.inputs.smode = File.sample(seed=29)
-    task.inputs.bg_image = File.sample(seed=32)
-    task.inputs.t_des = TextMatrix.sample(seed=35)
-    task.inputs.t_con = Con.sample(seed=36)
-    task.inputs.s_des = TextMatrix.sample(seed=37)
-    task.inputs.s_con = Con.sample(seed=38)
+def test_probtrackx_1():
+    task = ProbTrackX()
+    task.inputs.mask2 = File.sample(seed=1)
+    task.inputs.mesh = File.sample(seed=2)
+    task.inputs.thsamples = [Nifti1.sample(seed=3)]
+    task.inputs.phsamples = [Nifti1.sample(seed=4)]
+    task.inputs.fsamples = [Nifti1.sample(seed=5)]
+    task.inputs.samples_base_name = "merged"
+    task.inputs.mask = Nifti1.sample(seed=7)
+    task.inputs.target_masks = [Nifti1.sample(seed=9)]
+    task.inputs.waypoints = File.sample(seed=10)
+    task.inputs.seed_ref = File.sample(seed=12)
+    task.inputs.force_dir = True
+    task.inputs.opd = True
+    task.inputs.avoid_mp = File.sample(seed=18)
+    task.inputs.stop_mask = File.sample(seed=19)
+    task.inputs.xfm = TextMatrix.sample(seed=20)
+    task.inputs.inv_xfm = File.sample(seed=21)
+    task.inputs.n_samples = 5000
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
 
 
 @pytest.mark.xfail
-def test_melodic_2():
-    task = MELODIC()
-    task.inputs.in_files = [Nifti1.sample(seed=0)]
-    task.inputs.out_dir = "groupICA.out"
-    task.inputs.no_bet = True
-    task.inputs.bg_threshold = 10
-    task.inputs.approach = "tica"
-    task.inputs.mm_thresh = 0.5
-    task.inputs.tr_sec = 1.5
-    task.inputs.t_des = TextMatrix.sample(seed=35)
-    task.inputs.t_con = Con.sample(seed=36)
-    task.inputs.s_des = TextMatrix.sample(seed=37)
-    task.inputs.s_con = Con.sample(seed=38)
-    task.inputs.out_stats = True
+def test_probtrackx_2():
+    task = ProbTrackX()
+    task.inputs.mode = "seedmask"
+    task.inputs.thsamples = [Nifti1.sample(seed=3)]
+    task.inputs.phsamples = [Nifti1.sample(seed=4)]
+    task.inputs.fsamples = [Nifti1.sample(seed=5)]
+    task.inputs.samples_base_name = "merged"
+    task.inputs.mask = Nifti1.sample(seed=7)
+    task.inputs.seed = "MASK_average_thal_right.nii"
+    task.inputs.target_masks = [Nifti1.sample(seed=9)]
+    task.inputs.out_dir = "."
+    task.inputs.force_dir = True
+    task.inputs.opd = True
+    task.inputs.os2t = True
+    task.inputs.xfm = TextMatrix.sample(seed=20)
+    task.inputs.n_samples = 3
+    task.inputs.n_steps = 10
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_merge.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_merge.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.medimage.nifti import Nifti1
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.merge import Merge
+from pydra.tasks.fsl.auto.utils.merge import Merge
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_merge_1():
     task = Merge()
     task.inputs.in_files = [Nifti1.sample(seed=0)]
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_multiimagemaths.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_multiimagemaths.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.medimage.nifti import Nifti1
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.multi_image_maths import MultiImageMaths
+from pydra.tasks.fsl.auto.maths.multi_image_maths import MultiImageMaths
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_multiimagemaths_1():
     task = MultiImageMaths()
     task.inputs.operand_files = [Nifti1.sample(seed=1)]
     task.inputs.in_file = Nifti1.sample(seed=2)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_overlay.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_overlay.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.overlay import Overlay
+from pydra.tasks.fsl.auto.utils.overlay import Overlay
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_overlay_1():
     task = Overlay()
     task.inputs.transparency = True
     task.inputs.out_type = "float"
     task.inputs.background_image = File.sample(seed=3)
     task.inputs.stat_image = File.sample(seed=7)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_percentileimage.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_extractroi.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.percentile_image import PercentileImage
+from pydra.tasks.fsl.auto.utils.extract_roi import ExtractROI
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_percentileimage_1():
-    task = PercentileImage()
-    task.inputs.dimension = "T"
-    task.inputs.in_file = Nifti1.sample(seed=2)
+def test_extractroi_1():
+    task = ExtractROI()
+    task.inputs.in_file = File.sample(seed=0)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
 
 
 @pytest.mark.xfail
-def test_percentileimage_2():
-    task = PercentileImage()
-    task.inputs.in_file = Nifti1.sample(seed=2)
+def test_extractroi_2():
+    task = ExtractROI()
+    task.inputs.in_file = File.sample(seed=0)
+    task.inputs.roi_file = "bar.nii"
+    task.inputs.t_min = 0
+    task.inputs.t_size = 1
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_prelude.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/preprocess/tests/test_prelude.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.prelude import PRELUDE
+from pydra.tasks.fsl.auto.preprocess.prelude import PRELUDE
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_prelude_1():
     task = PRELUDE()
     task.inputs.complex_phase_file = File.sample(seed=0)
     task.inputs.magnitude_file = File.sample(seed=1)
     task.inputs.phase_file = File.sample(seed=2)
     task.inputs.mask_file = File.sample(seed=9)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_probtrackx2.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tests/test_probtrackx2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import NiftiGz
+from fileformats.generic import File
+from fileformats.medimage import NiftiGz
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.prob_track_x2 import ProbTrackX2
+from pydra.tasks.fsl.auto.dti.prob_track_x2 import ProbTrackX2
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_probtrackx2_1():
     task = ProbTrackX2()
     task.inputs.fopd = File.sample(seed=1)
     task.inputs.target2 = File.sample(seed=8)
     task.inputs.target3 = File.sample(seed=10)
     task.inputs.lrtarget3 = File.sample(seed=11)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_randomise.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/aroma/tests/test_ica_aroma.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,41 @@
-from fileformats.datascience.data import TextMatrix
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
-from fileformats.medimage_fsl import Con
+from fileformats.datascience import TextMatrix
+from fileformats.generic import Directory
+from fileformats.medimage import Nifti1, NiftiGz
+from fileformats.text import TextFile
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.randomise import Randomise
+from pydra.tasks.fsl.auto.aroma.ica__aroma import ICA_AROMA
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_randomise_1():
-    task = Randomise()
-    task.inputs.in_file = Nifti1.sample(seed=0)
-    task.inputs.base_name = "randomise"
-    task.inputs.design_mat = TextMatrix.sample(seed=2)
-    task.inputs.tcon = Con.sample(seed=3)
-    task.inputs.fcon = File.sample(seed=4)
-    task.inputs.mask = Nifti1.sample(seed=5)
-    task.inputs.x_block_labels = File.sample(seed=6)
+def test_ica_aroma_1():
+    task = ICA_AROMA()
+    task.inputs.feat_dir = Directory.sample(seed=0)
+    task.inputs.in_file = Nifti1.sample(seed=1)
+    task.inputs.mask = NiftiGz.sample(seed=3)
+    task.inputs.melodic_dir = Directory.sample(seed=6)
+    task.inputs.mat_file = TextMatrix.sample(seed=7)
+    task.inputs.fnirt_warp_file = Nifti1.sample(seed=8)
+    task.inputs.motion_parameters = TextFile.sample(seed=9)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
 
 
 @pytest.mark.xfail
-def test_randomise_2():
-    task = Randomise()
-    task.inputs.in_file = Nifti1.sample(seed=0)
-    task.inputs.design_mat = TextMatrix.sample(seed=2)
-    task.inputs.tcon = Con.sample(seed=3)
-    task.inputs.mask = Nifti1.sample(seed=5)
+def test_ica_aroma_2():
+    task = ICA_AROMA()
+    task.inputs.in_file = Nifti1.sample(seed=1)
+    task.inputs.out_dir = "ICA_testout"
+    task.inputs.mask = NiftiGz.sample(seed=3)
+    task.inputs.mat_file = TextMatrix.sample(seed=7)
+    task.inputs.fnirt_warp_file = Nifti1.sample(seed=8)
+    task.inputs.motion_parameters = TextFile.sample(seed=9)
+    task.inputs.denoise_type = "both"
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_slice.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tests/test_makedyadicvectors.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.slice import Slice
+from pydra.tasks.fsl.auto.dti.make_dyadic_vectors import MakeDyadicVectors
 import pytest
 
 
-@pytest.mark.xfail
-def test_slice_1():
-    task = Slice()
-    task.inputs.in_file = Nifti1.sample(seed=0)
-    print(f"CMDLINE: {task.cmdline}\n\n")
-    res = task(plugin=PassAfterTimeoutWorker)
-    print("RESULT: ", res)
+logger = logging.getLogger(__name__)
 
 
 @pytest.mark.xfail
-def test_slice_2():
-    task = Slice()
-    task.inputs.in_file = Nifti1.sample(seed=0)
-    task.inputs.out_base_name = "sl"
+def test_makedyadicvectors_1():
+    task = MakeDyadicVectors()
+    task.inputs.theta_vol = File.sample(seed=0)
+    task.inputs.phi_vol = File.sample(seed=1)
+    task.inputs.mask = File.sample(seed=2)
+    task.inputs.output = File.sample(seed=3)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_slicer.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/maths/tests/test_temporalfilter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.slicer import Slicer
+from pydra.tasks.fsl.auto.maths.temporal_filter import TemporalFilter
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_slicer_1():
-    task = Slicer()
-    task.inputs.in_file = File.sample(seed=0)
-    task.inputs.image_edges = File.sample(seed=1)
-    task.inputs.label_slices = True
-    task.inputs.colour_map = File.sample(seed=3)
-    task.inputs.show_orientation = True
+def test_temporalfilter_1():
+    task = TemporalFilter()
+    task.inputs.lowpass_sigma = -1
+    task.inputs.highpass_sigma = -1
+    task.inputs.in_file = File.sample(seed=2)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_smooth.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_smooth.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from fileformats.medimage.nifti import Nifti1
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.smooth import Smooth
+from pydra.tasks.fsl.auto.utils.smooth import Smooth
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_smooth_1():
     task = Smooth()
     task.inputs.in_file = Nifti1.sample(seed=0)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_smoothestimate.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_smoothestimate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
-from fileformats.medimage.nifti import NiftiGz
+from fileformats.generic import File
+from fileformats.medimage import Nifti1, NiftiGz
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.smooth_estimate import SmoothEstimate
+from pydra.tasks.fsl.auto.model.smooth_estimate import SmoothEstimate
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_smoothestimate_1():
     task = SmoothEstimate()
     task.inputs.mask_file = Nifti1.sample(seed=1)
     task.inputs.residual_fit_file = File.sample(seed=2)
     task.inputs.zstat_file = NiftiGz.sample(seed=3)
     print(f"CMDLINE: {task.cmdline}\n\n")
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_topup.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/tests/test_topup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
 from fileformats.text import TextFile
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.topup import TOPUP
+from pydra.tasks.fsl.auto.epi.topup import TOPUP
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_topup_1():
     task = TOPUP()
     task.inputs.in_file = Nifti1.sample(seed=0)
     task.inputs.encoding_file = TextFile.sample(seed=1)
     task.inputs.readout_times = [File.sample(seed=3)]
     task.inputs.out_warp_prefix = "warpfield"
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_tractskeleton.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_contrastmgr.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-from fileformats.generic.file import File
+from fileformats.generic import File
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.tract_skeleton import TractSkeleton
+from pydra.tasks.fsl.auto.model.contrast_mgr import ContrastMgr
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_tractskeleton_1():
-    task = TractSkeleton()
-    task.inputs.in_file = File.sample(seed=0)
-    task.inputs.distance_map = File.sample(seed=3)
-    task.inputs.search_mask_file = File.sample(seed=4)
-    task.inputs.use_cingulum_mask = True
-    task.inputs.data_file = File.sample(seed=6)
-    task.inputs.alt_data_file = File.sample(seed=7)
-    task.inputs.alt_skeleton = File.sample(seed=8)
+def test_contrastmgr_1():
+    task = ContrastMgr()
+    task.inputs.tcon_file = File.sample(seed=0)
+    task.inputs.fcon_file = File.sample(seed=1)
+    task.inputs.param_estimates = [File.sample(seed=2)]
+    task.inputs.corrections = File.sample(seed=3)
+    task.inputs.dof_file = File.sample(seed=4)
+    task.inputs.sigmasquareds = File.sample(seed=5)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_vecreg.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/dti/tests/test_vecreg.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-from fileformats.datascience.data import TextMatrix
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.datascience import TextMatrix
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.vec_reg import VecReg
+from pydra.tasks.fsl.auto.dti.vec_reg import VecReg
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_vecreg_1():
     task = VecReg()
     task.inputs.in_file = Nifti1.sample(seed=0)
     task.inputs.ref_vol = Nifti1.sample(seed=2)
     task.inputs.affine_mat = TextMatrix.sample(seed=3)
     task.inputs.warp_field = File.sample(seed=4)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_vest2text.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_convertxfm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,30 @@
-from fileformats.datascience.data import TextMatrix
-from fileformats.generic.file import File
+from fileformats.datascience import TextMatrix
+from fileformats.generic import File
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.vest_2_text import Vest2Text
+from pydra.tasks.fsl.auto.utils.convert_xfm import ConvertXFM
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_vest2text_1():
-    task = Vest2Text()
+def test_convertxfm_1():
+    task = ConvertXFM()
     task.inputs.in_file = TextMatrix.sample(seed=0)
-    task.inputs.out_file = "design.txt"
+    task.inputs.in_file2 = File.sample(seed=1)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
 
 
 @pytest.mark.xfail
-def test_vest2text_2():
-    task = Vest2Text()
+def test_convertxfm_2():
+    task = ConvertXFM()
     task.inputs.in_file = TextMatrix.sample(seed=0)
+    task.inputs.invert_xfm = True
+    task.inputs.out_file = "flirt_inv.mat"
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_warppoints.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/utils/tests/test_warppoints.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
 from fileformats.text import TextFile
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.warp_points import WarpPoints
+from pydra.tasks.fsl.auto.utils.warp_points import WarpPoints
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
 def test_warppoints_1():
     task = WarpPoints()
     task.inputs.src_file = Nifti1.sample(seed=0)
     task.inputs.dest_file = Nifti1.sample(seed=1)
     task.inputs.in_coords = TextFile.sample(seed=2)
     task.inputs.xfm_file = File.sample(seed=3)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_warppointsfromstd.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/epi/tests/test_eddyquad.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.generic import File
+from fileformats.medimage import Bval, Bvec
 from fileformats.text import TextFile
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.warp_points_from_std import WarpPointsFromStd
+from pydra.tasks.fsl.auto.epi.eddy_quad import EddyQuad
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_warppointsfromstd_1():
-    task = WarpPointsFromStd()
-    task.inputs.img_file = Nifti1.sample(seed=0)
-    task.inputs.std_file = Nifti1.sample(seed=1)
-    task.inputs.in_coords = TextFile.sample(seed=2)
-    task.inputs.xfm_file = File.sample(seed=3)
-    task.inputs.warp_file = Nifti1.sample(seed=4)
+def test_eddyquad_1():
+    task = EddyQuad()
+    task.inputs.base_name = "eddy_corrected"
+    task.inputs.idx_file = File.sample(seed=1)
+    task.inputs.param_file = TextFile.sample(seed=2)
+    task.inputs.mask_file = File.sample(seed=3)
+    task.inputs.bval_file = Bval.sample(seed=4)
+    task.inputs.bvec_file = Bvec.sample(seed=5)
+    task.inputs.field = File.sample(seed=7)
+    task.inputs.slice_spec = File.sample(seed=8)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
 
 
 @pytest.mark.xfail
-def test_warppointsfromstd_2():
-    task = WarpPointsFromStd()
-    task.inputs.img_file = Nifti1.sample(seed=0)
-    task.inputs.std_file = Nifti1.sample(seed=1)
-    task.inputs.in_coords = TextFile.sample(seed=2)
-    task.inputs.warp_file = Nifti1.sample(seed=4)
-    task.inputs.coord_mm = True
+def test_eddyquad_2():
+    task = EddyQuad()
+    task.inputs.param_file = TextFile.sample(seed=2)
+    task.inputs.output_dir = "eddy_corrected.qc"
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/auto/tests/test_warputils.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/auto/model/tests/test_randomise.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,38 @@
-from fileformats.generic.file import File
-from fileformats.medimage.nifti import Nifti1
+from fileformats.datascience import TextMatrix
+from fileformats.generic import File
+from fileformats.medimage import Nifti1
+from fileformats.medimage_fsl import Con
+import logging
 from nipype2pydra.testing import PassAfterTimeoutWorker
-from pydra.tasks.fsl.auto.warp_utils import WarpUtils
+from pydra.tasks.fsl.auto.model.randomise import Randomise
 import pytest
 
 
+logger = logging.getLogger(__name__)
+
+
 @pytest.mark.xfail
-def test_warputils_1():
-    task = WarpUtils()
+def test_randomise_1():
+    task = Randomise()
     task.inputs.in_file = Nifti1.sample(seed=0)
-    task.inputs.reference = Nifti1.sample(seed=1)
+    task.inputs.base_name = "randomise"
+    task.inputs.design_mat = TextMatrix.sample(seed=2)
+    task.inputs.tcon = Con.sample(seed=3)
+    task.inputs.fcon = File.sample(seed=4)
+    task.inputs.mask = Nifti1.sample(seed=5)
+    task.inputs.x_block_labels = File.sample(seed=6)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
 
 
 @pytest.mark.xfail
-def test_warputils_2():
-    task = WarpUtils()
+def test_randomise_2():
+    task = Randomise()
     task.inputs.in_file = Nifti1.sample(seed=0)
-    task.inputs.reference = Nifti1.sample(seed=1)
-    task.inputs.out_format = "spline"
-    task.inputs.warp_resolution = (10, 10, 10)
+    task.inputs.design_mat = TextMatrix.sample(seed=2)
+    task.inputs.tcon = Con.sample(seed=3)
+    task.inputs.mask = Nifti1.sample(seed=5)
     print(f"CMDLINE: {task.cmdline}\n\n")
     res = task(plugin=PassAfterTimeoutWorker)
     print("RESULT: ", res)
```

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/__init__.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/__init__.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fast.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fast.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/maths.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/maths.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/susan.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/susan.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/bet/bet.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/bet/bet.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/bet/robustfov.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/bet/robustfov.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/eddy/applytopup.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/eddy/applytopup.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/eddy/eddy.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/eddy/eddy.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/eddy/topup.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/eddy/topup.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/convertxfm.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/flirt/convertxfm.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/flirt.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/flirt/flirt.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/img2imgcoord.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/flirt/img2imgcoord.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/img2stdcoord.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/flirt/img2stdcoord.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/specs.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/flirt/specs.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/flirt/std2imgcoord.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/flirt/std2imgcoord.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/applywarp.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fnirt/applywarp.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/convertwarp.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fnirt/convertwarp.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/fnirt.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fnirt/fnirt.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/fnirtfileutils.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fnirt/fnirtfileutils.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fnirt/invwarp.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fnirt/invwarp.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fugue/fugue.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fugue/fugue.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fugue/prelude.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fugue/prelude.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fugue/prepare_fieldmap.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fugue/prepare_fieldmap.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/fugue/sigloss.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/fugue/sigloss.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/__init__.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/chfiletype.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/chfiletype.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/fft.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/fft.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/info.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/info.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/interleave.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/interleave.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/merge.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/merge.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/orient.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/orient.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/reorient2std.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/reorient2std.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/selectvols.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/selectvols.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/smoothfill.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/smoothfill.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/split.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/split.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pydra/tasks/fsl/v6_0/utils/swapdim.py` & `pydra_fsl-0.1.1/pydra/tasks/fsl/v6_0/utils/swapdim.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/related-packages/conftest.py` & `pydra_fsl-0.1.1/related-packages/conftest.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/related-packages/fileformats/LICENSE` & `pydra_fsl-0.1.1/related-packages/fileformats/LICENSE`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/related-packages/fileformats/README.rst` & `pydra_fsl-0.1.1/related-packages/fileformats/README.rst`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/related-packages/fileformats/pyproject.toml` & `pydra_fsl-0.1.1/related-packages/fileformats/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/related-packages/fileformats-extras/LICENSE` & `pydra_fsl-0.1.1/related-packages/fileformats-extras/LICENSE`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/related-packages/fileformats-extras/README.rst` & `pydra_fsl-0.1.1/related-packages/fileformats-extras/README.rst`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/related-packages/fileformats-extras/pyproject.toml` & `pydra_fsl-0.1.1/related-packages/fileformats-extras/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/tools/increment_tool_version.py` & `pydra_fsl-0.1.1/tools/increment_tool_version.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/tools/rename_template.py` & `pydra_fsl-0.1.1/tools/rename_template.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/tools/report_progress.py` & `pydra_fsl-0.1.1/tools/report_progress.py`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/.gitignore` & `pydra_fsl-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/LICENSE` & `pydra_fsl-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/NOTICE` & `pydra_fsl-0.1.1/NOTICE`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/README.md` & `pydra_fsl-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/pyproject.toml` & `pydra_fsl-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydra_fsl-0.1.0/PKG-INFO` & `pydra_fsl-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydra-fsl
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pydra tasks package for fsl
 Project-URL: Documentation, https://github.com/nipype/pydra-tasks-fsl#readme
 Project-URL: Issues, https://github.com/nipype/pydra-tasks-fsl/issues
 Project-URL: Source, https://github.com/nipype/pydra-tasks-fsl
 Author-email: Nipype developers <neuroimaging@python.org>, Ghislain Vaillant <ghislain.vaillant@icm-institute.org>
 Maintainer-email: Nipype developers <neuroimaging@python.org>, Ghislain Vaillant <ghislain.vaillant@icm-institute.org>
 License:                                  Apache License
```

