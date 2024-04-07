# Comparing `tmp/smaht_submitr-0.7.0.2b5.tar.gz` & `tmp/smaht_submitr-0.7.0.2b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smaht_submitr-0.7.0.2b5.tar", max compression
+gzip compressed data, was "smaht_submitr-0.7.0.2b6.tar", max compression
```

## Comparing `smaht_submitr-0.7.0.2b5.tar` & `smaht_submitr-0.7.0.2b6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1098 2024-04-07 15:01:42.184852 smaht_submitr-0.7.0.2b5/LICENSE.txt
--rw-r--r--   0        0        0     2602 2024-04-07 15:01:42.184852 smaht_submitr-0.7.0.2b5/README.rst
--rw-r--r--   0        0        0     3425 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/__init__.py
--rw-r--r--   0        0        0      731 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/base.py
--rw-r--r--   0        0        0      294 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/exceptions.py
--rw-r--r--   0        0        0     2628 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/output.py
--rw-r--r--   0        0        0    12781 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/progress_bar.py
--rw-r--r--   0        0        0    10819 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/s3_utils.py
--rw-r--r--   0        0        0        0 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/__init__.py
--rw-r--r--   0        0        0     4785 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/check_submission.py
--rw-r--r--   0        0        0     8466 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/cli_utils.py
--rw-r--r--   0        0        0     1828 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/list_submissions.py
--rw-r--r--   0        0        0      940 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/make_sample_fastq_file.py
--rw-r--r--   0        0        0     5709 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/resume_uploads.py
--rw-r--r--   0        0        0     1368 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/show_upload_info.py
--rw-r--r--   0        0        0     1572 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/submit_genelist.py
--rw-r--r--   0        0        0    19891 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/submit_metadata_bundle.py
--rw-r--r--   0        0        0     3437 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/submit_ontology.py
--rw-r--r--   0        0        0     1616 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/upload_item_data.py
--rw-r--r--   0        0        0    28731 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/view_portal_object.py
--rw-r--r--   0        0        0   152173 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/submission.py
--rw-r--r--   0        0        0        0 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/__init__.py
--rw-r--r--   0        0        0      355 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/conftest_settings.py
--rw-r--r--   0        0        0      163 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/f1_R1.fastq.gz
--rw-r--r--   0        0        0      165 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/f1_R2.fastq.gz
--rw-r--r--   0        0        0      167 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/f2_R1.fastq.gz
--rw-r--r--   0        0        0      164 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/f2_R2.fastq.gz
--rw-r--r--   0        0        0      272 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/simulated_bundle.json
--rw-r--r--   0        0        0    10870 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/submission_simple.xlsx
--rw-r--r--   0        0        0    10875 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/submission_simple2.xlsx
--rw-r--r--   0        0        0    13306 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/submission_test.xlsx
--rw-r--r--   0        0        0    13192 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/submission_test_with_errors.xlsx
--rw-r--r--   0        0        0      169 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/test1_R1.fastq.gz
--rw-r--r--   0        0        0      168 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/test1_R2.fastq.gz
--rw-r--r--   0        0        0     1333 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_base.py
--rw-r--r--   0        0        0     2629 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_check_submission.py
--rw-r--r--   0        0        0      551 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_exceptions.py
--rw-r--r--   0        0        0     1620 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_make_sample_fastq_file.py
--rw-r--r--   0        0        0     1421 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_misc.py
--rw-r--r--   0        0        0    11606 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_resume_uploads.py
--rw-r--r--   0        0        0     2478 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_show_upload_info.py
--rw-r--r--   0        0        0   157433 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_submission.py
--rw-r--r--   0        0        0     2836 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_submit_genelist.py
--rw-r--r--   0        0        0     6874 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_submit_metadata_bundle.py
--rw-r--r--   0        0        0     3013 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_submit_ontology.py
--rw-r--r--   0        0        0     1300 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_testing_helpers.py
--rw-r--r--   0        0        0     3661 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_upload_item_data.py
--rw-r--r--   0        0        0     4353 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_utils.py
--rw-r--r--   0        0        0     1351 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/testing_helpers.py
--rw-r--r--   0        0        0    12167 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/utils.py
--rw-r--r--   0        0        0     3994 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.2b5/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-07 15:20:45.797050 smaht_submitr-0.7.0.2b6/LICENSE.txt
+-rw-r--r--   0        0        0     2602 2024-04-07 15:20:45.797050 smaht_submitr-0.7.0.2b6/README.rst
+-rw-r--r--   0        0        0     3425 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/base.py
+-rw-r--r--   0        0        0      294 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/exceptions.py
+-rw-r--r--   0        0        0     2628 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/output.py
+-rw-r--r--   0        0        0    12781 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/progress_bar.py
+-rw-r--r--   0        0        0    10819 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/s3_utils.py
+-rw-r--r--   0        0        0        0 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/scripts/__init__.py
+-rw-r--r--   0        0        0     4785 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/scripts/check_submission.py
+-rw-r--r--   0        0        0     8466 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/scripts/cli_utils.py
+-rw-r--r--   0        0        0     1828 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/scripts/list_submissions.py
+-rw-r--r--   0        0        0      940 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/scripts/make_sample_fastq_file.py
+-rw-r--r--   0        0        0     5709 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/scripts/resume_uploads.py
+-rw-r--r--   0        0        0     1368 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/scripts/show_upload_info.py
+-rw-r--r--   0        0        0     1572 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/scripts/submit_genelist.py
+-rw-r--r--   0        0        0    19891 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/scripts/submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3437 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/scripts/submit_ontology.py
+-rw-r--r--   0        0        0     1616 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/scripts/upload_item_data.py
+-rw-r--r--   0        0        0    28731 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/scripts/view_portal_object.py
+-rw-r--r--   0        0        0   152386 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/submission.py
+-rw-r--r--   0        0        0        0 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/__init__.py
+-rw-r--r--   0        0        0      355 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/conftest_settings.py
+-rw-r--r--   0        0        0      163 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/data/f1_R1.fastq.gz
+-rw-r--r--   0        0        0      165 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/data/f1_R2.fastq.gz
+-rw-r--r--   0        0        0      167 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/data/f2_R1.fastq.gz
+-rw-r--r--   0        0        0      164 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/data/f2_R2.fastq.gz
+-rw-r--r--   0        0        0      272 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/data/simulated_bundle.json
+-rw-r--r--   0        0        0    10870 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/data/submission_simple.xlsx
+-rw-r--r--   0        0        0    10875 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/data/submission_simple2.xlsx
+-rw-r--r--   0        0        0    13306 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/data/submission_test.xlsx
+-rw-r--r--   0        0        0    13192 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/data/submission_test_with_errors.xlsx
+-rw-r--r--   0        0        0      169 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/data/test1_R1.fastq.gz
+-rw-r--r--   0        0        0      168 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/data/test1_R2.fastq.gz
+-rw-r--r--   0        0        0     1333 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/test_base.py
+-rw-r--r--   0        0        0     2629 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/test_check_submission.py
+-rw-r--r--   0        0        0      551 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1620 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/test_make_sample_fastq_file.py
+-rw-r--r--   0        0        0     1421 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/test_misc.py
+-rw-r--r--   0        0        0    11606 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/test_resume_uploads.py
+-rw-r--r--   0        0        0     2478 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/test_show_upload_info.py
+-rw-r--r--   0        0        0   157433 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/test_submission.py
+-rw-r--r--   0        0        0     2836 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/test_submit_genelist.py
+-rw-r--r--   0        0        0     6874 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/test_submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3013 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/test_submit_ontology.py
+-rw-r--r--   0        0        0     1300 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/test_testing_helpers.py
+-rw-r--r--   0        0        0     3661 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/test_upload_item_data.py
+-rw-r--r--   0        0        0     4353 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/test_utils.py
+-rw-r--r--   0        0        0     1351 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/tests/testing_helpers.py
+-rw-r--r--   0        0        0    12167 2024-04-07 15:20:45.837050 smaht_submitr-0.7.0.2b6/submitr/utils.py
+-rw-r--r--   0        0        0     3994 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.2b6/PKG-INFO
```

### Comparing `smaht_submitr-0.7.0.2b5/LICENSE.txt` & `smaht_submitr-0.7.0.2b6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/README.rst` & `smaht_submitr-0.7.0.2b6/README.rst`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/pyproject.toml` & `smaht_submitr-0.7.0.2b6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smaht-submitr"
-version = "0.7.0.2b5"  # TODO: To become 0.8.0
+version = "0.7.0.2b6"  # TODO: To become 0.8.0
 description = "Support for uploading file submissions to SMAHT."
 # TODO: Update this email address when a more specific one is available for SMaHT.
 authors = ["SMaHT DAC <smhelp@hms-dbmi.atlassian.net >"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["submitr", "smaht"]
 homepage = "https://github.com/smaht-dac/submitr"
```

