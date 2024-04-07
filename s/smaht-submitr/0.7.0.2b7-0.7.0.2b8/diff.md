# Comparing `tmp/smaht_submitr-0.7.0.2b7.tar.gz` & `tmp/smaht_submitr-0.7.0.2b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smaht_submitr-0.7.0.2b7.tar", max compression
+gzip compressed data, was "smaht_submitr-0.7.0.2b8.tar", max compression
```

## Comparing `smaht_submitr-0.7.0.2b7.tar` & `smaht_submitr-0.7.0.2b8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1098 2024-04-07 15:31:12.253193 smaht_submitr-0.7.0.2b7/LICENSE.txt
--rw-r--r--   0        0        0     2602 2024-04-07 15:31:12.253193 smaht_submitr-0.7.0.2b7/README.rst
--rw-r--r--   0        0        0     3425 2024-04-07 15:31:12.289193 smaht_submitr-0.7.0.2b7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-07 15:31:12.289193 smaht_submitr-0.7.0.2b7/submitr/__init__.py
--rw-r--r--   0        0        0      731 2024-04-07 15:31:12.289193 smaht_submitr-0.7.0.2b7/submitr/base.py
--rw-r--r--   0        0        0      294 2024-04-07 15:31:12.289193 smaht_submitr-0.7.0.2b7/submitr/exceptions.py
--rw-r--r--   0        0        0     2628 2024-04-07 15:31:12.289193 smaht_submitr-0.7.0.2b7/submitr/output.py
--rw-r--r--   0        0        0    12781 2024-04-07 15:31:12.289193 smaht_submitr-0.7.0.2b7/submitr/progress_bar.py
--rw-r--r--   0        0        0    10819 2024-04-07 15:31:12.289193 smaht_submitr-0.7.0.2b7/submitr/s3_utils.py
--rw-r--r--   0        0        0        0 2024-04-07 15:31:12.289193 smaht_submitr-0.7.0.2b7/submitr/scripts/__init__.py
--rw-r--r--   0        0        0     4785 2024-04-07 15:31:12.289193 smaht_submitr-0.7.0.2b7/submitr/scripts/check_submission.py
--rw-r--r--   0        0        0     8466 2024-04-07 15:31:12.289193 smaht_submitr-0.7.0.2b7/submitr/scripts/cli_utils.py
--rw-r--r--   0        0        0     1828 2024-04-07 15:31:12.289193 smaht_submitr-0.7.0.2b7/submitr/scripts/list_submissions.py
--rw-r--r--   0        0        0      940 2024-04-07 15:31:12.289193 smaht_submitr-0.7.0.2b7/submitr/scripts/make_sample_fastq_file.py
--rw-r--r--   0        0        0     5709 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/scripts/resume_uploads.py
--rw-r--r--   0        0        0     1368 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/scripts/show_upload_info.py
--rw-r--r--   0        0        0     1572 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/scripts/submit_genelist.py
--rw-r--r--   0        0        0    19891 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/scripts/submit_metadata_bundle.py
--rw-r--r--   0        0        0     3437 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/scripts/submit_ontology.py
--rw-r--r--   0        0        0     1616 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/scripts/upload_item_data.py
--rw-r--r--   0        0        0    28731 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/scripts/view_portal_object.py
--rw-r--r--   0        0        0   152386 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/submission.py
--rw-r--r--   0        0        0        0 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/__init__.py
--rw-r--r--   0        0        0      355 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/conftest_settings.py
--rw-r--r--   0        0        0      163 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/data/f1_R1.fastq.gz
--rw-r--r--   0        0        0      165 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/data/f1_R2.fastq.gz
--rw-r--r--   0        0        0      167 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/data/f2_R1.fastq.gz
--rw-r--r--   0        0        0      164 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/data/f2_R2.fastq.gz
--rw-r--r--   0        0        0      272 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/data/simulated_bundle.json
--rw-r--r--   0        0        0    10870 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/data/submission_simple.xlsx
--rw-r--r--   0        0        0    10875 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/data/submission_simple2.xlsx
--rw-r--r--   0        0        0    13306 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/data/submission_test.xlsx
--rw-r--r--   0        0        0    13192 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/data/submission_test_with_errors.xlsx
--rw-r--r--   0        0        0      169 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/data/test1_R1.fastq.gz
--rw-r--r--   0        0        0      168 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/data/test1_R2.fastq.gz
--rw-r--r--   0        0        0     1333 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/test_base.py
--rw-r--r--   0        0        0     2629 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/test_check_submission.py
--rw-r--r--   0        0        0      551 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/test_exceptions.py
--rw-r--r--   0        0        0     1620 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/test_make_sample_fastq_file.py
--rw-r--r--   0        0        0     1421 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/test_misc.py
--rw-r--r--   0        0        0    11606 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/test_resume_uploads.py
--rw-r--r--   0        0        0     2478 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/test_show_upload_info.py
--rw-r--r--   0        0        0   157433 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/test_submission.py
--rw-r--r--   0        0        0     2836 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/test_submit_genelist.py
--rw-r--r--   0        0        0     6874 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/test_submit_metadata_bundle.py
--rw-r--r--   0        0        0     3013 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/test_submit_ontology.py
--rw-r--r--   0        0        0     1300 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/test_testing_helpers.py
--rw-r--r--   0        0        0     3661 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/test_upload_item_data.py
--rw-r--r--   0        0        0     4353 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/test_utils.py
--rw-r--r--   0        0        0     1351 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/tests/testing_helpers.py
--rw-r--r--   0        0        0    12167 2024-04-07 15:31:12.293192 smaht_submitr-0.7.0.2b7/submitr/utils.py
--rw-r--r--   0        0        0     3994 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.2b7/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-07 18:33:59.305295 smaht_submitr-0.7.0.2b8/LICENSE.txt
+-rw-r--r--   0        0        0     2602 2024-04-07 18:33:59.305295 smaht_submitr-0.7.0.2b8/README.rst
+-rw-r--r--   0        0        0     3425 2024-04-07 18:33:59.341295 smaht_submitr-0.7.0.2b8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-07 18:33:59.341295 smaht_submitr-0.7.0.2b8/submitr/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-07 18:33:59.341295 smaht_submitr-0.7.0.2b8/submitr/base.py
+-rw-r--r--   0        0        0      294 2024-04-07 18:33:59.341295 smaht_submitr-0.7.0.2b8/submitr/exceptions.py
+-rw-r--r--   0        0        0     2628 2024-04-07 18:33:59.341295 smaht_submitr-0.7.0.2b8/submitr/output.py
+-rw-r--r--   0        0        0    12781 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/progress_bar.py
+-rw-r--r--   0        0        0    10819 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/s3_utils.py
+-rw-r--r--   0        0        0        0 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/scripts/__init__.py
+-rw-r--r--   0        0        0     4785 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/scripts/check_submission.py
+-rw-r--r--   0        0        0     8466 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/scripts/cli_utils.py
+-rw-r--r--   0        0        0     1828 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/scripts/list_submissions.py
+-rw-r--r--   0        0        0      940 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/scripts/make_sample_fastq_file.py
+-rw-r--r--   0        0        0     5709 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/scripts/resume_uploads.py
+-rw-r--r--   0        0        0     1368 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/scripts/show_upload_info.py
+-rw-r--r--   0        0        0     1572 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/scripts/submit_genelist.py
+-rw-r--r--   0        0        0    19891 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/scripts/submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3437 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/scripts/submit_ontology.py
+-rw-r--r--   0        0        0     1616 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/scripts/upload_item_data.py
+-rw-r--r--   0        0        0    28731 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/scripts/view_portal_object.py
+-rw-r--r--   0        0        0   152460 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/submission.py
+-rw-r--r--   0        0        0        0 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/__init__.py
+-rw-r--r--   0        0        0      355 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/conftest_settings.py
+-rw-r--r--   0        0        0      163 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/data/f1_R1.fastq.gz
+-rw-r--r--   0        0        0      165 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/data/f1_R2.fastq.gz
+-rw-r--r--   0        0        0      167 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/data/f2_R1.fastq.gz
+-rw-r--r--   0        0        0      164 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/data/f2_R2.fastq.gz
+-rw-r--r--   0        0        0      272 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/data/simulated_bundle.json
+-rw-r--r--   0        0        0    10870 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/data/submission_simple.xlsx
+-rw-r--r--   0        0        0    10875 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/data/submission_simple2.xlsx
+-rw-r--r--   0        0        0    13306 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/data/submission_test.xlsx
+-rw-r--r--   0        0        0    13192 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/data/submission_test_with_errors.xlsx
+-rw-r--r--   0        0        0      169 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/data/test1_R1.fastq.gz
+-rw-r--r--   0        0        0      168 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/data/test1_R2.fastq.gz
+-rw-r--r--   0        0        0     1333 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/test_base.py
+-rw-r--r--   0        0        0     2629 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/test_check_submission.py
+-rw-r--r--   0        0        0      551 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1620 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/test_make_sample_fastq_file.py
+-rw-r--r--   0        0        0     1421 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/test_misc.py
+-rw-r--r--   0        0        0    11606 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/test_resume_uploads.py
+-rw-r--r--   0        0        0     2478 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/test_show_upload_info.py
+-rw-r--r--   0        0        0   157490 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/test_submission.py
+-rw-r--r--   0        0        0     2836 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/test_submit_genelist.py
+-rw-r--r--   0        0        0     6874 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/test_submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3013 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/test_submit_ontology.py
+-rw-r--r--   0        0        0     1300 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/test_testing_helpers.py
+-rw-r--r--   0        0        0     3661 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/test_upload_item_data.py
+-rw-r--r--   0        0        0     4353 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/test_utils.py
+-rw-r--r--   0        0        0     1351 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/tests/testing_helpers.py
+-rw-r--r--   0        0        0    12167 2024-04-07 18:33:59.345295 smaht_submitr-0.7.0.2b8/submitr/utils.py
+-rw-r--r--   0        0        0     3994 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.2b8/PKG-INFO
```

### Comparing `smaht_submitr-0.7.0.2b7/LICENSE.txt` & `smaht_submitr-0.7.0.2b8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/README.rst` & `smaht_submitr-0.7.0.2b8/README.rst`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/pyproject.toml` & `smaht_submitr-0.7.0.2b8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smaht-submitr"
-version = "0.7.0.2b7"  # TODO: To become 0.8.0
+version = "0.7.0.2b8"  # TODO: To become 0.8.0
 description = "Support for uploading file submissions to SMAHT."
 # TODO: Update this email address when a more specific one is available for SMaHT.
 authors = ["SMaHT DAC <smhelp@hms-dbmi.atlassian.net >"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["submitr", "smaht"]
 homepage = "https://github.com/smaht-dac/submitr"
```

