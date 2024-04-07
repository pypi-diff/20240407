# Comparing `tmp/smaht_submitr-0.7.0.1b98.tar.gz` & `tmp/smaht_submitr-0.7.0.1b99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smaht_submitr-0.7.0.1b98.tar", max compression
+gzip compressed data, was "smaht_submitr-0.7.0.1b99.tar", max compression
```

## Comparing `smaht_submitr-0.7.0.1b98.tar` & `smaht_submitr-0.7.0.1b99.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1098 2024-04-07 12:12:12.954102 smaht_submitr-0.7.0.1b98/LICENSE.txt
--rw-r--r--   0        0        0     2602 2024-04-07 12:12:12.954102 smaht_submitr-0.7.0.1b98/README.rst
--rw-r--r--   0        0        0     3422 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/__init__.py
--rw-r--r--   0        0        0      731 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/base.py
--rw-r--r--   0        0        0      294 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/exceptions.py
--rw-r--r--   0        0        0     2628 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/output.py
--rw-r--r--   0        0        0    12784 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/progress_bar.py
--rw-r--r--   0        0        0    10819 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/s3_utils.py
--rw-r--r--   0        0        0        0 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/__init__.py
--rw-r--r--   0        0        0     4785 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/check_submission.py
--rw-r--r--   0        0        0     8008 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/cli_utils.py
--rw-r--r--   0        0        0     1828 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/list_submissions.py
--rw-r--r--   0        0        0      940 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/make_sample_fastq_file.py
--rw-r--r--   0        0        0     5709 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/resume_uploads.py
--rw-r--r--   0        0        0     1368 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/show_upload_info.py
--rw-r--r--   0        0        0     1572 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/submit_genelist.py
--rw-r--r--   0        0        0    19891 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/submit_metadata_bundle.py
--rw-r--r--   0        0        0     3437 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/submit_ontology.py
--rw-r--r--   0        0        0     1616 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/upload_item_data.py
--rw-r--r--   0        0        0    28731 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/view_portal_object.py
--rw-r--r--   0        0        0   151701 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/submission.py
--rw-r--r--   0        0        0        0 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/__init__.py
--rw-r--r--   0        0        0      355 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/conftest_settings.py
--rw-r--r--   0        0        0      163 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/f1_R1.fastq.gz
--rw-r--r--   0        0        0      165 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/f1_R2.fastq.gz
--rw-r--r--   0        0        0      167 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/f2_R1.fastq.gz
--rw-r--r--   0        0        0      164 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/f2_R2.fastq.gz
--rw-r--r--   0        0        0      272 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/simulated_bundle.json
--rw-r--r--   0        0        0    10870 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/submission_simple.xlsx
--rw-r--r--   0        0        0    10875 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/submission_simple2.xlsx
--rw-r--r--   0        0        0    13306 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/submission_test.xlsx
--rw-r--r--   0        0        0    13192 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/submission_test_with_errors.xlsx
--rw-r--r--   0        0        0      169 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/test1_R1.fastq.gz
--rw-r--r--   0        0        0      168 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/test1_R2.fastq.gz
--rw-r--r--   0        0        0     1333 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_base.py
--rw-r--r--   0        0        0     2629 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_check_submission.py
--rw-r--r--   0        0        0      551 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_exceptions.py
--rw-r--r--   0        0        0     1620 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_make_sample_fastq_file.py
--rw-r--r--   0        0        0     1421 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_misc.py
--rw-r--r--   0        0        0    11606 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_resume_uploads.py
--rw-r--r--   0        0        0     2478 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_show_upload_info.py
--rw-r--r--   0        0        0   157433 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_submission.py
--rw-r--r--   0        0        0     2836 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_submit_genelist.py
--rw-r--r--   0        0        0     6874 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_submit_metadata_bundle.py
--rw-r--r--   0        0        0     3013 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_submit_ontology.py
--rw-r--r--   0        0        0     1300 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_testing_helpers.py
--rw-r--r--   0        0        0     3661 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_upload_item_data.py
--rw-r--r--   0        0        0     4353 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_utils.py
--rw-r--r--   0        0        0     1351 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/testing_helpers.py
--rw-r--r--   0        0        0    11074 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/utils.py
--rw-r--r--   0        0        0     3989 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.1b98/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-07 13:07:19.201644 smaht_submitr-0.7.0.1b99/LICENSE.txt
+-rw-r--r--   0        0        0     2602 2024-04-07 13:07:19.201644 smaht_submitr-0.7.0.1b99/README.rst
+-rw-r--r--   0        0        0     3422 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/base.py
+-rw-r--r--   0        0        0      294 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/exceptions.py
+-rw-r--r--   0        0        0     2628 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/output.py
+-rw-r--r--   0        0        0    12784 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/progress_bar.py
+-rw-r--r--   0        0        0    10819 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/s3_utils.py
+-rw-r--r--   0        0        0        0 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/__init__.py
+-rw-r--r--   0        0        0     4785 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/check_submission.py
+-rw-r--r--   0        0        0     8458 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/cli_utils.py
+-rw-r--r--   0        0        0     1828 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/list_submissions.py
+-rw-r--r--   0        0        0      940 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/make_sample_fastq_file.py
+-rw-r--r--   0        0        0     5709 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/resume_uploads.py
+-rw-r--r--   0        0        0     1368 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/show_upload_info.py
+-rw-r--r--   0        0        0     1572 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/submit_genelist.py
+-rw-r--r--   0        0        0    19891 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3437 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/submit_ontology.py
+-rw-r--r--   0        0        0     1616 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/upload_item_data.py
+-rw-r--r--   0        0        0    28731 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/scripts/view_portal_object.py
+-rw-r--r--   0        0        0   151701 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/submission.py
+-rw-r--r--   0        0        0        0 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/__init__.py
+-rw-r--r--   0        0        0      355 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/conftest_settings.py
+-rw-r--r--   0        0        0      163 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/f1_R1.fastq.gz
+-rw-r--r--   0        0        0      165 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/f1_R2.fastq.gz
+-rw-r--r--   0        0        0      167 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/f2_R1.fastq.gz
+-rw-r--r--   0        0        0      164 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/f2_R2.fastq.gz
+-rw-r--r--   0        0        0      272 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/simulated_bundle.json
+-rw-r--r--   0        0        0    10870 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/submission_simple.xlsx
+-rw-r--r--   0        0        0    10875 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/submission_simple2.xlsx
+-rw-r--r--   0        0        0    13306 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/submission_test.xlsx
+-rw-r--r--   0        0        0    13192 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/submission_test_with_errors.xlsx
+-rw-r--r--   0        0        0      169 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/test1_R1.fastq.gz
+-rw-r--r--   0        0        0      168 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/data/test1_R2.fastq.gz
+-rw-r--r--   0        0        0     1333 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/test_base.py
+-rw-r--r--   0        0        0     2629 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/test_check_submission.py
+-rw-r--r--   0        0        0      551 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1620 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/test_make_sample_fastq_file.py
+-rw-r--r--   0        0        0     1421 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/test_misc.py
+-rw-r--r--   0        0        0    11606 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/test_resume_uploads.py
+-rw-r--r--   0        0        0     2478 2024-04-07 13:07:19.241645 smaht_submitr-0.7.0.1b99/submitr/tests/test_show_upload_info.py
+-rw-r--r--   0        0        0   157433 2024-04-07 13:07:19.245645 smaht_submitr-0.7.0.1b99/submitr/tests/test_submission.py
+-rw-r--r--   0        0        0     2836 2024-04-07 13:07:19.245645 smaht_submitr-0.7.0.1b99/submitr/tests/test_submit_genelist.py
+-rw-r--r--   0        0        0     6874 2024-04-07 13:07:19.245645 smaht_submitr-0.7.0.1b99/submitr/tests/test_submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3013 2024-04-07 13:07:19.245645 smaht_submitr-0.7.0.1b99/submitr/tests/test_submit_ontology.py
+-rw-r--r--   0        0        0     1300 2024-04-07 13:07:19.245645 smaht_submitr-0.7.0.1b99/submitr/tests/test_testing_helpers.py
+-rw-r--r--   0        0        0     3661 2024-04-07 13:07:19.245645 smaht_submitr-0.7.0.1b99/submitr/tests/test_upload_item_data.py
+-rw-r--r--   0        0        0     4353 2024-04-07 13:07:19.245645 smaht_submitr-0.7.0.1b99/submitr/tests/test_utils.py
+-rw-r--r--   0        0        0     1351 2024-04-07 13:07:19.245645 smaht_submitr-0.7.0.1b99/submitr/tests/testing_helpers.py
+-rw-r--r--   0        0        0    11801 2024-04-07 13:07:19.245645 smaht_submitr-0.7.0.1b99/submitr/utils.py
+-rw-r--r--   0        0        0     3989 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.1b99/PKG-INFO
```

### Comparing `smaht_submitr-0.7.0.1b98/LICENSE.txt` & `smaht_submitr-0.7.0.1b99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/README.rst` & `smaht_submitr-0.7.0.1b99/README.rst`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/pyproject.toml` & `smaht_submitr-0.7.0.1b99/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smaht-submitr"
-version = "0.7.0.1b98"  # TODO: To become 0.8.0
+version = "0.7.0.1b99"  # TODO: To become 0.8.0
 description = "Support for uploading file submissions to SMAHT."
 # TODO: Update this email address when a more specific one is available for SMaHT.
 authors = ["SMaHT DAC <smhelp@hms-dbmi.atlassian.net >"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["submitr", "smaht"]
 homepage = "https://github.com/smaht-dac/submitr"
```

