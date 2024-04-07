# Comparing `tmp/smaht_submitr-0.7.0.1b95.tar.gz` & `tmp/smaht_submitr-0.7.0.1b96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smaht_submitr-0.7.0.1b95.tar", max compression
+gzip compressed data, was "smaht_submitr-0.7.0.1b96.tar", max compression
```

## Comparing `smaht_submitr-0.7.0.1b95.tar` & `smaht_submitr-0.7.0.1b96.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1098 2024-04-07 03:34:27.098607 smaht_submitr-0.7.0.1b95/LICENSE.txt
--rw-r--r--   0        0        0     2602 2024-04-07 03:34:27.098607 smaht_submitr-0.7.0.1b95/README.rst
--rw-r--r--   0        0        0     3422 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/__init__.py
--rw-r--r--   0        0        0      731 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/base.py
--rw-r--r--   0        0        0      294 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/exceptions.py
--rw-r--r--   0        0        0     2628 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/output.py
--rw-r--r--   0        0        0    12723 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/progress_bar.py
--rw-r--r--   0        0        0    10819 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/s3_utils.py
--rw-r--r--   0        0        0        0 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/__init__.py
--rw-r--r--   0        0        0     4792 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/check_submission.py
--rw-r--r--   0        0        0     8008 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/cli_utils.py
--rw-r--r--   0        0        0     1835 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/list_submissions.py
--rw-r--r--   0        0        0      940 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/make_sample_fastq_file.py
--rw-r--r--   0        0        0     5684 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/resume_uploads.py
--rw-r--r--   0        0        0     1368 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/show_upload_info.py
--rw-r--r--   0        0        0     1572 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/submit_genelist.py
--rw-r--r--   0        0        0    19866 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/submit_metadata_bundle.py
--rw-r--r--   0        0        0     3437 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/submit_ontology.py
--rw-r--r--   0        0        0     1616 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/upload_item_data.py
--rw-r--r--   0        0        0    28731 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/view_portal_object.py
--rw-r--r--   0        0        0   149229 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/submission.py
--rw-r--r--   0        0        0        0 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/__init__.py
--rw-r--r--   0        0        0      355 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/conftest_settings.py
--rw-r--r--   0        0        0      163 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/f1_R1.fastq.gz
--rw-r--r--   0        0        0      165 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/f1_R2.fastq.gz
--rw-r--r--   0        0        0      167 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/f2_R1.fastq.gz
--rw-r--r--   0        0        0      164 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/f2_R2.fastq.gz
--rw-r--r--   0        0        0      272 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/simulated_bundle.json
--rw-r--r--   0        0        0    10870 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/submission_simple.xlsx
--rw-r--r--   0        0        0    10875 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/submission_simple2.xlsx
--rw-r--r--   0        0        0    13306 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/submission_test.xlsx
--rw-r--r--   0        0        0    13192 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/submission_test_with_errors.xlsx
--rw-r--r--   0        0        0      169 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/test1_R1.fastq.gz
--rw-r--r--   0        0        0      168 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/test1_R2.fastq.gz
--rw-r--r--   0        0        0     1333 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_base.py
--rw-r--r--   0        0        0     2629 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_check_submission.py
--rw-r--r--   0        0        0      551 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_exceptions.py
--rw-r--r--   0        0        0     1620 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_make_sample_fastq_file.py
--rw-r--r--   0        0        0     1421 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_misc.py
--rw-r--r--   0        0        0    11606 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_resume_uploads.py
--rw-r--r--   0        0        0     2478 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_show_upload_info.py
--rw-r--r--   0        0        0   157433 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_submission.py
--rw-r--r--   0        0        0     2836 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_submit_genelist.py
--rw-r--r--   0        0        0     6874 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_submit_metadata_bundle.py
--rw-r--r--   0        0        0     3013 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_submit_ontology.py
--rw-r--r--   0        0        0     1300 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_testing_helpers.py
--rw-r--r--   0        0        0     3661 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_upload_item_data.py
--rw-r--r--   0        0        0     4353 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_utils.py
--rw-r--r--   0        0        0     1351 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/testing_helpers.py
--rw-r--r--   0        0        0    11074 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/utils.py
--rw-r--r--   0        0        0     3989 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.1b95/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-07 03:38:38.483311 smaht_submitr-0.7.0.1b96/LICENSE.txt
+-rw-r--r--   0        0        0     2602 2024-04-07 03:38:38.483311 smaht_submitr-0.7.0.1b96/README.rst
+-rw-r--r--   0        0        0     3422 2024-04-07 03:38:38.519311 smaht_submitr-0.7.0.1b96/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-07 03:38:38.519311 smaht_submitr-0.7.0.1b96/submitr/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-07 03:38:38.519311 smaht_submitr-0.7.0.1b96/submitr/base.py
+-rw-r--r--   0        0        0      294 2024-04-07 03:38:38.519311 smaht_submitr-0.7.0.1b96/submitr/exceptions.py
+-rw-r--r--   0        0        0     2628 2024-04-07 03:38:38.519311 smaht_submitr-0.7.0.1b96/submitr/output.py
+-rw-r--r--   0        0        0    12784 2024-04-07 03:38:38.519311 smaht_submitr-0.7.0.1b96/submitr/progress_bar.py
+-rw-r--r--   0        0        0    10819 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/s3_utils.py
+-rw-r--r--   0        0        0        0 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/__init__.py
+-rw-r--r--   0        0        0     4792 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/check_submission.py
+-rw-r--r--   0        0        0     8008 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/cli_utils.py
+-rw-r--r--   0        0        0     1835 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/list_submissions.py
+-rw-r--r--   0        0        0      940 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/make_sample_fastq_file.py
+-rw-r--r--   0        0        0     5684 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/resume_uploads.py
+-rw-r--r--   0        0        0     1368 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/show_upload_info.py
+-rw-r--r--   0        0        0     1572 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/submit_genelist.py
+-rw-r--r--   0        0        0    19866 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3437 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/submit_ontology.py
+-rw-r--r--   0        0        0     1616 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/upload_item_data.py
+-rw-r--r--   0        0        0    28731 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/view_portal_object.py
+-rw-r--r--   0        0        0   149229 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/submission.py
+-rw-r--r--   0        0        0        0 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/__init__.py
+-rw-r--r--   0        0        0      355 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/conftest_settings.py
+-rw-r--r--   0        0        0      163 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/f1_R1.fastq.gz
+-rw-r--r--   0        0        0      165 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/f1_R2.fastq.gz
+-rw-r--r--   0        0        0      167 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/f2_R1.fastq.gz
+-rw-r--r--   0        0        0      164 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/f2_R2.fastq.gz
+-rw-r--r--   0        0        0      272 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/simulated_bundle.json
+-rw-r--r--   0        0        0    10870 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/submission_simple.xlsx
+-rw-r--r--   0        0        0    10875 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/submission_simple2.xlsx
+-rw-r--r--   0        0        0    13306 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/submission_test.xlsx
+-rw-r--r--   0        0        0    13192 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/submission_test_with_errors.xlsx
+-rw-r--r--   0        0        0      169 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/test1_R1.fastq.gz
+-rw-r--r--   0        0        0      168 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/test1_R2.fastq.gz
+-rw-r--r--   0        0        0     1333 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_base.py
+-rw-r--r--   0        0        0     2629 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_check_submission.py
+-rw-r--r--   0        0        0      551 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1620 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_make_sample_fastq_file.py
+-rw-r--r--   0        0        0     1421 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_misc.py
+-rw-r--r--   0        0        0    11606 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_resume_uploads.py
+-rw-r--r--   0        0        0     2478 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_show_upload_info.py
+-rw-r--r--   0        0        0   157433 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_submission.py
+-rw-r--r--   0        0        0     2836 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_submit_genelist.py
+-rw-r--r--   0        0        0     6874 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3013 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_submit_ontology.py
+-rw-r--r--   0        0        0     1300 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_testing_helpers.py
+-rw-r--r--   0        0        0     3661 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_upload_item_data.py
+-rw-r--r--   0        0        0     4353 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_utils.py
+-rw-r--r--   0        0        0     1351 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/testing_helpers.py
+-rw-r--r--   0        0        0    11074 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/utils.py
+-rw-r--r--   0        0        0     3989 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.1b96/PKG-INFO
```

### Comparing `smaht_submitr-0.7.0.1b95/LICENSE.txt` & `smaht_submitr-0.7.0.1b96/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/README.rst` & `smaht_submitr-0.7.0.1b96/README.rst`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/pyproject.toml` & `smaht_submitr-0.7.0.1b96/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smaht-submitr"
-version = "0.7.0.1b95"  # TODO: To become 0.8.0
+version = "0.7.0.1b96"  # TODO: To become 0.8.0
 description = "Support for uploading file submissions to SMAHT."
 # TODO: Update this email address when a more specific one is available for SMaHT.
 authors = ["SMaHT DAC <smhelp@hms-dbmi.atlassian.net >"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["submitr", "smaht"]
 homepage = "https://github.com/smaht-dac/submitr"
```

