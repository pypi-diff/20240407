# Comparing `tmp/dcm_classifier-0.7.0rc5.tar.gz` & `tmp/dcm_classifier-0.7.0rc6.tar.gz`

## Comparing `dcm_classifier-0.7.0rc5.tar` & `dcm_classifier-0.7.0rc6.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/push_pip.sh
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/requirements.txt
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/requirements_dev.txt
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/.github/ISSUE_TEMPLATE/chore-template.md
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/.github/ISSUE_TEMPLATE/documentation_improvement.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/.github/workflows/push_to_main.yml
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/Activate.ps1
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/activate
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/activate.csh
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/activate.fish
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/coloredlogs
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/f2py
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmanon
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmconv
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmdiff
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmdump
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmgendir
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmimg
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcminfo
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmpap3
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmraw
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmscanner
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmscu
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmtar
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/gdcmxml
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/humanfriendly
--rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/isympy
--rwxr-xr-x   0        0        0      280 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/onnxruntime_test
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/pip
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/pip3
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/pydicom
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/python -> python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/python3 -> /usr/bin/python3
--rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/min_req_venv/bin/tabulate
--rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/models/ova_rf_classifier.onnx
--rw-r--r--   0        0        0   197260 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/models/rf_classifier.onnx
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/anonymize_dicom_directory.py
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/classify_study.py
--rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/create_dicom_fields_sheet.py
--rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/create_training_sheet.py
--rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/dcm-classifier-training-tutorial.ipynb
--rw-r--r--   0        0        0    22366 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/modality_classifier_training.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/organize_dicom_to_bids.py
--rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/orientation_model_training.py
--rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/run_all_dicom_data_sheets.sh
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/running_classifier.ipynb
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/todo_list
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/training_config.py
--rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/scripts/utilities.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/README.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/__init__.py
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/dicom_config.py
--rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/dicom_series.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/dicom_validator.py
--rw-r--r--   0        0        0    18769 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/dicom_volume.py
--rw-r--r--   0        0        0    22684 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/example_image_processing.py
--rw-r--r--   0        0        0    18096 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/image_type_inference.py
--rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/study_processing.py
--rw-r--r--   0        0        0    32251 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/utility_functions.py
--rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/src/dcm_classifier/models/ova_rf_classifier.onnx
--rw-r--r--   0        0        0     8871 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/conftest.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/testing_data/.gitignore
--rw-r--r--   0        0        0  2200109 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/testing_data/anonymized_testing_data.tar.gz
--rw-r--r--   0        0        0   190042 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/testing_data/mock_data.txt
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/testing_data/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/testing_data/dummy_directory/dir_with_one_file/00.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/testing_data/dummy_directory/dir_with_two_files/100.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/testing_data/dummy_directory/dir_with_two_files/200.file
--rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/unit_testing/test_dicom_series.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/unit_testing/test_dicom_validator.py
--rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/unit_testing/test_dicom_volume.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/unit_testing/test_study_processing.py
--rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/tests/unit_testing/test_utility_functions.py
--rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/.gitignore
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/LICENSE
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/README.md
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/pyproject.toml
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc5/PKG-INFO
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/push_pip.sh
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/requirements.txt
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/requirements_dev.txt
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/.github/ISSUE_TEMPLATE/chore-template.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/.github/ISSUE_TEMPLATE/documentation_improvement.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/.github/workflows/push_to_main.yml
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/Activate.ps1
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/activate
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/activate.csh
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/activate.fish
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/coloredlogs
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/f2py
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmanon
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmconv
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmdiff
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmdump
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmgendir
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmimg
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcminfo
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmpap3
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmraw
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmscanner
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmscu
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmtar
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmxml
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/humanfriendly
+-rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/isympy
+-rwxr-xr-x   0        0        0      280 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/onnxruntime_test
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/pip
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/pip3
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/pydicom
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/python -> python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/python3 -> /usr/bin/python3
+-rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/tabulate
+-rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/models/ova_rf_classifier.onnx
+-rw-r--r--   0        0        0   197260 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/models/rf_classifier.onnx
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/anonymize_dicom_directory.py
+-rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/classify_study.py
+-rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/create_dicom_fields_sheet.py
+-rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/create_training_sheet.py
+-rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/dcm-classifier-training-tutorial.ipynb
+-rw-r--r--   0        0        0    22366 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/modality_classifier_training.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/organize_dicom_to_bids.py
+-rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/orientation_model_training.py
+-rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/run_all_dicom_data_sheets.sh
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/running_classifier.ipynb
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/todo_list
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/training_config.py
+-rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/utilities.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/README.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/__init__.py
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/dicom_config.py
+-rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/dicom_series.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/dicom_validator.py
+-rw-r--r--   0        0        0    18769 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/dicom_volume.py
+-rw-r--r--   0        0        0    22684 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/example_image_processing.py
+-rw-r--r--   0        0        0    18162 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/image_type_inference.py
+-rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/study_processing.py
+-rw-r--r--   0        0        0    32251 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/utility_functions.py
+-rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/models/ova_rf_classifier.onnx
+-rw-r--r--   0        0        0     8871 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/conftest.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/testing_data/.gitignore
+-rw-r--r--   0        0        0  2200109 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/testing_data/anonymized_testing_data.tar.gz
+-rw-r--r--   0        0        0   190042 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/testing_data/mock_data.txt
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/testing_data/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/testing_data/dummy_directory/dir_with_one_file/00.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/testing_data/dummy_directory/dir_with_two_files/100.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/testing_data/dummy_directory/dir_with_two_files/200.file
+-rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/unit_testing/test_dicom_series.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/unit_testing/test_dicom_validator.py
+-rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/unit_testing/test_dicom_volume.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/unit_testing/test_study_processing.py
+-rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/unit_testing/test_utility_functions.py
+-rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/.gitignore
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/LICENSE
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/README.md
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/pyproject.toml
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/PKG-INFO
```

### Comparing `dcm_classifier-0.7.0rc5/.pre-commit-config.yaml` & `dcm_classifier-0.7.0rc6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/.github/PULL_REQUEST_TEMPLATE.md` & `dcm_classifier-0.7.0rc6/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/.github/ISSUE_TEMPLATE/bug_report.md` & `dcm_classifier-0.7.0rc6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/.github/ISSUE_TEMPLATE/documentation_improvement.md` & `dcm_classifier-0.7.0rc6/.github/ISSUE_TEMPLATE/documentation_improvement.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/.github/ISSUE_TEMPLATE/feature_request.md` & `dcm_classifier-0.7.0rc6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/.github/workflows/push_to_main.yml` & `dcm_classifier-0.7.0rc6/.github/workflows/push_to_main.yml`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/min_req_venv/bin/Activate.ps1` & `dcm_classifier-0.7.0rc6/min_req_venv/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/min_req_venv/bin/activate` & `dcm_classifier-0.7.0rc6/min_req_venv/bin/activate`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/min_req_venv/bin/activate.csh` & `dcm_classifier-0.7.0rc6/min_req_venv/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/min_req_venv/bin/activate.fish` & `dcm_classifier-0.7.0rc6/min_req_venv/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/models/ova_rf_classifier.onnx` & `dcm_classifier-0.7.0rc6/models/ova_rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/models/rf_classifier.onnx` & `dcm_classifier-0.7.0rc6/models/rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/scripts/anonymize_dicom_directory.py` & `dcm_classifier-0.7.0rc6/scripts/anonymize_dicom_directory.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/scripts/classify_study.py` & `dcm_classifier-0.7.0rc6/scripts/classify_study.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         required=True,
         help="Path to the patient session directory with dicom data",
     )
     parser.add_argument(
         "-m",
         "--model",
         required=False,
-        default=None,
         help="Path to the model used for image type inference",
     )
     parser.add_argument(
         "-n",
         "--nifti_dir",
         required=False,
         default=None,
@@ -60,15 +59,19 @@
     nifti_dir: Path | None = Path(args.nifti_dir) if args.nifti_dir else None
     if nifti_dir:
         import itk
 
         nifti_dir.mkdir(parents=True, exist_ok=True)
 
     print(description)
-    inferer = ImageTypeClassifierBase(classification_model_filename=args.model)
+
+    if args.model is None:
+        inferer = ImageTypeClassifierBase()
+    else:
+        inferer = ImageTypeClassifierBase(classification_model_filename=args.model)
     study = ProcessOneDicomStudyToVolumesMappingBase(
         study_directory=args.session_directory, inferer=inferer
     )
     study.run_inference()
 
     list_of_inputs: list[dict[str, Any]] = []
     list_of_probabilities: list[pd.DataFrame] = []
```

### Comparing `dcm_classifier-0.7.0rc5/scripts/create_dicom_fields_sheet.py` & `dcm_classifier-0.7.0rc6/scripts/create_dicom_fields_sheet.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/scripts/create_training_sheet.py` & `dcm_classifier-0.7.0rc6/scripts/create_training_sheet.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/scripts/dcm-classifier-training-tutorial.ipynb` & `dcm_classifier-0.7.0rc6/scripts/dcm-classifier-training-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/scripts/modality_classifier_training.py` & `dcm_classifier-0.7.0rc6/scripts/modality_classifier_training.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/scripts/organize_dicom_to_bids.py` & `dcm_classifier-0.7.0rc6/scripts/organize_dicom_to_bids.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/scripts/orientation_model_training.py` & `dcm_classifier-0.7.0rc6/scripts/orientation_model_training.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/scripts/run_all_dicom_data_sheets.sh` & `dcm_classifier-0.7.0rc6/scripts/run_all_dicom_data_sheets.sh`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/scripts/running_classifier.ipynb` & `dcm_classifier-0.7.0rc6/scripts/running_classifier.ipynb`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/scripts/todo_list` & `dcm_classifier-0.7.0rc6/scripts/todo_list`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/scripts/training_config.py` & `dcm_classifier-0.7.0rc6/scripts/training_config.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/scripts/utilities.py` & `dcm_classifier-0.7.0rc6/scripts/utilities.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/src/dcm_classifier/dicom_config.py` & `dcm_classifier-0.7.0rc6/src/dcm_classifier/dicom_config.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/src/dcm_classifier/dicom_series.py` & `dcm_classifier-0.7.0rc6/src/dcm_classifier/dicom_series.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/src/dcm_classifier/dicom_validator.py` & `dcm_classifier-0.7.0rc6/src/dcm_classifier/dicom_validator.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/src/dcm_classifier/dicom_volume.py` & `dcm_classifier-0.7.0rc6/src/dcm_classifier/dicom_volume.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/src/dcm_classifier/example_image_processing.py` & `dcm_classifier-0.7.0rc6/src/dcm_classifier/example_image_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/src/dcm_classifier/image_type_inference.py` & `dcm_classifier-0.7.0rc6/src/dcm_classifier/image_type_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         infer_modality(self, feature_dict: dict = None) -> (str, pd.DataFrame):
 
         run_inference(self) -> None:
     """
 
     def __init__(
         self,
-        classification_model_filename: Optional[(str | Path)] = dcm_classifier_path
+        classification_model_filename: str | Path = dcm_classifier_path
         / "models"
         / "ova_rf_classifier.onnx",
         classification_feature_list: list[str] = inference_features,
         image_type_map: dict[str, int] = imagetype_to_integer_mapping,
         min_probability_threshold: float = 0.4,
     ):
         """
@@ -95,14 +95,15 @@
         Args:
             classification_model_filename (Union[str, Path]): Path to the classification model file (base implementation requires ONNX file).
             classification_feature_list (List[str]): List of features used for classification.
             image_type_map (Dict[str, str]): Mapping between class name and model integer output.
             mode (str): "series" or "volume" to run inference on series or volume level (a series could have multiple subvolumes).
             min_probability_threshold (float): Minimum probability threshold for classification, defaults to 0.4. If maximum class probability is below this threshold, the image type is set to "unknown".
         """
+        print("classification_model_filename", classification_model_filename)
         self.classification_model_filename: str | Path = Path(
             classification_model_filename
         )
         self.classification_feature_list: list[str] = classification_feature_list
         self.imagetype_to_int_map: dict[str, int] = image_type_map
         self.int_to_imagetype_map: dict[int, str] = self.get_int_to_type_map()
         self.min_probability_threshold: float = min_probability_threshold
```

### Comparing `dcm_classifier-0.7.0rc5/src/dcm_classifier/study_processing.py` & `dcm_classifier-0.7.0rc6/src/dcm_classifier/study_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/src/dcm_classifier/utility_functions.py` & `dcm_classifier-0.7.0rc6/src/dcm_classifier/utility_functions.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/src/dcm_classifier/models/ova_rf_classifier.onnx` & `dcm_classifier-0.7.0rc6/src/dcm_classifier/models/ova_rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/tests/conftest.py` & `dcm_classifier-0.7.0rc6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/tests/testing_data/anonymized_testing_data.tar.gz` & `dcm_classifier-0.7.0rc6/tests/testing_data/anonymized_testing_data.tar.gz`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/tests/testing_data/mock_data.txt` & `dcm_classifier-0.7.0rc6/tests/testing_data/mock_data.txt`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/tests/testing_data/test.py` & `dcm_classifier-0.7.0rc6/tests/testing_data/test.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/tests/unit_testing/test_dicom_series.py` & `dcm_classifier-0.7.0rc6/tests/unit_testing/test_dicom_series.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/tests/unit_testing/test_dicom_validator.py` & `dcm_classifier-0.7.0rc6/tests/unit_testing/test_dicom_validator.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/tests/unit_testing/test_dicom_volume.py` & `dcm_classifier-0.7.0rc6/tests/unit_testing/test_dicom_volume.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/tests/unit_testing/test_study_processing.py` & `dcm_classifier-0.7.0rc6/tests/unit_testing/test_study_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/tests/unit_testing/test_utility_functions.py` & `dcm_classifier-0.7.0rc6/tests/unit_testing/test_utility_functions.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/.gitignore` & `dcm_classifier-0.7.0rc6/.gitignore`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/LICENSE` & `dcm_classifier-0.7.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/README.md` & `dcm_classifier-0.7.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc5/pyproject.toml` & `dcm_classifier-0.7.0rc6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dcm_classifier"
-version = '0.7.0.rc5'
+version = '0.7.0.rc6'
 authors = [
   { name="Michal Brzus", email="michal-brzus@uiowa.edu" },
   { name="Hans Johnson", email="hans-johnson@uiowa.edu" },
 ]
 description = "This is a consolidation of work from NAMIC efforts primarily at the University of Iowa."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `dcm_classifier-0.7.0rc5/PKG-INFO` & `dcm_classifier-0.7.0rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dcm_classifier
-Version: 0.7.0rc5
+Version: 0.7.0rc6
 Summary: This is a consolidation of work from NAMIC efforts primarily at the University of Iowa.
 Author-email: Michal Brzus <michal-brzus@uiowa.edu>, Hans Johnson <hans-johnson@uiowa.edu>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: itk-core>=5.3.0
```