### Comparing `smaht_submitr-0.7.0.1b98/submitr/base.py` & `smaht_submitr-0.7.0.1b99/submitr/base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/output.py` & `smaht_submitr-0.7.0.1b99/submitr/output.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/progress_bar.py` & `smaht_submitr-0.7.0.1b99/submitr/progress_bar.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/s3_utils.py` & `smaht_submitr-0.7.0.1b99/submitr/s3_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/scripts/check_submission.py` & `smaht_submitr-0.7.0.1b99/submitr/scripts/check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/scripts/cli_utils.py` & `smaht_submitr-0.7.0.1b99/submitr/scripts/cli_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,30 +118,41 @@
 
     def _print_version(self, verbose: bool = False) -> None:
         if version := self._get_version(with_most_recent_check_mark=False):
             if verbose and (most_recent_version_info := get_most_recent_version_info()):
                 has_most_recent_version = (
                     (most_recent_version_info.version == version) or
                     (most_recent_version_info.beta_version == version))
-                print_boxed([
+                if most_recent_version_info.this_release_date:
+                    version_release_date = f" | {most_recent_version_info.this_release_date}"
+                else:
+                    version_release_date = ""
+                lines = [
                     "===",
                     "smaht-submitr [VERSION]",
                     "===",
-                    f"This version: {version}"
-                        f"{' ✓' if has_most_recent_version else ' ✗ A more recent version is available ◀'}",  # noqa
+                    f"This version: {version}{version_release_date}",
                     f"Most recent version: {most_recent_version_info.version}"
                         f" | {most_recent_version_info.release_date}",
                     f"More recent beta version: {most_recent_version_info.beta_version}"
                         f" | {most_recent_version_info.beta_release_date}",
+                ]
+                if not has_most_recent_version and most_recent_version_info.this_release_date:
+                    lines += [
+                        "===",
+                        f"▶ A more recent version is available ◀"
+                    ]
+                lines += [
                     "===",
-                    "For all version please see: https://pypi.org/project/smaht-submitr",
+                    "For all versions please see: https://pypi.org/project/smaht-submitr",
                     "===",
                     self.COPYRIGHT,
                     "==="
-                ], right_justified_macro=("[VERSION]", self._get_version))
+                ]
+                print_boxed(lines, right_justified_macro=("[VERSION]", self._get_version))
                 return
             else:
                 PRINT(f"{self._package or 'COMMAND'}: {version}")
                 return
         PRINT(f"{self._package or 'COMMAND'}: No version available")
 
     @lru_cache(maxsize=1)
