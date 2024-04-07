# Comparing `tmp/smaht_submitr-0.7.0.1b99.tar.gz` & `tmp/smaht_submitr-0.7.0.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smaht_submitr-0.7.0.1b99.tar", max compression
+gzip compressed data, was "smaht_submitr-0.7.0.2b1.tar", max compression
```

## Comparing `smaht_submitr-0.7.0.1b99.tar` & `smaht_submitr-0.7.0.2b1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1098 2024-04-07 13:07:19.201644 smaht_submitr-0.7.0.1b99/LICENSE.txt
--rw-r--r--   0        0        0     2602 2024-04-07 13:07:19.201644 smaht_submitr-0.7.0.1b99/README.rst
--rw-r--r--   0        0        0     3422 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/__init__.py
--rw-r--r--   0        0        0      731 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/base.py
--rw-r--r--   0        0        0      294 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/exceptions.py
--rw-r--r--   0        0        0     2628 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/output.py
--rw-r--r--   0        0        0    12784 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/progress_bar.py
--rw-r--r--   0        0        0    10819 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/s3_utils.py
--rw-r--r--   0        0        0        0 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/__init__.py
--rw-r--r--   0        0        0     4785 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/check_submission.py
--rw-r--r--   0        0        0     8458 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/cli_utils.py
--rw-r--r--   0        0        0     1828 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/list_submissions.py
--rw-r--r--   0        0        0      940 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/make_sample_fastq_file.py
--rw-r--r--   0        0        0     5709 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/resume_uploads.py
--rw-r--r--   0        0        0     1368 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/show_upload_info.py
--rw-r--r--   0        0        0     1572 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/submit_genelist.py
--rw-r--r--   0        0        0    19891 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/submit_metadata_bundle.py
--rw-r--r--   0        0        0     3437 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/submit_ontology.py
--rw-r--r--   0        0        0     1616 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/upload_item_data.py
--rw-r--r--   0        0        0    28731 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/view_portal_object.py
--rw-r--r--   0        0        0   151701 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/submission.py
--rw-r--r--   0        0        0        0 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/__init__.py
--rw-r--r--   0        0        0      355 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/conftest_settings.py
--rw-r--r--   0        0        0      163 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/f1_R1.fastq.gz
--rw-r--r--   0        0        0      165 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/f1_R2.fastq.gz
--rw-r--r--   0        0        0      167 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/f2_R1.fastq.gz
--rw-r--r--   0        0        0      164 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/f2_R2.fastq.gz
--rw-r--r--   0        0        0      272 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/simulated_bundle.json
--rw-r--r--   0        0        0    10870 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/submission_simple.xlsx
--rw-r--r--   0        0        0    10875 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/submission_simple2.xlsx
--rw-r--r--   0        0        0    13306 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/submission_test.xlsx
--rw-r--r--   0        0        0    13192 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/submission_test_with_errors.xlsx
--rw-r--r--   0        0        0      169 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/test1_R1.fastq.gz
--rw-r--r--   0        0        0      168 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/test1_R2.fastq.gz
--rw-r--r--   0        0        0     1333 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/test_base.py
--rw-r--r--   0        0        0     2629 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/test_check_submission.py
--rw-r--r--   0        0        0      551 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/test_exceptions.py
--rw-r--r--   0        0        0     1620 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/test_make_sample_fastq_file.py
--rw-r--r--   0        0        0     1421 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/test_misc.py
--rw-r--r--   0        0        0    11606 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/test_resume_uploads.py
--rw-r--r--   0        0        0     2478 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/test_show_upload_info.py
--rw-r--r--   0        0        0   157433 2024-04-07 13:07:19.245645 smaht_submitr-0.7.0.1b99/submitr/tests/test_submission.py
--rw-r--r--   0        0        0     2836 2024-04-07 13:07:19.245645 smaht_submitr-0.7.0.1b99/submitr/tests/test_submit_genelist.py
--rw-r--r--   0        0        0     6874 2024-04-07 13:07:19.245645 smaht_submitr-0.7.0.1b99/submitr/tests/test_submit_metadata_bundle.py
--rw-r--r--   0        0        0     3013 2024-04-07 13:07:19.245645 smaht_submitr-0.7.0.1b99/submitr/tests/test_submit_ontology.py
--rw-r--r--   0        0        0     1300 2024-04-07 13:07:19.245645 smaht_submitr-0.7.0.1b99/submitr/tests/test_testing_helpers.py
--rw-r--r--   0        0        0     3661 2024-04-07 13:07:19.245645 smaht_submitr-0.7.0.1b99/submitr/tests/test_upload_item_data.py
--rw-r--r--   0        0        0     4353 2024-04-07 13:07:19.245645 smaht_submitr-0.7.0.1b99/submitr/tests/test_utils.py
--rw-r--r--   0        0        0     1351 2024-04-07 13:07:19.245645 smaht_submitr-0.7.0.1b99/submitr/tests/testing_helpers.py
--rw-r--r--   0        0        0    11801 2024-04-07 13:07:19.245645 smaht_submitr-0.7.0.1b99/submitr/utils.py
--rw-r--r--   0        0        0     3989 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.1b99/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-07 13:15:33.143829 smaht_submitr-0.7.0.2b1/LICENSE.txt
+-rw-r--r--   0        0        0     2602 2024-04-07 13:15:33.143829 smaht_submitr-0.7.0.2b1/README.rst
+-rw-r--r--   0        0        0     3421 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/base.py
+-rw-r--r--   0        0        0      294 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/exceptions.py
+-rw-r--r--   0        0        0     2628 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/output.py
+-rw-r--r--   0        0        0    12781 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/progress_bar.py
+-rw-r--r--   0        0        0    10819 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/s3_utils.py
+-rw-r--r--   0        0        0        0 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/__init__.py
+-rw-r--r--   0        0        0     4785 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/check_submission.py
+-rw-r--r--   0        0        0     8466 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/cli_utils.py
+-rw-r--r--   0        0        0     1828 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/list_submissions.py
+-rw-r--r--   0        0        0      940 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/make_sample_fastq_file.py
+-rw-r--r--   0        0        0     5709 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/resume_uploads.py
+-rw-r--r--   0        0        0     1368 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/show_upload_info.py
+-rw-r--r--   0        0        0     1572 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/submit_genelist.py
+-rw-r--r--   0        0        0    19891 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3437 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/submit_ontology.py
+-rw-r--r--   0        0        0     1616 2024-04-07 13:15:33.183829 smaht_submitr-0.7.0.2b1/submitr/scripts/upload_item_data.py
+-rw-r--r--   0        0        0    28731 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/scripts/view_portal_object.py
+-rw-r--r--   0        0        0   151701 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/submission.py
+-rw-r--r--   0        0        0        0 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/__init__.py
+-rw-r--r--   0        0        0      355 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/conftest_settings.py
+-rw-r--r--   0        0        0      163 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/f1_R1.fastq.gz
+-rw-r--r--   0        0        0      165 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/f1_R2.fastq.gz
+-rw-r--r--   0        0        0      167 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/f2_R1.fastq.gz
+-rw-r--r--   0        0        0      164 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/f2_R2.fastq.gz
+-rw-r--r--   0        0        0      272 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/simulated_bundle.json
+-rw-r--r--   0        0        0    10870 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/submission_simple.xlsx
+-rw-r--r--   0        0        0    10875 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/submission_simple2.xlsx
+-rw-r--r--   0        0        0    13306 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/submission_test.xlsx
+-rw-r--r--   0        0        0    13192 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/submission_test_with_errors.xlsx
+-rw-r--r--   0        0        0      169 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/test1_R1.fastq.gz
+-rw-r--r--   0        0        0      168 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/data/test1_R2.fastq.gz
+-rw-r--r--   0        0        0     1333 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_base.py
+-rw-r--r--   0        0        0     2629 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_check_submission.py
+-rw-r--r--   0        0        0      551 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1620 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_make_sample_fastq_file.py
+-rw-r--r--   0        0        0     1421 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_misc.py
+-rw-r--r--   0        0        0    11606 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_resume_uploads.py
+-rw-r--r--   0        0        0     2478 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_show_upload_info.py
+-rw-r--r--   0        0        0   157433 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_submission.py
+-rw-r--r--   0        0        0     2836 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_submit_genelist.py
+-rw-r--r--   0        0        0     6874 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3013 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_submit_ontology.py
+-rw-r--r--   0        0        0     1300 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_testing_helpers.py
+-rw-r--r--   0        0        0     3661 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_upload_item_data.py
+-rw-r--r--   0        0        0     4353 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/test_utils.py
+-rw-r--r--   0        0        0     1351 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/tests/testing_helpers.py
+-rw-r--r--   0        0        0    11801 2024-04-07 13:15:33.187829 smaht_submitr-0.7.0.2b1/submitr/utils.py
+-rw-r--r--   0        0        0     3988 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.2b1/PKG-INFO
```

### Comparing `smaht_submitr-0.7.0.1b99/LICENSE.txt` & `smaht_submitr-0.7.0.2b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/README.rst` & `smaht_submitr-0.7.0.2b1/README.rst`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/pyproject.toml` & `smaht_submitr-0.7.0.2b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smaht-submitr"
-version = "0.7.0.1b99"  # TODO: To become 0.8.0
+version = "0.7.0.2b1"  # TODO: To become 0.8.0
 description = "Support for uploading file submissions to SMAHT."
 # TODO: Update this email address when a more specific one is available for SMaHT.
 authors = ["SMaHT DAC <smhelp@hms-dbmi.atlassian.net >"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["submitr", "smaht"]
 homepage = "https://github.com/smaht-dac/submitr"
```

