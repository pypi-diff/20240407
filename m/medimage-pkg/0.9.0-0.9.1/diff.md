# Comparing `tmp/medimage_pkg-0.9.0.tar.gz` & `tmp/medimage_pkg-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medimage_pkg-0.9.0.tar", max compression
+gzip compressed data, was "medimage_pkg-0.9.1.tar", max compression
```

## Comparing `medimage_pkg-0.9.0.tar` & `medimage_pkg-0.9.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    35149 2024-04-06 22:02:39.205950 medimage_pkg-0.9.0/LICENSE.md
--rw-r--r--   0        0        0    76226 2024-04-06 22:02:39.205950 medimage_pkg-0.9.0/MEDimage/MEDscan.py
--rw-r--r--   0        0        0      565 2024-04-06 22:02:39.205950 medimage_pkg-0.9.0/MEDimage/__init__.py
--rw-r--r--   0        0        0    31152 2024-04-06 22:02:39.205950 medimage_pkg-0.9.0/MEDimage/biomarkers/BatchExtractor.py
--rw-r--r--   0        0        0    33266 2024-04-06 22:02:39.205950 medimage_pkg-0.9.0/MEDimage/biomarkers/BatchExtractorTexturalFilters.py
--rw-r--r--   0        0        0      417 2024-04-06 22:02:39.205950 medimage_pkg-0.9.0/MEDimage/biomarkers/__init__.py
--rw-r--r--   0        0        0     4199 2024-04-06 22:02:39.205950 medimage_pkg-0.9.0/MEDimage/biomarkers/diagnostics.py
--rwxr-xr-x   0        0        0     4979 2024-04-06 22:02:39.209950 medimage_pkg-0.9.0/MEDimage/biomarkers/get_oriented_bound_box.py
--rwxr-xr-x   0        0        0    68346 2024-04-06 22:02:39.209950 medimage_pkg-0.9.0/MEDimage/biomarkers/glcm.py
--rwxr-xr-x   0        0        0    19443 2024-04-06 22:02:39.209950 medimage_pkg-0.9.0/MEDimage/biomarkers/gldzm.py
--rwxr-xr-x   0        0        0    55673 2024-04-06 22:02:39.209950 medimage_pkg-0.9.0/MEDimage/biomarkers/glrlm.py
--rwxr-xr-x   0        0        0    18564 2024-04-06 22:02:39.209950 medimage_pkg-0.9.0/MEDimage/biomarkers/glszm.py
--rwxr-xr-x   0        0        0    19481 2024-04-06 22:02:39.209950 medimage_pkg-0.9.0/MEDimage/biomarkers/int_vol_hist.py
--rwxr-xr-x   0        0        0    22494 2024-04-06 22:02:39.209950 medimage_pkg-0.9.0/MEDimage/biomarkers/intensity_histogram.py
--rwxr-xr-x   0        0        0     3488 2024-04-06 22:02:39.209950 medimage_pkg-0.9.0/MEDimage/biomarkers/local_intensity.py
--rwxr-xr-x   0        0        0    69854 2024-04-06 22:02:39.209950 medimage_pkg-0.9.0/MEDimage/biomarkers/morph.py
--rwxr-xr-x   0        0        0    28146 2024-04-06 22:02:39.209950 medimage_pkg-0.9.0/MEDimage/biomarkers/ngldm.py
--rwxr-xr-x   0        0        0    16450 2024-04-06 22:02:39.209950 medimage_pkg-0.9.0/MEDimage/biomarkers/ngtdm.py
--rwxr-xr-x   0        0        0    14996 2024-04-06 22:02:39.209950 medimage_pkg-0.9.0/MEDimage/biomarkers/stats.py
--rw-r--r--   0        0        0    12357 2024-04-06 22:02:39.209950 medimage_pkg-0.9.0/MEDimage/biomarkers/utils.py
--rw-r--r--   0        0        0    11452 2024-04-06 22:02:39.209950 medimage_pkg-0.9.0/MEDimage/filters/TexturalFilter.py
--rw-r--r--   0        0        0      198 2024-04-06 22:02:39.209950 medimage_pkg-0.9.0/MEDimage/filters/__init__.py
--rw-r--r--   0        0        0     5876 2024-04-06 22:02:39.209950 medimage_pkg-0.9.0/MEDimage/filters/apply_filter.py
--rw-r--r--   0        0        0     8879 2024-04-06 22:02:39.209950 medimage_pkg-0.9.0/MEDimage/filters/gabor.py
--rw-r--r--   0        0        0    11336 2024-04-06 22:02:39.213950 medimage_pkg-0.9.0/MEDimage/filters/laws.py
--rw-r--r--   0        0        0     5873 2024-04-06 22:02:39.213950 medimage_pkg-0.9.0/MEDimage/filters/log.py
--rw-r--r--   0        0        0     4479 2024-04-06 22:02:39.213950 medimage_pkg-0.9.0/MEDimage/filters/mean.py
--rw-r--r--   0        0        0    55254 2024-04-06 22:02:39.213950 medimage_pkg-0.9.0/MEDimage/filters/textural_filters_kernels.py
--rw-r--r--   0        0        0     4046 2024-04-06 22:02:39.213950 medimage_pkg-0.9.0/MEDimage/filters/utils.py
--rw-r--r--   0        0        0     8899 2024-04-06 22:02:39.213950 medimage_pkg-0.9.0/MEDimage/filters/wavelet.py
--rw-r--r--   0        0        0     8983 2024-04-06 22:02:39.213950 medimage_pkg-0.9.0/MEDimage/learning/DataCleaner.py
--rw-r--r--   0        0        0    22038 2024-04-06 22:02:39.213950 medimage_pkg-0.9.0/MEDimage/learning/DesignExperiment.py
--rw-r--r--   0        0        0    29070 2024-04-06 22:02:39.213950 medimage_pkg-0.9.0/MEDimage/learning/FSR.py
--rw-r--r--   0        0        0     4611 2024-04-06 22:02:39.213950 medimage_pkg-0.9.0/MEDimage/learning/Normalization.py
--rw-r--r--   0        0        0    32824 2024-04-06 22:02:39.213950 medimage_pkg-0.9.0/MEDimage/learning/RadiomicsLearner.py
--rw-r--r--   0        0        0   101281 2024-04-06 22:02:39.213950 medimage_pkg-0.9.0/MEDimage/learning/Results.py
--rw-r--r--   0        0        0    27090 2024-04-06 22:02:39.213950 medimage_pkg-0.9.0/MEDimage/learning/Stats.py
--rw-r--r--   0        0        0      317 2024-04-06 22:02:39.213950 medimage_pkg-0.9.0/MEDimage/learning/__init__.py
--rw-r--r--   0        0        0     3955 2024-04-06 22:02:39.213950 medimage_pkg-0.9.0/MEDimage/learning/cleaning_utils.py
--rw-r--r--   0        0        0    40944 2024-04-06 22:02:39.213950 medimage_pkg-0.9.0/MEDimage/learning/ml_utils.py
--rw-r--r--   0        0        0      164 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/processing/__init__.py
--rw-r--r--   0        0        0     4273 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/processing/compute_suv_map.py
--rw-r--r--   0        0        0     5354 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/processing/discretisation.py
--rw-r--r--   0        0        0    13092 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/processing/interpolation.py
--rw-r--r--   0        0        0     1897 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/processing/resegmentation.py
--rw-r--r--   0        0        0    37375 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/processing/segmentation.py
--rw-r--r--   0        0        0      782 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/utils/__init__.py
--rw-r--r--   0        0        0     1537 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/utils/batch_patients.py
--rw-r--r--   0        0        0     5317 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/utils/create_radiomics_table.py
--rw-r--r--   0        0        0     1375 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/utils/data_frame_export.py
--rw-r--r--   0        0        0      398 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/utils/find_process_names.py
--rw-r--r--   0        0        0     1169 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/utils/get_file_paths.py
--rw-r--r--   0        0        0      649 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/utils/get_full_rad_names.py
--rw-r--r--   0        0        0      532 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/utils/get_institutions_from_ids.py
--rw-r--r--   0        0        0      518 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/utils/get_patient_id_from_scan_name.py
--rw-r--r--   0        0        0      674 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/utils/get_patient_names.py
--rw-r--r--   0        0        0      682 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/utils/get_radiomic_names.py
--rw-r--r--   0        0        0      583 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/utils/get_scan_name_from_rad_name.py
--rw-r--r--   0        0        0     1215 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/utils/image_reader_SITK.py
--rw-r--r--   0        0        0      677 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/utils/image_volume_obj.py
--rw-r--r--   0        0        0    15426 2024-04-06 22:02:39.217949 medimage_pkg-0.9.0/MEDimage/utils/imref.py
--rw-r--r--   0        0        0     2779 2024-04-06 22:02:39.221950 medimage_pkg-0.9.0/MEDimage/utils/initialize_features_names.py
--rw-r--r--   0        0        0     5670 2024-04-06 22:02:39.221950 medimage_pkg-0.9.0/MEDimage/utils/inpolygon.py
--rw-r--r--   0        0        0     1371 2024-04-06 22:02:39.221950 medimage_pkg-0.9.0/MEDimage/utils/interp3.py
--rw-r--r--   0        0        0     2242 2024-04-06 22:02:39.221950 medimage_pkg-0.9.0/MEDimage/utils/json_utils.py
--rw-r--r--   0        0        0      928 2024-04-06 22:02:39.221950 medimage_pkg-0.9.0/MEDimage/utils/mode.py
--rw-r--r--   0        0        0     2119 2024-04-06 22:02:39.221950 medimage_pkg-0.9.0/MEDimage/utils/parse_contour_string.py
--rw-r--r--   0        0        0      801 2024-04-06 22:02:39.221950 medimage_pkg-0.9.0/MEDimage/utils/save_MEDscan.py
--rw-r--r--   0        0        0      877 2024-04-06 22:02:39.221950 medimage_pkg-0.9.0/MEDimage/utils/strfind.py
--rw-r--r--   0        0        0     6162 2024-04-06 22:02:39.221950 medimage_pkg-0.9.0/MEDimage/utils/textureTools.py
--rw-r--r--   0        0        0     2253 2024-04-06 22:02:39.221950 medimage_pkg-0.9.0/MEDimage/utils/texture_features_names.py
--rw-r--r--   0        0        0     1537 2024-04-06 22:02:39.221950 medimage_pkg-0.9.0/MEDimage/utils/write_radiomics_csv.py
--rw-r--r--   0        0        0    84047 2024-04-06 22:02:39.221950 medimage_pkg-0.9.0/MEDimage/wrangling/DataManager.py
--rw-r--r--   0        0        0    24511 2024-04-06 22:02:39.221950 medimage_pkg-0.9.0/MEDimage/wrangling/ProcessDICOM.py
--rw-r--r--   0        0        0       71 2024-04-06 22:02:39.221950 medimage_pkg-0.9.0/MEDimage/wrangling/__init__.py
--rw-r--r--   0        0        0     9777 2024-04-06 22:02:39.221950 medimage_pkg-0.9.0/README.md
--rw-r--r--   0        0        0     1484 2024-04-06 22:02:39.417949 medimage_pkg-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    11807 1970-01-01 00:00:00.000000 medimage_pkg-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-06 22:02:39.205950 medimage_pkg-0.9.1/LICENSE.md
+-rw-r--r--   0        0        0    76226 2024-04-06 22:02:39.205950 medimage_pkg-0.9.1/MEDimage/MEDscan.py
+-rw-r--r--   0        0        0      565 2024-04-06 22:22:17.068115 medimage_pkg-0.9.1/MEDimage/__init__.py
+-rw-r--r--   0        0        0    31152 2024-04-06 22:02:39.205950 medimage_pkg-0.9.1/MEDimage/biomarkers/BatchExtractor.py
+-rw-r--r--   0        0        0    33266 2024-04-06 22:02:39.205950 medimage_pkg-0.9.1/MEDimage/biomarkers/BatchExtractorTexturalFilters.py
+-rw-r--r--   0        0        0      417 2024-04-06 22:02:39.205950 medimage_pkg-0.9.1/MEDimage/biomarkers/__init__.py
+-rw-r--r--   0        0        0     4199 2024-04-06 22:02:39.205950 medimage_pkg-0.9.1/MEDimage/biomarkers/diagnostics.py
+-rwxr-xr-x   0        0        0     4979 2024-04-06 22:02:39.209950 medimage_pkg-0.9.1/MEDimage/biomarkers/get_oriented_bound_box.py
+-rwxr-xr-x   0        0        0    68346 2024-04-06 22:02:39.209950 medimage_pkg-0.9.1/MEDimage/biomarkers/glcm.py
+-rwxr-xr-x   0        0        0    19443 2024-04-06 22:02:39.209950 medimage_pkg-0.9.1/MEDimage/biomarkers/gldzm.py
+-rwxr-xr-x   0        0        0    55673 2024-04-06 22:02:39.209950 medimage_pkg-0.9.1/MEDimage/biomarkers/glrlm.py
+-rwxr-xr-x   0        0        0    18564 2024-04-06 22:02:39.209950 medimage_pkg-0.9.1/MEDimage/biomarkers/glszm.py
+-rwxr-xr-x   0        0        0    19481 2024-04-06 22:02:39.209950 medimage_pkg-0.9.1/MEDimage/biomarkers/int_vol_hist.py
+-rwxr-xr-x   0        0        0    22494 2024-04-06 22:02:39.209950 medimage_pkg-0.9.1/MEDimage/biomarkers/intensity_histogram.py
+-rwxr-xr-x   0        0        0     3488 2024-04-06 22:02:39.209950 medimage_pkg-0.9.1/MEDimage/biomarkers/local_intensity.py
+-rwxr-xr-x   0        0        0    69854 2024-04-06 22:02:39.209950 medimage_pkg-0.9.1/MEDimage/biomarkers/morph.py
+-rwxr-xr-x   0        0        0    28146 2024-04-06 22:02:39.209950 medimage_pkg-0.9.1/MEDimage/biomarkers/ngldm.py
+-rwxr-xr-x   0        0        0    16450 2024-04-06 22:02:39.209950 medimage_pkg-0.9.1/MEDimage/biomarkers/ngtdm.py
+-rwxr-xr-x   0        0        0    14996 2024-04-06 22:02:39.209950 medimage_pkg-0.9.1/MEDimage/biomarkers/stats.py
+-rw-r--r--   0        0        0    12357 2024-04-06 22:02:39.209950 medimage_pkg-0.9.1/MEDimage/biomarkers/utils.py
+-rw-r--r--   0        0        0    11452 2024-04-06 22:02:39.209950 medimage_pkg-0.9.1/MEDimage/filters/TexturalFilter.py
+-rw-r--r--   0        0        0      198 2024-04-06 22:02:39.209950 medimage_pkg-0.9.1/MEDimage/filters/__init__.py
+-rw-r--r--   0        0        0     5876 2024-04-06 22:02:39.209950 medimage_pkg-0.9.1/MEDimage/filters/apply_filter.py
+-rw-r--r--   0        0        0     8879 2024-04-06 22:02:39.209950 medimage_pkg-0.9.1/MEDimage/filters/gabor.py
+-rw-r--r--   0        0        0    11336 2024-04-06 22:02:39.213950 medimage_pkg-0.9.1/MEDimage/filters/laws.py
+-rw-r--r--   0        0        0     5873 2024-04-06 22:02:39.213950 medimage_pkg-0.9.1/MEDimage/filters/log.py
+-rw-r--r--   0        0        0     4479 2024-04-06 22:02:39.213950 medimage_pkg-0.9.1/MEDimage/filters/mean.py
+-rw-r--r--   0        0        0    55254 2024-04-06 22:02:39.213950 medimage_pkg-0.9.1/MEDimage/filters/textural_filters_kernels.py
+-rw-r--r--   0        0        0     4046 2024-04-06 22:02:39.213950 medimage_pkg-0.9.1/MEDimage/filters/utils.py
+-rw-r--r--   0        0        0     8899 2024-04-06 22:02:39.213950 medimage_pkg-0.9.1/MEDimage/filters/wavelet.py
+-rw-r--r--   0        0        0     8983 2024-04-06 22:02:39.213950 medimage_pkg-0.9.1/MEDimage/learning/DataCleaner.py
+-rw-r--r--   0        0        0    22038 2024-04-06 22:02:39.213950 medimage_pkg-0.9.1/MEDimage/learning/DesignExperiment.py
+-rw-r--r--   0        0        0    29070 2024-04-06 22:02:39.213950 medimage_pkg-0.9.1/MEDimage/learning/FSR.py
+-rw-r--r--   0        0        0     4611 2024-04-06 22:02:39.213950 medimage_pkg-0.9.1/MEDimage/learning/Normalization.py
+-rw-r--r--   0        0        0    32824 2024-04-06 22:02:39.213950 medimage_pkg-0.9.1/MEDimage/learning/RadiomicsLearner.py
+-rw-r--r--   0        0        0   101281 2024-04-06 22:02:39.213950 medimage_pkg-0.9.1/MEDimage/learning/Results.py
+-rw-r--r--   0        0        0    27090 2024-04-06 22:02:39.213950 medimage_pkg-0.9.1/MEDimage/learning/Stats.py
+-rw-r--r--   0        0        0      317 2024-04-06 22:02:39.213950 medimage_pkg-0.9.1/MEDimage/learning/__init__.py
+-rw-r--r--   0        0        0     3955 2024-04-06 22:02:39.213950 medimage_pkg-0.9.1/MEDimage/learning/cleaning_utils.py
+-rw-r--r--   0        0        0    40944 2024-04-06 22:02:39.213950 medimage_pkg-0.9.1/MEDimage/learning/ml_utils.py
+-rw-r--r--   0        0        0      164 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/processing/__init__.py
+-rw-r--r--   0        0        0     4273 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/processing/compute_suv_map.py
+-rw-r--r--   0        0        0     5354 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/processing/discretisation.py
+-rw-r--r--   0        0        0    13092 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/processing/interpolation.py
+-rw-r--r--   0        0        0     1897 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/processing/resegmentation.py
+-rw-r--r--   0        0        0    37375 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/processing/segmentation.py
+-rw-r--r--   0        0        0      782 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/utils/__init__.py
+-rw-r--r--   0        0        0     1537 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/utils/batch_patients.py
+-rw-r--r--   0        0        0     5317 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/utils/create_radiomics_table.py
+-rw-r--r--   0        0        0     1375 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/utils/data_frame_export.py
+-rw-r--r--   0        0        0      398 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/utils/find_process_names.py
+-rw-r--r--   0        0        0     1169 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/utils/get_file_paths.py
+-rw-r--r--   0        0        0      649 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/utils/get_full_rad_names.py
+-rw-r--r--   0        0        0      532 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/utils/get_institutions_from_ids.py
+-rw-r--r--   0        0        0      518 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/utils/get_patient_id_from_scan_name.py
+-rw-r--r--   0        0        0      674 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/utils/get_patient_names.py
+-rw-r--r--   0        0        0      682 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/utils/get_radiomic_names.py
+-rw-r--r--   0        0        0      583 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/utils/get_scan_name_from_rad_name.py
+-rw-r--r--   0        0        0     1215 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/utils/image_reader_SITK.py
+-rw-r--r--   0        0        0      677 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/utils/image_volume_obj.py
+-rw-r--r--   0        0        0    15426 2024-04-06 22:02:39.217949 medimage_pkg-0.9.1/MEDimage/utils/imref.py
+-rw-r--r--   0        0        0     2779 2024-04-06 22:02:39.221950 medimage_pkg-0.9.1/MEDimage/utils/initialize_features_names.py
+-rw-r--r--   0        0        0     5670 2024-04-06 22:02:39.221950 medimage_pkg-0.9.1/MEDimage/utils/inpolygon.py
+-rw-r--r--   0        0        0     1371 2024-04-06 22:02:39.221950 medimage_pkg-0.9.1/MEDimage/utils/interp3.py
+-rw-r--r--   0        0        0     2242 2024-04-06 22:02:39.221950 medimage_pkg-0.9.1/MEDimage/utils/json_utils.py
+-rw-r--r--   0        0        0      928 2024-04-06 22:02:39.221950 medimage_pkg-0.9.1/MEDimage/utils/mode.py
+-rw-r--r--   0        0        0     2119 2024-04-06 22:02:39.221950 medimage_pkg-0.9.1/MEDimage/utils/parse_contour_string.py
+-rw-r--r--   0        0        0      801 2024-04-06 22:02:39.221950 medimage_pkg-0.9.1/MEDimage/utils/save_MEDscan.py
+-rw-r--r--   0        0        0      877 2024-04-06 22:02:39.221950 medimage_pkg-0.9.1/MEDimage/utils/strfind.py
+-rw-r--r--   0        0        0     6162 2024-04-06 22:02:39.221950 medimage_pkg-0.9.1/MEDimage/utils/textureTools.py
+-rw-r--r--   0        0        0     2253 2024-04-06 22:02:39.221950 medimage_pkg-0.9.1/MEDimage/utils/texture_features_names.py
+-rw-r--r--   0        0        0     1537 2024-04-06 22:02:39.221950 medimage_pkg-0.9.1/MEDimage/utils/write_radiomics_csv.py
+-rw-r--r--   0        0        0    84047 2024-04-06 22:02:39.221950 medimage_pkg-0.9.1/MEDimage/wrangling/DataManager.py
+-rw-r--r--   0        0        0    24511 2024-04-06 22:02:39.221950 medimage_pkg-0.9.1/MEDimage/wrangling/ProcessDICOM.py
+-rw-r--r--   0        0        0       71 2024-04-06 22:02:39.221950 medimage_pkg-0.9.1/MEDimage/wrangling/__init__.py
+-rw-r--r--   0        0        0     9777 2024-04-06 22:02:39.221950 medimage_pkg-0.9.1/README.md
+-rw-r--r--   0        0        0     1360 2024-04-06 22:25:15.483890 medimage_pkg-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    11495 1970-01-01 00:00:00.000000 medimage_pkg-0.9.1/PKG-INFO
```

### Comparing `medimage_pkg-0.9.0/LICENSE.md` & `medimage_pkg-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/MEDscan.py` & `medimage_pkg-0.9.1/MEDimage/MEDscan.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/__init__.py` & `medimage_pkg-0.9.1/MEDimage/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 
 
 stream_handler = logging.StreamHandler()
 stream_handler.setLevel(logging.WARNING)
 logging.getLogger(__name__).addHandler(stream_handler)
 
 __author__ = "MEDomicsLab consortium"
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 __copyright__ = "Copyright (C) MEDomicsLab consortium"
 __license__ = "GNU General Public License 3.0"
 __maintainer__ = "MAHDI AIT LHAJ LOUTFI"
 __email__ = "medomics.info@gmail.com"
