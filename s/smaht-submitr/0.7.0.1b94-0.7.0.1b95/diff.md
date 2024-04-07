# Comparing `tmp/smaht_submitr-0.7.0.1b94.tar.gz` & `tmp/smaht_submitr-0.7.0.1b95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smaht_submitr-0.7.0.1b94.tar", max compression
+gzip compressed data, was "smaht_submitr-0.7.0.1b95.tar", max compression
```

## Comparing `smaht_submitr-0.7.0.1b94.tar` & `smaht_submitr-0.7.0.1b95.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1098 2024-04-06 21:54:40.257927 smaht_submitr-0.7.0.1b94/LICENSE.txt
--rw-r--r--   0        0        0     2602 2024-04-06 21:54:40.257927 smaht_submitr-0.7.0.1b94/README.rst
--rw-r--r--   0        0        0     3422 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/__init__.py
--rw-r--r--   0        0        0      731 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/base.py
--rw-r--r--   0        0        0      294 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/exceptions.py
--rw-r--r--   0        0        0     2628 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/output.py
--rw-r--r--   0        0        0    12723 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/progress_bar.py
--rw-r--r--   0        0        0    10819 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/s3_utils.py
--rw-r--r--   0        0        0        0 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/__init__.py
--rw-r--r--   0        0        0     3844 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/check_submission.py
--rw-r--r--   0        0        0     7601 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/cli_utils.py
--rw-r--r--   0        0        0     1835 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/list_submissions.py
--rw-r--r--   0        0        0      940 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/make_sample_fastq_file.py
--rw-r--r--   0        0        0     5718 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/resume_uploads.py
--rw-r--r--   0        0        0     1368 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/show_upload_info.py
--rw-r--r--   0        0        0     1572 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/submit_genelist.py
--rw-r--r--   0        0        0    19866 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/submit_metadata_bundle.py
--rw-r--r--   0        0        0     3437 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/submit_ontology.py
--rw-r--r--   0        0        0     1616 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/upload_item_data.py
--rw-r--r--   0        0        0    28731 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/view_portal_object.py
--rw-r--r--   0        0        0   149229 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/submission.py
--rw-r--r--   0        0        0        0 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/tests/__init__.py
--rw-r--r--   0        0        0      355 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/tests/conftest_settings.py
--rw-r--r--   0        0        0      163 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/tests/data/f1_R1.fastq.gz
--rw-r--r--   0        0        0      165 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/tests/data/f1_R2.fastq.gz
--rw-r--r--   0        0        0      167 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/tests/data/f2_R1.fastq.gz
--rw-r--r--   0        0        0      164 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/tests/data/f2_R2.fastq.gz
--rw-r--r--   0        0        0      272 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/data/simulated_bundle.json
--rw-r--r--   0        0        0    10870 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/data/submission_simple.xlsx
--rw-r--r--   0        0        0    10875 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/data/submission_simple2.xlsx
--rw-r--r--   0        0        0    13306 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/data/submission_test.xlsx
--rw-r--r--   0        0        0    13192 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/data/submission_test_with_errors.xlsx
--rw-r--r--   0        0        0      169 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/data/test1_R1.fastq.gz
--rw-r--r--   0        0        0      168 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/data/test1_R2.fastq.gz
--rw-r--r--   0        0        0     1333 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_base.py
--rw-r--r--   0        0        0     2629 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_check_submission.py
--rw-r--r--   0        0        0      551 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_exceptions.py
--rw-r--r--   0        0        0     1620 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_make_sample_fastq_file.py
--rw-r--r--   0        0        0     1421 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_misc.py
--rw-r--r--   0        0        0    11606 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_resume_uploads.py
--rw-r--r--   0        0        0     2478 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_show_upload_info.py
--rw-r--r--   0        0        0   157433 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_submission.py
--rw-r--r--   0        0        0     2836 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_submit_genelist.py
--rw-r--r--   0        0        0     6874 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_submit_metadata_bundle.py
--rw-r--r--   0        0        0     3013 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_submit_ontology.py
--rw-r--r--   0        0        0     1300 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_testing_helpers.py
--rw-r--r--   0        0        0     3661 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_upload_item_data.py
--rw-r--r--   0        0        0     4353 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_utils.py
--rw-r--r--   0        0        0     1351 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/testing_helpers.py
--rw-r--r--   0        0        0    11074 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/utils.py
--rw-r--r--   0        0        0     3989 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.1b94/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-07 03:34:27.098607 smaht_submitr-0.7.0.1b95/LICENSE.txt
+-rw-r--r--   0        0        0     2602 2024-04-07 03:34:27.098607 smaht_submitr-0.7.0.1b95/README.rst
+-rw-r--r--   0        0        0     3422 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/base.py
+-rw-r--r--   0        0        0      294 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/exceptions.py
+-rw-r--r--   0        0        0     2628 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/output.py
+-rw-r--r--   0        0        0    12723 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/progress_bar.py
+-rw-r--r--   0        0        0    10819 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/s3_utils.py
+-rw-r--r--   0        0        0        0 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/__init__.py
+-rw-r--r--   0        0        0     4792 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/check_submission.py
+-rw-r--r--   0        0        0     8008 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/cli_utils.py
+-rw-r--r--   0        0        0     1835 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/list_submissions.py
+-rw-r--r--   0        0        0      940 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/make_sample_fastq_file.py
+-rw-r--r--   0        0        0     5684 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/resume_uploads.py
+-rw-r--r--   0        0        0     1368 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/show_upload_info.py
+-rw-r--r--   0        0        0     1572 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/submit_genelist.py
+-rw-r--r--   0        0        0    19866 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3437 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/submit_ontology.py
+-rw-r--r--   0        0        0     1616 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/upload_item_data.py
+-rw-r--r--   0        0        0    28731 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/scripts/view_portal_object.py
+-rw-r--r--   0        0        0   149229 2024-04-07 03:34:27.138607 smaht_submitr-0.7.0.1b95/submitr/submission.py
+-rw-r--r--   0        0        0        0 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/__init__.py
+-rw-r--r--   0        0        0      355 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/conftest_settings.py
+-rw-r--r--   0        0        0      163 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/f1_R1.fastq.gz
+-rw-r--r--   0        0        0      165 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/f1_R2.fastq.gz
+-rw-r--r--   0        0        0      167 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/f2_R1.fastq.gz
+-rw-r--r--   0        0        0      164 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/f2_R2.fastq.gz
+-rw-r--r--   0        0        0      272 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/simulated_bundle.json
+-rw-r--r--   0        0        0    10870 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/submission_simple.xlsx
+-rw-r--r--   0        0        0    10875 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/submission_simple2.xlsx
+-rw-r--r--   0        0        0    13306 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/submission_test.xlsx
+-rw-r--r--   0        0        0    13192 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/submission_test_with_errors.xlsx
+-rw-r--r--   0        0        0      169 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/test1_R1.fastq.gz
+-rw-r--r--   0        0        0      168 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/data/test1_R2.fastq.gz
+-rw-r--r--   0        0        0     1333 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_base.py
+-rw-r--r--   0        0        0     2629 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_check_submission.py
+-rw-r--r--   0        0        0      551 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1620 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_make_sample_fastq_file.py
+-rw-r--r--   0        0        0     1421 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_misc.py
+-rw-r--r--   0        0        0    11606 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_resume_uploads.py
+-rw-r--r--   0        0        0     2478 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_show_upload_info.py
+-rw-r--r--   0        0        0   157433 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_submission.py
+-rw-r--r--   0        0        0     2836 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_submit_genelist.py
+-rw-r--r--   0        0        0     6874 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3013 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_submit_ontology.py
+-rw-r--r--   0        0        0     1300 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_testing_helpers.py
+-rw-r--r--   0        0        0     3661 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_upload_item_data.py
+-rw-r--r--   0        0        0     4353 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/test_utils.py
+-rw-r--r--   0        0        0     1351 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/tests/testing_helpers.py
+-rw-r--r--   0        0        0    11074 2024-04-07 03:34:27.142607 smaht_submitr-0.7.0.1b95/submitr/utils.py
+-rw-r--r--   0        0        0     3989 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.1b95/PKG-INFO
```

### Comparing `smaht_submitr-0.7.0.1b94/LICENSE.txt` & `smaht_submitr-0.7.0.1b95/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/README.rst` & `smaht_submitr-0.7.0.1b95/README.rst`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/pyproject.toml` & `smaht_submitr-0.7.0.1b95/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smaht-submitr"
-version = "0.7.0.1b94"  # TODO: To become 0.8.0
+version = "0.7.0.1b95"  # TODO: To become 0.8.0
 description = "Support for uploading file submissions to SMAHT."
 # TODO: Update this email address when a more specific one is available for SMaHT.
 authors = ["SMaHT DAC <smhelp@hms-dbmi.atlassian.net >"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["submitr", "smaht"]
 homepage = "https://github.com/smaht-dac/submitr"
```