### Comparing `smaht_submitr-0.7.0.2b5/submitr/base.py` & `smaht_submitr-0.7.0.2b6/submitr/base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/output.py` & `smaht_submitr-0.7.0.2b6/submitr/output.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/progress_bar.py` & `smaht_submitr-0.7.0.2b6/submitr/progress_bar.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/s3_utils.py` & `smaht_submitr-0.7.0.2b6/submitr/s3_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/scripts/check_submission.py` & `smaht_submitr-0.7.0.2b6/submitr/scripts/check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/scripts/cli_utils.py` & `smaht_submitr-0.7.0.2b6/submitr/scripts/cli_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/scripts/list_submissions.py` & `smaht_submitr-0.7.0.2b6/submitr/scripts/list_submissions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/scripts/make_sample_fastq_file.py` & `smaht_submitr-0.7.0.2b6/submitr/scripts/make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/scripts/resume_uploads.py` & `smaht_submitr-0.7.0.2b6/submitr/scripts/resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/scripts/show_upload_info.py` & `smaht_submitr-0.7.0.2b6/submitr/scripts/show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/scripts/submit_genelist.py` & `smaht_submitr-0.7.0.2b6/submitr/scripts/submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/scripts/submit_metadata_bundle.py` & `smaht_submitr-0.7.0.2b6/submitr/scripts/submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/scripts/submit_ontology.py` & `smaht_submitr-0.7.0.2b6/submitr/scripts/submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/scripts/upload_item_data.py` & `smaht_submitr-0.7.0.2b6/submitr/scripts/upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/scripts/view_portal_object.py` & `smaht_submitr-0.7.0.2b6/submitr/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/submission.py` & `smaht_submitr-0.7.0.2b6/submitr/submission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1056,14 +1056,15 @@
             ingester_parse_started = status.get(PROGRESS_INGESTER.PARSE_LOAD_INITIATE, None)
             ingester_parse_nrows = status.get(PROGRESS_PARSE.LOAD_COUNT_ROWS, 0)
             ingester_parse_nitems = status.get(PROGRESS_PARSE.LOAD_ITEM, 0)
             ingester_validate_started = status.get(PROGRESS_INGESTER.VALIDATE_LOAD_INITIATE, None)
             ingester_queued = status.get(PROGRESS_INGESTER.QUEUED, None)
             ingester_cleanup = status.get(PROGRESS_INGESTER.CLEANUP, None)
             ingester_queue_cleanup = status.get(PROGRESS_INGESTER.QUEUE_CLEANUP, None)
