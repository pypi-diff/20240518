# Comparing `tmp/ingredient_slicer-1.0.1.tar.gz` & `tmp/ingredient_slicer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ingredient_slicer-1.0.1.tar", last modified: Wed May  8 17:35:47 2024, max compression
+gzip compressed data, was "ingredient_slicer-1.0.2.tar", last modified: Sat May 18 16:16:52 2024, max compression
```

## Comparing `ingredient_slicer-1.0.1.tar` & `ingredient_slicer-1.0.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-08 17:35:47.783784 ingredient_slicer-1.0.1/
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-08 17:35:47.771068 ingredient_slicer-1.0.1/.github/
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-08 17:35:47.772807 ingredient_slicer-1.0.1/.github/workflows/
--rw-r--r--   0 anguswatters   (501) staff       (20)     3289 2024-05-07 12:28:17.000000 ingredient_slicer-1.0.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 anguswatters   (501) staff       (20)      782 2024-03-23 22:54:24.000000 ingredient_slicer-1.0.1/.github/workflows/run-unit-tests.yml
--rw-r--r--   0 anguswatters   (501) staff       (20)     3118 2024-03-17 16:59:19.000000 ingredient_slicer-1.0.1/.gitignore
--rw-r--r--   0 anguswatters   (501) staff       (20)     1075 2024-03-17 16:52:34.000000 ingredient_slicer-1.0.1/LICENSE
--rw-r--r--   0 anguswatters   (501) staff       (20)     3362 2024-05-08 17:35:47.783512 ingredient_slicer-1.0.1/PKG-INFO
--rw-r--r--   0 anguswatters   (501) staff       (20)     2389 2024-04-08 22:17:24.000000 ingredient_slicer-1.0.1/README.md
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-08 17:35:47.774109 ingredient_slicer-1.0.1/ingredient_slicer/
--rw-r--r--   0 anguswatters   (501) staff       (20)     1725 2024-05-08 17:34:45.000000 ingredient_slicer-1.0.1/ingredient_slicer/__init__.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   155567 2024-05-08 17:35:35.000000 ingredient_slicer-1.0.1/ingredient_slicer/_constants.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   102582 2024-05-06 17:09:54.000000 ingredient_slicer-1.0.1/ingredient_slicer/_ingredient_slicer.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    91104 2024-04-18 00:53:53.000000 ingredient_slicer-1.0.1/ingredient_slicer/_regex_patterns.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   101437 2024-05-06 17:10:27.000000 ingredient_slicer-1.0.1/ingredient_slicer/_utils.py
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-08 17:35:47.782853 ingredient_slicer-1.0.1/ingredient_slicer.egg-info/
--rw-r--r--   0 anguswatters   (501) staff       (20)     3362 2024-05-08 17:35:47.000000 ingredient_slicer-1.0.1/ingredient_slicer.egg-info/PKG-INFO
--rw-r--r--   0 anguswatters   (501) staff       (20)     2108 2024-05-08 17:35:47.000000 ingredient_slicer-1.0.1/ingredient_slicer.egg-info/SOURCES.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)        1 2024-05-08 17:35:47.000000 ingredient_slicer-1.0.1/ingredient_slicer.egg-info/dependency_links.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-05-08 17:35:47.000000 ingredient_slicer-1.0.1/ingredient_slicer.egg-info/requires.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)       18 2024-05-08 17:35:47.000000 ingredient_slicer-1.0.1/ingredient_slicer.egg-info/top_level.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)     1124 2024-05-08 17:34:40.000000 ingredient_slicer-1.0.1/pyproject.toml
--rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-05-08 17:35:47.783847 ingredient_slicer-1.0.1/setup.cfg
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-08 17:35:47.782606 ingredient_slicer-1.0.1/tests/
--rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 13:59:44.000000 ingredient_slicer-1.0.1/tests/__init__.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2402 2024-04-06 15:22:11.000000 ingredient_slicer-1.0.1/tests/test_avg_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5566 2024-04-10 14:53:42.000000 ingredient_slicer-1.0.1/tests/test_casual_ingredients.py
--rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:03.000000 ingredient_slicer-1.0.1/tests/test_clean_hyphen_padded_substrings.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5502 2024-04-06 15:27:00.000000 ingredient_slicer-1.0.1/tests/test_convert_fractions_to_decimals.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2145 2024-04-06 15:27:01.000000 ingredient_slicer-1.0.1/tests/test_convert_volumes_to_milliliters.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1182 2024-03-29 21:19:57.000000 ingredient_slicer-1.0.1/tests/test_duplicate_unit_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8507 2024-03-29 21:18:52.000000 ingredient_slicer-1.0.1/tests/test_extract_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3541 2024-03-29 21:19:50.000000 ingredient_slicer-1.0.1/tests/test_extract_quantities_utils.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3711 2024-03-29 21:19:48.000000 ingredient_slicer-1.0.1/tests/test_find_and_remove.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2842 2024-03-29 21:19:52.000000 ingredient_slicer-1.0.1/tests/test_find_and_remove_hyphen_substrings.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3352 2024-04-06 13:59:33.000000 ingredient_slicer-1.0.1/tests/test_fraction_str_to_decimal.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    26160 2024-05-06 14:16:39.000000 ingredient_slicer-1.0.1/tests/test_get_gram_weight.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2496 2024-05-06 15:32:33.000000 ingredient_slicer-1.0.1/tests/test_get_single_item_gram_weight.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    20386 2024-04-10 16:18:22.000000 ingredient_slicer-1.0.1/tests/test_ingredient_slicer.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3428 2024-04-08 13:04:03.000000 ingredient_slicer-1.0.1/tests/test_ingredient_slicer_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     4718 2024-04-10 14:52:58.000000 ingredient_slicer-1.0.1/tests/test_ingredient_slicer_fraction_conversions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1903 2024-05-06 17:14:21.000000 ingredient_slicer-1.0.1/tests/test_ingredient_slicer_gram_weights.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1515 2024-04-10 14:52:56.000000 ingredient_slicer-1.0.1/tests/test_ingredient_slicer_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     7502 2024-04-10 14:52:56.000000 ingredient_slicer-1.0.1/tests/test_ingredient_slicer_x_separators.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     4178 2024-04-10 14:52:54.000000 ingredient_slicer-1.0.1/tests/test_is_approximate_quantity_only_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2965 2024-04-10 14:52:54.000000 ingredient_slicer-1.0.1/tests/test_make_int_or_float_str.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2169 2024-04-06 15:26:57.000000 ingredient_slicer-1.0.1/tests/test_merge_misleading_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    14464 2024-03-29 21:19:43.000000 ingredient_slicer-1.0.1/tests/test_merge_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    43982 2024-04-06 14:42:17.000000 ingredient_slicer-1.0.1/tests/test_number_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    56318 2024-03-29 21:19:45.000000 ingredient_slicer-1.0.1/tests/test_number_ranges_separated_by_words.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5652 2024-04-06 13:59:36.000000 ingredient_slicer-1.0.1/tests/test_numbers_with_inch_symbols.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    15368 2024-03-29 21:19:20.000000 ingredient_slicer-1.0.1/tests/test_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    11036 2024-04-10 14:53:13.000000 ingredient_slicer-1.0.1/tests/test_parenthesis_utils.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2512 2024-03-29 21:19:22.000000 ingredient_slicer-1.0.1/tests/test_percentages.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3547 2024-03-29 21:19:26.000000 ingredient_slicer-1.0.1/tests/test_prefixed_number_words_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5013 2024-03-29 21:19:28.000000 ingredient_slicer-1.0.1/tests/test_prep_words.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5261 2024-03-29 21:19:25.000000 ingredient_slicer-1.0.1/tests/test_quantity_range_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    27045 2024-04-06 13:59:38.000000 ingredient_slicer-1.0.1/tests/test_quantity_units_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3571 2024-04-06 13:31:28.000000 ingredient_slicer-1.0.1/tests/test_remove_repeat_units_in_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)      633 2024-03-29 21:19:14.000000 ingredient_slicer-1.0.1/tests/test_remove_x_separators.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     6384 2024-03-29 21:19:12.000000 ingredient_slicer-1.0.1/tests/test_replace_a_or_an_quantities.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     6869 2024-03-29 21:19:08.000000 ingredient_slicer-1.0.1/tests/test_separate_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1808 2024-03-29 21:19:42.000000 ingredient_slicer-1.0.1/tests/test_size_modifiers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8974 2024-03-29 21:19:39.000000 ingredient_slicer-1.0.1/tests/test_spaced_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5838 2024-03-29 21:19:40.000000 ingredient_slicer-1.0.1/tests/test_unit_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    16676 2024-04-06 15:22:15.000000 ingredient_slicer-1.0.1/tests/test_wild_ingredients.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8022 2024-04-06 15:22:14.000000 ingredient_slicer-1.0.1/tests/test_word_fractions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     7167 2024-03-29 21:19:33.000000 ingredient_slicer-1.0.1/tests/test_word_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1337 2024-04-06 14:42:17.000000 ingredient_slicer-1.0.1/tests/test_x_after_number_regex.py
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-18 16:16:52.129885 ingredient_slicer-1.0.2/
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-18 16:16:52.116373 ingredient_slicer-1.0.2/.github/
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-18 16:16:52.118044 ingredient_slicer-1.0.2/.github/workflows/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3289 2024-05-07 12:28:17.000000 ingredient_slicer-1.0.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 anguswatters   (501) staff       (20)      782 2024-03-23 22:54:24.000000 ingredient_slicer-1.0.2/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3118 2024-03-17 16:59:19.000000 ingredient_slicer-1.0.2/.gitignore
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1075 2024-03-17 16:52:34.000000 ingredient_slicer-1.0.2/LICENSE
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3362 2024-05-18 16:16:52.129584 ingredient_slicer-1.0.2/PKG-INFO
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2389 2024-04-08 22:17:24.000000 ingredient_slicer-1.0.2/README.md
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-18 16:16:52.119927 ingredient_slicer-1.0.2/ingredient_slicer/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1725 2024-05-18 16:16:43.000000 ingredient_slicer-1.0.2/ingredient_slicer/__init__.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   156564 2024-05-18 16:16:01.000000 ingredient_slicer-1.0.2/ingredient_slicer/_constants.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   102582 2024-05-06 17:09:54.000000 ingredient_slicer-1.0.2/ingredient_slicer/_ingredient_slicer.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    91104 2024-04-18 00:53:53.000000 ingredient_slicer-1.0.2/ingredient_slicer/_regex_patterns.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   106410 2024-05-18 16:16:27.000000 ingredient_slicer-1.0.2/ingredient_slicer/_utils.py
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-18 16:16:52.128925 ingredient_slicer-1.0.2/ingredient_slicer.egg-info/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3362 2024-05-18 16:16:52.000000 ingredient_slicer-1.0.2/ingredient_slicer.egg-info/PKG-INFO
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2108 2024-05-18 16:16:52.000000 ingredient_slicer-1.0.2/ingredient_slicer.egg-info/SOURCES.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)        1 2024-05-18 16:16:52.000000 ingredient_slicer-1.0.2/ingredient_slicer.egg-info/dependency_links.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-05-18 16:16:52.000000 ingredient_slicer-1.0.2/ingredient_slicer.egg-info/requires.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)       18 2024-05-18 16:16:52.000000 ingredient_slicer-1.0.2/ingredient_slicer.egg-info/top_level.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1124 2024-05-18 16:16:39.000000 ingredient_slicer-1.0.2/pyproject.toml
+-rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-05-18 16:16:52.129940 ingredient_slicer-1.0.2/setup.cfg
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-18 16:16:52.128670 ingredient_slicer-1.0.2/tests/
+-rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 13:59:44.000000 ingredient_slicer-1.0.2/tests/__init__.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2402 2024-04-06 15:22:11.000000 ingredient_slicer-1.0.2/tests/test_avg_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5566 2024-04-10 14:53:42.000000 ingredient_slicer-1.0.2/tests/test_casual_ingredients.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:03.000000 ingredient_slicer-1.0.2/tests/test_clean_hyphen_padded_substrings.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5502 2024-04-06 15:27:00.000000 ingredient_slicer-1.0.2/tests/test_convert_fractions_to_decimals.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2145 2024-04-06 15:27:01.000000 ingredient_slicer-1.0.2/tests/test_convert_volumes_to_milliliters.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1182 2024-03-29 21:19:57.000000 ingredient_slicer-1.0.2/tests/test_duplicate_unit_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8507 2024-03-29 21:18:52.000000 ingredient_slicer-1.0.2/tests/test_extract_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3541 2024-03-29 21:19:50.000000 ingredient_slicer-1.0.2/tests/test_extract_quantities_utils.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3711 2024-03-29 21:19:48.000000 ingredient_slicer-1.0.2/tests/test_find_and_remove.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2842 2024-03-29 21:19:52.000000 ingredient_slicer-1.0.2/tests/test_find_and_remove_hyphen_substrings.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3352 2024-04-06 13:59:33.000000 ingredient_slicer-1.0.2/tests/test_fraction_str_to_decimal.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    26160 2024-05-06 14:16:39.000000 ingredient_slicer-1.0.2/tests/test_get_gram_weight.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2496 2024-05-06 15:32:33.000000 ingredient_slicer-1.0.2/tests/test_get_single_item_gram_weight.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    20386 2024-04-10 16:18:22.000000 ingredient_slicer-1.0.2/tests/test_ingredient_slicer.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3428 2024-04-08 13:04:03.000000 ingredient_slicer-1.0.2/tests/test_ingredient_slicer_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     4718 2024-04-10 14:52:58.000000 ingredient_slicer-1.0.2/tests/test_ingredient_slicer_fraction_conversions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1903 2024-05-06 17:14:21.000000 ingredient_slicer-1.0.2/tests/test_ingredient_slicer_gram_weights.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1515 2024-04-10 14:52:56.000000 ingredient_slicer-1.0.2/tests/test_ingredient_slicer_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     7502 2024-04-10 14:52:56.000000 ingredient_slicer-1.0.2/tests/test_ingredient_slicer_x_separators.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     4178 2024-04-10 14:52:54.000000 ingredient_slicer-1.0.2/tests/test_is_approximate_quantity_only_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2965 2024-04-10 14:52:54.000000 ingredient_slicer-1.0.2/tests/test_make_int_or_float_str.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2169 2024-04-06 15:26:57.000000 ingredient_slicer-1.0.2/tests/test_merge_misleading_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    14464 2024-03-29 21:19:43.000000 ingredient_slicer-1.0.2/tests/test_merge_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    43982 2024-04-06 14:42:17.000000 ingredient_slicer-1.0.2/tests/test_number_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    56318 2024-03-29 21:19:45.000000 ingredient_slicer-1.0.2/tests/test_number_ranges_separated_by_words.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5652 2024-04-06 13:59:36.000000 ingredient_slicer-1.0.2/tests/test_numbers_with_inch_symbols.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    15368 2024-03-29 21:19:20.000000 ingredient_slicer-1.0.2/tests/test_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    11036 2024-04-10 14:53:13.000000 ingredient_slicer-1.0.2/tests/test_parenthesis_utils.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2512 2024-03-29 21:19:22.000000 ingredient_slicer-1.0.2/tests/test_percentages.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3547 2024-03-29 21:19:26.000000 ingredient_slicer-1.0.2/tests/test_prefixed_number_words_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5013 2024-03-29 21:19:28.000000 ingredient_slicer-1.0.2/tests/test_prep_words.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5261 2024-03-29 21:19:25.000000 ingredient_slicer-1.0.2/tests/test_quantity_range_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    27045 2024-04-06 13:59:38.000000 ingredient_slicer-1.0.2/tests/test_quantity_units_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3571 2024-04-06 13:31:28.000000 ingredient_slicer-1.0.2/tests/test_remove_repeat_units_in_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)      633 2024-03-29 21:19:14.000000 ingredient_slicer-1.0.2/tests/test_remove_x_separators.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     6384 2024-03-29 21:19:12.000000 ingredient_slicer-1.0.2/tests/test_replace_a_or_an_quantities.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     6869 2024-03-29 21:19:08.000000 ingredient_slicer-1.0.2/tests/test_separate_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1808 2024-03-29 21:19:42.000000 ingredient_slicer-1.0.2/tests/test_size_modifiers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8974 2024-03-29 21:19:39.000000 ingredient_slicer-1.0.2/tests/test_spaced_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5838 2024-03-29 21:19:40.000000 ingredient_slicer-1.0.2/tests/test_unit_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    16676 2024-04-06 15:22:15.000000 ingredient_slicer-1.0.2/tests/test_wild_ingredients.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8022 2024-04-06 15:22:14.000000 ingredient_slicer-1.0.2/tests/test_word_fractions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     7167 2024-03-29 21:19:33.000000 ingredient_slicer-1.0.2/tests/test_word_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1337 2024-04-06 14:42:17.000000 ingredient_slicer-1.0.2/tests/test_x_after_number_regex.py
```

### Comparing `ingredient_slicer-1.0.1/.github/workflows/publish-to-pypi.yml` & `ingredient_slicer-1.0.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/.github/workflows/run-unit-tests.yml` & `ingredient_slicer-1.0.2/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/.gitignore` & `ingredient_slicer-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/LICENSE` & `ingredient_slicer-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/PKG-INFO` & `ingredient_slicer-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingredient_slicer
-Version: 1.0.1
+Version: 1.0.2
 Summary: Parses unstructured recipe ingredient text into standardized quantities, units, and foods
 Author-email: Angus Watters <anguswatters@gmail.com>
 License: MIT License
 Keywords: ingredient,parser,recipe,text processing,food,cooking,grocery,shopping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ingredient_slicer-1.0.1/README.md` & `ingredient_slicer-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/ingredient_slicer/__init__.py` & `ingredient_slicer-1.0.2/ingredient_slicer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # __init__.py
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 from ._ingredient_slicer import IngredientSlicer
 
 from ._constants import UNITS, WEIGHT_UNITS, VOLUME_UNITS, DIMENSION_UNITS, \
     CASUAL_UNITS, CASUAL_QUANTITIES, PREP_WORDS, \
     FOOD_CATALOG, FOOD_CATEGORIES, FOOD_DENSITY_BY_GROUP, \
     PRIMARY_CATEGORIES, SECONDARY_CATEGORIES, \