```

### Comparing `medimage_pkg-0.9.0/MEDimage/biomarkers/BatchExtractor.py` & `medimage_pkg-0.9.1/MEDimage/biomarkers/BatchExtractor.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/biomarkers/BatchExtractorTexturalFilters.py` & `medimage_pkg-0.9.1/MEDimage/biomarkers/BatchExtractorTexturalFilters.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/biomarkers/diagnostics.py` & `medimage_pkg-0.9.1/MEDimage/biomarkers/diagnostics.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/biomarkers/get_oriented_bound_box.py` & `medimage_pkg-0.9.1/MEDimage/biomarkers/get_oriented_bound_box.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/biomarkers/glcm.py` & `medimage_pkg-0.9.1/MEDimage/biomarkers/glcm.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/biomarkers/gldzm.py` & `medimage_pkg-0.9.1/MEDimage/biomarkers/gldzm.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/biomarkers/glrlm.py` & `medimage_pkg-0.9.1/MEDimage/biomarkers/glrlm.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/biomarkers/glszm.py` & `medimage_pkg-0.9.1/MEDimage/biomarkers/glszm.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/biomarkers/int_vol_hist.py` & `medimage_pkg-0.9.1/MEDimage/biomarkers/int_vol_hist.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/biomarkers/intensity_histogram.py` & `medimage_pkg-0.9.1/MEDimage/biomarkers/intensity_histogram.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/biomarkers/local_intensity.py` & `medimage_pkg-0.9.1/MEDimage/biomarkers/local_intensity.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/biomarkers/morph.py` & `medimage_pkg-0.9.1/MEDimage/biomarkers/morph.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/biomarkers/ngldm.py` & `medimage_pkg-0.9.1/MEDimage/biomarkers/ngldm.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/biomarkers/ngtdm.py` & `medimage_pkg-0.9.1/MEDimage/biomarkers/ngtdm.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/biomarkers/stats.py` & `medimage_pkg-0.9.1/MEDimage/biomarkers/stats.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/biomarkers/utils.py` & `medimage_pkg-0.9.1/MEDimage/biomarkers/utils.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/filters/TexturalFilter.py` & `medimage_pkg-0.9.1/MEDimage/filters/TexturalFilter.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/filters/apply_filter.py` & `medimage_pkg-0.9.1/MEDimage/filters/apply_filter.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/filters/gabor.py` & `medimage_pkg-0.9.1/MEDimage/filters/gabor.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/filters/laws.py` & `medimage_pkg-0.9.1/MEDimage/filters/laws.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/filters/log.py` & `medimage_pkg-0.9.1/MEDimage/filters/log.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/filters/mean.py` & `medimage_pkg-0.9.1/MEDimage/filters/mean.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/filters/textural_filters_kernels.py` & `medimage_pkg-0.9.1/MEDimage/filters/textural_filters_kernels.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/filters/utils.py` & `medimage_pkg-0.9.1/MEDimage/filters/utils.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/filters/wavelet.py` & `medimage_pkg-0.9.1/MEDimage/filters/wavelet.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/learning/DataCleaner.py` & `medimage_pkg-0.9.1/MEDimage/learning/DataCleaner.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/learning/DesignExperiment.py` & `medimage_pkg-0.9.1/MEDimage/learning/DesignExperiment.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/learning/FSR.py` & `medimage_pkg-0.9.1/MEDimage/learning/FSR.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/learning/Normalization.py` & `medimage_pkg-0.9.1/MEDimage/learning/Normalization.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/learning/RadiomicsLearner.py` & `medimage_pkg-0.9.1/MEDimage/learning/RadiomicsLearner.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/learning/Results.py` & `medimage_pkg-0.9.1/MEDimage/learning/Results.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/learning/Stats.py` & `medimage_pkg-0.9.1/MEDimage/learning/Stats.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/learning/cleaning_utils.py` & `medimage_pkg-0.9.1/MEDimage/learning/cleaning_utils.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/learning/ml_utils.py` & `medimage_pkg-0.9.1/MEDimage/learning/ml_utils.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/processing/compute_suv_map.py` & `medimage_pkg-0.9.1/MEDimage/processing/compute_suv_map.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/processing/discretisation.py` & `medimage_pkg-0.9.1/MEDimage/processing/discretisation.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/processing/interpolation.py` & `medimage_pkg-0.9.1/MEDimage/processing/interpolation.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/processing/resegmentation.py` & `medimage_pkg-0.9.1/MEDimage/processing/resegmentation.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/processing/segmentation.py` & `medimage_pkg-0.9.1/MEDimage/processing/segmentation.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/__init__.py` & `medimage_pkg-0.9.1/MEDimage/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/batch_patients.py` & `medimage_pkg-0.9.1/MEDimage/utils/batch_patients.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/create_radiomics_table.py` & `medimage_pkg-0.9.1/MEDimage/utils/create_radiomics_table.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/data_frame_export.py` & `medimage_pkg-0.9.1/MEDimage/utils/data_frame_export.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/get_file_paths.py` & `medimage_pkg-0.9.1/MEDimage/utils/get_file_paths.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/get_full_rad_names.py` & `medimage_pkg-0.9.1/MEDimage/utils/get_full_rad_names.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/get_institutions_from_ids.py` & `medimage_pkg-0.9.1/MEDimage/utils/get_institutions_from_ids.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/get_patient_id_from_scan_name.py` & `medimage_pkg-0.9.1/MEDimage/utils/get_patient_id_from_scan_name.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/get_patient_names.py` & `medimage_pkg-0.9.1/MEDimage/utils/get_patient_names.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/get_radiomic_names.py` & `medimage_pkg-0.9.1/MEDimage/utils/get_radiomic_names.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/get_scan_name_from_rad_name.py` & `medimage_pkg-0.9.1/MEDimage/utils/get_scan_name_from_rad_name.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/image_reader_SITK.py` & `medimage_pkg-0.9.1/MEDimage/utils/image_reader_SITK.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/image_volume_obj.py` & `medimage_pkg-0.9.1/MEDimage/utils/image_volume_obj.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/imref.py` & `medimage_pkg-0.9.1/MEDimage/utils/imref.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/initialize_features_names.py` & `medimage_pkg-0.9.1/MEDimage/utils/initialize_features_names.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/inpolygon.py` & `medimage_pkg-0.9.1/MEDimage/utils/inpolygon.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/interp3.py` & `medimage_pkg-0.9.1/MEDimage/utils/interp3.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/json_utils.py` & `medimage_pkg-0.9.1/MEDimage/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/mode.py` & `medimage_pkg-0.9.1/MEDimage/utils/mode.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/parse_contour_string.py` & `medimage_pkg-0.9.1/MEDimage/utils/parse_contour_string.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/save_MEDscan.py` & `medimage_pkg-0.9.1/MEDimage/utils/save_MEDscan.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/strfind.py` & `medimage_pkg-0.9.1/MEDimage/utils/strfind.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/textureTools.py` & `medimage_pkg-0.9.1/MEDimage/utils/textureTools.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/texture_features_names.py` & `medimage_pkg-0.9.1/MEDimage/utils/texture_features_names.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/utils/write_radiomics_csv.py` & `medimage_pkg-0.9.1/MEDimage/utils/write_radiomics_csv.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/wrangling/DataManager.py` & `medimage_pkg-0.9.1/MEDimage/wrangling/DataManager.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/MEDimage/wrangling/ProcessDICOM.py` & `medimage_pkg-0.9.1/MEDimage/wrangling/ProcessDICOM.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/README.md` & `medimage_pkg-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.0/PKG-INFO` & `medimage_pkg-0.9.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 Metadata-Version: 2.1
 Name: medimage-pkg
