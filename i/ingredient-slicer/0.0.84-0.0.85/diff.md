# Comparing `tmp/ingredient_slicer-0.0.84.tar.gz` & `tmp/ingredient_slicer-0.0.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ingredient_slicer-0.0.84.tar", last modified: Sat Apr  6 15:22:36 2024, max compression
+gzip compressed data, was "ingredient_slicer-0.0.85.tar", last modified: Sun Apr  7 21:00:27 2024, max compression
```

## Comparing `ingredient_slicer-0.0.84.tar` & `ingredient_slicer-0.0.85.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:36.308244 ingredient_slicer-0.0.84/
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:36.294554 ingredient_slicer-0.0.84/.github/
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:36.296349 ingredient_slicer-0.0.84/.github/workflows/
--rw-r--r--   0 anguswatters   (501) staff       (20)     3289 2024-03-30 17:04:31.000000 ingredient_slicer-0.0.84/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 anguswatters   (501) staff       (20)      782 2024-03-23 22:54:24.000000 ingredient_slicer-0.0.84/.github/workflows/run-unit-tests.yml
--rw-r--r--   0 anguswatters   (501) staff       (20)     3118 2024-03-17 16:59:19.000000 ingredient_slicer-0.0.84/.gitignore
--rw-r--r--   0 anguswatters   (501) staff       (20)     1075 2024-03-17 16:52:34.000000 ingredient_slicer-0.0.84/LICENSE
--rw-r--r--   0 anguswatters   (501) staff       (20)     3391 2024-04-06 15:22:36.307814 ingredient_slicer-0.0.84/PKG-INFO
--rw-r--r--   0 anguswatters   (501) staff       (20)     2417 2024-04-06 15:21:31.000000 ingredient_slicer-0.0.84/README.md
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:36.297611 ingredient_slicer-0.0.84/ingredient_slicer/
--rw-r--r--   0 anguswatters   (501) staff       (20)     1491 2024-04-06 15:22:10.000000 ingredient_slicer-0.0.84/ingredient_slicer/__init__.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   155365 2024-04-06 15:22:08.000000 ingredient_slicer-0.0.84/ingredient_slicer/_constants.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   104901 2024-04-06 15:08:23.000000 ingredient_slicer-0.0.84/ingredient_slicer/_ingredient_slicer.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   108094 2024-04-06 13:59:47.000000 ingredient_slicer-0.0.84/ingredient_slicer/_regex_patterns.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    92674 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.84/ingredient_slicer/_utils.py
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:36.306478 ingredient_slicer-0.0.84/ingredient_slicer.egg-info/
--rw-r--r--   0 anguswatters   (501) staff       (20)     3391 2024-04-06 15:22:36.000000 ingredient_slicer-0.0.84/ingredient_slicer.egg-info/PKG-INFO
--rw-r--r--   0 anguswatters   (501) staff       (20)     1922 2024-04-06 15:22:36.000000 ingredient_slicer-0.0.84/ingredient_slicer.egg-info/SOURCES.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)        1 2024-04-06 15:22:36.000000 ingredient_slicer-0.0.84/ingredient_slicer.egg-info/dependency_links.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-04-06 15:22:36.000000 ingredient_slicer-0.0.84/ingredient_slicer.egg-info/requires.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)       18 2024-04-06 15:22:36.000000 ingredient_slicer-0.0.84/ingredient_slicer.egg-info/top_level.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)     1125 2024-04-06 15:22:06.000000 ingredient_slicer-0.0.84/pyproject.toml
--rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-04-06 15:22:36.308316 ingredient_slicer-0.0.84/setup.cfg
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:36.306074 ingredient_slicer-0.0.84/tests/
--rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 13:59:44.000000 ingredient_slicer-0.0.84/tests/__init__.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2402 2024-04-06 15:22:11.000000 ingredient_slicer-0.0.84/tests/test_avg_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5832 2024-03-29 21:20:16.000000 ingredient_slicer-0.0.84/tests/test_casual_ingredients.py
--rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:03.000000 ingredient_slicer-0.0.84/tests/test_clean_hyphen_padded_substrings.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5502 2024-03-30 17:00:12.000000 ingredient_slicer-0.0.84/tests/test_convert_fractions_to_decimals.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1309 2024-04-06 12:45:26.000000 ingredient_slicer-0.0.84/tests/test_convert_volumes_to_milliliters.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1182 2024-03-29 21:19:57.000000 ingredient_slicer-0.0.84/tests/test_duplicate_unit_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8507 2024-03-29 21:18:52.000000 ingredient_slicer-0.0.84/tests/test_extract_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3541 2024-03-29 21:19:50.000000 ingredient_slicer-0.0.84/tests/test_extract_quantities_utils.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3711 2024-03-29 21:19:48.000000 ingredient_slicer-0.0.84/tests/test_find_and_remove.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2842 2024-03-29 21:19:52.000000 ingredient_slicer-0.0.84/tests/test_find_and_remove_hyphen_substrings.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3352 2024-04-06 13:59:33.000000 ingredient_slicer-0.0.84/tests/test_fraction_str_to_decimal.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    24889 2024-04-06 13:04:35.000000 ingredient_slicer-0.0.84/tests/test_get_gram_weight.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    20385 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.84/tests/test_ingredient_slicer.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3374 2024-04-06 15:22:17.000000 ingredient_slicer-0.0.84/tests/test_ingredient_slicer_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     4718 2024-04-06 15:22:20.000000 ingredient_slicer-0.0.84/tests/test_ingredient_slicer_fraction_conversions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     7502 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.84/tests/test_ingredient_slicer_x_separators.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2965 2024-03-29 21:19:46.000000 ingredient_slicer-0.0.84/tests/test_make_int_or_float_str.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2167 2024-04-06 12:30:44.000000 ingredient_slicer-0.0.84/tests/test_merge_misleading_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    14464 2024-03-29 21:19:43.000000 ingredient_slicer-0.0.84/tests/test_merge_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    43982 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.84/tests/test_number_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    56318 2024-03-29 21:19:45.000000 ingredient_slicer-0.0.84/tests/test_number_ranges_separated_by_words.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5652 2024-04-06 13:59:36.000000 ingredient_slicer-0.0.84/tests/test_numbers_with_inch_symbols.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    15368 2024-03-29 21:19:20.000000 ingredient_slicer-0.0.84/tests/test_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    11034 2024-03-29 21:19:23.000000 ingredient_slicer-0.0.84/tests/test_parenthesis_utils.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2512 2024-03-29 21:19:22.000000 ingredient_slicer-0.0.84/tests/test_percentages.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3547 2024-03-29 21:19:26.000000 ingredient_slicer-0.0.84/tests/test_prefixed_number_words_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5013 2024-03-29 21:19:28.000000 ingredient_slicer-0.0.84/tests/test_prep_words.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5261 2024-03-29 21:19:25.000000 ingredient_slicer-0.0.84/tests/test_quantity_range_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    27045 2024-04-06 13:59:38.000000 ingredient_slicer-0.0.84/tests/test_quantity_units_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3571 2024-04-06 13:31:28.000000 ingredient_slicer-0.0.84/tests/test_remove_repeat_units_in_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)      633 2024-03-29 21:19:14.000000 ingredient_slicer-0.0.84/tests/test_remove_x_separators.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     6384 2024-03-29 21:19:12.000000 ingredient_slicer-0.0.84/tests/test_replace_a_or_an_quantities.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     6869 2024-03-29 21:19:08.000000 ingredient_slicer-0.0.84/tests/test_separate_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1808 2024-03-29 21:19:42.000000 ingredient_slicer-0.0.84/tests/test_size_modifiers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8974 2024-03-29 21:19:39.000000 ingredient_slicer-0.0.84/tests/test_spaced_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5838 2024-03-29 21:19:40.000000 ingredient_slicer-0.0.84/tests/test_unit_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    16676 2024-04-06 15:22:15.000000 ingredient_slicer-0.0.84/tests/test_wild_ingredients.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8022 2024-04-06 15:22:14.000000 ingredient_slicer-0.0.84/tests/test_word_fractions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     7167 2024-03-29 21:19:33.000000 ingredient_slicer-0.0.84/tests/test_word_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1337 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.84/tests/test_x_after_number_regex.py
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-07 21:00:27.401708 ingredient_slicer-0.0.85/
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-07 21:00:27.390391 ingredient_slicer-0.0.85/.github/
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-07 21:00:27.391512 ingredient_slicer-0.0.85/.github/workflows/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3289 2024-03-30 17:04:31.000000 ingredient_slicer-0.0.85/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 anguswatters   (501) staff       (20)      782 2024-03-23 22:54:24.000000 ingredient_slicer-0.0.85/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3118 2024-03-17 16:59:19.000000 ingredient_slicer-0.0.85/.gitignore
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1075 2024-03-17 16:52:34.000000 ingredient_slicer-0.0.85/LICENSE
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3263 2024-04-07 21:00:27.401433 ingredient_slicer-0.0.85/PKG-INFO
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2289 2024-04-06 15:25:45.000000 ingredient_slicer-0.0.85/README.md
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-07 21:00:27.392538 ingredient_slicer-0.0.85/ingredient_slicer/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1491 2024-04-07 20:59:38.000000 ingredient_slicer-0.0.85/ingredient_slicer/__init__.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   155365 2024-04-06 15:22:08.000000 ingredient_slicer-0.0.85/ingredient_slicer/_constants.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   104894 2024-04-07 20:59:11.000000 ingredient_slicer-0.0.85/ingredient_slicer/_ingredient_slicer.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   108094 2024-04-06 13:59:47.000000 ingredient_slicer-0.0.85/ingredient_slicer/_regex_patterns.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    92634 2024-04-07 20:58:21.000000 ingredient_slicer-0.0.85/ingredient_slicer/_utils.py
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-07 21:00:27.400781 ingredient_slicer-0.0.85/ingredient_slicer.egg-info/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3263 2024-04-07 21:00:27.000000 ingredient_slicer-0.0.85/ingredient_slicer.egg-info/PKG-INFO
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1922 2024-04-07 21:00:27.000000 ingredient_slicer-0.0.85/ingredient_slicer.egg-info/SOURCES.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)        1 2024-04-07 21:00:27.000000 ingredient_slicer-0.0.85/ingredient_slicer.egg-info/dependency_links.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-04-07 21:00:27.000000 ingredient_slicer-0.0.85/ingredient_slicer.egg-info/requires.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)       18 2024-04-07 21:00:27.000000 ingredient_slicer-0.0.85/ingredient_slicer.egg-info/top_level.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1125 2024-04-07 20:59:23.000000 ingredient_slicer-0.0.85/pyproject.toml
+-rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-04-07 21:00:27.401765 ingredient_slicer-0.0.85/setup.cfg
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-07 21:00:27.400557 ingredient_slicer-0.0.85/tests/
+-rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 13:59:44.000000 ingredient_slicer-0.0.85/tests/__init__.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2402 2024-04-06 15:22:11.000000 ingredient_slicer-0.0.85/tests/test_avg_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5832 2024-03-29 21:20:16.000000 ingredient_slicer-0.0.85/tests/test_casual_ingredients.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:03.000000 ingredient_slicer-0.0.85/tests/test_clean_hyphen_padded_substrings.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5502 2024-04-06 15:27:00.000000 ingredient_slicer-0.0.85/tests/test_convert_fractions_to_decimals.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2145 2024-04-06 15:27:01.000000 ingredient_slicer-0.0.85/tests/test_convert_volumes_to_milliliters.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1182 2024-03-29 21:19:57.000000 ingredient_slicer-0.0.85/tests/test_duplicate_unit_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8507 2024-03-29 21:18:52.000000 ingredient_slicer-0.0.85/tests/test_extract_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3541 2024-03-29 21:19:50.000000 ingredient_slicer-0.0.85/tests/test_extract_quantities_utils.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3711 2024-03-29 21:19:48.000000 ingredient_slicer-0.0.85/tests/test_find_and_remove.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2842 2024-03-29 21:19:52.000000 ingredient_slicer-0.0.85/tests/test_find_and_remove_hyphen_substrings.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3352 2024-04-06 13:59:33.000000 ingredient_slicer-0.0.85/tests/test_fraction_str_to_decimal.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    24889 2024-04-06 13:04:35.000000 ingredient_slicer-0.0.85/tests/test_get_gram_weight.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    20385 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.85/tests/test_ingredient_slicer.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3374 2024-04-06 15:22:17.000000 ingredient_slicer-0.0.85/tests/test_ingredient_slicer_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     4718 2024-04-06 15:22:20.000000 ingredient_slicer-0.0.85/tests/test_ingredient_slicer_fraction_conversions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     7502 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.85/tests/test_ingredient_slicer_x_separators.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2965 2024-03-29 21:19:46.000000 ingredient_slicer-0.0.85/tests/test_make_int_or_float_str.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2169 2024-04-06 15:26:57.000000 ingredient_slicer-0.0.85/tests/test_merge_misleading_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    14464 2024-03-29 21:19:43.000000 ingredient_slicer-0.0.85/tests/test_merge_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    43982 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.85/tests/test_number_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    56318 2024-03-29 21:19:45.000000 ingredient_slicer-0.0.85/tests/test_number_ranges_separated_by_words.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5652 2024-04-06 13:59:36.000000 ingredient_slicer-0.0.85/tests/test_numbers_with_inch_symbols.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    15368 2024-03-29 21:19:20.000000 ingredient_slicer-0.0.85/tests/test_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    11034 2024-03-29 21:19:23.000000 ingredient_slicer-0.0.85/tests/test_parenthesis_utils.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2512 2024-03-29 21:19:22.000000 ingredient_slicer-0.0.85/tests/test_percentages.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3547 2024-03-29 21:19:26.000000 ingredient_slicer-0.0.85/tests/test_prefixed_number_words_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5013 2024-03-29 21:19:28.000000 ingredient_slicer-0.0.85/tests/test_prep_words.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5261 2024-03-29 21:19:25.000000 ingredient_slicer-0.0.85/tests/test_quantity_range_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    27045 2024-04-06 13:59:38.000000 ingredient_slicer-0.0.85/tests/test_quantity_units_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3571 2024-04-06 13:31:28.000000 ingredient_slicer-0.0.85/tests/test_remove_repeat_units_in_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)      633 2024-03-29 21:19:14.000000 ingredient_slicer-0.0.85/tests/test_remove_x_separators.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     6384 2024-03-29 21:19:12.000000 ingredient_slicer-0.0.85/tests/test_replace_a_or_an_quantities.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     6869 2024-03-29 21:19:08.000000 ingredient_slicer-0.0.85/tests/test_separate_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1808 2024-03-29 21:19:42.000000 ingredient_slicer-0.0.85/tests/test_size_modifiers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8974 2024-03-29 21:19:39.000000 ingredient_slicer-0.0.85/tests/test_spaced_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5838 2024-03-29 21:19:40.000000 ingredient_slicer-0.0.85/tests/test_unit_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    16676 2024-04-06 15:22:15.000000 ingredient_slicer-0.0.85/tests/test_wild_ingredients.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8022 2024-04-06 15:22:14.000000 ingredient_slicer-0.0.85/tests/test_word_fractions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     7167 2024-03-29 21:19:33.000000 ingredient_slicer-0.0.85/tests/test_word_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1337 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.85/tests/test_x_after_number_regex.py
```

### Comparing `ingredient_slicer-0.0.84/.github/workflows/publish-to-pypi.yml` & `ingredient_slicer-0.0.85/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/.github/workflows/run-unit-tests.yml` & `ingredient_slicer-0.0.85/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/.gitignore` & `ingredient_slicer-0.0.85/.gitignore`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/LICENSE` & `ingredient_slicer-0.0.85/LICENSE`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/PKG-INFO` & `ingredient_slicer-0.0.85/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingredient_slicer
-Version: 0.0.84
+Version: 0.0.85
 Summary: Parses unstructured recipe ingredient text into standardized quantities, units, and foods
 Author-email: Angus Watters <anguswatters@gmail.com>
 License: MIT License
 Keywords: ingredient,parser,recipe,text processing,food,cooking,grocery,shopping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -42,72 +42,73 @@
 <br>
 
 Installation:
 -----------------------
 `ingredient_slicer` can be downloaded from PyPI via `pip` like so:
 
 ``` shell
-    pip install ingredient-slicer
+pip install ingredient-slicer
 ```
 
 Usage:
 -----------------------
 
 Provide a string to the `IngredientSlicer` class and thats it. Invoke the `to_json()` method to return the parsed ingredient.
 
 ```pycon
 
-    import ingredient_slicer
+import ingredient_slicer
 
-    slicer = ingredient_slicer.IngredientSlicer("2 (15-ounces) cans chickpeas, rinsed and drained")
+slicer = ingredient_slicer.IngredientSlicer("2 (15-ounces) cans chickpeas, rinsed and drained")
 
-    slicer.to_json()
-    {
-        'standardized_ingredient': '2 cans chickpeas, rinsed and drained', 
-        'food': 'chickpeas', 
-        
-        # primary units
-        'quantity': '30', 
-        'unit': 'ounces', 
-        'standardized_unit': 'ounce', 
-
-        # any other secondary units found in the string
-        'secondary_quantity': '2', 
-        'secondary_unit': 'cans', 
-        'standardized_secondary_unit': 'can', 
-
-        'gram_weight': '850.49', 
-        'prep': ['drained', 'rinsed'], 
-        'size_modifiers': [], 
-        'dimensions': [], 
-        'is_required': True, 
-        'parenthesis_content': ['15 ounce']
-    }
+slicer.to_json()
+
+{
+    'standardized_ingredient': '2 cans chickpeas, rinsed and drained', 
+    'food': 'chickpeas', 
+
+    # primary units
+    'quantity': '30', 
+    'unit': 'ounces', 
+    'standardized_unit': 'ounce', 
+
+    # any other secondary units found in the string
+    'secondary_quantity': '2', 
+    'secondary_unit': 'cans', 
+    'standardized_secondary_unit': 'can', 
+
+    'gram_weight': '850.49', 
+    'prep': ['drained', 'rinsed'], 
+    'size_modifiers': [], 
+    'dimensions': [], 
+    'is_required': True, 
+    'parenthesis_content': ['15 ounce']
+}
 ```
 