+            ingester_done = status.get(PROGRESS_INGESTER.DONE, None)
             loadxl_initiated = status.get(PROGRESS_INGESTER.LOADXL_INITIATE, None)
             loadxl_total = status.get(PROGRESS_LOADXL.TOTAL, 0)
             loadxl_started = status.get(PROGRESS_LOADXL.START, None)
             loadxl_item = status.get(PROGRESS_LOADXL.ITEM, 0)
             loadxl_started_second_round = status.get(PROGRESS_LOADXL.START_SECOND_ROUND, None)
             loadxl_item_second_round = status.get(PROGRESS_LOADXL.ITEM_SECOND_ROUND, 0)
             loadxl_done = status.get(PROGRESS_LOADXL.DONE, None)
@@ -1071,31 +1072,34 @@
             # so we don't have to cobble together our own string; but we could also build the
             # message ourselves manually here from the counts contained in the same response.
             ingestion_message = (status.get("loadxl_message_verbose", "")
                                  if verbose else status.get("loadxl_message", ""))
             # Phases: 0 means waiting for server response; 1 means loadxl round one; 2 means loadxl round two.
             loadxl_phase = 2 if loadxl_started_second_round is not None else (1 if loadxl_started is not None else 0)
             done = False
-            if status.get("finish") or nchecks >= max_checks:
+            message = f"▶ Pings: {nchecks_server}"
+            if ingester_done is not None:
+                message += " | Done"
+                bar.set_progress(bar.total)
+                done = True
+            elif status.get("finish") or (nchecks >= max_checks):
                 check_status = status.get("status")
                 if loadxl_phase == 0:
                     bar.increment_progress(max_checks - nchecks)
                 done = True
             elif status.get("check_server"):
                 check_status = status.get("status")
                 nchecks_server += 1
             elif status.get("check"):
                 if (next_check := status.get("next")) is not None:
                     next_check = round(status.get("next") or 0)
                 nchecks += 1
                 if loadxl_phase == 0:
                     bar.increment_progress(1)
