# Comparing `tmp/smaht_submitr-0.7.0.2b1.tar.gz` & `tmp/smaht_submitr-0.7.0.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smaht_submitr-0.7.0.2b1.tar", max compression
+gzip compressed data, was "smaht_submitr-0.7.0.2b2.tar", max compression
```

## Comparing `smaht_submitr-0.7.0.2b1.tar` & `smaht_submitr-0.7.0.2b2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1098 2024-04-07 13:15:33.143829 smaht_submitr-0.7.0.2b1/LICENSE.txt
--rw-r--r--   0        0        0     2602 2024-04-07 13:15:33.143829 smaht_submitr-0.7.0.2b1/README.rst
--rw-r--r--   0        0        0     3421 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/__init__.py
--rw-r--r--   0        0        0      731 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/base.py
--rw-r--r--   0        0        0      294 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/exceptions.py
--rw-r--r--   0        0        0     2628 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/output.py
--rw-r--r--   0        0        0    12781 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/progress_bar.py
--rw-r--r--   0        0        0    10819 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/s3_utils.py
--rw-r--r--   0        0        0        0 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/__init__.py
--rw-r--r--   0        0        0     4785 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/check_submission.py
--rw-r--r--   0        0        0     8466 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/cli_utils.py
--rw-r--r--   0        0        0     1828 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/list_submissions.py
--rw-r--r--   0        0        0      940 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/make_sample_fastq_file.py
--rw-r--r--   0        0        0     5709 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/resume_uploads.py
--rw-r--r--   0        0        0     1368 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/show_upload_info.py
--rw-r--r--   0        0        0     1572 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/submit_genelist.py
--rw-r--r--   0        0        0    19891 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/submit_metadata_bundle.py
--rw-r--r--   0        0        0     3437 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/submit_ontology.py
--rw-r--r--   0        0        0     1616 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/upload_item_data.py
--rw-r--r--   0        0        0    28731 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/scripts/view_portal_object.py
--rw-r--r--   0        0        0   151701 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/submission.py
--rw-r--r--   0        0        0        0 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/__init__.py
--rw-r--r--   0        0        0      355 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/conftest_settings.py
--rw-r--r--   0        0        0      163 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/f1_R1.fastq.gz
--rw-r--r--   0        0        0      165 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/f1_R2.fastq.gz
--rw-r--r--   0        0        0      167 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/f2_R1.fastq.gz
--rw-r--r--   0        0        0      164 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/f2_R2.fastq.gz
--rw-r--r--   0        0        0      272 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/simulated_bundle.json
--rw-r--r--   0        0        0    10870 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/submission_simple.xlsx
--rw-r--r--   0        0        0    10875 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/submission_simple2.xlsx
--rw-r--r--   0        0        0    13306 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/submission_test.xlsx
--rw-r--r--   0        0        0    13192 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/submission_test_with_errors.xlsx
--rw-r--r--   0        0        0      169 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/test1_R1.fastq.gz
--rw-r--r--   0        0        0      168 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/test1_R2.fastq.gz
--rw-r--r--   0        0        0     1333 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_base.py
--rw-r--r--   0        0        0     2629 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_check_submission.py
--rw-r--r--   0        0        0      551 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_exceptions.py
--rw-r--r--   0        0        0     1620 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_make_sample_fastq_file.py
--rw-r--r--   0        0        0     1421 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_misc.py
--rw-r--r--   0        0        0    11606 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_resume_uploads.py
--rw-r--r--   0        0        0     2478 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_show_upload_info.py
--rw-r--r--   0        0        0   157433 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_submission.py
--rw-r--r--   0        0        0     2836 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_submit_genelist.py
--rw-r--r--   0        0        0     6874 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_submit_metadata_bundle.py
--rw-r--r--   0        0        0     3013 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_submit_ontology.py
--rw-r--r--   0        0        0     1300 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_testing_helpers.py
--rw-r--r--   0        0        0     3661 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_upload_item_data.py
--rw-r--r--   0        0        0     4353 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_utils.py
--rw-r--r--   0        0        0     1351 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/testing_helpers.py
--rw-r--r--   0        0        0    11801 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/utils.py
--rw-r--r--   0        0        0     3988 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.2b1/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-07 13:26:31.544342 smaht_submitr-0.7.0.2b2/LICENSE.txt
+-rw-r--r--   0        0        0     2602 2024-04-07 13:26:31.544342 smaht_submitr-0.7.0.2b2/README.rst
+-rw-r--r--   0        0        0     3421 2024-04-07 13:26:31.580342 smaht_submitr-0.7.0.2b2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-07 13:26:31.580342 smaht_submitr-0.7.0.2b2/submitr/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-07 13:26:31.580342 smaht_submitr-0.7.0.2b2/submitr/base.py
+-rw-r--r--   0        0        0      294 2024-04-07 13:26:31.580342 smaht_submitr-0.7.0.2b2/submitr/exceptions.py
+-rw-r--r--   0        0        0     2628 2024-04-07 13:26:31.580342 smaht_submitr-0.7.0.2b2/submitr/output.py
+-rw-r--r--   0        0        0    12781 2024-04-07 13:26:31.580342 smaht_submitr-0.7.0.2b2/submitr/progress_bar.py
+-rw-r--r--   0        0        0    10819 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/s3_utils.py
+-rw-r--r--   0        0        0        0 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/scripts/__init__.py
+-rw-r--r--   0        0        0     4785 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/scripts/check_submission.py
+-rw-r--r--   0        0        0     8466 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/scripts/cli_utils.py
+-rw-r--r--   0        0        0     1828 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/scripts/list_submissions.py
+-rw-r--r--   0        0        0      940 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/scripts/make_sample_fastq_file.py
+-rw-r--r--   0        0        0     5709 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/scripts/resume_uploads.py
+-rw-r--r--   0        0        0     1368 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/scripts/show_upload_info.py
+-rw-r--r--   0        0        0     1572 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/scripts/submit_genelist.py
+-rw-r--r--   0        0        0    19891 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/scripts/submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3437 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/scripts/submit_ontology.py
+-rw-r--r--   0        0        0     1616 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/scripts/upload_item_data.py
+-rw-r--r--   0        0        0    28731 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/scripts/view_portal_object.py
+-rw-r--r--   0        0        0   151701 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/submission.py
+-rw-r--r--   0        0        0        0 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/__init__.py
+-rw-r--r--   0        0        0      355 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/conftest_settings.py
+-rw-r--r--   0        0        0      163 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/data/f1_R1.fastq.gz
+-rw-r--r--   0        0        0      165 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/data/f1_R2.fastq.gz
+-rw-r--r--   0        0        0      167 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/data/f2_R1.fastq.gz
+-rw-r--r--   0        0        0      164 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/data/f2_R2.fastq.gz
+-rw-r--r--   0        0        0      272 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/data/simulated_bundle.json
+-rw-r--r--   0        0        0    10870 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/data/submission_simple.xlsx
+-rw-r--r--   0        0        0    10875 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/data/submission_simple2.xlsx
+-rw-r--r--   0        0        0    13306 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/data/submission_test.xlsx
+-rw-r--r--   0        0        0    13192 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/data/submission_test_with_errors.xlsx
+-rw-r--r--   0        0        0      169 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/data/test1_R1.fastq.gz
+-rw-r--r--   0        0        0      168 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/data/test1_R2.fastq.gz
+-rw-r--r--   0        0        0     1333 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/test_base.py
+-rw-r--r--   0        0        0     2629 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/test_check_submission.py
+-rw-r--r--   0        0        0      551 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1620 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/test_make_sample_fastq_file.py
+-rw-r--r--   0        0        0     1421 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/test_misc.py
+-rw-r--r--   0        0        0    11606 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/test_resume_uploads.py
+-rw-r--r--   0        0        0     2478 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/test_show_upload_info.py
+-rw-r--r--   0        0        0   157433 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/test_submission.py
+-rw-r--r--   0        0        0     2836 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/test_submit_genelist.py
+-rw-r--r--   0        0        0     6874 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/test_submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3013 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/test_submit_ontology.py
+-rw-r--r--   0        0        0     1300 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/test_testing_helpers.py
+-rw-r--r--   0        0        0     3661 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/test_upload_item_data.py
+-rw-r--r--   0        0        0     4353 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/test_utils.py
+-rw-r--r--   0        0        0     1351 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/tests/testing_helpers.py
+-rw-r--r--   0        0        0    12124 2024-04-07 13:26:31.584342 smaht_submitr-0.7.0.2b2/submitr/utils.py
+-rw-r--r--   0        0        0     3988 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.2b2/PKG-INFO
```

### Comparing `smaht_submitr-0.7.0.2b1/LICENSE.txt` & `smaht_submitr-0.7.0.2b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/README.rst` & `smaht_submitr-0.7.0.2b2/README.rst`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/pyproject.toml` & `smaht_submitr-0.7.0.2b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smaht-submitr"
-version = "0.7.0.2b1"  # TODO: To become 0.8.0
+version = "0.7.0.2b2"  # TODO: To become 0.8.0
 description = "Support for uploading file submissions to SMAHT."
 # TODO: Update this email address when a more specific one is available for SMaHT.
 authors = ["SMaHT DAC <smhelp@hms-dbmi.atlassian.net >"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["submitr", "smaht"]
 homepage = "https://github.com/smaht-dac/submitr"
```