### Comparing `smaht_submitr-0.7.0.1b94/submitr/base.py` & `smaht_submitr-0.7.0.1b95/submitr/base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/output.py` & `smaht_submitr-0.7.0.1b95/submitr/output.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/progress_bar.py` & `smaht_submitr-0.7.0.1b95/submitr/progress_bar.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/s3_utils.py` & `smaht_submitr-0.7.0.1b95/submitr/s3_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/scripts/check_submission.py` & `smaht_submitr-0.7.0.1b95/submitr/scripts/check_submission.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,71 @@
-import argparse
 import os
 from dcicutils.command_utils import script_catch_errors
 from dcicutils.common import ORCHESTRATED_APPS
 from ..base import DEFAULT_APP
 from ..submission import _monitor_ingestion_process, _pytesting
+from .cli_utils import CustomArgumentParser
 
-
-EPILOG = __doc__
+_HELP = f"""
+===
+check-submission [VERSION]
+===
+Tool to check the status of previously submitted metedata.
+If the given UUID is for a validation rather than a submission
+then you will have the opportunity to continue with its submission.
+See: {CustomArgumentParser.HELP_URL}#check-submission
+===
+USAGE: check-submission UUID OPTIONS
+-----
+UUID: This is UUID of your submission.
+===
+OPTIONS:
+===
+--env ENVIRONMENT-NAME
+  To specify your environment name; from your ~/.smaht-keys.json file.
+--KEYS-FILE
+  To specify an alternate credentials/keys
+  file to the default ~/.smaht-keys.json file.
+--directory DIRECTORY
+  To specify a directory containing the files to upload;
+  this directory will be search, recursively.
+--directory-only
+  Same as --directory but does NOT search recursively.
+--output OUTPUT-FILE
+  Writes all logging output to the specified file;
+  and refrains from printing lengthy content to output/stdout.
+--verbose
+  Displays more verbose output.
+--help
+  Prints this documentation.
+--help-web
+  Opens your browser to the Web based documentation.
+  {CustomArgumentParser.HELP_URL}
+===
+"""
 
 
 def main(simulated_args_for_testing=None):
 