-Individual ingredient components can also be found using methods like `food()` or `unit()`
+Individual ingredient components can also be found using methods like `food()`, `quantity()`, or `unit()`
 
 ```pycon
 
-    import ingredient_slicer
+import ingredient_slicer
 
-    slicer = ingredient_slicer.IngredientSlicer("3 tbsp unsalted butter, softened at room temperature")
+slicer = ingredient_slicer.IngredientSlicer("3 tbsp unsalted butter, softened at room temperature")
 
-    slicer.food() 
-    >>> 'unsalted butter'
+slicer.food() 
+>>> 'unsalted butter'
 
-    slicer.unit() 
-    >>> 'tbsp'
+slicer.quantity() 
+>>> '3' 
 
-    slicer.standardized_unit() 
-    >>> 'tablespoon'
+slicer.unit() 
+>>> 'tbsp'
 
-    slicer.quantity() 
-    >>> '3' 
+slicer.standardized_unit() 
+>>> 'tablespoon'
 
-    slicer.prep() 
-    >>> ['room temperature', 'softened']
+slicer.prep() 
+>>> ['room temperature', 'softened']
 ```
 
 Contributing/Issues:
 -----------------------
 If you find a bug or have an idea for a new feature, please open an issue or submit a pull request.
```

### Comparing `ingredient_slicer-0.0.84/README.md` & `ingredient_slicer-0.0.85/ingredient_slicer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: ingredient_slicer
+Version: 0.0.85
+Summary: Parses unstructured recipe ingredient text into standardized quantities, units, and foods
+Author-email: Angus Watters <anguswatters@gmail.com>
+License: MIT License
+Keywords: ingredient,parser,recipe,text processing,food,cooking,grocery,shopping
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pip-tools; extra == "test"
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+
 ingredient-slicer
 ------
 
 Python 📦 package for extracting quantities, units, and food words from unstructured recipe ingredients text. 
 
 `ingredient-slicer` works by standardizing the input text and then applying a set of rules and heuristic methods to parse out quantities, units, and food words from unstructured recipe ingredients text.
 `ingredient-slicer` was designed to provide a robust and lightweight method for parsing recipe ingredients 