### Comparing `smaht_submitr-0.7.0.2b7/submitr/base.py` & `smaht_submitr-0.7.0.2b8/submitr/base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/output.py` & `smaht_submitr-0.7.0.2b8/submitr/output.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/progress_bar.py` & `smaht_submitr-0.7.0.2b8/submitr/progress_bar.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/s3_utils.py` & `smaht_submitr-0.7.0.2b8/submitr/s3_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/scripts/check_submission.py` & `smaht_submitr-0.7.0.2b8/submitr/scripts/check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/scripts/cli_utils.py` & `smaht_submitr-0.7.0.2b8/submitr/scripts/cli_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/scripts/list_submissions.py` & `smaht_submitr-0.7.0.2b8/submitr/scripts/list_submissions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/scripts/make_sample_fastq_file.py` & `smaht_submitr-0.7.0.2b8/submitr/scripts/make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/scripts/resume_uploads.py` & `smaht_submitr-0.7.0.2b8/submitr/scripts/resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/scripts/show_upload_info.py` & `smaht_submitr-0.7.0.2b8/submitr/scripts/show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/scripts/submit_genelist.py` & `smaht_submitr-0.7.0.2b8/submitr/scripts/submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/scripts/submit_metadata_bundle.py` & `smaht_submitr-0.7.0.2b8/submitr/scripts/submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/scripts/submit_ontology.py` & `smaht_submitr-0.7.0.2b8/submitr/scripts/submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/scripts/upload_item_data.py` & `smaht_submitr-0.7.0.2b8/submitr/scripts/upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/scripts/view_portal_object.py` & `smaht_submitr-0.7.0.2b8/submitr/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/submission.py` & `smaht_submitr-0.7.0.2b8/submitr/submission.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 DEFAULT_INGESTION_TYPE = 'metadata_bundle'
 GENERIC_SCHEMA_TYPE = 'FileOther'
 
 
 # Maximum amount of time (approximately) we will wait for a response from server (seconds).
 PROGRESS_TIMEOUT = 60 * 5  # five minutes (note this is for both server validation and submission)
 # How often we actually check the server (seconds).