-    args = argparse.ArgumentParser(  # noqa - PyCharm wrongly thinks the formatter_class is invalid
-        description="Check previously submitted submission.",
-        epilog=EPILOG,
-        formatter_class=argparse.RawDescriptionHelpFormatter
-    )
-    args.add_argument('submission_uuid', nargs="?", help='UUID of previously submitted submission.')
-    args.add_argument('--app', choices=ORCHESTRATED_APPS, default=DEFAULT_APP,
-                      help=f"An application (default {DEFAULT_APP!r}. Only for debugging."
-                           f" Normally this should not be given.")
-    args.add_argument('--server', '-s', help="an http or https address of the server to use", default=None)
-    args.add_argument("--env", "-e",
-                      help="Portal environment name for server/credentials (e.g. in ~/.smaht-keys.json).")
-    args.add_argument('--keys', help="Path to keys file (rather than default ~/.smaht-keys.json).", default=None)
-    args.add_argument('--directory', '-d', help="Directory of the upload files (if resuming submission).")
-    args.add_argument('--directory-only', help="Same as --directory but NOT recursively.", default=False)
-    args.add_argument('--output', help="Output file for results.", default=False)
-    args.add_argument('--details', action="store_true", help="More detailed output.", default=False)
-    args.add_argument('--timeout', help="Wait timeout for server validation/submission.")
-    args.add_argument('--verbose', action="store_true", help="More verbose output.", default=False)
-    args.add_argument('--debug', action="store_true", help="Debugging output.", default=False)
-    args = args.parse_args(args=simulated_args_for_testing)
+    parser = CustomArgumentParser(help=_HELP, help_url=CustomArgumentParser.HELP_URL)
+    parser.add_argument('submission_uuid', nargs="?", help='UUID of previously submitted submission.')
+    parser.add_argument('--app', choices=ORCHESTRATED_APPS, default=DEFAULT_APP,
+                        help=f"An application (default {DEFAULT_APP!r}. Only for debugging."
+                             f" Normally this should not be given.")
+    parser.add_argument('--server', help="An http or https address of the server to use.", default=None)
+    parser.add_argument("--env", help="Portal environment name for server/credentials (e.g. in ~/.smaht-keys.json).")
+    parser.add_argument('--keys', help="Path to keys file (rather than default ~/.smaht-keys.json).", default=None)
+    parser.add_argument('--directory', '-d', help="Directory of the upload files (if resuming submission).")
+    parser.add_argument('--directory-only', help="Same as --directory but NOT recursively.", default=False)
+    parser.add_argument('--output', help="Output file for results.", default=False)
+    parser.add_argument('--details', action="store_true", help="More detailed output.", default=False)
+    parser.add_argument('--verbose', action="store_true", help="More verbose output.", default=False)
+    parser.add_argument('--timeout', help="Wait timeout for server validation/submission.")
+    parser.add_argument('--debug', action="store_true", help="Debugging output.", default=False)
+    args = parser.parse_args(args=simulated_args_for_testing)
 
     if not args.submission_uuid:
         if _pytesting():
             exit(2)
         args.submission_uuid = "dummy"
 
     env_from_env = False