### Comparing `smaht_submitr-0.7.0.2b1/submitr/base.py` & `smaht_submitr-0.7.0.2b2/submitr/base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/output.py` & `smaht_submitr-0.7.0.2b2/submitr/output.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/progress_bar.py` & `smaht_submitr-0.7.0.2b2/submitr/progress_bar.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/s3_utils.py` & `smaht_submitr-0.7.0.2b2/submitr/s3_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/scripts/check_submission.py` & `smaht_submitr-0.7.0.2b2/submitr/scripts/check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/scripts/cli_utils.py` & `smaht_submitr-0.7.0.2b2/submitr/scripts/cli_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/scripts/list_submissions.py` & `smaht_submitr-0.7.0.2b2/submitr/scripts/list_submissions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/scripts/make_sample_fastq_file.py` & `smaht_submitr-0.7.0.2b2/submitr/scripts/make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/scripts/resume_uploads.py` & `smaht_submitr-0.7.0.2b2/submitr/scripts/resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/scripts/show_upload_info.py` & `smaht_submitr-0.7.0.2b2/submitr/scripts/show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/scripts/submit_genelist.py` & `smaht_submitr-0.7.0.2b2/submitr/scripts/submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/scripts/submit_metadata_bundle.py` & `smaht_submitr-0.7.0.2b2/submitr/scripts/submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/scripts/submit_ontology.py` & `smaht_submitr-0.7.0.2b2/submitr/scripts/submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/scripts/upload_item_data.py` & `smaht_submitr-0.7.0.2b2/submitr/scripts/upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/scripts/view_portal_object.py` & `smaht_submitr-0.7.0.2b2/submitr/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/submission.py` & `smaht_submitr-0.7.0.2b2/submitr/submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/tests/data/submission_simple.xlsx` & `smaht_submitr-0.7.0.2b2/submitr/tests/data/submission_simple.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/tests/data/submission_simple2.xlsx` & `smaht_submitr-0.7.0.2b2/submitr/tests/data/submission_simple2.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/tests/data/submission_test.xlsx` & `smaht_submitr-0.7.0.2b2/submitr/tests/data/submission_test.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/tests/data/submission_test_with_errors.xlsx` & `smaht_submitr-0.7.0.2b2/submitr/tests/data/submission_test_with_errors.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/tests/test_base.py` & `smaht_submitr-0.7.0.2b2/submitr/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/tests/test_check_submission.py` & `smaht_submitr-0.7.0.2b2/submitr/tests/test_check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/tests/test_exceptions.py` & `smaht_submitr-0.7.0.2b2/submitr/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/tests/test_make_sample_fastq_file.py` & `smaht_submitr-0.7.0.2b2/submitr/tests/test_make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/tests/test_misc.py` & `smaht_submitr-0.7.0.2b2/submitr/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/tests/test_resume_uploads.py` & `smaht_submitr-0.7.0.2b2/submitr/tests/test_resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/tests/test_show_upload_info.py` & `smaht_submitr-0.7.0.2b2/submitr/tests/test_show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/tests/test_submission.py` & `smaht_submitr-0.7.0.2b2/submitr/tests/test_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/tests/test_submit_genelist.py` & `smaht_submitr-0.7.0.2b2/submitr/tests/test_submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/tests/test_submit_metadata_bundle.py` & `smaht_submitr-0.7.0.2b2/submitr/tests/test_submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/tests/test_submit_ontology.py` & `smaht_submitr-0.7.0.2b2/submitr/tests/test_submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/tests/test_testing_helpers.py` & `smaht_submitr-0.7.0.2b2/submitr/tests/test_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/tests/test_upload_item_data.py` & `smaht_submitr-0.7.0.2b2/submitr/tests/test_upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/tests/test_utils.py` & `smaht_submitr-0.7.0.2b2/submitr/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/tests/testing_helpers.py` & `smaht_submitr-0.7.0.2b2/submitr/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b1/submitr/utils.py` & `smaht_submitr-0.7.0.2b2/submitr/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from collections import namedtuple
 from datetime import datetime
 from functools import lru_cache
 import io
 import hashlib
 import pkg_resources
