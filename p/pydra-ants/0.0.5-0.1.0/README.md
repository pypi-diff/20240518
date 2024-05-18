# Comparing `tmp/pydra_ants-0.0.5.tar.gz` & `tmp/pydra_ants-0.1.0.tar.gz`

## Comparing `pydra_ants-0.0.5.tar` & `pydra_ants-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,186 @@
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pydra_ants-0.0.5/.editorconfig
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydra_ants-0.0.5/.github/dependabot.yaml
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pydra_ants-0.0.5/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pydra_ants-0.0.5/.github/workflows/test.yaml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 pydra_ants-0.0.5/src/pydra/tasks/ants/__init__.py
--rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 pydra_ants-0.0.5/src/pydra/tasks/ants/apply_transforms.py
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 pydra_ants-0.0.5/src/pydra/tasks/ants/bias_correction.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 pydra_ants-0.0.5/src/pydra/tasks/ants/create_jacobian_determinant_image.py
--rw-r--r--   0        0        0    30430 2020-02-02 00:00:00.000000 pydra_ants-0.0.5/src/pydra/tasks/ants/registration.py
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 pydra_ants-0.0.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pydra_ants-0.0.5/LICENSE
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 pydra_ants-0.0.5/README.md
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pydra_ants-0.0.5/hatch.toml
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 pydra_ants-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 pydra_ants-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/.coveragerc
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/.editorconfig
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/.flake8
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/.gitattributes
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/codecov.yml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/.github/dependabot.yaml
+-rw-r--r--   0        0        0    11463 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/.github/workflows/ci-cd.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/docs/Makefile
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/docs/make.bat
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/docs/source/api.rst
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/docs/source/conf.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/docs/source/index.rst
+-rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/generate
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/requirements.txt
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/package.yaml
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/classes/nipype.interfaces.ants.base.Info.yaml
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/classes/nipype.interfaces.base.core.PackageInfo.yaml
+-rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/affine_initializer.yaml
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/affine_initializer_callables.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/ai.yaml
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/ai_callables.py
+-rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/ants.yaml
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/ants_callables.py
+-rw-r--r--   0        0        0     8985 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/ants_introduction.yaml
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/ants_introduction_callables.py
+-rw-r--r--   0        0        0    24197 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/apply_transforms.yaml
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/apply_transforms_callables.py
+-rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/apply_transforms_to_points.yaml
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/apply_transforms_to_points_callables.py
+-rw-r--r--   0        0        0    28224 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/atropos.yaml
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/atropos_callables.py
+-rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/average_affine_transform.yaml
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/average_affine_transform_callables.py
+-rw-r--r--   0        0        0     7615 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/average_images.yaml
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/average_images_callables.py
+-rw-r--r--   0        0        0    12166 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/brain_extraction.yaml
+-rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/brain_extraction_callables.py
+-rw-r--r--   0        0        0     8763 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/buildtemplateparallel.yaml
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/buildtemplateparallel_callables.py
+-rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/compose_multi_transform.yaml
+-rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/compose_multi_transform_callables.py
+-rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/composite_transform_util.yaml
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/composite_transform_util_callables.py
+-rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/convert_scalar_image_to_rgb.yaml
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/convert_scalar_image_to_rgb_callables.py
+-rw-r--r--   0        0        0    15274 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/cortical_thickness.yaml
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/cortical_thickness_callables.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/create_jacobian_determinant_image.yaml
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/create_jacobian_determinant_image_callables.py
+-rw-r--r--   0        0        0    12068 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/create_tiled_mosaic.yaml
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/create_tiled_mosaic_callables.py
+-rw-r--r--   0        0        0    13890 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/denoise_image.yaml
+-rw-r--r--   0        0        0     6285 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/denoise_image_callables.py
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/gen_warp_fields.yaml
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/gen_warp_fields_callables.py
+-rw-r--r--   0        0        0    23234 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/image_math.yaml
+-rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/image_math_callables.py
+-rw-r--r--   0        0        0    29560 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/joint_fusion.yaml
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/joint_fusion_callables.py
+-rw-r--r--   0        0        0    12468 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/kelly_kapowski.yaml
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/kelly_kapowski_callables.py
+-rw-r--r--   0        0        0     8958 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/label_geometry.yaml
+-rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/label_geometry_callables.py
+-rw-r--r--   0        0        0     9429 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/laplacian_thickness.yaml
+-rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/laplacian_thickness_callables.py
+-rw-r--r--   0        0        0    10709 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/measure_image_similarity.yaml
+-rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/measure_image_similarity_callables.py
+-rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/multiply_images.yaml
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/multiply_images_callables.py
+-rw-r--r--   0        0        0    21455 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/n4_bias_field_correction.yaml
+-rw-r--r--   0        0        0     6663 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/n4_bias_field_correction_callables.py
+-rw-r--r--   0        0        0    90307 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/registration.yaml
+-rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/registration_callables.py
+-rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/registration_syn_quick.yaml
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/registration_syn_quick_callables.py
+-rw-r--r--   0        0        0    13460 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/resample_image_by_spacing.yaml
+-rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/resample_image_by_spacing_callables.py
+-rw-r--r--   0        0        0    11053 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/threshold_image.yaml
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/threshold_image_callables.py
+-rw-r--r--   0        0        0    13283 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/warp_image_multi_transform.yaml
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/warp_image_multi_transform_callables.py
+-rw-r--r--   0        0        0    12424 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/warp_time_series_image_multi_transform.yaml
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/nipype-auto-conv/specs/interfaces/warp_time_series_image_multi_transform_callables.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/_version.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/latest.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/__init__.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/_post_release.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/base.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/legacy/__init__.py
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/legacy/ants_introduction.py
+-rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/legacy/buildtemplateparallel.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/legacy/gen_warp_fields.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/legacy/tests/conftest.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/legacy/tests/test_antsintroduction.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/legacy/tests/test_buildtemplateparallel.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/legacy/tests/test_genwarpfields.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/nipype_ports/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/nipype_ports/interfaces/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/nipype_ports/interfaces/base/__init__.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/nipype_ports/interfaces/base/core.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/registration/__init__.py
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/registration/ants.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/registration/composite_transform_util.py
+-rw-r--r--   0        0        0     4717 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/registration/measure_image_similarity.py
+-rw-r--r--   0        0        0    32897 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/registration/registration.py
+-rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/registration/registration_syn_quick.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/registration/tests/conftest.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/registration/tests/test_ants.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/registration/tests/test_compositetransformutil.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/registration/tests/test_measureimagesimilarity.py
+-rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/registration/tests/test_registration.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/registration/tests/test_registrationsynquick.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/resampling/__init__.py
+-rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/resampling/apply_transforms.py
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/resampling/apply_transforms_to_points.py
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/resampling/warp_image_multi_transform.py
+-rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/resampling/warp_time_series_image_multi_transform.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/resampling/tests/conftest.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/resampling/tests/test_applytransforms.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/resampling/tests/test_applytransformstopoints.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/resampling/tests/test_warpimagemultitransform.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/resampling/tests/test_warptimeseriesimagemultitransform.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/segmentation/__init__.py
+-rw-r--r--   0        0        0    10359 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/segmentation/atropos.py
+-rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/segmentation/brain_extraction.py
+-rw-r--r--   0        0        0     9779 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/segmentation/cortical_thickness.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/segmentation/denoise_image.py
+-rw-r--r--   0        0        0    10056 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/segmentation/joint_fusion.py
+-rw-r--r--   0        0        0     7567 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/segmentation/kelly_kapowski.py
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/segmentation/laplacian_thickness.py
+-rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/segmentation/n4_bias_field_correction.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/segmentation/tests/conftest.py
+-rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/segmentation/tests/test_atropos.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/segmentation/tests/test_brainextraction.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/segmentation/tests/test_corticalthickness.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/segmentation/tests/test_denoiseimage.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/segmentation/tests/test_jointfusion.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/segmentation/tests/test_kellykapowski.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/segmentation/tests/test_laplacianthickness.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/segmentation/tests/test_n4biasfieldcorrection.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/__init__.py
+-rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/affine_initializer.py
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/ai.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/average_affine_transform.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/average_images.py
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/compose_multi_transform.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/create_jacobian_determinant_image.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/image_math.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/label_geometry.py
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/multiply_images.py
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/resample_image_by_spacing.py
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/threshold_image.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/tests/conftest.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/tests/test_affineinitializer.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/tests/test_ai.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/tests/test_averageaffinetransform.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/tests/test_averageimages.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/tests/test_composemultitransform.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/tests/test_createjacobiandeterminantimage.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/tests/test_imagemath.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/tests/test_labelgeometry.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/tests/test_multiplyimages.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/tests/test_resampleimagebyspacing.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/utils/tests/test_thresholdimage.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/visualization/__init__.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/visualization/convert_scalar_image_to_rgb.py
+-rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/visualization/create_tiled_mosaic.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/visualization/tests/conftest.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/visualization/tests/test_convertscalarimagetorgb.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/auto/visualization/tests/test_createtiledmosaic.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/v2_5/__init__.py
+-rw-r--r--   0        0        0     7686 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/v2_5/apply_transforms.py
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/v2_5/bias_correction.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/v2_5/create_jacobian_determinant_image.py
+-rw-r--r--   0        0        0    32561 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pydra/tasks/ants/v2_5/registration.py
+-rwxr-xr-x   0        0        0     2272 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/tools/increment_tool_version.py
+-rwxr-xr-x   0        0        0      803 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/tools/report_progress.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/tools/requirements.txt
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/LICENSE
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/NOTICE
+-rw-r--r--   0        0        0     6470 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/README.md
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    21735 2020-02-02 00:00:00.000000 pydra_ants-0.1.0/PKG-INFO
```

### Comparing `pydra_ants-0.0.5/src/pydra/tasks/ants/apply_transforms.py` & `pydra_ants-0.1.0/pydra/tasks/ants/v2_5/apply_transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,119 +13,152 @@
     save_warp_field: bool,
     output_warp_field: PathLike,
     save_transform: bool,
     output_transform: PathLike,
     invert_transform: bool,
 ) -> str:
     return "-o {}".format(
-        "Linear[{},{:%d}]".format(output_transform, invert_transform)
+        f"Linear[{output_transform},{invert_transform:%d}]"
         if save_transform
-        else "[{},{:%d}]".format(output_warp_field, save_warp_field)
-        if save_warp_field
-        else f"{output_image}"
+        else (
+            f"[{output_warp_field},{save_warp_field:%d}]"
+            if save_warp_field
+            else f"{output_image}"
+        )
     )
 
 