### Comparing `smaht_submitr-0.7.0.1b95/submitr/base.py` & `smaht_submitr-0.7.0.1b96/submitr/base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/output.py` & `smaht_submitr-0.7.0.1b96/submitr/output.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/progress_bar.py` & `smaht_submitr-0.7.0.1b96/submitr/progress_bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,15 +234,16 @@
                 # Another hack to really disable output on interrupt; in this case we set
                 # tqdm.disable to True, but output can still dribble out, so if the output
                 # looks like it is from tqdm and we are disabled/done then do no output.
                 return
             if sentinel_internal in text:
                 spinc = spina[spini % spinn] if not ("100%|" in text) else "| ✓" ; spini += 1  # noqa
                 text = replace_first(text, sentinel_internal, f" {spinc}")
-                text = replace_first(text, "%|", "% ◀‖")
+                # text = replace_first(text, "%|", "% ◀‖")
+                text = replace_first(text, "%|", "% ◀|")
                 # Another oddity: for the rate sometimes tqdm intermittently prints
                 # something like "1.54s/" rather than "1.54/s"; something to do with
                 # the unit we gave, which is empty; idunno; just replace it here.
                 text = replace_first(text, "s/ ", "/s ")
             sys_stdout_write(text)
             sys.stdout.flush()
         def restore_stdout_write() -> None:  # noqa