-PROGRESS_CHECK_SERVER_INTERVAL = 3  # xyzzy
+PROGRESS_CHECK_SERVER_INTERVAL = 3
 # How often the (tqdm) progress meter updates (seconds).
 PROGRESS_INTERVAL = 1
 # How many times the (tqdm) progress meter updates (derived from above).
 PROGRESS_MAX_CHECKS = round(PROGRESS_TIMEOUT / PROGRESS_INTERVAL)
 
 
 class SubmissionProtocol:
@@ -459,15 +459,16 @@
         else:
             [SHOW(line) for line in section_data]
     else:  # We don't expect this, but such should be shown as-is, mostly to see what it is.
         SHOW(section_data)
 
 
 def _ingestion_submission_item_url(server, uuid):
-    return url_path_join(server, "ingestion-submissions", uuid) + "?format=json"
+    # Note that we use datastore=database for quicker feedback.
+    return url_path_join(server, "ingestion-submissions", uuid) + "?format=json&datastore=database"
 
 
 # TRY_OLD_PROTOCOL = True
 DEBUG_PROTOCOL = environ_bool("DEBUG_PROTOCOL", default=False)
 
 
 def _initiate_server_ingestion_process(
```

### Comparing `smaht_submitr-0.7.0.2b7/submitr/tests/data/submission_simple.xlsx` & `smaht_submitr-0.7.0.2b8/submitr/tests/data/submission_simple.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/tests/data/submission_simple2.xlsx` & `smaht_submitr-0.7.0.2b8/submitr/tests/data/submission_simple2.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/tests/data/submission_test.xlsx` & `smaht_submitr-0.7.0.2b8/submitr/tests/data/submission_test.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/tests/data/submission_test_with_errors.xlsx` & `smaht_submitr-0.7.0.2b8/submitr/tests/data/submission_test_with_errors.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/tests/test_base.py` & `smaht_submitr-0.7.0.2b8/submitr/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/tests/test_check_submission.py` & `smaht_submitr-0.7.0.2b8/submitr/tests/test_check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/tests/test_exceptions.py` & `smaht_submitr-0.7.0.2b8/submitr/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/tests/test_make_sample_fastq_file.py` & `smaht_submitr-0.7.0.2b8/submitr/tests/test_make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/tests/test_misc.py` & `smaht_submitr-0.7.0.2b8/submitr/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/tests/test_resume_uploads.py` & `smaht_submitr-0.7.0.2b8/submitr/tests/test_resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/tests/test_show_upload_info.py` & `smaht_submitr-0.7.0.2b8/submitr/tests/test_show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/tests/test_submission.py` & `smaht_submitr-0.7.0.2b8/submitr/tests/test_submission.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,25 +342,25 @@
 
 
 def test_ingestion_submission_item_url():
 
     assert _ingestion_submission_item_url(
         server='http://foo.com',
         uuid='123-4567-890'
-    ) == 'http://foo.com/ingestion-submissions/123-4567-890?format=json'
+    ) == 'http://foo.com/ingestion-submissions/123-4567-890?format=json&datastore=database'
 
 
 def test_show_upload_info():
 
     json_result = None  # Actual value comes later
 
     index = 0
 
     URLS = [
-        f"{SOME_SERVER}/ingestion-submissions/{SOME_UUID}?format=json",
+        f"{SOME_SERVER}/ingestion-submissions/{SOME_UUID}?format=json&datastore=database",
         f"{SOME_SERVER}/health",
         f"{SOME_SERVER}/{SOME_UPLOAD_INFO[0]['uuid']}",
         f"{SOME_SERVER}/{SOME_UPLOAD_INFO[1]['uuid']}"
     ]
 
     def mocked_get(url, *, auth, **kwargs):
         nonlocal index