-def _format_interpolation(interpolator: str, sigma: float, alpha: float, order: int) -> str:
+def _format_interpolation(
+    interpolator: str, sigma: float, alpha: float, order: int
+) -> str:
     return "-n {}{}".format(
         interpolator,
-        f"[{order}]"
-        if interpolator == "BSpline"
-        else f"[{sigma},{alpha}]"
-        if interpolator in ("MultiLabel", "Gaussian")
-        else "",
+        (
+            f"[{order}]"
+            if interpolator == "BSpline"
+            else (
+                f"[{sigma},{alpha}]"
+                if interpolator in ("MultiLabel", "Gaussian")
+                else ""
+            )
+        ),
     )
 
 
 class ApplyTransforms(ShellCommandTask):
     """Task definition for antsApplyTransforms.
 
     Examples
     --------
     >>> task = ApplyTransforms(moving_image="moving.nii", fixed_image="fixed.nii")
-    >>> task.cmdline    # doctest: +ELLIPSIS
+    >>> task.cmdline  # doctest: +ELLIPSIS
     'antsApplyTransforms -e scalar -i moving.nii -r fixed.nii -o .../moving_warped.nii -n Linear ...'
 
     >>> task = ApplyTransforms(
     ...     moving_image="moving.nii",
     ...     fixed_image="fixed.nii",
     ...     interpolator="BSpline",
     ...     input_transforms=["affine.mat"],
     ... )
-    >>> task.cmdline    # doctest: +ELLIPSIS
+    >>> task.cmdline  # doctest: +ELLIPSIS
     'antsApplyTransforms ... -n BSpline[3] -t affine.mat ...'
 
     >>> task = ApplyTransforms(
     ...     moving_image="moving.nii",
     ...     fixed_image="fixed.nii",
     ...     interpolator="Gaussian",
     ...     sigma=4.0,
     ...     alpha=1.0,
     ...     input_transforms=["affine.mat", "warp_field.nii.gz"],
     ...     invert_transforms=[True, False],
     ... )
-    >>> task.cmdline    # doctest: +ELLIPSIS
+    >>> task.cmdline  # doctest: +ELLIPSIS
     'antsApplyTransforms ... -n Gaussian[4.0,1.0] -t [affine.mat,1] -t [warp_field.nii.gz,0] ...'
     """
 
     @define(kw_only=True)
     class InputSpec(ShellSpec):
         dimensionality: int = field(
-            metadata={"help_string": "image dimensionality", "argstr": "-d", "allowed_values": {2, 3, 4}}
+            metadata={
+                "help_string": "image dimensionality",
+                "argstr": "-d",
+                "allowed_values": {2, 3, 4},
+            }
         )
 
         image_type: str = field(
             default="scalar",
             metadata={
                 "help_string": (
                     "specify the image type (0: scalar, 1: vector, 2: tensor, 3: time-series, 4: multichannel,"
                     " 5: five-dimensional)"
                 ),
                 "argstr": "-e",
                 "allowed_values": {0, 1, 2, 3, 4, 5},
             },
         )
 