```

### Comparing `smaht_submitr-0.7.0.1b95/submitr/s3_utils.py` & `smaht_submitr-0.7.0.1b96/submitr/s3_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/scripts/check_submission.py` & `smaht_submitr-0.7.0.1b96/submitr/scripts/check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/scripts/cli_utils.py` & `smaht_submitr-0.7.0.1b96/submitr/scripts/cli_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/scripts/list_submissions.py` & `smaht_submitr-0.7.0.1b96/submitr/scripts/list_submissions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/scripts/make_sample_fastq_file.py` & `smaht_submitr-0.7.0.1b96/submitr/scripts/make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/scripts/resume_uploads.py` & `smaht_submitr-0.7.0.1b96/submitr/scripts/resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/scripts/show_upload_info.py` & `smaht_submitr-0.7.0.1b96/submitr/scripts/show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/scripts/submit_genelist.py` & `smaht_submitr-0.7.0.1b96/submitr/scripts/submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/scripts/submit_metadata_bundle.py` & `smaht_submitr-0.7.0.1b96/submitr/scripts/submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/scripts/submit_ontology.py` & `smaht_submitr-0.7.0.1b96/submitr/scripts/submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/scripts/upload_item_data.py` & `smaht_submitr-0.7.0.1b96/submitr/scripts/upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/scripts/view_portal_object.py` & `smaht_submitr-0.7.0.1b96/submitr/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/submission.py` & `smaht_submitr-0.7.0.1b96/submitr/submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/tests/data/submission_simple.xlsx` & `smaht_submitr-0.7.0.1b96/submitr/tests/data/submission_simple.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/tests/data/submission_simple2.xlsx` & `smaht_submitr-0.7.0.1b96/submitr/tests/data/submission_simple2.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/tests/data/submission_test.xlsx` & `smaht_submitr-0.7.0.1b96/submitr/tests/data/submission_test.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/tests/data/submission_test_with_errors.xlsx` & `smaht_submitr-0.7.0.1b96/submitr/tests/data/submission_test_with_errors.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/tests/test_base.py` & `smaht_submitr-0.7.0.1b96/submitr/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/tests/test_check_submission.py` & `smaht_submitr-0.7.0.1b96/submitr/tests/test_check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/tests/test_exceptions.py` & `smaht_submitr-0.7.0.1b96/submitr/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/tests/test_make_sample_fastq_file.py` & `smaht_submitr-0.7.0.1b96/submitr/tests/test_make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/tests/test_misc.py` & `smaht_submitr-0.7.0.1b96/submitr/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/tests/test_resume_uploads.py` & `smaht_submitr-0.7.0.1b96/submitr/tests/test_resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/tests/test_show_upload_info.py` & `smaht_submitr-0.7.0.1b96/submitr/tests/test_show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/tests/test_submission.py` & `smaht_submitr-0.7.0.1b96/submitr/tests/test_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/tests/test_submit_genelist.py` & `smaht_submitr-0.7.0.1b96/submitr/tests/test_submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/tests/test_submit_metadata_bundle.py` & `smaht_submitr-0.7.0.1b96/submitr/tests/test_submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/tests/test_submit_ontology.py` & `smaht_submitr-0.7.0.1b96/submitr/tests/test_submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/tests/test_testing_helpers.py` & `smaht_submitr-0.7.0.1b96/submitr/tests/test_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/tests/test_upload_item_data.py` & `smaht_submitr-0.7.0.1b96/submitr/tests/test_upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/tests/test_utils.py` & `smaht_submitr-0.7.0.1b96/submitr/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/tests/testing_helpers.py` & `smaht_submitr-0.7.0.1b96/submitr/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/submitr/utils.py` & `smaht_submitr-0.7.0.1b96/submitr/utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b95/PKG-INFO` & `smaht_submitr-0.7.0.1b96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smaht-submitr
-Version: 0.7.0.1b95
+Version: 0.7.0.1b96
 Summary: Support for uploading file submissions to SMAHT.
 Home-page: https://github.com/smaht-dac/submitr
 License: MIT
 Keywords: submitr,smaht
 Author: SMaHT DAC
 Author-email: smhelp@hms-dbmi.atlassian.net 
 Requires-Python: >=3.8.0,<3.12
```