### Comparing `smaht_submitr-0.7.0.1b99/submitr/base.py` & `smaht_submitr-0.7.0.2b1/submitr/base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/output.py` & `smaht_submitr-0.7.0.2b1/submitr/output.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/progress_bar.py` & `smaht_submitr-0.7.0.2b1/submitr/progress_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         self._bar = None
         self._disabled = False
         self._done = False
         self._printf = printf if callable(printf) else print
         self._tidy_output_hack = (tidy_output_hack is True)
         self._started = time.time()
         self._stop_requested = False
-        # Interrupt handling. We do not in do the actual (signal) interrupt setup
+        # Interrupt handling. We do not do the actual (signal) interrupt setup
         # in self._initialiaze as that could be called from a (sub) thread; and in
         # Python we can only set a signal (SIGINT in our case) on the main thread.
         self._catch_interrupt = (catch_interrupt is True)
         self._interrupt = interrupt if callable(interrupt) else None
         self._interrupt_continue = interrupt_continue if callable(interrupt_continue) else None
         self._interrupt_stop = interrupt_stop if callable(interrupt_stop) else None
         if interrupt_exit in [True, False]:
```

### Comparing `smaht_submitr-0.7.0.1b99/submitr/s3_utils.py` & `smaht_submitr-0.7.0.2b1/submitr/s3_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/scripts/check_submission.py` & `smaht_submitr-0.7.0.2b1/submitr/scripts/check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/scripts/cli_utils.py` & `smaht_submitr-0.7.0.2b1/submitr/scripts/cli_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
                     version_release_date = ""
                 lines = [
                     "===",
                     "smaht-submitr [VERSION]",
                     "===",
                     f"This version: {version}{version_release_date}",
                     f"Most recent version: {most_recent_version_info.version}"
-                        f" | {most_recent_version_info.release_date}",
+                        f" | {most_recent_version_info.release_date}",  # noqa
                     f"More recent beta version: {most_recent_version_info.beta_version}"
                         f" | {most_recent_version_info.beta_release_date}",
                 ]
                 if not has_most_recent_version and most_recent_version_info.this_release_date:
                     lines += [
                         "===",
                         f"▶ A more recent version is available ◀"
```

### Comparing `smaht_submitr-0.7.0.1b99/submitr/scripts/list_submissions.py` & `smaht_submitr-0.7.0.2b1/submitr/scripts/list_submissions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/scripts/make_sample_fastq_file.py` & `smaht_submitr-0.7.0.2b1/submitr/scripts/make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/scripts/resume_uploads.py` & `smaht_submitr-0.7.0.2b1/submitr/scripts/resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/scripts/show_upload_info.py` & `smaht_submitr-0.7.0.2b1/submitr/scripts/show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/scripts/submit_genelist.py` & `smaht_submitr-0.7.0.2b1/submitr/scripts/submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/scripts/submit_metadata_bundle.py` & `smaht_submitr-0.7.0.2b1/submitr/scripts/submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/scripts/submit_ontology.py` & `smaht_submitr-0.7.0.2b1/submitr/scripts/submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/scripts/upload_item_data.py` & `smaht_submitr-0.7.0.2b1/submitr/scripts/upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/scripts/view_portal_object.py` & `smaht_submitr-0.7.0.2b1/submitr/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/submission.py` & `smaht_submitr-0.7.0.2b1/submitr/submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/tests/data/submission_simple.xlsx` & `smaht_submitr-0.7.0.2b1/submitr/tests/data/submission_simple.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/tests/data/submission_simple2.xlsx` & `smaht_submitr-0.7.0.2b1/submitr/tests/data/submission_simple2.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/tests/data/submission_test.xlsx` & `smaht_submitr-0.7.0.2b1/submitr/tests/data/submission_test.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/tests/data/submission_test_with_errors.xlsx` & `smaht_submitr-0.7.0.2b1/submitr/tests/data/submission_test_with_errors.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/tests/test_base.py` & `smaht_submitr-0.7.0.2b1/submitr/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/tests/test_check_submission.py` & `smaht_submitr-0.7.0.2b1/submitr/tests/test_check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/tests/test_exceptions.py` & `smaht_submitr-0.7.0.2b1/submitr/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/tests/test_make_sample_fastq_file.py` & `smaht_submitr-0.7.0.2b1/submitr/tests/test_make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/tests/test_misc.py` & `smaht_submitr-0.7.0.2b1/submitr/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/tests/test_resume_uploads.py` & `smaht_submitr-0.7.0.2b1/submitr/tests/test_resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/tests/test_show_upload_info.py` & `smaht_submitr-0.7.0.2b1/submitr/tests/test_show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/tests/test_submission.py` & `smaht_submitr-0.7.0.2b1/submitr/tests/test_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/tests/test_submit_genelist.py` & `smaht_submitr-0.7.0.2b1/submitr/tests/test_submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/tests/test_submit_metadata_bundle.py` & `smaht_submitr-0.7.0.2b1/submitr/tests/test_submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/tests/test_submit_ontology.py` & `smaht_submitr-0.7.0.2b1/submitr/tests/test_submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/tests/test_testing_helpers.py` & `smaht_submitr-0.7.0.2b1/submitr/tests/test_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/tests/test_upload_item_data.py` & `smaht_submitr-0.7.0.2b1/submitr/tests/test_upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/tests/test_utils.py` & `smaht_submitr-0.7.0.2b1/submitr/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/tests/testing_helpers.py` & `smaht_submitr-0.7.0.2b1/submitr/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/submitr/utils.py` & `smaht_submitr-0.7.0.2b1/submitr/utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b99/PKG-INFO` & `smaht_submitr-0.7.0.2b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smaht-submitr
-Version: 0.7.0.1b99
+Version: 0.7.0.2b1
 Summary: Support for uploading file submissions to SMAHT.
 Home-page: https://github.com/smaht-dac/submitr
 License: MIT
 Keywords: submitr,smaht
 Author: SMaHT DAC
 Author-email: smhelp@hms-dbmi.atlassian.net 
 Requires-Python: >=3.8.0,<3.12
```
