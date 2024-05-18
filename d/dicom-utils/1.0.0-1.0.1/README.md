# Comparing `tmp/dicom-utils-1.0.0.tar.gz` & `tmp/dicom-utils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicom-utils-1.0.0.tar", last modified: Sat May 18 12:24:28 2024, max compression
+gzip compressed data, was "dicom-utils-1.0.1.tar", last modified: Sat May 18 12:44:35 2024, max compression
```

## Comparing `dicom-utils-1.0.0.tar` & `dicom-utils-1.0.1.tar`

### file list

```diff
@@ -1,83 +1,77 @@
--rw-r--r--   0        0        0    11357 2021-04-29 16:25:52.009578 dicom-utils-1.0.0/LICENSE
--rw-r--r--   0        0        0     1828 2023-04-04 02:03:36.613199 dicom-utils-1.0.0/README.md
--rw-r--r--   0        0        0     1863 2023-10-02 16:04:01.973992 dicom-utils-1.0.0/dicom_utils/__init__.py
--rw-r--r--   0        0        0     3704 2023-07-14 19:17:46.074907 dicom-utils-1.0.0/dicom_utils/__main__.py
--rw-r--r--   0        0        0   190485 2022-01-17 12:35:58.517804 dicom-utils-1.0.0/dicom_utils/_tag_enum.py
--rw-r--r--   0        0        0     2551 2024-05-16 16:37:53.391489 dicom-utils-1.0.0/dicom_utils/anonymize.py
--rw-r--r--   0        0        0     6276 2024-03-01 13:38:29.845529 dicom-utils-1.0.0/dicom_utils/basic_offset_table.py
--rw-r--r--   0        0        0      201 2022-01-07 17:53:52.694567 dicom-utils-1.0.0/dicom_utils/cli/__init__.py
--rw-r--r--   0        0        0     1543 2022-01-07 17:53:52.694567 dicom-utils-1.0.0/dicom_utils/cli/cat.py
--rw-r--r--   0        0        0     2161 2023-03-13 18:57:48.339255 dicom-utils-1.0.0/dicom_utils/cli/decompress.py
--rw-r--r--   0        0        0     7052 2023-07-06 16:13:53.840752 dicom-utils-1.0.0/dicom_utils/cli/dicom2img.py
--rw-r--r--   0        0        0     2602 2022-05-05 16:22:18.336416 dicom-utils-1.0.0/dicom_utils/cli/dicom_types.py
--rw-r--r--   0        0        0      872 2022-10-21 15:46:52.840194 dicom-utils-1.0.0/dicom_utils/cli/dicomphi.py
--rw-r--r--   0        0        0     2450 2022-05-05 16:22:18.336416 dicom-utils-1.0.0/dicom_utils/cli/find.py
--rw-r--r--   0        0        0     2311 2023-07-06 16:13:53.840752 dicom-utils-1.0.0/dicom_utils/cli/hash.py
--rw-r--r--   0        0        0      536 2023-07-14 19:17:46.074907 dicom-utils-1.0.0/dicom_utils/cli/merge_series.py
--rw-r--r--   0        0        0     3583 2023-10-02 16:04:01.973992 dicom-utils-1.0.0/dicom_utils/cli/organize.py
--rw-r--r--   0        0        0     2804 2023-07-06 16:13:53.840752 dicom-utils-1.0.0/dicom_utils/cli/overlap.py
--rw-r--r--   0        0        0     2083 2023-03-13 18:57:48.343255 dicom-utils-1.0.0/dicom_utils/cli/project.py
--rw-r--r--   0        0        0      968 2022-01-07 17:53:52.694567 dicom-utils-1.0.0/dicom_utils/cli/strip.py
--rw-r--r--   0        0        0     1054 2022-01-17 12:35:58.521804 dicom-utils-1.0.0/dicom_utils/cli/validate.py
--rw-r--r--   0        0        0     1249 2023-02-07 15:32:47.657116 dicom-utils-1.0.0/dicom_utils/container/__init__.py
--rw-r--r--   0        0        0    24168 2024-03-01 13:38:29.845529 dicom-utils-1.0.0/dicom_utils/container/collection.py
--rw-r--r--   0        0        0     5689 2024-01-03 19:32:01.937743 dicom-utils-1.0.0/dicom_utils/container/group.py
--rw-r--r--   0        0        0      206 2022-06-09 11:36:01.591689 dicom-utils-1.0.0/dicom_utils/container/helpers.py
--rw-r--r--   0        0        0     9431 2023-10-02 16:04:01.973992 dicom-utils-1.0.0/dicom_utils/container/input.py
--rw-r--r--   0        0        0    14764 2024-03-01 13:38:29.845529 dicom-utils-1.0.0/dicom_utils/container/output.py
--rw-r--r--   0        0        0     5619 2023-09-14 17:41:20.066426 dicom-utils-1.0.0/dicom_utils/container/protocols.py
--rw-r--r--   0        0        0    48079 2024-03-01 13:38:29.845529 dicom-utils-1.0.0/dicom_utils/container/record.py
--rw-r--r--   0        0        0    19074 2024-04-05 20:23:26.698277 dicom-utils-1.0.0/dicom_utils/dicom.py
--rw-r--r--   0        0        0    10877 2024-03-01 13:38:29.845529 dicom-utils-1.0.0/dicom_utils/dicom_factory.py
--rw-r--r--   0        0        0     2380 2022-01-10 22:39:26.524874 dicom-utils-1.0.0/dicom_utils/find_phi.py
--rw-r--r--   0        0        0     1283 2023-07-07 14:38:41.967451 dicom-utils-1.0.0/dicom_utils/logging.py
--rw-r--r--   0        0        0     1740 2023-10-02 16:04:01.977992 dicom-utils-1.0.0/dicom_utils/merge_series.py
--rw-r--r--   0        0        0     5308 2022-01-17 12:35:58.521804 dicom-utils-1.0.0/dicom_utils/metadata.py
--rw-r--r--   0        0        0     3064 2022-05-11 15:09:00.984495 dicom-utils-1.0.0/dicom_utils/private.py
--rw-r--r--   0        0        0      822 2022-01-17 12:35:58.521804 dicom-utils-1.0.0/dicom_utils/tags.py
--rw-r--r--   0        0        0    22771 2024-03-01 13:38:29.845529 dicom-utils-1.0.0/dicom_utils/types.py
--rw-r--r--   0        0        0    13348 2022-01-17 12:35:58.521804 dicom-utils-1.0.0/dicom_utils/validation.py
--rw-r--r--   0        0        0      122 2024-05-18 12:23:44.274223 dicom-utils-1.0.0/dicom_utils/version.py
--rw-r--r--   0        0        0    12473 2024-03-01 15:54:58.799103 dicom-utils-1.0.0/dicom_utils/visualize.py
--rw-r--r--   0        0        0    15165 2024-03-01 13:38:29.845529 dicom-utils-1.0.0/dicom_utils/volume.py
--rw-r--r--   0        0        0     2734 2024-05-18 12:20:58.296554 dicom-utils-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       37 2021-06-06 02:14:45.527927 dicom-utils-1.0.0/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      194 2021-06-06 02:14:45.527927 dicom-utils-1.0.0/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      295 2021-06-06 02:14:45.527927 dicom-utils-1.0.0/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0     1923 2023-02-15 22:33:27.228900 dicom-utils-1.0.0/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0   136507 2023-02-23 15:17:38.526718 dicom-utils-1.0.0/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-02-23 15:17:38.530718 dicom-utils-1.0.0/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     3479 2024-03-01 13:38:29.845529 dicom-utils-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0   105872 2023-03-13 18:57:48.347255 dicom-utils-1.0.0/tests/jpeg2k_3d.dcm
--rw-r--r--   0        0        0     2446 2024-03-01 13:38:29.845529 dicom-utils-1.0.0/tests/test_anonymize.py
--rw-r--r--   0        0        0     4739 2023-10-02 16:04:01.981992 dicom-utils-1.0.0/tests/test_basic_offset_table.py
--rw-r--r--   0        0        0       46 2022-02-17 16:14:02.173636 dicom-utils-1.0.0/tests/test_container/conftest.py
--rw-r--r--   0        0        0    12279 2023-10-02 16:04:01.981992 dicom-utils-1.0.0/tests/test_container/test_collection.py
--rw-r--r--   0        0        0      958 2023-08-08 14:14:19.859926 dicom-utils-1.0.0/tests/test_container/test_input.py
--rw-r--r--   0        0        0     4741 2023-02-07 15:32:47.661115 dicom-utils-1.0.0/tests/test_container/test_output.py
--rw-r--r--   0        0        0     4803 2022-10-17 15:28:24.000378 dicom-utils-1.0.0/tests/test_container/test_protocols.py
--rw-r--r--   0        0        0    71945 2023-10-02 16:04:01.981992 dicom-utils-1.0.0/tests/test_container/test_record.py
--rw-r--r--   0        0        0    13556 2024-01-03 19:32:01.937743 dicom-utils-1.0.0/tests/test_dicom.py
--rw-r--r--   0        0        0     4039 2024-01-03 19:32:01.941743 dicom-utils-1.0.0/tests/test_dicom_factory.py
--rw-r--r--   0        0        0      828 2021-10-05 16:18:31.866362 dicom-utils-1.0.0/tests/test_logging.py
--rw-r--r--   0        0        0      426 2024-03-01 13:38:29.845529 dicom-utils-1.0.0/tests/test_main/conftest.py
--rw-r--r--   0        0        0      910 2021-06-03 16:06:56.773891 dicom-utils-1.0.0/tests/test_main/test_cat.py
--rw-r--r--   0        0        0     1374 2023-02-07 15:32:47.661115 dicom-utils-1.0.0/tests/test_main/test_decompress.py
--rw-r--r--   0        0        0     3418 2023-07-06 16:13:53.848752 dicom-utils-1.0.0/tests/test_main/test_dicom2img.py
--rw-r--r--   0        0        0      991 2022-05-05 16:22:18.336416 dicom-utils-1.0.0/tests/test_main/test_dicom_types.py
--rw-r--r--   0        0        0      245 2024-03-01 13:38:29.845529 dicom-utils-1.0.0/tests/test_main/test_dicomphi.py
--rw-r--r--   0        0        0     1713 2022-01-17 12:35:58.521804 dicom-utils-1.0.0/tests/test_main/test_find.py
--rw-r--r--   0        0        0      765 2023-07-06 16:13:53.848752 dicom-utils-1.0.0/tests/test_main/test_hash.py
--rw-r--r--   0        0        0     1237 2023-07-14 19:17:46.078907 dicom-utils-1.0.0/tests/test_main/test_merge_series.py
--rw-r--r--   0        0        0     2996 2023-03-13 18:57:48.351255 dicom-utils-1.0.0/tests/test_main/test_organize.py
--rw-r--r--   0        0        0     1332 2023-03-13 18:57:48.351255 dicom-utils-1.0.0/tests/test_main/test_project.py
--rw-r--r--   0        0        0     1502 2022-01-17 12:35:58.521804 dicom-utils-1.0.0/tests/test_main/test_validate.py
--rw-r--r--   0        0        0       46 2021-06-03 16:06:56.773891 dicom-utils-1.0.0/tests/test_metadata.py
--rw-r--r--   0        0        0     1461 2024-03-01 13:38:29.845529 dicom-utils-1.0.0/tests/test_private.py
--rw-r--r--   0        0        0     1081 2022-05-05 16:22:18.340417 dicom-utils-1.0.0/tests/test_silence_warnings.py
--rw-r--r--   0        0        0      985 2021-12-20 22:11:21.920646 dicom-utils-1.0.0/tests/test_strip.py
--rw-r--r--   0        0        0     2389 2022-01-17 12:35:58.521804 dicom-utils-1.0.0/tests/test_tag.py
--rw-r--r--   0        0        0    31052 2023-05-10 12:36:44.058824 dicom-utils-1.0.0/tests/test_types.py
--rw-r--r--   0        0        0     4082 2021-12-20 22:11:21.920646 dicom-utils-1.0.0/tests/test_visualize.py
--rw-r--r--   0        0        0     7411 2023-05-10 12:36:44.058824 dicom-utils-1.0.0/tests/test_volume.py
--rw-r--r--   0        0        0     2082 1970-01-01 00:00:00.000000 dicom-utils-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1828 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/README.md
+-rw-r--r--   0        0        0     1863 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/__init__.py
+-rw-r--r--   0        0        0     3704 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/__main__.py
+-rw-r--r--   0        0        0   190485 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/_tag_enum.py
+-rw-r--r--   0        0        0     2551 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/anonymize.py
+-rw-r--r--   0        0        0     6276 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/basic_offset_table.py
+-rw-r--r--   0        0        0      201 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/cli/__init__.py
+-rw-r--r--   0        0        0     1543 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/cli/cat.py
+-rw-r--r--   0        0        0     2161 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/cli/decompress.py
+-rw-r--r--   0        0        0     7052 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/cli/dicom2img.py
+-rw-r--r--   0        0        0     2602 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/cli/dicom_types.py
+-rw-r--r--   0        0        0      872 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/cli/dicomphi.py
+-rw-r--r--   0        0        0     2450 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/cli/find.py
+-rw-r--r--   0        0        0     2311 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/cli/hash.py
+-rw-r--r--   0        0        0      536 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/cli/merge_series.py
+-rw-r--r--   0        0        0     3583 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/cli/organize.py
+-rw-r--r--   0        0        0     2804 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/cli/overlap.py
+-rw-r--r--   0        0        0     2083 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/cli/project.py
+-rw-r--r--   0        0        0      968 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/cli/strip.py
+-rw-r--r--   0        0        0     1054 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/cli/validate.py
+-rw-r--r--   0        0        0     1249 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/container/__init__.py
+-rw-r--r--   0        0        0    24168 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/container/collection.py
+-rw-r--r--   0        0        0     5689 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/container/group.py
+-rw-r--r--   0        0        0      206 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/container/helpers.py
+-rw-r--r--   0        0        0     9431 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/container/input.py
+-rw-r--r--   0        0        0    14764 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/container/output.py
+-rw-r--r--   0        0        0     5619 2024-05-18 12:42:15.573561 dicom-utils-1.0.1/dicom_utils/container/protocols.py
+-rw-r--r--   0        0        0    48079 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/dicom_utils/container/record.py
+-rw-r--r--   0        0        0    19074 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/dicom_utils/dicom.py
+-rw-r--r--   0        0        0    10877 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/dicom_utils/dicom_factory.py
+-rw-r--r--   0        0        0     2380 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/dicom_utils/find_phi.py
+-rw-r--r--   0        0        0     1283 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/dicom_utils/logging.py
+-rw-r--r--   0        0        0     1740 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/dicom_utils/merge_series.py
+-rw-r--r--   0        0        0     5308 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/dicom_utils/metadata.py
+-rw-r--r--   0        0        0     3064 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/dicom_utils/private.py
+-rw-r--r--   0        0        0      822 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/dicom_utils/tags.py
+-rw-r--r--   0        0        0    22771 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/dicom_utils/types.py
+-rw-r--r--   0        0        0    13348 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/dicom_utils/validation.py
+-rw-r--r--   0        0        0      122 2024-05-18 12:42:23.657530 dicom-utils-1.0.1/dicom_utils/version.py
+-rw-r--r--   0        0        0    12473 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/dicom_utils/visualize.py
+-rw-r--r--   0        0        0    15165 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/dicom_utils/volume.py
+-rw-r--r--   0        0        0     2734 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3479 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0   105872 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/tests/jpeg2k_3d.dcm
+-rw-r--r--   0        0        0     2446 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/tests/test_anonymize.py
+-rw-r--r--   0        0        0     4739 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/tests/test_basic_offset_table.py
+-rw-r--r--   0        0        0       46 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/tests/test_container/conftest.py
+-rw-r--r--   0        0        0    12279 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/tests/test_container/test_collection.py
+-rw-r--r--   0        0        0      958 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/tests/test_container/test_input.py
+-rw-r--r--   0        0        0     4741 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/tests/test_container/test_output.py
+-rw-r--r--   0        0        0     4803 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/tests/test_container/test_protocols.py
+-rw-r--r--   0        0        0    71945 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/tests/test_container/test_record.py
+-rw-r--r--   0        0        0    13556 2024-05-18 12:42:15.577561 dicom-utils-1.0.1/tests/test_dicom.py
+-rw-r--r--   0        0        0     4039 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_dicom_factory.py
+-rw-r--r--   0        0        0      828 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_logging.py
+-rw-r--r--   0        0        0      426 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_main/conftest.py
+-rw-r--r--   0        0        0      910 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_main/test_cat.py
+-rw-r--r--   0        0        0     1374 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_main/test_decompress.py
+-rw-r--r--   0        0        0     3418 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_main/test_dicom2img.py
+-rw-r--r--   0        0        0      991 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_main/test_dicom_types.py
+-rw-r--r--   0        0        0      245 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_main/test_dicomphi.py
+-rw-r--r--   0        0        0     1713 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_main/test_find.py
+-rw-r--r--   0        0        0      765 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_main/test_hash.py
+-rw-r--r--   0        0        0     1237 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_main/test_merge_series.py
+-rw-r--r--   0        0        0     2996 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_main/test_organize.py
+-rw-r--r--   0        0        0     1332 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_main/test_project.py
+-rw-r--r--   0        0        0     1502 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_main/test_validate.py
+-rw-r--r--   0        0        0       46 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_metadata.py
+-rw-r--r--   0        0        0     1461 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_private.py
+-rw-r--r--   0        0        0     1081 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_silence_warnings.py
+-rw-r--r--   0        0        0      985 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_strip.py
+-rw-r--r--   0        0        0     2389 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_tag.py
+-rw-r--r--   0        0        0    31052 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_types.py
+-rw-r--r--   0        0        0     4082 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_visualize.py
+-rw-r--r--   0        0        0     7411 2024-05-18 12:42:15.581561 dicom-utils-1.0.1/tests/test_volume.py
+-rw-r--r--   0        0        0     2082 1970-01-01 00:00:00.000000 dicom-utils-1.0.1/PKG-INFO
```

### Comparing `dicom-utils-1.0.0/LICENSE` & `dicom-utils-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/README.md` & `dicom-utils-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/__init__.py` & `dicom-utils-1.0.1/dicom_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/__main__.py` & `dicom-utils-1.0.1/dicom_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/_tag_enum.py` & `dicom-utils-1.0.1/dicom_utils/_tag_enum.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/anonymize.py` & `dicom-utils-1.0.1/dicom_utils/anonymize.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/basic_offset_table.py` & `dicom-utils-1.0.1/dicom_utils/basic_offset_table.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/cli/cat.py` & `dicom-utils-1.0.1/dicom_utils/cli/cat.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/cli/decompress.py` & `dicom-utils-1.0.1/dicom_utils/cli/decompress.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/cli/dicom2img.py` & `dicom-utils-1.0.1/dicom_utils/cli/dicom2img.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/cli/dicom_types.py` & `dicom-utils-1.0.1/dicom_utils/cli/dicom_types.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/cli/dicomphi.py` & `dicom-utils-1.0.1/dicom_utils/cli/dicomphi.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/cli/find.py` & `dicom-utils-1.0.1/dicom_utils/cli/find.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/cli/hash.py` & `dicom-utils-1.0.1/dicom_utils/cli/hash.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/cli/merge_series.py` & `dicom-utils-1.0.1/dicom_utils/cli/merge_series.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/cli/organize.py` & `dicom-utils-1.0.1/dicom_utils/cli/organize.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/cli/overlap.py` & `dicom-utils-1.0.1/dicom_utils/cli/overlap.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/cli/project.py` & `dicom-utils-1.0.1/dicom_utils/cli/project.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/cli/strip.py` & `dicom-utils-1.0.1/dicom_utils/cli/strip.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/cli/validate.py` & `dicom-utils-1.0.1/dicom_utils/cli/validate.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/container/__init__.py` & `dicom-utils-1.0.1/dicom_utils/container/__init__.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/container/collection.py` & `dicom-utils-1.0.1/dicom_utils/container/collection.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/container/group.py` & `dicom-utils-1.0.1/dicom_utils/container/group.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/container/input.py` & `dicom-utils-1.0.1/dicom_utils/container/input.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/container/output.py` & `dicom-utils-1.0.1/dicom_utils/container/output.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/container/protocols.py` & `dicom-utils-1.0.1/dicom_utils/container/protocols.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/container/record.py` & `dicom-utils-1.0.1/dicom_utils/container/record.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/dicom.py` & `dicom-utils-1.0.1/dicom_utils/dicom.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/dicom_factory.py` & `dicom-utils-1.0.1/dicom_utils/dicom_factory.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/find_phi.py` & `dicom-utils-1.0.1/dicom_utils/find_phi.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/logging.py` & `dicom-utils-1.0.1/dicom_utils/logging.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/merge_series.py` & `dicom-utils-1.0.1/dicom_utils/merge_series.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/metadata.py` & `dicom-utils-1.0.1/dicom_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/private.py` & `dicom-utils-1.0.1/dicom_utils/private.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/tags.py` & `dicom-utils-1.0.1/dicom_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/types.py` & `dicom-utils-1.0.1/dicom_utils/types.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/validation.py` & `dicom-utils-1.0.1/dicom_utils/validation.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/visualize.py` & `dicom-utils-1.0.1/dicom_utils/visualize.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/dicom_utils/volume.py` & `dicom-utils-1.0.1/dicom_utils/volume.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/pyproject.toml` & `dicom-utils-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "pylibjpeg-libjpeg",
     "pylibjpeg-openjpeg",
     "tqdm-multiprocessing",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 dynamic = []