```

### Comparing `smaht_submitr-0.7.0.1b94/submitr/scripts/cli_utils.py` & `smaht_submitr-0.7.0.1b95/submitr/scripts/cli_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
+from functools import lru_cache
 import io
 import sys
 import webbrowser
-from typing import List, Optional, Tuple
+from typing import List, Optional, Union
 from dcicutils.misc_utils import PRINT
 from submitr.utils import get_version, get_most_recent_version_info, print_boxed
 
 
 class CustomArgumentParser(argparse.ArgumentParser):
 
     PACKAGE = "smaht-submitr"
@@ -84,15 +85,15 @@
                        "--help-raw", "--help-advanced", "--help-web"]:
                 self.print_help()
                 exit(0)
 
     def _check_version_options(self) -> None:
         for arg in sys.argv:
             if arg in ["version", "-version", "--version", "-v", "--v"]:
-                self._print_version(verbose="-v" not in sys.argv)
+                self._print_version(verbose=("-v" not in sys.argv) and ("--v" not in sys.argv))
                 exit(0)
 
     def print_help(self) -> None:
         if "--help-raw" in sys.argv:
             super().print_help()
             return
         if ("--help-web" in sys.argv or "--doc" in sys.argv) and self._help_url:
@@ -104,33 +105,33 @@
             help_message = self._help
         help_message += f"{self.COPYRIGHT}\n==="
         lines = help_message.split("\n")
         if lines[0] == "":
             lines = lines[1:]
         if lines[len(lines) - 1] == "":
             lines = lines[:len(lines) - 1]