```

### Comparing `ingredient_slicer-1.0.1/ingredient_slicer/_constants.py` & `ingredient_slicer-1.0.2/ingredient_slicer/_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1283,14 +1283,15 @@
             # "chicken egg": ("meat_and_meat_products", "egg"),
             # "chicken eggs": ("meat_and_meat_products", "egg"),
             # "duck egg": ("meat_and_meat_products", "egg"),
             # "duck eggs": ("meat_and_meat_products", "egg"),
             # "quail egg": ("meat_and_meat_products", "egg"),
             # "quail eggs": ("meat_and_meat_products", "egg"),
 
+
             # -------------------------------------------------------------------------------------------------------
             # ----- Egg & egg products ("egg_and_egg_products") -----
             # -------------------------------------------------------------------------------------------------------
 
             # EGG PRODUCTS
             "egg": ("egg_and_egg_products", "egg"),
             "eggs": ("egg_and_egg_products", "egg"),
@@ -1538,15 +1539,20 @@
             "oat flour": ("cereal_and_cereal_products", "flour"),
             "oat bran": ("cereal_and_cereal_products", "flour"),
             "almond flour": ("cereal_and_cereal_products", "flour"),
             "cake": ("cereal_and_cereal_products", "miscellaneous_foods"),
             "cake mix": ("cereal_and_cereal_products", "flour"),
             "dough": ("cereal_and_cereal_products", "miscellaneous_foods"),
             "dough mix": ("cereal_and_cereal_products", "miscellaneous_foods"),
