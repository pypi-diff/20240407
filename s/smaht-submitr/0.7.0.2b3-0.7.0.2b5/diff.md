# Comparing `tmp/smaht_submitr-0.7.0.2b3.tar.gz` & `tmp/smaht_submitr-0.7.0.2b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smaht_submitr-0.7.0.2b3.tar", max compression
+gzip compressed data, was "smaht_submitr-0.7.0.2b5.tar", max compression
```

## Comparing `smaht_submitr-0.7.0.2b3.tar` & `smaht_submitr-0.7.0.2b5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1098 2024-04-07 13:28:50.473862 smaht_submitr-0.7.0.2b3/LICENSE.txt
--rw-r--r--   0        0        0     2602 2024-04-07 13:28:50.473862 smaht_submitr-0.7.0.2b3/README.rst
--rw-r--r--   0        0        0     3421 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/__init__.py
--rw-r--r--   0        0        0      731 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/base.py
--rw-r--r--   0        0        0      294 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/exceptions.py
--rw-r--r--   0        0        0     2628 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/output.py
--rw-r--r--   0        0        0    12781 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/progress_bar.py
--rw-r--r--   0        0        0    10819 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/s3_utils.py
--rw-r--r--   0        0        0        0 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/scripts/__init__.py
--rw-r--r--   0        0        0     4785 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/scripts/check_submission.py
--rw-r--r--   0        0        0     8466 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/scripts/cli_utils.py
--rw-r--r--   0        0        0     1828 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/scripts/list_submissions.py
--rw-r--r--   0        0        0      940 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/scripts/make_sample_fastq_file.py
--rw-r--r--   0        0        0     5709 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/scripts/resume_uploads.py
--rw-r--r--   0        0        0     1368 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/scripts/show_upload_info.py
--rw-r--r--   0        0        0     1572 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/scripts/submit_genelist.py
--rw-r--r--   0        0        0    19891 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/scripts/submit_metadata_bundle.py
--rw-r--r--   0        0        0     3437 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/scripts/submit_ontology.py
--rw-r--r--   0        0        0     1616 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/scripts/upload_item_data.py
--rw-r--r--   0        0        0    28731 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/scripts/view_portal_object.py
--rw-r--r--   0        0        0   151701 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/submission.py
--rw-r--r--   0        0        0        0 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/__init__.py
--rw-r--r--   0        0        0      355 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/conftest_settings.py
--rw-r--r--   0        0        0      163 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/data/f1_R1.fastq.gz
--rw-r--r--   0        0        0      165 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/data/f1_R2.fastq.gz
--rw-r--r--   0        0        0      167 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/data/f2_R1.fastq.gz
--rw-r--r--   0        0        0      164 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/data/f2_R2.fastq.gz
--rw-r--r--   0        0        0      272 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/data/simulated_bundle.json
--rw-r--r--   0        0        0    10870 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/data/submission_simple.xlsx
--rw-r--r--   0        0        0    10875 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/data/submission_simple2.xlsx
--rw-r--r--   0        0        0    13306 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/data/submission_test.xlsx
--rw-r--r--   0        0        0    13192 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/data/submission_test_with_errors.xlsx
--rw-r--r--   0        0        0      169 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/data/test1_R1.fastq.gz
--rw-r--r--   0        0        0      168 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/data/test1_R2.fastq.gz
--rw-r--r--   0        0        0     1333 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/test_base.py
--rw-r--r--   0        0        0     2629 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/test_check_submission.py
--rw-r--r--   0        0        0      551 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/test_exceptions.py
--rw-r--r--   0        0        0     1620 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/test_make_sample_fastq_file.py
--rw-r--r--   0        0        0     1421 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/test_misc.py
--rw-r--r--   0        0        0    11606 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/test_resume_uploads.py
--rw-r--r--   0        0        0     2478 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/test_show_upload_info.py
--rw-r--r--   0        0        0   157433 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/test_submission.py
--rw-r--r--   0        0        0     2836 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/test_submit_genelist.py
--rw-r--r--   0        0        0     6874 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/test_submit_metadata_bundle.py
--rw-r--r--   0        0        0     3013 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/test_submit_ontology.py
--rw-r--r--   0        0        0     1300 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/test_testing_helpers.py
--rw-r--r--   0        0        0     3661 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/test_upload_item_data.py
--rw-r--r--   0        0        0     4353 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/test_utils.py
--rw-r--r--   0        0        0     1351 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/tests/testing_helpers.py
--rw-r--r--   0        0        0    12167 2024-04-07 13:28:50.513862 smaht_submitr-0.7.0.2b3/submitr/utils.py
--rw-r--r--   0        0        0     3988 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.2b3/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-07 15:01:42.184852 smaht_submitr-0.7.0.2b5/LICENSE.txt
+-rw-r--r--   0        0        0     2602 2024-04-07 15:01:42.184852 smaht_submitr-0.7.0.2b5/README.rst
+-rw-r--r--   0        0        0     3425 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/base.py
+-rw-r--r--   0        0        0      294 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/exceptions.py
+-rw-r--r--   0        0        0     2628 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/output.py
+-rw-r--r--   0        0        0    12781 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/progress_bar.py
+-rw-r--r--   0        0        0    10819 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/s3_utils.py
+-rw-r--r--   0        0        0        0 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/__init__.py
+-rw-r--r--   0        0        0     4785 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/check_submission.py
+-rw-r--r--   0        0        0     8466 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/cli_utils.py
+-rw-r--r--   0        0        0     1828 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/list_submissions.py
+-rw-r--r--   0        0        0      940 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/make_sample_fastq_file.py
+-rw-r--r--   0        0        0     5709 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/resume_uploads.py
+-rw-r--r--   0        0        0     1368 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/show_upload_info.py
+-rw-r--r--   0        0        0     1572 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/submit_genelist.py
+-rw-r--r--   0        0        0    19891 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3437 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/submit_ontology.py
+-rw-r--r--   0        0        0     1616 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/upload_item_data.py
+-rw-r--r--   0        0        0    28731 2024-04-07 15:01:42.224852 smaht_submitr-0.7.0.2b5/submitr/scripts/view_portal_object.py
+-rw-r--r--   0        0        0   152173 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/submission.py
+-rw-r--r--   0        0        0        0 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/__init__.py
+-rw-r--r--   0        0        0      355 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/conftest_settings.py
+-rw-r--r--   0        0        0      163 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/f1_R1.fastq.gz
+-rw-r--r--   0        0        0      165 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/f1_R2.fastq.gz
+-rw-r--r--   0        0        0      167 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/f2_R1.fastq.gz
+-rw-r--r--   0        0        0      164 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/f2_R2.fastq.gz
+-rw-r--r--   0        0        0      272 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/simulated_bundle.json
+-rw-r--r--   0        0        0    10870 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/submission_simple.xlsx
+-rw-r--r--   0        0        0    10875 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/submission_simple2.xlsx
+-rw-r--r--   0        0        0    13306 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/submission_test.xlsx
+-rw-r--r--   0        0        0    13192 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/submission_test_with_errors.xlsx
+-rw-r--r--   0        0        0      169 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/test1_R1.fastq.gz
+-rw-r--r--   0        0        0      168 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/data/test1_R2.fastq.gz
+-rw-r--r--   0        0        0     1333 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_base.py
+-rw-r--r--   0        0        0     2629 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_check_submission.py
+-rw-r--r--   0        0        0      551 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1620 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_make_sample_fastq_file.py
+-rw-r--r--   0        0        0     1421 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_misc.py
+-rw-r--r--   0        0        0    11606 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_resume_uploads.py
+-rw-r--r--   0        0        0     2478 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_show_upload_info.py
+-rw-r--r--   0        0        0   157433 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_submission.py
+-rw-r--r--   0        0        0     2836 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_submit_genelist.py
+-rw-r--r--   0        0        0     6874 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3013 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_submit_ontology.py
+-rw-r--r--   0        0        0     1300 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_testing_helpers.py
+-rw-r--r--   0        0        0     3661 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_upload_item_data.py
+-rw-r--r--   0        0        0     4353 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/test_utils.py
+-rw-r--r--   0        0        0     1351 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/tests/testing_helpers.py
+-rw-r--r--   0        0        0    12167 2024-04-07 15:01:42.228852 smaht_submitr-0.7.0.2b5/submitr/utils.py
+-rw-r--r--   0        0        0     3994 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.2b5/PKG-INFO
```

### Comparing `smaht_submitr-0.7.0.2b3/LICENSE.txt` & `smaht_submitr-0.7.0.2b5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/README.rst` & `smaht_submitr-0.7.0.2b5/README.rst`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/pyproject.toml` & `smaht_submitr-0.7.0.2b5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smaht-submitr"
-version = "0.7.0.2b3"  # TODO: To become 0.8.0
+version = "0.7.0.2b5"  # TODO: To become 0.8.0
 description = "Support for uploading file submissions to SMAHT."
 # TODO: Update this email address when a more specific one is available for SMaHT.
 authors = ["SMaHT DAC <smhelp@hms-dbmi.atlassian.net >"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["submitr", "smaht"]
 homepage = "https://github.com/smaht-dac/submitr"
@@ -45,15 +45,15 @@
 ]
 
 [tool.poetry.dependencies]
 
 python = ">=3.8.0,<3.12"
 awscli = ">=1.32.49"
 boto3 = "^1.34.49"
-dcicutils = "^8.8.2"
+dcicutils = "^8.8.2.1b1"
 PyYAML = "^6.0.1"
 requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
 
 # Coverage
 codacy-coverage = ">=1.3.11"
```