@@ -17,72 +42,73 @@
 <br>
 
 Installation:
 -----------------------
 `ingredient_slicer` can be downloaded from PyPI via `pip` like so:
 
 ``` shell
-    pip install ingredient-slicer
+pip install ingredient-slicer
 ```
 
 Usage:
 -----------------------
 
 Provide a string to the `IngredientSlicer` class and thats it. Invoke the `to_json()` method to return the parsed ingredient.
 
 ```pycon
 
-    import ingredient_slicer
+import ingredient_slicer
+
+slicer = ingredient_slicer.IngredientSlicer("2 (15-ounces) cans chickpeas, rinsed and drained")
 
-    slicer = ingredient_slicer.IngredientSlicer("2 (15-ounces) cans chickpeas, rinsed and drained")
+slicer.to_json()
 
-    slicer.to_json()
-    {
-        'standardized_ingredient': '2 cans chickpeas, rinsed and drained', 
-        'food': 'chickpeas', 
-        
-        # primary units
-        'quantity': '30', 
-        'unit': 'ounces', 
-        'standardized_unit': 'ounce', 
-
-        # any other secondary units found in the string
-        'secondary_quantity': '2', 
-        'secondary_unit': 'cans', 
-        'standardized_secondary_unit': 'can', 
-
-        'gram_weight': '850.49', 
-        'prep': ['drained', 'rinsed'], 
-        'size_modifiers': [], 
-        'dimensions': [], 
-        'is_required': True, 
-        'parenthesis_content': ['15 ounce']
-    }
+{
+    'standardized_ingredient': '2 cans chickpeas, rinsed and drained', 
+    'food': 'chickpeas', 
+
+    # primary units
+    'quantity': '30', 
+    'unit': 'ounces', 
+    'standardized_unit': 'ounce', 
+
+    # any other secondary units found in the string
+    'secondary_quantity': '2', 
+    'secondary_unit': 'cans', 
+    'standardized_secondary_unit': 'can', 
+
+    'gram_weight': '850.49', 
+    'prep': ['drained', 'rinsed'], 
+    'size_modifiers': [], 
+    'dimensions': [], 
+    'is_required': True, 
+    'parenthesis_content': ['15 ounce']
+}
 ```
 