-        _, more_recent_version_message = self._get_most_recent_version_info()
-        if more_recent_version_message:
-            lines.append(more_recent_version_message)
+        most_recent_version_info = self._get_most_recent_version_info()
+        most_recent_version_info = self._get_most_recent_version_info()
+        if isinstance(most_recent_version_info, str):
+            lines.append(most_recent_version_info)
             lines.append("===")
         print_boxed(lines, right_justified_macro=("[VERSION]", self._get_version))
 
     def _print_version(self, verbose: bool = False) -> None:
-        if version := self._get_version():
+        if version := self._get_version(with_most_recent_check_mark=False):
             if verbose and (most_recent_version_info := get_most_recent_version_info()):
                 has_most_recent_version = (
                     (most_recent_version_info.version == version) or
                     (most_recent_version_info.beta_version == version))
-                version = get_version()
                 print_boxed([
                     "===",
                     "smaht-submitr [VERSION]",
                     "===",
                     f"This version: {version}"
-                        f"{' ✓' if has_most_recent_version else ' ✗ A more recent version is available.'}",  # noqa
+                        f"{' ✓' if has_most_recent_version else ' ✗ A more recent version is available ◀'}",  # noqa
                     f"Most recent version: {most_recent_version_info.version}"
                         f" | {most_recent_version_info.release_date}",
                     f"More recent beta version: {most_recent_version_info.beta_version}"
                         f" | {most_recent_version_info.beta_release_date}",
                     "===",
                     "For all version please see: https://pypi.org/project/smaht-submitr",
                     "===",
@@ -139,34 +140,42 @@
                 ], right_justified_macro=("[VERSION]", self._get_version))
                 return
             else:
                 PRINT(f"{self._package or 'COMMAND'}: {version}")
                 return
         PRINT(f"{self._package or 'COMMAND'}: No version available")
 
-    def _get_version(self) -> str:
-        return get_version(self._package)
+    @lru_cache(maxsize=1)
+    def _get_version(self, with_most_recent_check_mark: bool = True) -> str:
+        version = get_version(self._package)
+        if with_most_recent_check_mark and (self._get_most_recent_version_info(version) is True):
+            version = f"✓ {version}"
+        return version
 
-    def _get_most_recent_version_info(self, this_version: Optional[str] = None) -> Tuple[Optional[bool], Optional[str]]:
+    @lru_cache(maxsize=1)
+    def _get_most_recent_version_info(self, this_version: Optional[str] = None) -> Union[bool, str]:
         if not this_version:
             this_version = self._get_version()
+        if this_version.startswith("✓ "):
+            this_version = this_version[2:]
         is_beta_version = ("a" in this_version or "b" in this_version)
         is_most_recent_version = False
         more_recent_version_message = None
         if most_recent_version_info := get_most_recent_version_info():
             if ((most_recent_version_info.version == this_version) or
                 (most_recent_version_info.beta_version == this_version)):  # noqa
                 is_most_recent_version = True
         more_recent_version_message = (
-            f"{self._package or 'COMMAND'}: {this_version}{' ✓' if is_most_recent_version else ''} | {self.COPYRIGHT}")
-        if not is_most_recent_version:
-            if is_beta_version and most_recent_version_info.beta_version:
-                most_recent_version = most_recent_version_info.beta_version
-            else:
-                most_recent_version = most_recent_version_info.version
-            more_recent_version_message = (
-                f"A more recent version of this{' beta' if is_beta_version else ''}"
-                f" software is available: {most_recent_version}")
-        return (is_most_recent_version, more_recent_version_message)
+            f"{self._package or 'COMMAND'}: {this_version}{' ✓' if is_most_recent_version else ''}")
+        if is_most_recent_version:
+            return True
+        if is_beta_version and most_recent_version_info.beta_version:
+            most_recent_version = most_recent_version_info.beta_version
+        else:
+            most_recent_version = most_recent_version_info.version
+        more_recent_version_message = (
+            f"A more recent version of this{' beta' if is_beta_version else ''}"
+            f" software is available: {most_recent_version}")
+        return more_recent_version_message
 
     def is_pytest(self) -> bool:
         return "pytest" in sys.modules