### Comparing `smaht_submitr-0.7.0.2b3/submitr/base.py` & `smaht_submitr-0.7.0.2b5/submitr/base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/output.py` & `smaht_submitr-0.7.0.2b5/submitr/output.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/progress_bar.py` & `smaht_submitr-0.7.0.2b5/submitr/progress_bar.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/s3_utils.py` & `smaht_submitr-0.7.0.2b5/submitr/s3_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/scripts/check_submission.py` & `smaht_submitr-0.7.0.2b5/submitr/scripts/check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/scripts/cli_utils.py` & `smaht_submitr-0.7.0.2b5/submitr/scripts/cli_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/scripts/list_submissions.py` & `smaht_submitr-0.7.0.2b5/submitr/scripts/list_submissions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/scripts/make_sample_fastq_file.py` & `smaht_submitr-0.7.0.2b5/submitr/scripts/make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/scripts/resume_uploads.py` & `smaht_submitr-0.7.0.2b5/submitr/scripts/resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/scripts/show_upload_info.py` & `smaht_submitr-0.7.0.2b5/submitr/scripts/show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/scripts/submit_genelist.py` & `smaht_submitr-0.7.0.2b5/submitr/scripts/submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/scripts/submit_metadata_bundle.py` & `smaht_submitr-0.7.0.2b5/submitr/scripts/submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/scripts/submit_ontology.py` & `smaht_submitr-0.7.0.2b5/submitr/scripts/submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/scripts/upload_item_data.py` & `smaht_submitr-0.7.0.2b5/submitr/scripts/upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/scripts/view_portal_object.py` & `smaht_submitr-0.7.0.2b5/submitr/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/submission.py` & `smaht_submitr-0.7.0.2b5/submitr/submission.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 
 # Maximum amount of time (approximately) we will wait for a response from server (seconds).
 PROGRESS_TIMEOUT = 60 * 5  # five minutes (note this is for both server validation and submission)
 # How often we actually check the server (seconds).
 PROGRESS_CHECK_SERVER_INTERVAL = 3  # xyzzy
 # How often the (tqdm) progress meter updates (seconds).