-Individual ingredient components can also be found using methods like `food()` or `unit()`
+Individual ingredient components can also be found using methods like `food()`, `quantity()`, or `unit()`
 
 ```pycon
 
-    import ingredient_slicer
+import ingredient_slicer
 
-    slicer = ingredient_slicer.IngredientSlicer("3 tbsp unsalted butter, softened at room temperature")
+slicer = ingredient_slicer.IngredientSlicer("3 tbsp unsalted butter, softened at room temperature")
 
-    slicer.food() 
-    >>> 'unsalted butter'
+slicer.food() 
+>>> 'unsalted butter'
 
-    slicer.unit() 
-    >>> 'tbsp'
+slicer.quantity() 
+>>> '3' 
 
-    slicer.standardized_unit() 
-    >>> 'tablespoon'
+slicer.unit() 
+>>> 'tbsp'
 
-    slicer.quantity() 
-    >>> '3' 
+slicer.standardized_unit() 
+>>> 'tablespoon'
 
-    slicer.prep() 
-    >>> ['room temperature', 'softened']
+slicer.prep() 
+>>> ['room temperature', 'softened']
 ```
 
 Contributing/Issues:
 -----------------------
-If you find a bug or have an idea for a new feature, please open an issue or submit a pull request.
+If you find a bug or have an idea for a new feature, please open an issue or submit a pull request.
```

### Comparing `ingredient_slicer-0.0.84/ingredient_slicer/__init__.py` & `ingredient_slicer-0.0.85/ingredient_slicer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # __init__.py
 