-Version: 0.9.0
+Version: 0.9.1
 Summary: MEDimage is a Python package for processing and extracting features from medical images
 Home-page: https://github.com/medomics/MEDomicsLab-develop
 License: GPL-3.0
 Keywords: python,ibsi,medical-imaging,cancer-imaging-research,radiomics,medical-image-analysis,features-extraction,radiomics-extraction,radiomics-features,radiomics-analysis
 Author: MEDomics Consortium
 Author-email: medomics.info@gmail.com
 Requires-Python: >=3.8.0,<=3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: Pillow (==9.2.0)
-Requires-Dist: PyWavelets (==1.1.1)
-Requires-Dist: SimpleITK (==2.1.1.2)
-Requires-Dist: Sphinx (==7.2.6)
-Requires-Dist: ipykernel (>=6.15.1,<7.0.0)
-Requires-Dist: ipywidgets (>=8.0.1,<9.0.0)
-Requires-Dist: isort (==5.10.1)
-Requires-Dist: jupyter (>=1.0.0,<2.0.0)
-Requires-Dist: matplotlib (==3.7.0)
-Requires-Dist: networkx (==2.8.5)
-Requires-Dist: neuroCombat (==0.2.12)
-Requires-Dist: nibabel (==3.2.2)
-Requires-Dist: nilearn (==0.10.1)
-Requires-Dist: numpy (==1.22.4)
-Requires-Dist: numpyencoder (==0.3.0)
-Requires-Dist: pandas (==1.5.3)
-Requires-Dist: protobuf (==3.20.*)
-Requires-Dist: pycaret (==3.0.4)
-Requires-Dist: pydicom (==1.2.2)
-Requires-Dist: ray (==2.5.1)
-Requires-Dist: scikit-image (==0.18.2)
-Requires-Dist: scikit_learn (==1.2.2)
-Requires-Dist: scipy (==1.7.0)
-Requires-Dist: seaborn (==0.13.2)
-Requires-Dist: setuptools (==62.2.0)
+Requires-Dist: Pillow
+Requires-Dist: PyWavelets
+Requires-Dist: SimpleITK
+Requires-Dist: Sphinx
+Requires-Dist: ipykernel
+Requires-Dist: ipywidgets
+Requires-Dist: isort
+Requires-Dist: jupyter
+Requires-Dist: matplotlib
+Requires-Dist: networkx
+Requires-Dist: neuroCombat
+Requires-Dist: nibabel
+Requires-Dist: nilearn
+Requires-Dist: numpy
+Requires-Dist: numpyencoder
+Requires-Dist: pandas (<2.0.0)
+Requires-Dist: protobuf
+Requires-Dist: pycaret
+Requires-Dist: pydicom
+Requires-Dist: ray
+Requires-Dist: scikit_image
+Requires-Dist: scikit_learn
+Requires-Dist: scipy
+Requires-Dist: seaborn
+Requires-Dist: setuptools
 Requires-Dist: sphinx-carousel (==1.2.0)
 Requires-Dist: sphinx-jsonschema (==1.19.1)
 Requires-Dist: sphinx-rtd-dark-mode (==1.2.4)
-Requires-Dist: tabulate (==0.9.0)
-Requires-Dist: tqdm (==4.65.0)
-Requires-Dist: wget (==3.2)
-Requires-Dist: xgboost (==1.7.6)
+Requires-Dist: tabulate
+Requires-Dist: tqdm
+Requires-Dist: wget
+Requires-Dist: xgboost
 Project-URL: Repository, https://github.com/medomics/MEDomicsLab-develop
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 <img src="https://raw.githubusercontent.com/MahdiAll99/MEDimage/dev/docs/figures/MEDimageLogo.png" style="width:150px;"/>
```