-        moving_image: PathLike = field(metadata={"help_string": "moving image", "mandatory": True, "argstr": "-i"})
+        moving_image: PathLike = field(
+            metadata={"help_string": "moving image", "mandatory": True, "argstr": "-i"}
+        )
 
-        fixed_image: PathLike = field(metadata={"help_string": "fixed image", "mandatory": True, "argstr": "-r"})
+        fixed_image: PathLike = field(
+            metadata={"help_string": "fixed image", "mandatory": True, "argstr": "-r"}
+        )
 
         output_: str = field(
-            metadata={"help_string": "output parameter", "readonly": True, "formatter": _format_output}
+            metadata={
+                "help_string": "output parameter",
+                "readonly": True,
+                "formatter": _format_output,
+            }
         )
 
         output_image: str = field(
-            metadata={"help_string": "output image", "output_file_template": "{moving_image}_warped"}
+            metadata={
+                "help_string": "output image",
+                "output_file_template": "{moving_image}_warped",
+            }
         )
 
-        save_warp_field: bool = field(metadata={"help_string": "save composite warp field"})
+        save_warp_field: bool = field(
+            metadata={"help_string": "save composite warp field"}
+        )
 
         output_warp_field: str = field(
             metadata={
                 "help_string": "output warp field",
                 "output_file_template": "{moving_image}_warpfield",
                 "requires": {"save_warp_field"},
             }
         )
 
-        save_transform: bool = field(metadata={"help_string": "save composite transform"})
+        save_transform: bool = field(
+            metadata={"help_string": "save composite transform"}
+        )
 
         output_transform: str = field(
             metadata={
                 "help_string": "output transform",
                 "output_file_template": "{moving_image}_affine.mat",
                 "keep_extension": False,
                 "requires": {"save_transform"},
             }
         )
 
-        invert_transform: bool = field(default=False, metadata={"help_string": "invert composite transform"})
+        invert_transform: bool = field(
+            default=False, metadata={"help_string": "invert composite transform"}
+        )
 
         interpolation_: str = field(
-            metadata={"help_string": "interpolation parameter", "readonly": True, "formatter": _format_interpolation}
+            metadata={
+                "help_string": "interpolation parameter",
+                "readonly": True,
+                "formatter": _format_interpolation,
+            }
         )
 
         interpolator: str = field(
             default="Linear",
             metadata={
                 "help_string": "interpolation method",
                 "allowed_values": {
@@ -137,46 +170,70 @@
                     "WelchWindowedSinc",
                     "HammingWindowedSinc",
                     "LanczosWindowedSinc",
                 },
             },
         )
 
-        sigma: float = field(default=1.0, metadata={"help_string": "sigma parameter interpolation"})
+        sigma: float = field(
+            default=1.0, metadata={"help_string": "sigma parameter interpolation"}
+        )
 
-        alpha: float = field(default=1.0, metadata={"help_string": "alpha parameter for interpolation"})
+        alpha: float = field(
+            default=1.0, metadata={"help_string": "alpha parameter for interpolation"}
+        )
 
-        order: int = field(default=3, metadata={"help_string": "order parameter for interpolation"})
+        order: int = field(
+            default=3, metadata={"help_string": "order parameter for interpolation"}
+        )
 
         output_datatype: str = field(
             metadata={
                 "help_string": "force output image datatype",
                 "argstr": "-u",
-                "allowed_values": {"char", "uchar", "short", "int", "float", "double", "default"},
+                "allowed_values": {
+                    "char",
+                    "uchar",
+                    "short",
+                    "int",
+                    "float",
+                    "double",
+                    "default",
+                },
             }
         )
 
         input_transforms: Sequence[PathLike] = field(
             metadata={
                 "help_string": "input transforms to apply",
                 "formatter": lambda input_transforms, invert_transforms: (
                     ""
                     if not input_transforms
-                    else " ".join(f"-t {f}" for f in input_transforms)
-                    if not invert_transforms
-                    else " ".join(f"-t [{f},{int(i)}]" for f, i in zip(input_transforms, invert_transforms))
+                    else (
+                        " ".join(f"-t {f}" for f in input_transforms)
+                        if not invert_transforms
+                        else " ".join(
+                            f"-t [{f},{int(i)}]"
+                            for f, i in zip(input_transforms, invert_transforms)
+                        )
+                    )
                 ),
             }
         )
 
         invert_transforms: Sequence[bool] = field(
-            metadata={"help_string": "which transforms to invert", "requires": {"input_transforms"}}
+            metadata={
+                "help_string": "which transforms to invert",
+                "requires": {"input_transforms"},
+            }
         )
 