```

### Comparing `smaht_submitr-0.7.0.1b98/submitr/scripts/list_submissions.py` & `smaht_submitr-0.7.0.1b99/submitr/scripts/list_submissions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/scripts/make_sample_fastq_file.py` & `smaht_submitr-0.7.0.1b99/submitr/scripts/make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/scripts/resume_uploads.py` & `smaht_submitr-0.7.0.1b99/submitr/scripts/resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/scripts/show_upload_info.py` & `smaht_submitr-0.7.0.1b99/submitr/scripts/show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/scripts/submit_genelist.py` & `smaht_submitr-0.7.0.1b99/submitr/scripts/submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/scripts/submit_metadata_bundle.py` & `smaht_submitr-0.7.0.1b99/submitr/scripts/submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/scripts/submit_ontology.py` & `smaht_submitr-0.7.0.1b99/submitr/scripts/submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/scripts/upload_item_data.py` & `smaht_submitr-0.7.0.1b99/submitr/scripts/upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/scripts/view_portal_object.py` & `smaht_submitr-0.7.0.1b99/submitr/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/submission.py` & `smaht_submitr-0.7.0.1b99/submitr/submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/tests/data/submission_simple.xlsx` & `smaht_submitr-0.7.0.1b99/submitr/tests/data/submission_simple.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/tests/data/submission_simple2.xlsx` & `smaht_submitr-0.7.0.1b99/submitr/tests/data/submission_simple2.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/tests/data/submission_test.xlsx` & `smaht_submitr-0.7.0.1b99/submitr/tests/data/submission_test.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/tests/data/submission_test_with_errors.xlsx` & `smaht_submitr-0.7.0.1b99/submitr/tests/data/submission_test_with_errors.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/tests/test_base.py` & `smaht_submitr-0.7.0.1b99/submitr/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/tests/test_check_submission.py` & `smaht_submitr-0.7.0.1b99/submitr/tests/test_check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/tests/test_exceptions.py` & `smaht_submitr-0.7.0.1b99/submitr/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/tests/test_make_sample_fastq_file.py` & `smaht_submitr-0.7.0.1b99/submitr/tests/test_make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/tests/test_misc.py` & `smaht_submitr-0.7.0.1b99/submitr/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/tests/test_resume_uploads.py` & `smaht_submitr-0.7.0.1b99/submitr/tests/test_resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/tests/test_show_upload_info.py` & `smaht_submitr-0.7.0.1b99/submitr/tests/test_show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/tests/test_submission.py` & `smaht_submitr-0.7.0.1b99/submitr/tests/test_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/tests/test_submit_genelist.py` & `smaht_submitr-0.7.0.1b99/submitr/tests/test_submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/tests/test_submit_metadata_bundle.py` & `smaht_submitr-0.7.0.1b99/submitr/tests/test_submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/tests/test_submit_ontology.py` & `smaht_submitr-0.7.0.1b99/submitr/tests/test_submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/tests/test_testing_helpers.py` & `smaht_submitr-0.7.0.1b99/submitr/tests/test_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/tests/test_upload_item_data.py` & `smaht_submitr-0.7.0.1b99/submitr/tests/test_upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/tests/test_utils.py` & `smaht_submitr-0.7.0.1b99/submitr/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/tests/testing_helpers.py` & `smaht_submitr-0.7.0.1b99/submitr/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b98/submitr/utils.py` & `smaht_submitr-0.7.0.1b99/submitr/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import namedtuple
 from datetime import datetime