-            # message = f"▶ {title} Pings: {nchecks_server}"
-            message = f"▶ Pings: {nchecks_server}"
-            if loadxl_started is None:
+            if (loadxl_started is None) and (ingester_done is None):
                 if loadxl_initiated is not None:
                     message += f" | Initializing"
                 elif ingester_parse_started is not None:
                     message += f" | Parsing"
                     if ingester_parse_nrows > 0:
                         bar.set_total(ingester_parse_nrows)
                         bar.set_progress(ingester_parse_nitems)
@@ -1103,15 +1107,15 @@
                     message += f" | Validating"
                 elif ingester_initiated is not None:
                     message += f" | Acknowledged"
                 elif ingester_queued is not None:
                     message += f" | Queued"
                 else:
                     message += f" | Waiting on server"
-            else:
+            elif ingester_done is None:
                 if loadxl_done is not None:
                     bar.set_total(loadxl_total)
                     bar.set_progress(loadxl_total)
                 elif loadxl_phase == 2:
                     bar.set_total(loadxl_total)
                     bar.set_progress(loadxl_item_second_round)
                 elif loadxl_phase == 1:
```

### Comparing `smaht_submitr-0.7.0.2b5/submitr/tests/data/submission_simple.xlsx` & `smaht_submitr-0.7.0.2b6/submitr/tests/data/submission_simple.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/tests/data/submission_simple2.xlsx` & `smaht_submitr-0.7.0.2b6/submitr/tests/data/submission_simple2.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/tests/data/submission_test.xlsx` & `smaht_submitr-0.7.0.2b6/submitr/tests/data/submission_test.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/tests/data/submission_test_with_errors.xlsx` & `smaht_submitr-0.7.0.2b6/submitr/tests/data/submission_test_with_errors.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/tests/test_base.py` & `smaht_submitr-0.7.0.2b6/submitr/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/tests/test_check_submission.py` & `smaht_submitr-0.7.0.2b6/submitr/tests/test_check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/tests/test_exceptions.py` & `smaht_submitr-0.7.0.2b6/submitr/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/tests/test_make_sample_fastq_file.py` & `smaht_submitr-0.7.0.2b6/submitr/tests/test_make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/tests/test_misc.py` & `smaht_submitr-0.7.0.2b6/submitr/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/tests/test_resume_uploads.py` & `smaht_submitr-0.7.0.2b6/submitr/tests/test_resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/tests/test_show_upload_info.py` & `smaht_submitr-0.7.0.2b6/submitr/tests/test_show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/tests/test_submission.py` & `smaht_submitr-0.7.0.2b6/submitr/tests/test_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/tests/test_submit_genelist.py` & `smaht_submitr-0.7.0.2b6/submitr/tests/test_submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/tests/test_submit_metadata_bundle.py` & `smaht_submitr-0.7.0.2b6/submitr/tests/test_submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/tests/test_submit_ontology.py` & `smaht_submitr-0.7.0.2b6/submitr/tests/test_submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/tests/test_testing_helpers.py` & `smaht_submitr-0.7.0.2b6/submitr/tests/test_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/tests/test_upload_item_data.py` & `smaht_submitr-0.7.0.2b6/submitr/tests/test_upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/tests/test_utils.py` & `smaht_submitr-0.7.0.2b6/submitr/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/tests/testing_helpers.py` & `smaht_submitr-0.7.0.2b6/submitr/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/submitr/utils.py` & `smaht_submitr-0.7.0.2b6/submitr/utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b5/PKG-INFO` & `smaht_submitr-0.7.0.2b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smaht-submitr
-Version: 0.7.0.2b5
+Version: 0.7.0.2b6
 Summary: Support for uploading file submissions to SMAHT.
 Home-page: https://github.com/smaht-dac/submitr
 License: MIT
 Keywords: submitr,smaht
 Author: SMaHT DAC
 Author-email: smhelp@hms-dbmi.atlassian.net 
 Requires-Python: >=3.8.0,<3.12
```