```

### Comparing `smaht_submitr-0.7.0.1b94/submitr/scripts/list_submissions.py` & `smaht_submitr-0.7.0.1b95/submitr/scripts/list_submissions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/scripts/make_sample_fastq_file.py` & `smaht_submitr-0.7.0.1b95/submitr/scripts/make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/scripts/resume_uploads.py` & `smaht_submitr-0.7.0.1b95/submitr/scripts/resume_uploads.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,46 +8,46 @@
 
 _HELP = f"""
 ===
 resume-uploads [VERSION]
 ===
 Tool to upload files referenced in a metadata file,
 previously submitted using submit-metadata-bundle, to SMaHT Portal.
-See: {CustomArgumentParser.HELP_URL}#resuming-uploads
+See: {CustomArgumentParser.HELP_URL}
 ===
 USAGE: resume-uploads UUID OPTIONS
 -----
 UUID: This is UUID of your submission; or the UUID of an individual file
       referenced; or the accession ID of an individual file referenced.
 ===
 OPTIONS:
 ===
 --env ENVIRONMENT-NAME
   To specify your environment name; from your ~/.smaht-keys.json file.
+--KEYS-FILE
+  To specify an alternate credentials/keys
+  file to the default ~/.smaht-keys.json file.
 --validate
   To validate metadata before submitting.
   This is the DEFAULT behavior for most (non-admin) users.
 --bundle METADATA-FILE
   To specifiy the path to your metatdata file;
   only the directory of this is used to locate your upload files.
 --directory DIRECTORY
   To specify a directory containing the files to upload;
   this directory will be search, recursively.
 --directory-only
   Same as --directory but does NOT search recursively.
---KEYS-FILE
-  To specify an alternate credentials/keys
-  file to the default ~/.smaht-keys.json file.
 --help
   Prints this documentation.
 --help-advanced
   Prints this plus more advanced documentation.
 --help-web
   Opens your browser to the Web based documentation.
-  {CustomArgumentParser.HELP_URL}#resuming-uploads
+  {CustomArgumentParser.HELP_URL}
 ===
 """
 _OBSOLETE_OPTIONS = [
     {"option": "-e", "message": "Use --env."},
     {"option": "-s", "message": "Use --server."},
     {"option": "-b", "message": "Use --bundle."},
     {"option": "--bundle_filename", "message": "Use --bundle."},
```

### Comparing `smaht_submitr-0.7.0.1b94/submitr/scripts/show_upload_info.py` & `smaht_submitr-0.7.0.1b95/submitr/scripts/show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/scripts/submit_genelist.py` & `smaht_submitr-0.7.0.1b95/submitr/scripts/submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/scripts/submit_metadata_bundle.py` & `smaht_submitr-0.7.0.1b95/submitr/scripts/submit_metadata_bundle.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 METADATA-FILE: This is the path to your metatdata file.
 ===
 OPTIONS:
 ===
 --env ENVIRONMENT-NAME
   To specify your environment name; from your ~/.smaht-keys.json file.
   Alternatively, set your SMAHT_ENV environment variable.
+--keys KEYS-FILE
+  To specify an alternate credentials/keys file,
+  rather than the default ~/.smaht-keys.json file.
+  Alternatively, set your SMAHT_KEYS environment variable.
 --validate
   To ONLY validate metadata WITHOUT submitting.
   Either this or --submit is required.
 --submit
   To actually submit the metadata for ingestion (validates first).
   Either this or --validation is required.
 --consortium CONSORTIUM
@@ -46,18 +50,14 @@
 --submission-center SUBMISSION-CENTER
   To specify your submission center.
   Default is to use the submission center associated with your account.
 --directory DIRECTORY
   To specify a directory containing the files to upload; in addition
   to the default of using the directory containing the submitted file;
   this directory will be searched recursively.
---keys KEYS-FILE
-  To specify an alternate credentials/keys file,
-  rather than the default ~/.smaht-keys.json file.
-  Alternatively, set your SMAHT_KEYS environment variable.
 --output OUTPUT-FILE
   Writes all logging output to the specified file;
   and refrains from printing lengthy content to output/stdout.
 --verbose
   Displays more verbose output.
 --help
   Displays this documentation.
```

### Comparing `smaht_submitr-0.7.0.1b94/submitr/scripts/submit_ontology.py` & `smaht_submitr-0.7.0.1b95/submitr/scripts/submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/scripts/upload_item_data.py` & `smaht_submitr-0.7.0.1b95/submitr/scripts/upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/scripts/view_portal_object.py` & `smaht_submitr-0.7.0.1b95/submitr/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/submission.py` & `smaht_submitr-0.7.0.1b95/submitr/submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/tests/data/submission_simple.xlsx` & `smaht_submitr-0.7.0.1b95/submitr/tests/data/submission_simple.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/tests/data/submission_simple2.xlsx` & `smaht_submitr-0.7.0.1b95/submitr/tests/data/submission_simple2.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/tests/data/submission_test.xlsx` & `smaht_submitr-0.7.0.1b95/submitr/tests/data/submission_test.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/tests/data/submission_test_with_errors.xlsx` & `smaht_submitr-0.7.0.1b95/submitr/tests/data/submission_test_with_errors.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/tests/test_base.py` & `smaht_submitr-0.7.0.1b95/submitr/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/tests/test_check_submission.py` & `smaht_submitr-0.7.0.1b95/submitr/tests/test_check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/tests/test_exceptions.py` & `smaht_submitr-0.7.0.1b95/submitr/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/tests/test_make_sample_fastq_file.py` & `smaht_submitr-0.7.0.1b95/submitr/tests/test_make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/tests/test_misc.py` & `smaht_submitr-0.7.0.1b95/submitr/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/tests/test_resume_uploads.py` & `smaht_submitr-0.7.0.1b95/submitr/tests/test_resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/tests/test_show_upload_info.py` & `smaht_submitr-0.7.0.1b95/submitr/tests/test_show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/tests/test_submission.py` & `smaht_submitr-0.7.0.1b95/submitr/tests/test_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/tests/test_submit_genelist.py` & `smaht_submitr-0.7.0.1b95/submitr/tests/test_submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/tests/test_submit_metadata_bundle.py` & `smaht_submitr-0.7.0.1b95/submitr/tests/test_submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/tests/test_submit_ontology.py` & `smaht_submitr-0.7.0.1b95/submitr/tests/test_submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/tests/test_testing_helpers.py` & `smaht_submitr-0.7.0.1b95/submitr/tests/test_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/tests/test_upload_item_data.py` & `smaht_submitr-0.7.0.1b95/submitr/tests/test_upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/tests/test_utils.py` & `smaht_submitr-0.7.0.1b95/submitr/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/tests/testing_helpers.py` & `smaht_submitr-0.7.0.1b95/submitr/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/submitr/utils.py` & `smaht_submitr-0.7.0.1b95/submitr/utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b94/PKG-INFO` & `smaht_submitr-0.7.0.1b95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smaht-submitr
-Version: 0.7.0.1b94
+Version: 0.7.0.1b95
 Summary: Support for uploading file submissions to SMAHT.
 Home-page: https://github.com/smaht-dac/submitr
 License: MIT
 Keywords: submitr,smaht
 Author: SMaHT DAC
 Author-email: smhelp@hms-dbmi.atlassian.net 
 Requires-Python: >=3.8.0,<3.12
```