-
+            "toast": ("cereal_and_cereal_products", "bread"),
+            "toasts" : ("cereal_and_cereal_products", "bread"),
+            "toasts bread": ("cereal_and_cereal_products", "bread"),
+            "toasted bread": ("cereal_and_cereal_products", "bread"),
+            "cracker" : ("cereal_and_cereal_products", "miscellaneous_foods"),
+            "crackers" : ("cereal_and_cereal_products", "miscellaneous_foods"),
             # -------------------------------------------------------------------------------------------------------
             # ----- Nuts and Seeds ("nuts_and_seeds") -----
             # -------------------------------------------------------------------------------------------------------
 
             # NUTS
             "almond": ("nuts_and_seeds", "miscellaneous_foods"),
             "almonds": ("nuts_and_seeds", "miscellaneous_foods"),
@@ -1911,14 +1917,17 @@
             "vegetable broth": ("soups", "soup"),
             "chicken stock": ("soups", "soup"),
             "beef stock": ("soups", "soup"),
             "vegetable stock": ("soups", "soup"),
             "miso soup": ("soups", "soup"),
             "tomato soup": ("soups", "soup"),
             "tomato bisque": ("soups", "soup"),
+            "bouillon": ("soups", "soup"),
+            "beef bouillon": ("soups", "soup"),
+            "chicken bouillon": ("soups", "soup"),
             "chicken noodle soup": ("soups", "soup"),
             "cream of mushroom soup": ("soups", "soup"),
             "cream of chicken soup": ("soups", "soup"),
             "cream of celery soup": ("soups", "soup"),
             "cream of broccoli soup": ("soups", "soup"),
             "cream of potato soup": ("soups", "soup"),
             "cream of tomato soup": ("soups", "soup"),