-__version__ = "0.0.84"
+__version__ = "0.0.85"
 
 from ._constants import UNITS, WEIGHT_UNITS, VOLUME_UNITS, DIMENSION_UNITS, \
     CASUAL_UNITS, CASUAL_QUANTITIES, PREP_WORDS, \
     FOOD_CATALOG, FOOD_CATEGORIES, FOOD_DENSITY_BY_GROUP
 
 from ._ingredient_slicer import IngredientSlicer
 # from ._regex_patterns import IngredientTools
```

### Comparing `ingredient_slicer-0.0.84/ingredient_slicer/_constants.py` & `ingredient_slicer-0.0.85/ingredient_slicer/_constants.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/ingredient_slicer/_ingredient_slicer.py` & `ingredient_slicer-0.0.85/ingredient_slicer/_ingredient_slicer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1602,15 +1602,15 @@
     #     # ingredient = "2 1/2 cups of sugar (about 1/2 inch squares of sugar)"
     #     dimension_units = _regex_patterns.QUANTITY_DIMENSION_UNIT_GROUPS.findall(ingredient)
     #     return dimension_units
     
     def _add_gram_weights(self):
         """Add gram weights to the units variables if they are the only possible units after the ingredient has been parsed."""
         # ingredient = "2 1/2 cups of sugar (about 1/2 inch squares of sugar)"