+import pytz
 import re
 import requests
 import os
 from pathlib import Path
 from typing import Any, Callable, List, Optional, Tuple, Union
 from dcicutils.misc_utils import PRINT, str_to_bool
 from json import dumps as json_dumps, loads as json_loads
@@ -146,14 +147,21 @@
             return value.astimezone(tzlocal).strftime(f"%A, %B %-d, %Y | %-I:%M %p %Z")
         else:
             return value.astimezone(tzlocal).strftime(f"%Y-%m-%d %H:%M:%S %Z")
     except Exception:
         return None
 
 
+def parse_datetime_string_into_utc_datetime(value: str) -> Optional[datetime]:
+    try:
+        return datetime.fromisoformat(value).replace(tzinfo=pytz.utc)
+    except Exception:
+        return None
+
+
 def format_path(path: str) -> str:
     if isinstance(path, str) and os.path.isabs(path) and path.startswith(os.path.expanduser("~")):
         path = "~/" + Path(path).relative_to(Path.home()).as_posix()
     return path
 
 
 def get_file_size(file: str) -> int:
@@ -285,29 +293,31 @@
         if (response := requests.get(pypi_url)).status_code == 200 and (response := response.json()):
             latest_non_beta_version = response["info"]["version"]
             this_version = get_version(package_name=package_name)
             this_release_date = None
             releases = response["releases"]
             if releases and isinstance(this_release_info := releases.get(this_version), list) and this_release_info:
                 if isinstance(this_release_info := this_release_info[0], dict):