-        default_value: float = field(metadata={"help_string": "default voxel value", "argstr": "-f"})
+        default_value: float = field(
+            metadata={"help_string": "default voxel value", "argstr": "-f"}
+        )
 
         use_float_precision: bool = field(
             default=False,
             metadata={
                 "help_string": "use float precision instead of double",
                 "formatter": lambda use_float_precision: f"--float {use_float_precision:d}",
             },
```

### Comparing `pydra_ants-0.0.5/src/pydra/tasks/ants/create_jacobian_determinant_image.py` & `pydra_ants-0.1.0/pydra/tasks/ants/v2_5/create_jacobian_determinant_image.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,53 @@
-__all__ = ["CreateJacobianDeterminantImage"]
-
 from os import PathLike
 
 from attrs import define, field
 from pydra.engine.specs import ShellSpec, SpecInfo
 from pydra.engine.task import ShellCommandTask
 
+__all__ = ["CreateJacobianDeterminantImage"]
+
 
 class CreateJacobianDeterminantImage(ShellCommandTask):
     """Task definition for CreateJacobianDeterminantImage.
 
     Examples
     --------
-    >>> task = CreateJacobianDeterminantImage(dimensionality=3, warp_field="warp.nii.gz")
-    >>> task.cmdline    # doctest: +ELLIPSIS
+    >>> task = CreateJacobianDeterminantImage(
+    ...     dimensionality=3, warp_field="warp.nii.gz"
+    ... )
+    >>> task.cmdline  # doctest: +ELLIPSIS
     'CreateJacobianDeterminantImage 3 warp.nii.gz .../warp_jac.nii.gz 0 0'
     """
 
     @define(kw_only=True)
     class InputSpec(ShellSpec):
         dimensionality: int = field(
-            metadata={"help_string": "image dimensionality", "mandatory": True, "argstr": "", "allowed_values": {2, 3}}
+            metadata={
+                "help_string": "image dimensionality",
+                "mandatory": True,
+                "argstr": "",
+                "allowed_values": {2, 3},
+            }
         )
 
-        warp_field: PathLike = field(metadata={"help_string": "displacement field", "mandatory": True, "argstr": ""})
+        warp_field: PathLike = field(
+            metadata={
+                "help_string": "displacement field",
+                "mandatory": True,
+                "argstr": "",
+            }
+        )
 
         output_image: str = field(
-            metadata={"help_string": "output image", "argstr": "", "output_file_template": "{warp_field}_jac"}
+            metadata={
+                "help_string": "output image",
+                "argstr": "",
+                "output_file_template": "{warp_field}_jac",
+            }
         )
 
         calculate_log_jacobian: bool = field(
             default=False,
             metadata={
                 "help_string": "calculate log jacobian",
                 "formatter": lambda calculate_log_jacobian: f"{calculate_log_jacobian:d}",
```

### Comparing `pydra_ants-0.0.5/src/pydra/tasks/ants/registration.py` & `pydra_ants-0.1.0/pydra/tasks/ants/v2_5/registration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,135 @@
-__all__ = ["Registration", "registration_syn", "registration_syn_quick"]
-
 from functools import partial
 from os import PathLike
 from pathlib import Path
 from typing import Optional, Sequence
 
 from attrs import NOTHING, define, field
 from pydra.engine.specs import File, ShellOutSpec, ShellSpec, SpecInfo
 from pydra.engine.task import ShellCommandTask
 
+__all__ = ["Registration", "registration_syn", "registration_syn_quick"]
+
+
+def _format_rigid_metric(
+    enable_rigid_stage,
+    rigid_metric,
+    fixed_image,
+    moving_image,
+    rigid_radius,
+    rigid_num_bins,
+    rigid_sampling_strategy,
+    rigid_sampling_rate,
+):
+    return (
+        "-m {}[{},{},1,{},{},{}]".format(
+            rigid_metric,
+            fixed_image,
+            moving_image,
+            rigid_num_bins if rigid_metric in {"MI", "Mattes"} else rigid_radius,
+            rigid_sampling_strategy,
+            rigid_sampling_rate,
+        )
+        if enable_rigid_stage
+        else ""
+    )
+
+
+def _format_affine_metric(
+    enable_affine_stage,
+    affine_metric,
+    fixed_image,
+    moving_image,
+    affine_radius,
+    affine_num_bins,
+    affine_sampling_strategy,
+    affine_sampling_rate,
+):
+    return (
+        "-m {}[{},{},1,{},{},{}]".format(
+            affine_metric,
+            fixed_image,
+            moving_image,
+            affine_num_bins if affine_metric in {"MI", "Mattes"} else affine_radius,
+            affine_sampling_strategy,
+            affine_sampling_rate,
+        )
+        if enable_affine_stage
+        else ""
+    )
+
+
+def _format_syn_metric(
+    enable_syn_stage,
+    syn_metric,
+    fixed_image,
+    moving_image,
+    syn_radius,
+    syn_num_bins,
+    syn_sampling_strategy,
+    syn_sampling_rate,
+):
+    return (
+        "-m {}[{},{},1,{},{},{}]".format(
+            syn_metric,
+            fixed_image,
+            moving_image,
+            syn_num_bins if syn_metric in {"MI", "Mattes"} else syn_radius,
+            syn_sampling_strategy,
+            syn_sampling_rate,
+        )
+        if enable_syn_stage
+        else ""
+    )
+
+
+def _format_syn_transform_type(
+    enable_syn_stage,
+    syn_transform_type,
+    syn_gradient_step,
+    syn_flow_sigma,
+    syn_total_sigma,
+    syn_spline_distance,
+    syn_spline_order,
+):
+    return (
+        "-t {}[{}]".format(
+            syn_transform_type,
+            (
+                f"{syn_gradient_step},{syn_spline_distance},0,{syn_spline_order}"
+                if syn_transform_type == "BSplineSyn"
+                else f"{syn_gradient_step},{syn_flow_sigma},{syn_total_sigma}"
+            ),
+        )
+        if enable_syn_stage
+        else ""
+    )
+
 
 class Registration(ShellCommandTask):
     """Task definition for antsRegistration."""
 
     @define(kw_only=True)
     class InputSpec(ShellSpec):
         dimensionality: int = field(
-            default=3, metadata={"help_string": "image dimensionality", "argstr": "-d", "allowed_values": {2, 3, 4}}
+            default=3,
+            metadata={
+                "help_string": "image dimensionality",
+                "argstr": "-d",
+                "allowed_values": {2, 3, 4},
+            },
         )
 
-        fixed_image: PathLike = field(metadata={"help_string": "fixed image", "mandatory": True})
+        fixed_image: PathLike = field(
+            metadata={"help_string": "fixed image", "mandatory": True}
+        )
 
-        moving_image: PathLike = field(metadata={"help_string": "moving image", "mandatory": True})
+        moving_image: PathLike = field(
+            metadata={"help_string": "moving image", "mandatory": True}
+        )
 
         output_: str = field(
             metadata={
                 "help_string": "output parameter",
                 "readonly": True,
                 "formatter": lambda output_transform_prefix, warped_image, inverse_warped_image: (
                     "-o {}".format(
@@ -33,15 +137,17 @@
                         if all([warped_image, inverse_warped_image])
                         else output_transform_prefix
                     )
                 ),
             }
         )
 
-        output_transform_prefix: str = field(default="output", metadata={"help_string": "output transform prefix"})
+        output_transform_prefix: str = field(
+            default="output", metadata={"help_string": "output transform prefix"}
+        )
 
         warped_image: str = field(
             metadata={
                 "help_string": "warped moving image to fixed image space",
                 "output_file_template": "{moving_image}_warped",
             }
         )
@@ -64,19 +170,19 @@
         interpolation_: str = field(
             metadata={
                 "help_string": "interpolation parameter",
                 "readonly": True,
                 "formatter": lambda interpolator, sigma, alpha, order: (
                     "-n {}{}".format(
                         interpolator,
-                        f"[{sigma},{alpha}]"
-                        if interpolator == "Gaussian"
-                        else f"[{order}]"
-                        if interpolator == "BSpline"
-                        else "",
+                        (
+                            f"[{sigma},{alpha}]"
+                            if interpolator == "Gaussian"
+                            else f"[{order}]" if interpolator == "BSpline" else ""
+                        ),
                     )
                 ),
             }
         )
 
         interpolator: str = field(
             default="Linear",
@@ -91,65 +197,90 @@
                     "WelchWindowedSinc",
                     "HammingWindowedSinc",
                     "LanczosWindowedSinc",
                 },
             },
         )
 
-        sigma: float = field(default=1.0, metadata={"help_string": "sigma parameter for interpolation"})
+        sigma: float = field(
+            default=1.0, metadata={"help_string": "sigma parameter for interpolation"}
+        )
 
-        alpha: float = field(default=1.0, metadata={"help_string": "alpha parameter for interpolation"})
+        alpha: float = field(
+            default=1.0, metadata={"help_string": "alpha parameter for interpolation"}
+        )
 
-        order: int = field(default=3, metadata={"help_string": "order parameter for interpolation"})
+        order: int = field(
+            default=3, metadata={"help_string": "order parameter for interpolation"}
+        )
 
         masks_: str = field(
             metadata={
                 "help_string": "masks parameter",
                 "readonly": True,
                 "formatter": lambda fixed_mask, moving_mask: (
-                    f"-x [{fixed_mask or 'NULL'},{moving_mask or 'NULL'}]" if any([fixed_mask, moving_mask]) else ""
+                    f"-x [{fixed_mask or 'NULL'},{moving_mask or 'NULL'}]"
+                    if any([fixed_mask, moving_mask])
+                    else ""
                 ),
             }
         )
 
-        fixed_mask: PathLike = field(metadata={"help_string": "mask applied to the fixed image"})
+        fixed_mask: PathLike = field(
+            metadata={"help_string": "mask applied to the fixed image"}
+        )
 
-        moving_mask: PathLike = field(metadata={"help_string": "mask applied to the moving image"})
+        moving_mask: PathLike = field(
+            metadata={"help_string": "mask applied to the moving image"}
+        )
 
         use_histogram_matching: bool = field(
             default=False,
             metadata={
                 "help_string": "use histogram matching",
                 "formatter": lambda use_histogram_matching: f"-u {use_histogram_matching:d}",
             },
         )
 
         winsorize_image_intensities: bool = field(
             default=False,
             metadata={
                 "help_string": "winsorize image intensities",
                 "formatter": lambda winsorize_image_intensities, lower_quantile, upper_quantile: (
-                    f"-w [{lower_quantile},{upper_quantile}]" if winsorize_image_intensities else ""
+                    f"-w [{lower_quantile},{upper_quantile}]"
+                    if winsorize_image_intensities
+                    else ""
                 ),
             },
         )
 
-        lower_quantile: float = field(default=0.0, metadata={"help_string": "lower quantile"})
+        lower_quantile: float = field(
+            default=0.0, metadata={"help_string": "lower quantile"}
+        )
 
-        upper_quantile: float = field(default=1.0, metadata={"help_string": "upper quantile"})
+        upper_quantile: float = field(
+            default=1.0, metadata={"help_string": "upper quantile"}
+        )
 
         initial_fixed_transforms: Sequence[PathLike] = field(
             metadata={
                 "help_string": "initialize composite fixed transform with these transforms",
                 "formatter": lambda initial_fixed_transforms, invert_fixed_transforms: (
                     ""
                     if not initial_fixed_transforms
-                    else " ".join(f"-q {x}" for x in initial_fixed_transforms)
-                    if not invert_fixed_transforms
-                    else " ".join(f"-q [{x},{y:d}]" for x, y in zip(initial_fixed_transforms, invert_fixed_transforms))
+                    else (
+                        " ".join(f"-q {x}" for x in initial_fixed_transforms)
+                        if not invert_fixed_transforms
+                        else " ".join(
+                            f"-q [{x},{y:d}]"
+                            for x, y in zip(
+                                initial_fixed_transforms, invert_fixed_transforms
+                            )
+                        )
+                    )
                 ),
             }
         )
 
         invert_fixed_transforms: Sequence[bool] = field(
             metadata={
                 "help_string": "specify which initial fixed transforms to invert",
@@ -159,337 +290,391 @@
 
         initial_moving_transforms: Sequence[PathLike] = field(
             metadata={
                 "help_string": "initialize composite moving transform with these transforms",
                 "formatter": lambda initial_moving_transforms, invert_moving_transforms, fixed_image, moving_image: (
                     f"-r [{fixed_image},{moving_image},1]"
                     if not initial_moving_transforms
-                    else " ".join(f"-r {x}" for x in initial_moving_transforms)
-                    if not invert_moving_transforms
-                    else " ".join(
-                        f"-r [{x},{y:d}]" for x, y in zip(initial_moving_transforms, invert_moving_transforms)
+                    else (
+                        " ".join(f"-r {x}" for x in initial_moving_transforms)
+                        if not invert_moving_transforms
+                        else " ".join(
+                            f"-r [{x},{y:d}]"
+                            for x, y in zip(
+                                initial_moving_transforms, invert_moving_transforms
+                            )
+                        )
                     )
                 ),
             }
         )
 
         invert_moving_transforms: Sequence[bool] = field(
             metadata={
                 "help_string": "specify which initial moving transforms to invert",
                 "requires": {"initial_moving_transforms"},
             }
         )
 
-        enable_rigid_stage = field(default=True, metadata={"help_string": "enable rigid registration stage"})
+        enable_rigid_stage = field(
+            default=True, metadata={"help_string": "enable rigid registration stage"}
+        )
 
         rigid_transform_type: str = field(
             default="Rigid",
             metadata={
                 "help_string": "transform type for rigid stage",
                 "allowed_values": {"Rigid", "Translation"},
                 "formatter": lambda enable_rigid_stage, rigid_transform_type, rigid_gradient_step: (
-                    f"-t {rigid_transform_type}[{rigid_gradient_step}]" if enable_rigid_stage else ""
+                    f"-t {rigid_transform_type}[{rigid_gradient_step}]"
+                    if enable_rigid_stage
+                    else ""
                 ),
             },
         )
 
-        rigid_gradient_step: bool = field(default=0.1, metadata={"help_string": "gradient step for rigid stage"})
+        rigid_gradient_step: bool = field(
+            default=0.1, metadata={"help_string": "gradient step for rigid stage"}
+        )
 
         rigid_metric: str = field(
             metadata={
                 "help_string": "rigid metric parameter",
                 "allowed_values": {"CC", "MI", "Mattes", "MeanSquares", "Demons", "GC"},
-                "formatter": lambda enable_rigid_stage, rigid_metric, fixed_image, moving_image, rigid_radius, rigid_num_bins, rigid_sampling_strategy, rigid_sampling_rate: (
-                    "-m {}[{},{},1,{},{},{}]".format(
-                        rigid_metric,
-                        fixed_image,
-                        moving_image,
-                        rigid_num_bins if rigid_metric in {"MI", "Mattes"} else rigid_radius,
-                        rigid_sampling_strategy,
-                        rigid_sampling_rate,
-                    )
-                    if enable_rigid_stage
-                    else ""
-                ),
+                "formatter": _format_rigid_metric,
             }
         )
 
-        rigid_radius: int = field(default=4, metadata={"help_string": "radius for rigid stage"})
+        rigid_radius: int = field(
+            default=4, metadata={"help_string": "radius for rigid stage"}
+        )
 
-        rigid_num_bins: int = field(default=32, metadata={"help_string": "number of bins for rigid stage"})
+        rigid_num_bins: int = field(
+            default=32, metadata={"help_string": "number of bins for rigid stage"}
+        )
 
         rigid_sampling_strategy: str = field(
             default="None",
             metadata={
                 "help_string": "sampling strategy for rigid stage",
                 "allowed_values": {"None", "Regular", "Random"},
             },
         )
 
-        rigid_sampling_rate: float = field(default=1.0, metadata={"help_string": "sampling rate for rigid stage"})
+        rigid_sampling_rate: float = field(
+            default=1.0, metadata={"help_string": "sampling rate for rigid stage"}
+        )
 
         rigid_convergence_: Sequence[int] = field(
             metadata={
                 "help_string": "convergence parameter for rigid stage",
                 "readonly": True,
                 "formatter": lambda enable_rigid_stage, rigid_num_iterations, rigid_threshold, rigid_window_size: (
                     "-c [{},{},{}]".format(
-                        "x".join(str(c) for c in rigid_num_iterations), rigid_threshold, rigid_window_size
+                        "x".join(str(c) for c in rigid_num_iterations),
+                        rigid_threshold,
+                        rigid_window_size,
                     )
                     if enable_rigid_stage
                     else ""
                 ),
             },
         )
 
         rigid_num_iterations: Sequence[int] = field(
-            default=(1000, 500, 250, 0), metadata={"help_string": "number of iterations for rigid stage"}
+            default=(1000, 500, 250, 0),
+            metadata={"help_string": "number of iterations for rigid stage"},
         )
 
-        rigid_threshold: float = field(default=1e-6, metadata={"help_string": "convergence threshold for rigid stage"})
+        rigid_threshold: float = field(
+            default=1e-6,
+            metadata={"help_string": "convergence threshold for rigid stage"},
+        )
 
-        rigid_window_size: int = field(default=10, metadata={"help_string": "convergence window size for rigid stage"})
+        rigid_window_size: int = field(
+            default=10,
+            metadata={"help_string": "convergence window size for rigid stage"},
+        )
 
         rigid_shrink_factors: Sequence[int] = field(
             default=(8, 4, 2, 1),
             metadata={
                 "help_string": "shrink factors for rigid stage",
                 "formatter": lambda enable_rigid_stage, rigid_shrink_factors: (
-                    "-f {}".format("x".join(str(f) for f in rigid_shrink_factors)) if enable_rigid_stage else ""
+                    "-f {}".format("x".join(str(f) for f in rigid_shrink_factors))
+                    if enable_rigid_stage
+                    else ""
                 ),
             },
         )
 
         rigid_smoothing_sigmas: Sequence[int] = field(
             default=(3, 2, 1, 0),
             metadata={
                 "help_string": "smoothing sigmas for rigid stage",
                 "formatter": lambda enable_rigid_stage, rigid_smoothing_sigmas, rigid_smoothing_units: (
-                    "-s {}{}".format("x".join(str(s) for s in rigid_smoothing_sigmas), rigid_smoothing_units)
+                    "-s {}{}".format(
+                        "x".join(str(s) for s in rigid_smoothing_sigmas),
+                        rigid_smoothing_units,
+                    )
                     if enable_rigid_stage
                     else ""
                 ),
             },
         )
 
         rigid_smoothing_units: str = field(
             default="vox",
-            metadata={"help_string": "smoothing units for rigid stage", "allowed_values": {"vox", "mm"}},
+            metadata={
+                "help_string": "smoothing units for rigid stage",
+                "allowed_values": {"vox", "mm"},
+            },
         )
 
-        enable_affine_stage: bool = field(default=True, metadata={"help_string": "enable affine registration stage"})
+        enable_affine_stage: bool = field(
+            default=True, metadata={"help_string": "enable affine registration stage"}
+        )
 
         affine_transform_type: str = field(
             default="Affine",
             metadata={
                 "help_string": "transform type for affine stage",
                 "allowed_values": {"Affine", "CompositeAffine", "Similarity"},
                 "formatter": lambda enable_affine_stage, affine_transform_type, affine_gradient_step: (
-                    f"-t {affine_transform_type}[{affine_gradient_step}]" if enable_affine_stage else ""
+                    f"-t {affine_transform_type}[{affine_gradient_step}]"
+                    if enable_affine_stage
+                    else ""
                 ),
             },
         )
 
-        affine_gradient_step: bool = field(default=0.1, metadata={"help_string": "gradient step for affine stage"})
+        affine_gradient_step: bool = field(
+            default=0.1, metadata={"help_string": "gradient step for affine stage"}
+        )
 
         affine_metric: str = field(
             metadata={
                 "help_string": "metric parameter for affine stage",
                 "allowed_values": {"CC", "MI", "Mattes", "MeanSquares", "Demons", "GC"},
-                "formatter": lambda enable_affine_stage, affine_metric, fixed_image, moving_image, affine_radius, affine_num_bins, affine_sampling_strategy, affine_sampling_rate: (
-                    "-m {}[{},{},1,{},{},{}]".format(
-                        affine_metric,
-                        fixed_image,
-                        moving_image,
-                        affine_num_bins if affine_metric in {"MI", "Mattes"} else affine_radius,
-                        affine_sampling_strategy,
-                        affine_sampling_rate,
-                    )
-                    if enable_affine_stage
-                    else ""
-                ),
+                "formatter": _format_affine_metric,
             }
         )
 
-        affine_radius: int = field(default=4, metadata={"help_string": "radius for affine stage"})
+        affine_radius: int = field(
+            default=4, metadata={"help_string": "radius for affine stage"}
+        )
 
-        affine_num_bins: int = field(default=32, metadata={"help_string": "number of bins for affine stage"})
+        affine_num_bins: int = field(
+            default=32, metadata={"help_string": "number of bins for affine stage"}
+        )
 
         affine_sampling_strategy: str = field(
             default="None",
             metadata={
                 "help_string": "sampling strategy for affine stage",
                 "allowed_values": {"None", "Regular", "Random"},
             },
         )
 
-        affine_sampling_rate: float = field(default=1.0, metadata={"help_string": "sampling rate for affine stage"})
+        affine_sampling_rate: float = field(
+            default=1.0, metadata={"help_string": "sampling rate for affine stage"}
+        )
 
         affine_convergence_: Sequence[int] = field(
             metadata={
                 "help_string": "convergence parameter for affine stage",
                 "readonly": True,
                 "formatter": lambda enable_affine_stage, affine_num_iterations, affine_threshold, affine_window_size: (
                     "-c [{},{},{}]".format(
-                        "x".join(str(c) for c in affine_num_iterations), affine_threshold, affine_window_size
+                        "x".join(str(c) for c in affine_num_iterations),
+                        affine_threshold,
+                        affine_window_size,
                     )
                     if enable_affine_stage
                     else ""
                 ),
             },
         )
 
         affine_num_iterations: Sequence[int] = field(
-            default=(1000, 500, 250, 0), metadata={"help_string": "number of iterations for affine stage"}
+            default=(1000, 500, 250, 0),
+            metadata={"help_string": "number of iterations for affine stage"},
         )
 
         affine_threshold: float = field(
-            default=1e-6, metadata={"help_string": "convergence threshold for affine stage"}
+            default=1e-6,
+            metadata={"help_string": "convergence threshold for affine stage"},
         )
 
         affine_window_size: int = field(
-            default=10, metadata={"help_string": "convergence window size for affine stage"}
+            default=10,
+            metadata={"help_string": "convergence window size for affine stage"},
         )
 
         affine_shrink_factors: Sequence[int] = field(
             default=(8, 4, 2, 1),
             metadata={
                 "help_string": "shrink factors for affine stage",
                 "formatter": lambda enable_affine_stage, affine_shrink_factors: (
-                    "-f {}".format("x".join(str(f) for f in affine_shrink_factors)) if enable_affine_stage else ""
+                    "-f {}".format("x".join(str(f) for f in affine_shrink_factors))
+                    if enable_affine_stage
+                    else ""
                 ),
             },
         )
 
         affine_smoothing_sigmas: Sequence[int] = field(
             default=(3, 2, 1, 0),
             metadata={
                 "help_string": "smoothing sigmas for affine stage",
                 "formatter": lambda enable_affine_stage, affine_smoothing_sigmas, affine_smoothing_units: (
-                    "-s {}{}".format("x".join(str(s) for s in affine_smoothing_sigmas), affine_smoothing_units)
+                    "-s {}{}".format(
+                        "x".join(str(s) for s in affine_smoothing_sigmas),
+                        affine_smoothing_units,
+                    )
                     if enable_affine_stage
                     else ""
                 ),
             },
         )
 
         affine_smoothing_units: str = field(
             default="vox",
-            metadata={"help_string": "smoothing units for affine stage", "allowed_values": {"vox", "mm"}},
+            metadata={
+                "help_string": "smoothing units for affine stage",
+                "allowed_values": {"vox", "mm"},
+            },
         )
 
-        enable_syn_stage: str = field(default=True, metadata={"help_string": "enable SyN registration stage"})
+        enable_syn_stage: str = field(
+            default=True, metadata={"help_string": "enable SyN registration stage"}
+        )
 
         syn_transform_type: str = field(
             default="Syn",
             metadata={
                 "help_string": "transform type for SyN stage",
                 "allowed_values": {"GaussianDisplacementField", "SyN", "BSplineSyN"},
-                "formatter": lambda enable_syn_stage, syn_transform_type, syn_gradient_step, syn_flow_sigma, syn_total_sigma, syn_spline_distance, syn_spline_order: (
-                    "-t {}[{}]".format(
-                        syn_transform_type,
-                        f"{syn_gradient_step},{syn_spline_distance},0,{syn_spline_order}"
-                        if syn_transform_type == "BSplineSyn"
-                        else f"{syn_gradient_step},{syn_flow_sigma},{syn_total_sigma}",
-                    )
-                    if enable_syn_stage
-                    else ""
-                ),
+                "formatter": _format_syn_transform_type,
             },
         )
 
-        syn_gradient_step: bool = field(default=0.1, metadata={"help_string": "gradient step for SyN stage"})
+        syn_gradient_step: bool = field(
+            default=0.1, metadata={"help_string": "gradient step for SyN stage"}
+        )
 
-        syn_flow_sigma: float = field(default=3, metadata={"help_string": "sigma for flow field in SyN stage"})
+        syn_flow_sigma: float = field(
+            default=3, metadata={"help_string": "sigma for flow field in SyN stage"}
+        )
 
-        syn_total_sigma: float = field(default=0, metadata={"help_string": "sigma for total field in SyN stage"})
+        syn_total_sigma: float = field(
+            default=0, metadata={"help_string": "sigma for total field in SyN stage"}
+        )
 
-        syn_spline_distance: int = field(default=26, metadata={"help_string": "spline distance for SyN stage"})
+        syn_spline_distance: int = field(
+            default=26, metadata={"help_string": "spline distance for SyN stage"}
+        )
 
-        syn_spline_order: int = field(default=3, metadata={"help_string": "spline order for SyN stage"})
+        syn_spline_order: int = field(
+            default=3, metadata={"help_string": "spline order for SyN stage"}
+        )
 
         syn_metric: str = field(
             default="MI",
             metadata={
                 "help_string": "metric for SyN stage",
                 "allowed_values": {"CC", "MI", "Mattes", "MeanSquares", "Demons", "GC"},
-                "formatter": lambda enable_syn_stage, syn_metric, fixed_image, moving_image, syn_radius, syn_num_bins, syn_sampling_strategy, syn_sampling_rate: (
-                    "-m {}[{},{},1,{},{},{}]".format(
-                        syn_metric,
-                        fixed_image,
-                        moving_image,
-                        syn_num_bins if syn_metric in {"MI", "Mattes"} else syn_radius,
-                        syn_sampling_strategy,
-                        syn_sampling_rate,
-                    )
-                    if enable_syn_stage
-                    else ""
-                ),
+                "formatter": _format_syn_metric,
             },
         )
 
-        syn_radius: int = field(default=4, metadata={"help_string": "radius for SyN stage"})
+        syn_radius: int = field(
+            default=4, metadata={"help_string": "radius for SyN stage"}
+        )
 
-        syn_num_bins: int = field(default=32, metadata={"help_string": "number of bins for SyN stage"})
+        syn_num_bins: int = field(
+            default=32, metadata={"help_string": "number of bins for SyN stage"}
+        )
 
         syn_sampling_strategy: str = field(
             default="None",
             metadata={
                 "help_string": "sampling strategy for SyN stage",
                 "allowed_values": {"None", "Regular", "Random"},
             },
         )
 
-        syn_sampling_rate: float = field(default=1.0, metadata={"help_string": "sampling rate for SyN stage"})
+        syn_sampling_rate: float = field(
+            default=1.0, metadata={"help_string": "sampling rate for SyN stage"}
+        )
 
         syn_convergence_: str = field(
             metadata={
                 "help_string": "convergence parameter for SyN stage",
                 "readonly": True,
                 "formatter": lambda enable_syn_stage, syn_num_iterations, syn_threshold, syn_window_size: (
-                    "-c [{},{},{}]".format("x".join(str(c) for c in syn_num_iterations), syn_threshold, syn_window_size)
+                    "-c [{},{},{}]".format(
+                        "x".join(str(c) for c in syn_num_iterations),
+                        syn_threshold,
+                        syn_window_size,
+                    )
                     if enable_syn_stage
                     else ""
                 ),
             },
         )
 
         syn_num_iterations: Sequence[int] = field(
-            default=(100, 70, 50, 20), metadata={"help_string": "number of iterations for SyN stage"}
+            default=(100, 70, 50, 20),
+            metadata={"help_string": "number of iterations for SyN stage"},
         )
 
-        syn_threshold: float = field(default=1e-6, metadata={"help_string": "convergence threshold for SyN stage"})
+        syn_threshold: float = field(
+            default=1e-6,
+            metadata={"help_string": "convergence threshold for SyN stage"},
+        )
 
-        syn_window_size: int = field(default=10, metadata={"help_string": "convergence window size for SyN stage"})
+        syn_window_size: int = field(
+            default=10,
+            metadata={"help_string": "convergence window size for SyN stage"},
+        )
 
         syn_shrink_factors: Sequence[int] = field(
             default=(8, 4, 2, 1),
             metadata={
                 "help_string": "shrink factors for SyN stage",
                 "formatter": lambda enable_syn_stage, syn_shrink_factors: (
-                    "-f {}".format("x".join(str(f) for f in syn_shrink_factors)) if enable_syn_stage else ""
+                    "-f {}".format("x".join(str(f) for f in syn_shrink_factors))
+                    if enable_syn_stage
+                    else ""
                 ),
             },
         )
 
         syn_smoothing_sigmas: Sequence[int] = field(
             default=(3, 2, 1, 0),
             metadata={
                 "help_string": "smoothing sigmas for SyN stage",
                 "formatter": lambda enable_syn_stage, syn_smoothing_sigmas, syn_smoothing_units: (
-                    "-s {}{}".format("x".join(str(s) for s in syn_smoothing_sigmas), syn_smoothing_units)
+                    "-s {}{}".format(
+                        "x".join(str(s) for s in syn_smoothing_sigmas),
+                        syn_smoothing_units,
+                    )
                     if enable_syn_stage
                     else ""
                 ),
             },
         )
 
         syn_smoothing_units: str = field(
             default="vox",
-            metadata={"help_string": "smoothing units for SyN stage", "allowed_values": {"vox", "mm"}},
+            metadata={
+                "help_string": "smoothing units for SyN stage",
+                "allowed_values": {"vox", "mm"},
+            },
         )
 
         use_float_precision: bool = field(
             default=False,
             metadata={
                 "help_string": "use float precision instead of double",
                 "formatter": lambda use_float_precision: f"--float {use_float_precision:d}",
@@ -500,15 +685,17 @@
             default=False,
             metadata={
                 "help_string": "save output transforms to MINC format",
                 "formatter": lambda use_minc_format: f"--minc {use_minc_format:d}",
             },
         )
 
-        random_seed: int = field(metadata={"help_string": "random seed", "argstr": "--random-seed"})
+        random_seed: int = field(
+            metadata={"help_string": "random seed", "argstr": "--random-seed"}
+        )
 
         verbose: bool = field(
             default=False,
             metadata={
                 "help_string": "enable verbose output",
                 "formatter": lambda verbose: f"--verbose {verbose:d}",
             },
@@ -519,15 +706,17 @@
     @define(kw_only=True)
     class OutputSpec(ShellOutSpec):
         affine_transform: File = field(
             metadata={
                 "help_string": "affine transform",
                 "callable": lambda output_transform_prefix, use_minc_format: (
                     Path.cwd()
-                    / "{}0GenericAffine{}".format(output_transform_prefix, ".xfm" if use_minc_format else ".mat")
+                    / "{}0GenericAffine{}".format(
+                        output_transform_prefix, ".xfm" if use_minc_format else ".mat"
+                    )
                 ),
             }
         )
 
         warp_field: File = field(
             metadata={
                 "help_string": "warp field from moving to fixed image space",
@@ -544,14 +733,15 @@
 
     output_spec = SpecInfo(name="Output", bases=(OutputSpec,))
 
     executable = "antsRegistration"
 
 
 def registration_syn(
+    *,
     dimensionality: int,
     fixed_image: PathLike,
     moving_image: PathLike,
     output_prefix: str = "output",
     transform_type: str = "s",
     num_bins: int = 32,
     gradient_step: float = 0.1,
@@ -719,15 +909,19 @@
         enable_syn_stage=transform_type[0] in {"b", "s"},
         syn_transform_type="BSplineSyn" if transform_type[0] == "b" else "Syn",
         syn_gradient_step=gradient_step,
         syn_spline_distance=spline_distance,
         syn_metric="CC" if reproducible else "MI",
         syn_radius=radius,
         syn_num_bins=num_bins,
-        syn_num_iterations=((100, 100, 70, 50, 0 if quick else 20) if large else (100, 70, 50, 0 if quick else 20)),
+        syn_num_iterations=(
+            (100, 100, 70, 50, 0 if quick else 20)
+            if large
+            else (100, 70, 50, 0 if quick else 20)
+        ),
         syn_shrink_factors=(10, 6, 4, 2, 1) if large else (8, 4, 2, 1),
         syn_smoothing_sigmas=(5, 3, 2, 1, 0) if large else (3, 2, 1, 0),
         use_histogram_matching=use_histogram_matching,
         use_float_precision=use_float_precision,
         use_minc_format=use_minc_format,
         random_seed=random_seed or (1 if reproducible else NOTHING),
         verbose=verbose,
```

### Comparing `pydra_ants-0.0.5/.gitignore` & `pydra_ants-0.1.0/.gitignore`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
 var/
 wheels/
+pip-wheel-metadata/
 share/python-wheels/
 *.egg-info/
 .installed.cfg
 *.egg
 MANIFEST
 
 # PyInstaller
@@ -82,14 +83,25 @@
 profile_default/
 ipython_config.py
 
 # Hatch
 .hatch/
 
 # PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
+# pyenv
+.python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow
 __pypackages__/
 
 # Celery stuff
 celerybeat-schedule
 celerybeat.pid
 
 # SageMath parsed files
@@ -134,7 +146,22 @@
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .fleet/
 .idea/
 
 # macOS
 .DS_Store
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
+# Generated files
+/pydra/tasks/ants/_version.py
+/pydra/tasks/ants/nipype_ports
```

### Comparing `pydra_ants-0.0.5/LICENSE` & `pydra_ants-0.1.0/LICENSE`

 * *Files identical despite different names*