-        grams_map = _utils._get_gram_weight(self._food, self._quantity, self._unit, "levenshtein")
+        grams_map = _utils._get_gram_weight(self._food, self._quantity, self._unit, "dice")
 
         if grams_map:
             self._gram_weight      = grams_map.get("gram_weight", None)
             self._min_gram_weight = grams_map.get("min_gram_weight", None)
             self._max_gram_weight = grams_map.get("max_gram_weight", None)
 
         return
```

### Comparing `ingredient_slicer-0.0.84/ingredient_slicer/_regex_patterns.py` & `ingredient_slicer-0.0.85/ingredient_slicer/_regex_patterns.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/ingredient_slicer/_utils.py` & `ingredient_slicer-0.0.85/ingredient_slicer/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1401,15 +1401,15 @@
         # if the units are the same, replace the original string with the quantities and units
         if unit1 == unit2:
             ingredient = ingredient.replace(original_string, f"{quantity1} - {quantity2} {unit1}")
 
     return ingredient 
 
 
-def _get_gram_weight(food:str, quantity:str, unit:str, method:str = "levenshtein") -> dict:
+def _get_gram_weight(food:str, quantity:str, unit:str, method:str = "dice") -> dict:
 
     """ Get the gram weight of a given quantity of food item.
     Args:
         food (str): The food item to convert.
         quantity (Union[str, int, float]): The quantity of the food item.
         unit (str): The unit of measurement for the quantity.
     Returns:
@@ -1765,36 +1765,35 @@
         "levenshtein" : _levenshtein_similarity,
         "jaccard" : _jaccard_similarity,
         "dice" : _dice_coeff_similarity
         }
 
     return fuzzy_matchers[method]
 
-# _convert_volume_to_grams(food, quantity, unit)
-def _levenshtein_dist(str1, str2):
-    # set up a matrix with the dimensions of the two strings
-    matrix = [[0] * (len(str2) + 1) for _ in range(len(str1) + 1)]
-    
-    # initialize the matrix with the values of the first row and column
-    for i in range(len(str1) + 1):
-        matrix[i][0] = i
+def _levenshtein_dist(str1: str, str2: str) -> int:
+    matrix = [[float("inf")] * (len(str2) + 1) for i in range(len(str1) + 1)]
+
     for j in range(len(str2) + 1):
-        matrix[0][j] = j
+        matrix[len(str1)][j] = len(str2) - j
 
-    for i in range(1, len(str1) + 1):
-        for j in range(1, len(str2) + 1):
-            substitute = 0 if str1[i - 1] == str2[j - 1] else 1
-            matrix[i][j] = min(
-                matrix[i - 1][j] + 1,              # delete
-                matrix[i][j - 1] + 1,               # isert 
-                matrix[i - 1][j - 1] + substitute  # substitute
-            )
+    for i in range(len(str1) + 1):
+        matrix[i][len(str2)] = len(str1) - i
 
+    for i in range(len(str1) - 1, -1, -1):
+        for j in range(len(str2) - 1, -1, -1):
+            if str1[i] == str2[j]:
+                matrix[i][j] = matrix[i + 1][j + 1]
+            else:
+                matrix[i][j] = 1 + min(
+                                    matrix[i + 1][j],    # delete
+                                    matrix[i][j + 1],     # isert 
+                                    matrix[i + 1][j + 1] # substitute
+                                    )
     # levenstein distance == bottom right corner of matrix
-    return matrix[len(str1)][len(str2)]
+    return matrix[0][0]
 
 def _levenshtein_similarity(str1, str2):
     distance = _levenshtein_dist(str1, str2)
     max_len = max(len(str1), len(str2))
     return 1 - (distance / max_len)
 
 def _jaccard_similarity(str1, str2):
```

### Comparing `ingredient_slicer-0.0.84/ingredient_slicer.egg-info/SOURCES.txt` & `ingredient_slicer-0.0.85/ingredient_slicer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/pyproject.toml` & `ingredient_slicer-0.0.85/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "ingredient_slicer"
 authors = [
   {name = "Angus Watters", email = "anguswatters@gmail.com"},
 ]
-version = "0.0.84"
+version = "0.0.85"
 description = "Parses unstructured recipe ingredient text into standardized quantities, units, and foods"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: Unix",
```

### Comparing `ingredient_slicer-0.0.84/tests/test_avg_ranges.py` & `ingredient_slicer-0.0.85/tests/test_avg_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_casual_ingredients.py` & `ingredient_slicer-0.0.85/tests/test_casual_ingredients.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_convert_fractions_to_decimals.py` & `ingredient_slicer-0.0.85/tests/test_convert_fractions_to_decimals.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_duplicate_unit_ranges.py` & `ingredient_slicer-0.0.85/tests/test_duplicate_unit_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_extract_dimensions.py` & `ingredient_slicer-0.0.85/tests/test_extract_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_extract_quantities_utils.py` & `ingredient_slicer-0.0.85/tests/test_extract_quantities_utils.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_find_and_remove.py` & `ingredient_slicer-0.0.85/tests/test_find_and_remove.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_find_and_remove_hyphen_substrings.py` & `ingredient_slicer-0.0.85/tests/test_find_and_remove_hyphen_substrings.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_fraction_str_to_decimal.py` & `ingredient_slicer-0.0.85/tests/test_fraction_str_to_decimal.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_get_gram_weight.py` & `ingredient_slicer-0.0.85/tests/test_get_gram_weight.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_ingredient_slicer.py` & `ingredient_slicer-0.0.85/tests/test_ingredient_slicer.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_ingredient_slicer_dimensions.py` & `ingredient_slicer-0.0.85/tests/test_ingredient_slicer_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_ingredient_slicer_fraction_conversions.py` & `ingredient_slicer-0.0.85/tests/test_ingredient_slicer_fraction_conversions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_ingredient_slicer_x_separators.py` & `ingredient_slicer-0.0.85/tests/test_ingredient_slicer_x_separators.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_make_int_or_float_str.py` & `ingredient_slicer-0.0.85/tests/test_make_int_or_float_str.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_merge_misleading_ranges.py` & `ingredient_slicer-0.0.85/tests/test_merge_misleading_ranges.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,8 +46,9 @@
 
 def test_misleading_range_tuple_error():
     with pytest.raises(TypeError):
         assert _utils._merge_misleading_ranges((1,2,3))
 
 def test_misleading_range_float_error():
     with pytest.raises(TypeError):
-        assert _utils._merge_misleading_ranges(1.5)
+        assert _utils._merge_misleading_ranges(1.5)
+
```

### Comparing `ingredient_slicer-0.0.84/tests/test_merge_numbers.py` & `ingredient_slicer-0.0.85/tests/test_merge_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_number_ranges.py` & `ingredient_slicer-0.0.85/tests/test_number_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_number_ranges_separated_by_words.py` & `ingredient_slicer-0.0.85/tests/test_number_ranges_separated_by_words.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_numbers_with_inch_symbols.py` & `ingredient_slicer-0.0.85/tests/test_numbers_with_inch_symbols.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_parenthesis.py` & `ingredient_slicer-0.0.85/tests/test_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_parenthesis_utils.py` & `ingredient_slicer-0.0.85/tests/test_parenthesis_utils.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_percentages.py` & `ingredient_slicer-0.0.85/tests/test_percentages.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_prefixed_number_words_regex.py` & `ingredient_slicer-0.0.85/tests/test_prefixed_number_words_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_prep_words.py` & `ingredient_slicer-0.0.85/tests/test_prep_words.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_quantity_range_regex.py` & `ingredient_slicer-0.0.85/tests/test_quantity_range_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_quantity_units_regex.py` & `ingredient_slicer-0.0.85/tests/test_quantity_units_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_remove_repeat_units_in_ranges.py` & `ingredient_slicer-0.0.85/tests/test_remove_repeat_units_in_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_remove_x_separators.py` & `ingredient_slicer-0.0.85/tests/test_remove_x_separators.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_replace_a_or_an_quantities.py` & `ingredient_slicer-0.0.85/tests/test_replace_a_or_an_quantities.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_separate_dimensions.py` & `ingredient_slicer-0.0.85/tests/test_separate_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_size_modifiers.py` & `ingredient_slicer-0.0.85/tests/test_size_modifiers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_spaced_numbers.py` & `ingredient_slicer-0.0.85/tests/test_spaced_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_unit_regex.py` & `ingredient_slicer-0.0.85/tests/test_unit_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_wild_ingredients.py` & `ingredient_slicer-0.0.85/tests/test_wild_ingredients.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_word_fractions.py` & `ingredient_slicer-0.0.85/tests/test_word_fractions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_word_numbers.py` & `ingredient_slicer-0.0.85/tests/test_word_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.84/tests/test_x_after_number_regex.py` & `ingredient_slicer-0.0.85/tests/test_x_after_number_regex.py`

 * *Files identical despite different names*