-                    this_release_date = datetime.fromisoformat(this_release_info.get("upload_time"))
-            latest_non_beta_release_date = datetime.fromisoformat(releases[latest_non_beta_version][0]["upload_time"])
+                    this_release_date = parse_datetime_string_into_utc_datetime(this_release_info.get("upload_time"))
+            latest_non_beta_release_date = (
+                parse_datetime_string_into_utc_datetime(releases[latest_non_beta_version][0].get("upload_time")))
             latest_beta_version = None
             latest_beta_release_date = None
             if beta:
                 # Return the latest beta version but only if it
                 # is more recent than the latest non-beta version.
                 try:
                     releases_reverse_sorted_by_time = (
                         sorted(releases.items(), key=lambda item: item[1][0]["upload_time"], reverse=True))
                     latest_beta_info = next(iter(releases_reverse_sorted_by_time))
                     if (latest_beta_version := latest_beta_info[0]) == latest_non_beta_version:
                         latest_beta_version = None
                     else:
-                        latest_beta_release_date = datetime.fromisoformat(latest_beta_info[1][0]["upload_time"])
+                        latest_beta_release_date = (
+                            parse_datetime_string_into_utc_datetime(latest_beta_info[1][0].get("upload_time")))
                         if latest_non_beta_release_date > latest_beta_release_date:
                             latest_beta_version = None
                             latest_beta_release_date = None
                 except Exception:
                     pass
             return (namedtuple("most_recent_pypi_package_version",
                                ["version", "release_date",
```

### Comparing `smaht_submitr-0.7.0.2b1/PKG-INFO` & `smaht_submitr-0.7.0.2b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smaht-submitr
-Version: 0.7.0.2b1
+Version: 0.7.0.2b2
 Summary: Support for uploading file submissions to SMAHT.
 Home-page: https://github.com/smaht-dac/submitr
 License: MIT
 Keywords: submitr,smaht
 Author: SMaHT DAC
 Author-email: smhelp@hms-dbmi.atlassian.net 
 Requires-Python: >=3.8.0,<3.12
```