+from functools import lru_cache
 import io
 import hashlib
 import pkg_resources
 import re
 import requests
 import os
 from pathlib import Path
@@ -245,43 +246,54 @@
     macro_name = None
     macro_value = None
     if right_justified_macro and (len(right_justified_macro) == 2):
         macro_name = right_justified_macro[0]
         macro_value = right_justified_macro[1]()
         lines_tmp = []
         for line in lines:
+            if line is None:
+                continue
             if line.endswith(macro_name):
                 line = line.replace(macro_name, right_justified_macro[1]() + " ")
             lines_tmp.append(line)
         length = max(len(line) for line in lines_tmp)
     else:
         length = max(len(line) for line in lines)
     for line in lines:
+        if line is None:
+            continue
         if line == "===":
             printf(f"+{'-' * (length - len(line) + 5)}+")
         elif macro_name and line.endswith(macro_name):
             line = line.replace(macro_name, "")
             printf(f"| {line}{' ' * (length - len(line) - len(macro_value) - 1)} {macro_value} |")
         else:
             printf(f"| {line}{' ' * (length - len(line))} |")
 
 
-def get_version(package: str = "smaht-submitr") -> str:
+@lru_cache(maxsize=1)
+def get_version(package_name: str = "smaht-submitr") -> str:
     try:
-        return pkg_resources.get_distribution(package).version
+        return pkg_resources.get_distribution(package_name).version
     except Exception:
         return ""
 
 
+@lru_cache(maxsize=2)
 def get_most_recent_version_info(package_name: str = "smaht-submitr", beta: bool = True) -> object:
     pypi_url = f"https://pypi.org/pypi/{package_name}/json"
     try:
         if (response := requests.get(pypi_url)).status_code == 200 and (response := response.json()):
             latest_non_beta_version = response["info"]["version"]
+            this_version = get_version(package_name=package_name)
+            this_release_date = None
             releases = response["releases"]
+            if releases and isinstance(this_release_info := releases.get(this_version), list) and this_release_info:
+                if isinstance(this_release_info := this_release_info[0], dict):
+                    this_release_date = datetime.fromisoformat(this_release_info.get("upload_time"))
             latest_non_beta_release_date = datetime.fromisoformat(releases[latest_non_beta_version][0]["upload_time"])
             latest_beta_version = None
             latest_beta_release_date = None
             if beta:
                 # Return the latest beta version but only if it
                 # is more recent than the latest non-beta version.
                 try:
@@ -294,13 +306,15 @@
                         latest_beta_release_date = datetime.fromisoformat(latest_beta_info[1][0]["upload_time"])
                         if latest_non_beta_release_date > latest_beta_release_date:
                             latest_beta_version = None
                             latest_beta_release_date = None
                 except Exception:
                     pass
             return (namedtuple("most_recent_pypi_package_version",
-                               ["version", "release_date", "beta_version", "beta_release_date"])
+                               ["version", "release_date",
+                                "beta_version", "beta_release_date", "this_version", "this_release_date"])
                     (latest_non_beta_version, format_datetime(latest_non_beta_release_date),
-                     latest_beta_version, format_datetime(latest_beta_release_date)))
+                     latest_beta_version, format_datetime(latest_beta_release_date),
+                     this_version, format_datetime(this_release_date)))
     except Exception:
         pass
     return None
```

### Comparing `smaht_submitr-0.7.0.1b98/PKG-INFO` & `smaht_submitr-0.7.0.1b99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smaht-submitr
-Version: 0.7.0.1b98
+Version: 0.7.0.1b99
 Summary: Support for uploading file submissions to SMAHT.
 Home-page: https://github.com/smaht-dac/submitr
 License: MIT
 Keywords: submitr,smaht
 Author: SMaHT DAC
 Author-email: smhelp@hms-dbmi.atlassian.net 
 Requires-Python: >=3.8.0,<3.12
```