-PROGRESS_INTERVAL = 1  # xyzzy
+PROGRESS_INTERVAL = 1
 # How many times the (tqdm) progress meter updates (derived from above).
 PROGRESS_MAX_CHECKS = round(PROGRESS_TIMEOUT / PROGRESS_INTERVAL)
 
 
 class SubmissionProtocol:
     S3 = 's3'
     UPLOAD = 'upload'
@@ -1050,14 +1050,16 @@
                 return
             # This are from the (new/2024-03-25) /ingestion-status/{submission_uuid} call.
             # Some of these key name come ultimately from snovault.loadxl.PROGRESS; others
             # from smaht-portal/ingestion. Note difference between ingester_initiated and
             # loadxl_started; the former is when the ingester listener is first hit.
             ingester_initiated = status.get(PROGRESS_INGESTER.INITIATE, None)
             ingester_parse_started = status.get(PROGRESS_INGESTER.PARSE_LOAD_INITIATE, None)
+            ingester_parse_nrows = status.get(PROGRESS_PARSE.LOAD_COUNT_ROWS, 0)
+            ingester_parse_nitems = status.get(PROGRESS_PARSE.LOAD_ITEM, 0)
             ingester_validate_started = status.get(PROGRESS_INGESTER.VALIDATE_LOAD_INITIATE, None)
             ingester_queued = status.get(PROGRESS_INGESTER.QUEUED, None)
             ingester_cleanup = status.get(PROGRESS_INGESTER.CLEANUP, None)
             ingester_queue_cleanup = status.get(PROGRESS_INGESTER.QUEUE_CLEANUP, None)
             loadxl_initiated = status.get(PROGRESS_INGESTER.LOADXL_INITIATE, None)
             loadxl_total = status.get(PROGRESS_LOADXL.TOTAL, 0)
             loadxl_started = status.get(PROGRESS_LOADXL.START, None)