@@ -2011,25 +2020,33 @@
             "Maltitol": ("sweets", "sugar alcohol"),
             "xylitol": ("sweets", "sugar alcohol"),
             "erythritol": ("sweets", "sugar alcohol"),
             "sorbitol": ("sweets", "sugar alcohol"),
             "maltitol": ("sweets", "sugar alcohol"),
             "chocolate chips": ("sweets", "chocolate"),
             "chocolate": ("sweets", "chocolate"),
+            "white chocolate": ("sweets", "chocolate"),
+            "dark chocolate": ("sweets", "chocolate"),
+            "milk chocolate": ("sweets", "chocolate"),
+            "cocoa": ("sweets", "chocolate"),
+            "ladyfinger": ("sweets", "cookie"),
+            "ladysfingers": ("sweets", "cookie"),
+            "ladyfingers": ("sweets", "cookie"),
 
             # SYRUPS
             "corn syrup": ("syrups", "syrup"),
             "high fructose corn syrup": ("syrups", "syrup"),
             "honey": ("syrups", "honey"),
             "organic honey": ("syrups", "honey"),
             "maple syrup": ("syrups", "syrup"),
             "maple sugar": ("syrups", "sugar"),
             "agave": ("syrups", "nectar"),
             "agave nectar": ("syrups", "nectar"),
             "fruit syrup": ("syrups", "syrup"),