-version = "1.0.0"
+version = "1.0.1"
 
 [project.license]
 text = "Apache"
 
 [project.optional-dependencies]
 j2k = [
     "pynvjpeg2k",
```

### Comparing `dicom-utils-1.0.0/tests/conftest.py` & `dicom-utils-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/jpeg2k_3d.dcm` & `dicom-utils-1.0.1/tests/jpeg2k_3d.dcm`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_anonymize.py` & `dicom-utils-1.0.1/tests/test_anonymize.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_basic_offset_table.py` & `dicom-utils-1.0.1/tests/test_basic_offset_table.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_container/test_collection.py` & `dicom-utils-1.0.1/tests/test_container/test_collection.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_container/test_input.py` & `dicom-utils-1.0.1/tests/test_container/test_input.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_container/test_output.py` & `dicom-utils-1.0.1/tests/test_container/test_output.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_container/test_protocols.py` & `dicom-utils-1.0.1/tests/test_container/test_protocols.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_container/test_record.py` & `dicom-utils-1.0.1/tests/test_container/test_record.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_dicom.py` & `dicom-utils-1.0.1/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_dicom_factory.py` & `dicom-utils-1.0.1/tests/test_dicom_factory.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_logging.py` & `dicom-utils-1.0.1/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_main/test_cat.py` & `dicom-utils-1.0.1/tests/test_main/test_cat.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_main/test_decompress.py` & `dicom-utils-1.0.1/tests/test_main/test_decompress.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_main/test_dicom2img.py` & `dicom-utils-1.0.1/tests/test_main/test_dicom2img.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_main/test_dicom_types.py` & `dicom-utils-1.0.1/tests/test_main/test_dicom_types.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_main/test_find.py` & `dicom-utils-1.0.1/tests/test_main/test_find.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_main/test_hash.py` & `dicom-utils-1.0.1/tests/test_main/test_hash.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_main/test_merge_series.py` & `dicom-utils-1.0.1/tests/test_main/test_merge_series.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_main/test_organize.py` & `dicom-utils-1.0.1/tests/test_main/test_organize.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_main/test_project.py` & `dicom-utils-1.0.1/tests/test_main/test_project.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_main/test_validate.py` & `dicom-utils-1.0.1/tests/test_main/test_validate.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_private.py` & `dicom-utils-1.0.1/tests/test_private.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_silence_warnings.py` & `dicom-utils-1.0.1/tests/test_silence_warnings.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_strip.py` & `dicom-utils-1.0.1/tests/test_strip.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_tag.py` & `dicom-utils-1.0.1/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_types.py` & `dicom-utils-1.0.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_visualize.py` & `dicom-utils-1.0.1/tests/test_visualize.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/tests/test_volume.py` & `dicom-utils-1.0.1/tests/test_volume.py`

 * *Files identical despite different names*

### Comparing `dicom-utils-1.0.0/PKG-INFO` & `dicom-utils-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicom-utils
-Version: 1.0.0
+Version: 1.0.1
 License: Apache
 Author-email: Scott Chase Waggener <tidalpaladin@protonmail.com>,Tim Cogan <tim@medcognetics.com>
 Requires-Python: >=3.9
 Provides-Extra: j2k
 Description-Content-Type: text/markdown
 
 # DICOM Utils
```