@@ -1090,14 +1092,17 @@
             # message = f"▶ {title} Pings: {nchecks_server}"
             message = f"▶ Pings: {nchecks_server}"
             if loadxl_started is None:
                 if loadxl_initiated is not None:
                     message += f" | Initializing"
                 elif ingester_parse_started is not None:
                     message += f" | Parsing"
+                    if ingester_parse_nrows > 0:
+                        bar.set_total(ingester_parse_nrows)
+                        bar.set_progress(ingester_parse_nitems)
                 elif ingester_validate_started is not None:
                     message += f" | Validating"
                 elif ingester_initiated is not None:
                     message += f" | Acknowledged"
                 elif ingester_queued is not None:
                     message += f" | Queued"
                 else:
@@ -1307,15 +1312,15 @@
                     if ((validation_errors := validation_info.get("validation")) and
                         isinstance(validation_errors, list) and validation_errors):  # noqa
                         if not printed_newline:
                             PRINT_OUTPUT()
                             printed_newline = True
                         PRINT_OUTPUT(f"- Data errors: {len(validation_errors)}")
                         for validation_error in validation_errors:
-                            PRINT_OUTPUT(f"    - {_format_issue(validation_error)}")
+                            PRINT_OUTPUT(f"  - {_format_issue(validation_error)}")
                     if debug:
                         ref_errors = validation_info.get("ref")
                     elif not (ref_errors := validation_info.get("ref_grouped")):
                         ref_errors = validation_info.get("ref")
                     if ref_errors and (ref_errors := _validate_references(ref_errors, None, debug=debug)):
                         if not printed_newline:
                             PRINT_OUTPUT()
@@ -1633,15 +1638,18 @@
     if lines:
         lines = ["===", f"SMaHT {'Validation' if validation else 'Submission'} Summary [UUID]", "==="] + lines + ["==="]
         if errors and include_errors:
             lines += ["ERRORS ITEMIZED BELOW ...", "==="]
         print_boxed(lines, right_justified_macro=("[UUID]", lambda: submission_uuid), printf=PRINT)
         if errors and include_errors:
             for error in errors:
-                PRINT(f"- {_format_server_error(error, indent=2, debug=debug)}")
+                if check_submission_script:
+                    PRINT(f"{_format_server_error(error, indent=2, debug=debug)}")
+                else:
+                    PRINT(f"- {_format_server_error(error, indent=2, debug=debug)}")
 
 
 def _show_upload_info(uuid, server=None, env=None, keydict=None, app: str = None,
                       show_primary_result=True,
                       show_validation_output=True,
                       show_processing_status=True,
                       show_datafile_url=True,
```

### Comparing `smaht_submitr-0.7.0.2b3/submitr/tests/data/submission_simple.xlsx` & `smaht_submitr-0.7.0.2b5/submitr/tests/data/submission_simple.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/tests/data/submission_simple2.xlsx` & `smaht_submitr-0.7.0.2b5/submitr/tests/data/submission_simple2.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/tests/data/submission_test.xlsx` & `smaht_submitr-0.7.0.2b5/submitr/tests/data/submission_test.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/tests/data/submission_test_with_errors.xlsx` & `smaht_submitr-0.7.0.2b5/submitr/tests/data/submission_test_with_errors.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/tests/test_base.py` & `smaht_submitr-0.7.0.2b5/submitr/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/tests/test_check_submission.py` & `smaht_submitr-0.7.0.2b5/submitr/tests/test_check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/tests/test_exceptions.py` & `smaht_submitr-0.7.0.2b5/submitr/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/tests/test_make_sample_fastq_file.py` & `smaht_submitr-0.7.0.2b5/submitr/tests/test_make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/tests/test_misc.py` & `smaht_submitr-0.7.0.2b5/submitr/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/tests/test_resume_uploads.py` & `smaht_submitr-0.7.0.2b5/submitr/tests/test_resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/tests/test_show_upload_info.py` & `smaht_submitr-0.7.0.2b5/submitr/tests/test_show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/tests/test_submission.py` & `smaht_submitr-0.7.0.2b5/submitr/tests/test_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/tests/test_submit_genelist.py` & `smaht_submitr-0.7.0.2b5/submitr/tests/test_submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/tests/test_submit_metadata_bundle.py` & `smaht_submitr-0.7.0.2b5/submitr/tests/test_submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/tests/test_submit_ontology.py` & `smaht_submitr-0.7.0.2b5/submitr/tests/test_submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/tests/test_testing_helpers.py` & `smaht_submitr-0.7.0.2b5/submitr/tests/test_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/tests/test_upload_item_data.py` & `smaht_submitr-0.7.0.2b5/submitr/tests/test_upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/tests/test_utils.py` & `smaht_submitr-0.7.0.2b5/submitr/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/tests/testing_helpers.py` & `smaht_submitr-0.7.0.2b5/submitr/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/submitr/utils.py` & `smaht_submitr-0.7.0.2b5/submitr/utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.2b3/PKG-INFO` & `smaht_submitr-0.7.0.2b5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smaht-submitr
-Version: 0.7.0.2b3
+Version: 0.7.0.2b5
 Summary: Support for uploading file submissions to SMAHT.
 Home-page: https://github.com/smaht-dac/submitr
 License: MIT
 Keywords: submitr,smaht
 Author: SMaHT DAC
 Author-email: smhelp@hms-dbmi.atlassian.net 
 Requires-Python: >=3.8.0,<3.12
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database :: Database Engines/Servers
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: awscli (>=1.32.49)
 Requires-Dist: boto3 (>=1.34.49,<2.0.0)
-Requires-Dist: dcicutils (>=8.8.2,<9.0.0)
+Requires-Dist: dcicutils (>=8.8.2.1b1,<9.0.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/smaht-dac/submitr.git
 Description-Content-Type: text/x-rst
 
 
 .. image:: https://staging.smaht.org/static/img/docs/submitr_logo.png
     :target: https://pypi.org/project/smaht-submitr/
```