+            "molasses" : ("syrups", "sugar"),
             "pancake syrup": ("syrups", "syrup"),
             "light corn syrup": ("syrups", "syrup"),
             "grenadine syrup": ("syrups", "syrup"),
             "strawberry syrup": ("syrups", "syrup"),
             "chocolate syrup": ("syrups", "syrup"),
             "caramel syrup": ("syrups", "syrup"),
             "simple syrup": ("syrups", "syrup"),
@@ -2366,14 +2383,15 @@
 # Words that are so obviously pointing to a specific category that they can be used to determine the category of a food
 # (i.e. if a food contains the word "flour", it is most likely a cereal product)
 INDICATOR_STRINGS_MAP = {
     "flour" : "cereal_and_cereal_products",
     "flours" : "cereal_and_cereal_products",
     "bread" : "cereal_and_cereal_products",
     "breads" : "cereal_and_cereal_products",
+    "bouillon" : "soups",
     "oil" : "oils",
     "oils" : "oils",
     "milk" : "milk",
     "milks" : "milk",
     "syrup" : "syrups",
     "syrups" : "syrups",
     "sugar" : "sweets",
```

### Comparing `ingredient_slicer-1.0.1/ingredient_slicer/_ingredient_slicer.py` & `ingredient_slicer-1.0.2/ingredient_slicer/_ingredient_slicer.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/ingredient_slicer/_regex_patterns.py` & `ingredient_slicer-1.0.2/ingredient_slicer/_regex_patterns.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/ingredient_slicer/_utils.py` & `ingredient_slicer-1.0.2/ingredient_slicer/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1759,14 +1759,125 @@
 
     return {
         "gram_weight" : gram_weight, 
         "min_gram_weight" : min_gram_weight,
         "max_gram_weight" : max_gram_weight, 
         }
 
+def _fuzzy_match_food_to_food_group(food:str, method:str) -> str:
+    """
+    Given a food item, compare it to all of the foods in each food group and return the food group that the food item most closely matches.
+    Args:
+        food: string, a food item
+        method: string, the method to use for comparison (options: "dice", "jaccard", "levenshtein")
+    Returns:
+        str: the food group that the food item most closely matches
+    """
+
+    method = method.lower()
+
+    if method not in ["dice", "jaccard", "levenshtein"]:
+        raise ValueError("Invalid method. Options are 'dice', 'jaccard', or 'levenshtein'")
+    
+    fuzzy_matcher = _get_fuzzy_matcher(method)
+
+    similarity_scores = {}
+    top_scoring_foods = {}
+
+    for category in _constants.FOOD_DENSITY_BY_GROUP:
+        # print(f"Category: {category}")
+        # category = "cereal_and_cereal_products"
+        # group_list_of_foods = list(ingredient_slicer._constants.FOODS_BY_CATEGORY[category])
+        food_set = _constants.FOODS_BY_CATEGORY[category]
+        # print(f"Category: {category}\nFood set: {food_set}")
+
+        # TODO: Don't think i need this code here anymore, no reason to get the top scoring foods in each category
+        # find the closeness from the given food to each food in the current category
+        # and extract that food and its value, to stash the top matched food and its score for each category
+        # scores =  {i: round(fuzzy_matcher(food, i), 2) for i in food_set}
+        # top_score_key = max(scores, key=scores.get) 
+        # top_score_value = scores[top_score_key] if top_score_key else 0
+        
+        # # NOTE: keep track of the food with the highest similarity score for each category
+        # top_scoring_foods[category] = [top_score_key, top_score_value]
+        # print(f" - Top score key/value:\n ----> '{top_score_key} ({scores[top_score_key]})'\n")
+
+        max_similarity = max([round(fuzzy_matcher(food, i), 2) for i in food_set])
+        # max_similarity = max([round(_utils.score_sentence_similarity(food, i), 2) for i in food_set])
+
+        similarity_scores[category] = max_similarity
+        # print()
+
+    # get the key that has the highest similarity score in the dictionary of similarity scores
+    best_category_match = max(similarity_scores, key=similarity_scores.get)
+
+    return best_category_match
+
+def _get_closest_fuzzy_food_groups(food:str = None, group_metric:str = "max", method:str = "dice") -> list[list]:
+    """
+    Given a food item, get the top closest food group by fuzzy matching similarity scores of all foods
+      in each food group against the given food
+    Args:
+        food: string, a food item. Default is None
+        group_metric: str, the metric to use for comparison. Either max, mean, or min. Default is max
+        method: string, the method to use for comparison (options: "dice", "jaccard", "levenshtein"). Default is "dice"
+    Returns:
+        list[list]: a list of lists containing the similarity score and the food group ordered from highest to lowest similarity score
+    """
+
+    group_metric = group_metric.lower()
+
+    if group_metric not in ["max", "mean", "min"]:
+        raise ValueError("Invalid group metric. Options are 'max', 'mean', or 'min'")
+
+    method = method.lower()
+
+    if method not in ["dice", "jaccard", "levenshtein"]:
+        raise ValueError("Invalid method. Options are 'dice', 'jaccard', or 'levenshtein'")
+    
+    fuzzy_matcher = _get_fuzzy_matcher(method)
+
+    def non_zero_mean(lst):
+        non_zero_scores = [i for i in lst if i > 0]
+        non_zero_total = sum(non_zero_scores)
+        non_zero_length = len(non_zero_scores) if non_zero_scores else 1
+        return round(non_zero_total / non_zero_length, 4)
+    
+    # list of available metric functions
+    group_metric_functions = {
+        "max" : max,
+        "mean" : non_zero_mean,
+        "min" : min
+        }
+
+    group_metric_func = group_metric_functions.get(group_metric, max)
+
+    scored_categories = []
+    
+    for category in _constants.FOOD_DENSITY_BY_GROUP:
+        # print(f"Category: {category}")
+        # category = "cereal_and_cereal_products"
+        # group_list_of_foods = list(ingredient_slicer._constants.FOODS_BY_CATEGORY[category])
+        food_set = _constants.FOODS_BY_CATEGORY[category]
+        # print(f"Category: {category}\nFood set: {food_set}")
+
+        # find the closeness from the given food to each food in the current category
+        # compute the similarity score for each food in the category and then apply a function across the all of the scores
+        scores =  {i: round(fuzzy_matcher(food, i), 2) for i in food_set}
+        non_zero_scores = [scores[i] for i in scores if scores[i] > 0]
+        non_zero_scores = non_zero_scores if non_zero_scores else [0]
+
+        group_score = group_metric_func(non_zero_scores)
+
+        scored_categories.append([group_score, category])
+
+    scored_categories.sort(reverse = True)
+
+    return scored_categories
+
 # # ingredient = "1 1/2 cups of all purpose almond flour, grounded"
 # ingredient = "1 1/2 cups of chick nuggets, grounded"
 
 # # ingredient = "1 1/2 cups of chicken nuggets, grounded"
 # # ingredient = "1 1/2 cups of White whole wheat flour, grounded"
 
 # slicer = IngredientSlicer(ingredient)
```

### Comparing `ingredient_slicer-1.0.1/ingredient_slicer.egg-info/PKG-INFO` & `ingredient_slicer-1.0.2/ingredient_slicer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingredient_slicer
-Version: 1.0.1
+Version: 1.0.2
 Summary: Parses unstructured recipe ingredient text into standardized quantities, units, and foods
 Author-email: Angus Watters <anguswatters@gmail.com>
 License: MIT License
 Keywords: ingredient,parser,recipe,text processing,food,cooking,grocery,shopping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ingredient_slicer-1.0.1/ingredient_slicer.egg-info/SOURCES.txt` & `ingredient_slicer-1.0.2/ingredient_slicer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/pyproject.toml` & `ingredient_slicer-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "ingredient_slicer"
 authors = [
   {name = "Angus Watters", email = "anguswatters@gmail.com"},
 ]
-version = "1.0.1"
+version = "1.0.2"
 description = "Parses unstructured recipe ingredient text into standardized quantities, units, and foods"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: Unix",
```

### Comparing `ingredient_slicer-1.0.1/tests/test_avg_ranges.py` & `ingredient_slicer-1.0.2/tests/test_avg_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_casual_ingredients.py` & `ingredient_slicer-1.0.2/tests/test_casual_ingredients.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_convert_fractions_to_decimals.py` & `ingredient_slicer-1.0.2/tests/test_convert_fractions_to_decimals.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_convert_volumes_to_milliliters.py` & `ingredient_slicer-1.0.2/tests/test_convert_volumes_to_milliliters.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_duplicate_unit_ranges.py` & `ingredient_slicer-1.0.2/tests/test_duplicate_unit_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_extract_dimensions.py` & `ingredient_slicer-1.0.2/tests/test_extract_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_extract_quantities_utils.py` & `ingredient_slicer-1.0.2/tests/test_extract_quantities_utils.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_find_and_remove.py` & `ingredient_slicer-1.0.2/tests/test_find_and_remove.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_find_and_remove_hyphen_substrings.py` & `ingredient_slicer-1.0.2/tests/test_find_and_remove_hyphen_substrings.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_fraction_str_to_decimal.py` & `ingredient_slicer-1.0.2/tests/test_fraction_str_to_decimal.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_get_gram_weight.py` & `ingredient_slicer-1.0.2/tests/test_get_gram_weight.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_get_single_item_gram_weight.py` & `ingredient_slicer-1.0.2/tests/test_get_single_item_gram_weight.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_ingredient_slicer.py` & `ingredient_slicer-1.0.2/tests/test_ingredient_slicer.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_ingredient_slicer_dimensions.py` & `ingredient_slicer-1.0.2/tests/test_ingredient_slicer_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_ingredient_slicer_fraction_conversions.py` & `ingredient_slicer-1.0.2/tests/test_ingredient_slicer_fraction_conversions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_ingredient_slicer_gram_weights.py` & `ingredient_slicer-1.0.2/tests/test_ingredient_slicer_gram_weights.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_ingredient_slicer_parenthesis.py` & `ingredient_slicer-1.0.2/tests/test_ingredient_slicer_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_ingredient_slicer_x_separators.py` & `ingredient_slicer-1.0.2/tests/test_ingredient_slicer_x_separators.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_is_approximate_quantity_only_parenthesis.py` & `ingredient_slicer-1.0.2/tests/test_is_approximate_quantity_only_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_make_int_or_float_str.py` & `ingredient_slicer-1.0.2/tests/test_make_int_or_float_str.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_merge_misleading_ranges.py` & `ingredient_slicer-1.0.2/tests/test_merge_misleading_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_merge_numbers.py` & `ingredient_slicer-1.0.2/tests/test_merge_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_number_ranges.py` & `ingredient_slicer-1.0.2/tests/test_number_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_number_ranges_separated_by_words.py` & `ingredient_slicer-1.0.2/tests/test_number_ranges_separated_by_words.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_numbers_with_inch_symbols.py` & `ingredient_slicer-1.0.2/tests/test_numbers_with_inch_symbols.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_parenthesis.py` & `ingredient_slicer-1.0.2/tests/test_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_parenthesis_utils.py` & `ingredient_slicer-1.0.2/tests/test_parenthesis_utils.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_percentages.py` & `ingredient_slicer-1.0.2/tests/test_percentages.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_prefixed_number_words_regex.py` & `ingredient_slicer-1.0.2/tests/test_prefixed_number_words_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_prep_words.py` & `ingredient_slicer-1.0.2/tests/test_prep_words.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_quantity_range_regex.py` & `ingredient_slicer-1.0.2/tests/test_quantity_range_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_quantity_units_regex.py` & `ingredient_slicer-1.0.2/tests/test_quantity_units_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_remove_repeat_units_in_ranges.py` & `ingredient_slicer-1.0.2/tests/test_remove_repeat_units_in_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_remove_x_separators.py` & `ingredient_slicer-1.0.2/tests/test_remove_x_separators.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_replace_a_or_an_quantities.py` & `ingredient_slicer-1.0.2/tests/test_replace_a_or_an_quantities.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_separate_dimensions.py` & `ingredient_slicer-1.0.2/tests/test_separate_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_size_modifiers.py` & `ingredient_slicer-1.0.2/tests/test_size_modifiers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_spaced_numbers.py` & `ingredient_slicer-1.0.2/tests/test_spaced_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_unit_regex.py` & `ingredient_slicer-1.0.2/tests/test_unit_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_wild_ingredients.py` & `ingredient_slicer-1.0.2/tests/test_wild_ingredients.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_word_fractions.py` & `ingredient_slicer-1.0.2/tests/test_word_fractions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_word_numbers.py` & `ingredient_slicer-1.0.2/tests/test_word_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.1/tests/test_x_after_number_regex.py` & `ingredient_slicer-1.0.2/tests/test_x_after_number_regex.py`

 * *Files identical despite different names*