@@ -2009,15 +2009,15 @@
                     submission_center=SOME_SUBMISSION_CENTER,
                     # project=SOME_PROJECT,
                     # user_institution=[
                     #     {'@id': SOME_INSTITUTION}
                     # ]
                 ))
             else:
-                assert url.endswith('/ingestion-submissions/' + SOME_UUID + "?format=json")
+                assert url.endswith('/ingestion-submissions/' + SOME_UUID + "?format=json&datastore=database")
                 return FakeResponse(200, json=response_maker())
         return mocked_get
 
     mfs = MockFileSystem()
 
     dt = ControlledTime()
```

### Comparing `smaht_submitr-0.7.0.2b7/submitr/tests/test_submit_genelist.py` & `smaht_submitr-0.7.0.2b8/submitr/tests/test_submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/tests/test_submit_metadata_bundle.py` & `smaht_submitr-0.7.0.2b8/submitr/tests/test_submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/tests/test_submit_ontology.py` & `smaht_submitr-0.7.0.2b8/submitr/tests/test_submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/tests/test_testing_helpers.py` & `smaht_submitr-0.7.0.2b8/submitr/tests/test_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/tests/test_upload_item_data.py` & `smaht_submitr-0.7.0.2b8/submitr/tests/test_upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/tests/test_utils.py` & `smaht_submitr-0.7.0.2b8/submitr/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/tests/testing_helpers.py` & `smaht_submitr-0.7.0.2b8/submitr/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/submitr/utils.py` & `smaht_submitr-0.7.0.2b8/submitr/utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b7/PKG-INFO` & `smaht_submitr-0.7.0.2b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smaht-submitr
-Version: 0.7.0.2b7
+Version: 0.7.0.2b8
 Summary: Support for uploading file submissions to SMAHT.
 Home-page: https://github.com/smaht-dac/submitr
 License: MIT
 Keywords: submitr,smaht
 Author: SMaHT DAC
 Author-email: smhelp@hms-dbmi.atlassian.net 
 Requires-Python: >=3.8.0,<3.12
```

