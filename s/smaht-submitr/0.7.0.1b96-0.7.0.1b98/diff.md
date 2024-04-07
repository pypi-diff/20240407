# Comparing `tmp/smaht_submitr-0.7.0.1b96.tar.gz` & `tmp/smaht_submitr-0.7.0.1b98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smaht_submitr-0.7.0.1b96.tar", max compression
+gzip compressed data, was "smaht_submitr-0.7.0.1b98.tar", max compression
```

## Comparing `smaht_submitr-0.7.0.1b96.tar` & `smaht_submitr-0.7.0.1b98.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1098 2024-04-07 03:38:38.483311 smaht_submitr-0.7.0.1b96/LICENSE.txt
--rw-r--r--   0        0        0     2602 2024-04-07 03:38:38.483311 smaht_submitr-0.7.0.1b96/README.rst
--rw-r--r--   0        0        0     3422 2024-04-07 03:38:38.519311 smaht_submitr-0.7.0.1b96/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-07 03:38:38.519311 smaht_submitr-0.7.0.1b96/submitr/__init__.py
--rw-r--r--   0        0        0      731 2024-04-07 03:38:38.519311 smaht_submitr-0.7.0.1b96/submitr/base.py
--rw-r--r--   0        0        0      294 2024-04-07 03:38:38.519311 smaht_submitr-0.7.0.1b96/submitr/exceptions.py
--rw-r--r--   0        0        0     2628 2024-04-07 03:38:38.519311 smaht_submitr-0.7.0.1b96/submitr/output.py
--rw-r--r--   0        0        0    12784 2024-04-07 03:38:38.519311 smaht_submitr-0.7.0.1b96/submitr/progress_bar.py
--rw-r--r--   0        0        0    10819 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/s3_utils.py
--rw-r--r--   0        0        0        0 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/__init__.py
--rw-r--r--   0        0        0     4792 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/check_submission.py
--rw-r--r--   0        0        0     8008 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/cli_utils.py
--rw-r--r--   0        0        0     1835 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/list_submissions.py
--rw-r--r--   0        0        0      940 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/make_sample_fastq_file.py
--rw-r--r--   0        0        0     5684 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/resume_uploads.py
--rw-r--r--   0        0        0     1368 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/show_upload_info.py
--rw-r--r--   0        0        0     1572 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/submit_genelist.py
--rw-r--r--   0        0        0    19866 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/submit_metadata_bundle.py
--rw-r--r--   0        0        0     3437 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/submit_ontology.py
--rw-r--r--   0        0        0     1616 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/upload_item_data.py
--rw-r--r--   0        0        0    28731 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/scripts/view_portal_object.py
--rw-r--r--   0        0        0   149229 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/submission.py
--rw-r--r--   0        0        0        0 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/__init__.py
--rw-r--r--   0        0        0      355 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/conftest_settings.py
--rw-r--r--   0        0        0      163 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/f1_R1.fastq.gz
--rw-r--r--   0        0        0      165 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/f1_R2.fastq.gz
--rw-r--r--   0        0        0      167 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/f2_R1.fastq.gz
--rw-r--r--   0        0        0      164 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/f2_R2.fastq.gz
--rw-r--r--   0        0        0      272 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/simulated_bundle.json
--rw-r--r--   0        0        0    10870 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/submission_simple.xlsx
--rw-r--r--   0        0        0    10875 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/submission_simple2.xlsx
--rw-r--r--   0        0        0    13306 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/submission_test.xlsx
--rw-r--r--   0        0        0    13192 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/submission_test_with_errors.xlsx
--rw-r--r--   0        0        0      169 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/test1_R1.fastq.gz
--rw-r--r--   0        0        0      168 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/data/test1_R2.fastq.gz
--rw-r--r--   0        0        0     1333 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_base.py
--rw-r--r--   0        0        0     2629 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_check_submission.py
--rw-r--r--   0        0        0      551 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_exceptions.py
--rw-r--r--   0        0        0     1620 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_make_sample_fastq_file.py
--rw-r--r--   0        0        0     1421 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_misc.py
--rw-r--r--   0        0        0    11606 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_resume_uploads.py
--rw-r--r--   0        0        0     2478 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_show_upload_info.py
--rw-r--r--   0        0        0   157433 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_submission.py
--rw-r--r--   0        0        0     2836 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_submit_genelist.py
--rw-r--r--   0        0        0     6874 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_submit_metadata_bundle.py
--rw-r--r--   0        0        0     3013 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_submit_ontology.py
--rw-r--r--   0        0        0     1300 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_testing_helpers.py
--rw-r--r--   0        0        0     3661 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_upload_item_data.py
--rw-r--r--   0        0        0     4353 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/test_utils.py
--rw-r--r--   0        0        0     1351 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/tests/testing_helpers.py
--rw-r--r--   0        0        0    11074 2024-04-07 03:38:38.523311 smaht_submitr-0.7.0.1b96/submitr/utils.py
--rw-r--r--   0        0        0     3989 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.1b96/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-07 12:12:12.954102 smaht_submitr-0.7.0.1b98/LICENSE.txt
+-rw-r--r--   0        0        0     2602 2024-04-07 12:12:12.954102 smaht_submitr-0.7.0.1b98/README.rst
+-rw-r--r--   0        0        0     3422 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/base.py
+-rw-r--r--   0        0        0      294 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/exceptions.py
+-rw-r--r--   0        0        0     2628 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/output.py
+-rw-r--r--   0        0        0    12784 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/progress_bar.py
+-rw-r--r--   0        0        0    10819 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/s3_utils.py
+-rw-r--r--   0        0        0        0 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/__init__.py
+-rw-r--r--   0        0        0     4785 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/check_submission.py
+-rw-r--r--   0        0        0     8008 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/cli_utils.py
+-rw-r--r--   0        0        0     1828 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/list_submissions.py
+-rw-r--r--   0        0        0      940 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/make_sample_fastq_file.py
+-rw-r--r--   0        0        0     5709 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/resume_uploads.py
+-rw-r--r--   0        0        0     1368 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/show_upload_info.py
+-rw-r--r--   0        0        0     1572 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/submit_genelist.py
+-rw-r--r--   0        0        0    19891 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3437 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/submit_ontology.py
+-rw-r--r--   0        0        0     1616 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/upload_item_data.py
+-rw-r--r--   0        0        0    28731 2024-04-07 12:12:12.994101 smaht_submitr-0.7.0.1b98/submitr/scripts/view_portal_object.py
+-rw-r--r--   0        0        0   151701 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/submission.py
+-rw-r--r--   0        0        0        0 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/__init__.py
+-rw-r--r--   0        0        0      355 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/conftest_settings.py
+-rw-r--r--   0        0        0      163 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/f1_R1.fastq.gz
+-rw-r--r--   0        0        0      165 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/f1_R2.fastq.gz
+-rw-r--r--   0        0        0      167 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/f2_R1.fastq.gz
+-rw-r--r--   0        0        0      164 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/f2_R2.fastq.gz
+-rw-r--r--   0        0        0      272 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/simulated_bundle.json
+-rw-r--r--   0        0        0    10870 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/submission_simple.xlsx
+-rw-r--r--   0        0        0    10875 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/submission_simple2.xlsx
+-rw-r--r--   0        0        0    13306 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/submission_test.xlsx
+-rw-r--r--   0        0        0    13192 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/submission_test_with_errors.xlsx
+-rw-r--r--   0        0        0      169 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/test1_R1.fastq.gz
+-rw-r--r--   0        0        0      168 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/data/test1_R2.fastq.gz
+-rw-r--r--   0        0        0     1333 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_base.py
+-rw-r--r--   0        0        0     2629 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_check_submission.py
+-rw-r--r--   0        0        0      551 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1620 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_make_sample_fastq_file.py
+-rw-r--r--   0        0        0     1421 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_misc.py
+-rw-r--r--   0        0        0    11606 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_resume_uploads.py
+-rw-r--r--   0        0        0     2478 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_show_upload_info.py
+-rw-r--r--   0        0        0   157433 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_submission.py
+-rw-r--r--   0        0        0     2836 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_submit_genelist.py
+-rw-r--r--   0        0        0     6874 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3013 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_submit_ontology.py
+-rw-r--r--   0        0        0     1300 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_testing_helpers.py
+-rw-r--r--   0        0        0     3661 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_upload_item_data.py
+-rw-r--r--   0        0        0     4353 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/test_utils.py
+-rw-r--r--   0        0        0     1351 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/tests/testing_helpers.py
+-rw-r--r--   0        0        0    11074 2024-04-07 12:12:12.998101 smaht_submitr-0.7.0.1b98/submitr/utils.py
+-rw-r--r--   0        0        0     3989 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.1b98/PKG-INFO
```

### Comparing `smaht_submitr-0.7.0.1b96/LICENSE.txt` & `smaht_submitr-0.7.0.1b98/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/README.rst` & `smaht_submitr-0.7.0.1b98/README.rst`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/pyproject.toml` & `smaht_submitr-0.7.0.1b98/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smaht-submitr"
-version = "0.7.0.1b96"  # TODO: To become 0.8.0
+version = "0.7.0.1b98"  # TODO: To become 0.8.0
 description = "Support for uploading file submissions to SMAHT."
 # TODO: Update this email address when a more specific one is available for SMaHT.
 authors = ["SMaHT DAC <smhelp@hms-dbmi.atlassian.net >"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["submitr", "smaht"]
 homepage = "https://github.com/smaht-dac/submitr"
```

### Comparing `smaht_submitr-0.7.0.1b96/submitr/base.py` & `smaht_submitr-0.7.0.1b98/submitr/base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/output.py` & `smaht_submitr-0.7.0.1b98/submitr/output.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/progress_bar.py` & `smaht_submitr-0.7.0.1b98/submitr/progress_bar.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/s3_utils.py` & `smaht_submitr-0.7.0.1b98/submitr/s3_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/scripts/check_submission.py` & `smaht_submitr-0.7.0.1b98/submitr/scripts/check_submission.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,16 @@
         if _pytesting():
             exit(2)
         args.submission_uuid = "dummy"
 
     env_from_env = False
     if not args.env:
         args.env = os.environ.get("SMAHT_ENV")
-        env_from_env = True
+        if args.env:
+            env_from_env = True
 
     # We would we want to specify an upload directy for checks-submissions?
     # Because if the check is for a server validation "submission" which on which
     # we previously timed out waiting for (via submit-metadata-bundler) this
     # command will give the user the option of continueing on with the submission.
     upload_directory = None
     upload_directory_only = True
@@ -96,15 +97,15 @@
         else:
             args.timeout = int(args.timeout)
 
     with script_catch_errors():
         return _monitor_ingestion_process(
                 args.submission_uuid,
                 env=args.env,
-                keys_file=args.keys or os.environ.get("SMAHT_KEYS"),
+                keys_file=args.keys,
                 server=args.server,
                 env_from_env=env_from_env,
                 show_details=(args.verbose or args.details),
                 check_submission_script=True,
                 verbose=args.verbose,
                 debug=args.debug,
                 upload_directory=upload_directory,
```

### Comparing `smaht_submitr-0.7.0.1b96/submitr/scripts/cli_utils.py` & `smaht_submitr-0.7.0.1b98/submitr/scripts/cli_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/scripts/list_submissions.py` & `smaht_submitr-0.7.0.1b98/submitr/scripts/list_submissions.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,22 +19,23 @@
     args.add_argument("--verbose", action="store_true", help="Verbose output.", default=False)
     args.add_argument("--quiet", action="store_true", help="Quiet output.", default=False)
     args = args.parse_args()
 
     env_from_env = False
     if not args.env:
         args.env = os.environ.get("SMAHT_ENV")
-        env_from_env = True
+        if args.env:
+            env_from_env = True
 
     # TODO: handle --mine and --user
 
     with script_catch_errors():
         portal = _define_portal(env=args.env,
                                 env_from_env=env_from_env,
-                                keys_file=args.keys or os.environ.get("SMAHT_KEYS"),
+                                keys_file=args.keys,
                                 report=not args.quiet, note="Listing Submissions")
         _print_recent_submissions(portal, details=args.details, verbose=args.verbose,
                                   count=args.count, mine=args.mine, user=args.user)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `smaht_submitr-0.7.0.1b96/submitr/scripts/make_sample_fastq_file.py` & `smaht_submitr-0.7.0.1b98/submitr/scripts/make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/scripts/resume_uploads.py` & `smaht_submitr-0.7.0.1b98/submitr/scripts/resume_uploads.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,19 +92,19 @@
     if args.yes:
         args.no_query = True
 
     if not args.uuid:
         PRINT("Missing submission UUID or referenced file UUID or accession ID.")
         exit(2)
 
-    keys_file = args.keys or os.environ.get("SMAHT_KEYS")
-    if keys_file:
-        if not keys_file.endswith(".json") or not os.path.exists(keys_file):
-            PRINT(f"The --keys argument ({keys_file}) must be the name of an existing .json file.")
-            exit(1)
+#   keys_file = args.keys or os.environ.get("SMAHT_KEYS")
+#   if keys_file:
+#       if not keys_file.endswith(".json") or not os.path.exists(keys_file):
+#           PRINT(f"The --keys argument ({keys_file}) must be the name of an existing .json file.")
+#           exit(1)
 
     if args.upload_folder and not os.path.isdir(args.upload_folder):
         PRINT(f"Directory does not exist: {args.upload_folder}")
         exit(1)
 
     if args.bundle and not os.path.isdir(os.path.normpath(os.path.dirname(args.bundle))):
         PRINT(f"Specified bundle file not found: {args.bundle}")
@@ -116,22 +116,23 @@
     if args.upload_folder and not os.path.isdir(args.upload_folder):
         PRINT(f"Specified upload directory not found: {args.upload_folder}")
         exit(1)
 
     env_from_env = False
     if not args.env:
         args.env = os.environ.get("SMAHT_ENV")
-        env_from_env = True
+        if args.env:
+            env_from_env = True
 
     with script_catch_errors():
 
         resume_uploads(uuid=args.uuid,
                        env=args.env,
                        env_from_env=env_from_env,
-                       keys_file=keys_file,
+                       keys_file=args.keys,
                        bundle_filename=args.bundle,
                        server=args.server,
                        upload_folder=args.upload_folder,
                        no_query=args.yes,
                        subfolders=not directory_only,
                        output_file=args.output,
                        app=args.app)
```

### Comparing `smaht_submitr-0.7.0.1b96/submitr/scripts/show_upload_info.py` & `smaht_submitr-0.7.0.1b98/submitr/scripts/show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/scripts/submit_genelist.py` & `smaht_submitr-0.7.0.1b98/submitr/scripts/submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/scripts/submit_metadata_bundle.py` & `smaht_submitr-0.7.0.1b98/submitr/scripts/submit_metadata_bundle.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,35 +219,36 @@
     if args.directory:
         args.upload_folder = args.directory
         directory_only = False
     if args.directory_only:
         args.upload_folder = args.directory_only
         directory_only = True
 
-    keys_file = args.keys or os.environ.get("SMAHT_KEYS")
-    if keys_file:
-        if not keys_file.endswith(".json"):
-            PRINT(f"ERROR: The specified keys file is not a .json file: {keys_file}")
-            exit(1)
-        if not keys_file.endswith(".json") or not os.path.exists(keys_file):
-            PRINT(f"ERROR: The --keys argument must be the name of an existing .json file: {keys_file}")
-            exit(1)
+#   keys_file = args.keys or os.environ.get("SMAHT_KEYS")
+#   if keys_file:
+#       if not keys_file.endswith(".json"):
+#           PRINT(f"ERROR: The specified keys file is not a .json file: {keys_file}")
+#           exit(1)
+#       if not keys_file.endswith(".json") or not os.path.exists(keys_file):
+#           PRINT(f"ERROR: The --keys argument must be the name of an existing .json file: {keys_file}")
+#           exit(1)
 
     env_from_env = False
     if not args.env:
         args.env = os.environ.get("SMAHT_ENV")
-        env_from_env = True
+        if args.env:
+            env_from_env = True
 
     if args.ping or (args.bundle_filename and args.bundle_filename.lower() == "ping"):
         ping_okay = _ping(
             env=args.env or os.environ.get("SMAHT_ENV"),
             env_from_env=env_from_env,
             server=args.server,
             app=args.app,
-            keys_file=keys_file,
+            keys_file=args.keys,
             verbose=True)
         if ping_okay:
             PRINT("Ping success. Your connection appears to be OK.")
             exit(0)
         else:
             PRINT("Ping failure. Your connection appears to be problematic.")
             exit(1)
@@ -310,15 +311,15 @@
     with script_catch_errors():
 
         if not _sanity_check_submitted_file(args.bundle_filename):
             exit(1)
 
         submit_any_ingestion(ingestion_filename=args.bundle_filename, ingestion_type=args.ingestion_type,
                              env=args.env, env_from_env=env_from_env,
-                             keys_file=keys_file,
+                             keys_file=args.keys,
                              server=args.server,
                              consortium=args.consortium,
                              submission_center=args.submission_center,
                              add_submission_center=args.add_submission_center,
                              no_query=args.no_query,
                              subfolders=not directory_only,
                              app=args.app,
```

### Comparing `smaht_submitr-0.7.0.1b96/submitr/scripts/submit_ontology.py` & `smaht_submitr-0.7.0.1b98/submitr/scripts/submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/scripts/upload_item_data.py` & `smaht_submitr-0.7.0.1b98/submitr/scripts/upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/scripts/view_portal_object.py` & `smaht_submitr-0.7.0.1b98/submitr/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/submission.py` & `smaht_submitr-0.7.0.1b98/submitr/submission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1127,17 +1127,20 @@
             if done:
                 bar.done()
         return progress_report
 
     portal = _define_portal(env=env, server=server, app=app or DEFAULT_APP,
                             env_from_env=env_from_env, report=report, note=note)
 
-    if not (uuid_metadata := portal.get_metadata(uuid)):
+    if not (uuid_metadata := portal.get_metadata(uuid, raise_exception=False)):
         message = f"Submission ID not found: {uuid}" if uuid != "dummy" else "No submission ID specified."
-        if _print_recent_submissions(portal, message=message):
+        message += "\nSome recent submission IDs below. Use list-submissions to view more."
+        if _print_recent_submissions(portal, message=message, count=4):
+            if check_submission_script:
+                exit(1)
             return
         raise Exception(f"Cannot find object given uuid: {uuid}")
     if not portal.is_schema_type(uuid_metadata, INGESTION_SUBMISSION_TYPE_NAME):
         undesired_type = portal.get_schema_type(uuid_metadata)
         raise Exception(f"Given ID is not for a submission or validation: {uuid} ({undesired_type})"
                         f" | Accession: {uuid_metadata.get('accession')}")
     if tobool(uuid_metadata.get("parameters", {}).get("validate_only")):
@@ -1870,14 +1873,17 @@
 
         undesired_type = portal.get_schema_type(response)
         raise Exception(f"Given ID is not an {INGESTION_SUBMISSION_TYPE_NAME} type: {uuid} ({undesired_type})")
 
     if submission_parameters := response.get("parameters", {}):
         if tobool(submission_parameters.get("validate_only")):
             PRINT(f"This submission ID ({uuid}) is for a validation not an actual submission.")
+            if submission_uuid := submission_parameters.get("submission_uuid"):
+                PRINT(f"▶ Perhaps you meant to use the submission ID"
+                      f" associated with this: {submission_uuid}")  # noqa
             exit(1)
 
     do_any_uploads(response,
                    keydict=portal.key,
                    ingestion_filename=bundle_filename,
                    upload_folder=upload_folder,
                    no_query=no_query,
@@ -2885,53 +2891,94 @@
                    app: Optional[str] = None, keys_file: Optional[str] = None, env_from_env: bool = False,
                    report: bool = False, verbose: bool = False, note: Optional[str] = None) -> Portal:
 
     def get_default_keys_file():
         nonlocal app
         return os.path.expanduser(os.path.join(Portal.KEYS_FILE_DIRECTORY, f".{app.lower()}-keys.json"))
 
+    def sanity_check_keys_file(keys_file: Optional[str] = None) -> Optional[str]:
+        keys_file_from_env = False
+        if not keys_file:
+            keys_file = os.environ.get("SMAHT_KEYS")
+            keys_file_from_env = os.environ.get("SMAHT_KEYS")
+        if keys_file:
+            if not keys_file.endswith(".json"):
+                PRINT(f"ERROR: The specified keys file{' (from SMAHT_KEYS)' if keys_file_from_env else ''}"
+                      f" is not a .json file: {keys_file}")
+                exit(1)
+            if not keys_file.endswith(".json") or not os.path.exists(keys_file):
+                PRINT(f"ERROR: The specified keys file{' (from SMAHT_KEYS)' if keys_file_from_env else ''}"
+                      f" must be the name of an existing .json file: {keys_file}")
+                exit(1)
+            try:
+                with open(keys_file, "r") as f:
+                    json.load(f)
+            except Exception:
+                PRINT(f"ERROR: The specified keys file{' (from SMAHT_KEYS)' if keys_file_from_env else ''}"
+                      f" cannot be loaded as JSON: {keys_file}")
+                exit(1)
+        return keys_file
+
     if not env and not env_from_env:
         env_from_env = os.environ.get("SMAHT_ENV")
 
     raise_exception = True
     if not app:
         app = DEFAULT_APP
         app_default = True
     else:
         app_default = False
     portal = None
+    keys_file = sanity_check_keys_file(keys_file)
     try:
         # TODO: raise_exception does not totally work here (see portal_utils.py).
         portal = Portal(key or keys_file, env=env, server=server, app=app, raise_exception=True)
     except Exception as e:
         if "not found in keys-file" in str(e):
-            PRINT(f"ERROR: Environment ({env}) not found in keys file: {keys_file or get_default_keys_file()}")
+            if not env:
+                PRINT(f"No environment specified from keys file: {keys_file or get_default_keys_file()}")
+                PRINT(f"Use the --env option with a name from that file; or set your SMAHT_ENV environment variable.")
+            else:
+                PRINT(f"Environment ({env}) not found in keys file: {keys_file or get_default_keys_file()}")
+            exit(1)
+        else:
+            PRINT(e)
             exit(1)
     if not portal or not portal.key:
         try:
             if keys_file and not os.path.exists(keys_file):
-                PRINT(f"ERROR: No keys file found: {keys_file or get_default_keys_file()}")
+                PRINT(f"No keys file found: {keys_file or get_default_keys_file()}")
                 exit(1)
             else:
                 default_keys_file = get_default_keys_file()
                 if not os.path.exists(default_keys_file):
-                    PRINT(f"ERROR: No default keys file found: {default_keys_file}")
+                    PRINT(f"No default keys file found: {default_keys_file}")
                     exit(1)
         except Exception:
             pass
         if raise_exception:
             raise Exception(
                 f"No portal key defined; setup your ~/.{app or 'smaht'}-keys.json file and use the --env argument.")
     if report:
         message = f"SMaHT submitr version: {get_version()}"
         if note:
             message += f" | {note}"
         PRINT(message)
         if verbose:
             PRINT(f"Portal app name is{' (default)' if app_default else ''}: {app}")
+        if not env and server and not portal.env:
+            # TODO: Handle portal_utils bug where not setting corresponding portal.env if server specified.
+            if portal.keys_file:
+                try:
+                    with io.open(portal.keys_file) as f:
+                        keys = json.load(f)
+                        if env := [k for k in keys if Portal._normalize_server(keys[k].get("server")) == server]:
+                            portal._env = env[0]
+                except Exception:
+                    pass
         PRINT(f"Portal environment (in keys file) is: {portal.env}{' (from SMAHT_ENV)' if env_from_env else ''}")
         PRINT(f"Portal keys file is: {format_path(portal.keys_file)}")
         PRINT(f"Portal server is: {portal.server}")
         if portal.key_id and len(portal.key_id) > 2:
             PRINT(f"Portal key prefix is: {portal.key_id[:2]}******")
     return portal
```

### Comparing `smaht_submitr-0.7.0.1b96/submitr/tests/data/submission_simple.xlsx` & `smaht_submitr-0.7.0.1b98/submitr/tests/data/submission_simple.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/tests/data/submission_simple2.xlsx` & `smaht_submitr-0.7.0.1b98/submitr/tests/data/submission_simple2.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/tests/data/submission_test.xlsx` & `smaht_submitr-0.7.0.1b98/submitr/tests/data/submission_test.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/tests/data/submission_test_with_errors.xlsx` & `smaht_submitr-0.7.0.1b98/submitr/tests/data/submission_test_with_errors.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/tests/test_base.py` & `smaht_submitr-0.7.0.1b98/submitr/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/tests/test_check_submission.py` & `smaht_submitr-0.7.0.1b98/submitr/tests/test_check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/tests/test_exceptions.py` & `smaht_submitr-0.7.0.1b98/submitr/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/tests/test_make_sample_fastq_file.py` & `smaht_submitr-0.7.0.1b98/submitr/tests/test_make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/tests/test_misc.py` & `smaht_submitr-0.7.0.1b98/submitr/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/tests/test_resume_uploads.py` & `smaht_submitr-0.7.0.1b98/submitr/tests/test_resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/tests/test_show_upload_info.py` & `smaht_submitr-0.7.0.1b98/submitr/tests/test_show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/tests/test_submission.py` & `smaht_submitr-0.7.0.1b98/submitr/tests/test_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/tests/test_submit_genelist.py` & `smaht_submitr-0.7.0.1b98/submitr/tests/test_submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/tests/test_submit_metadata_bundle.py` & `smaht_submitr-0.7.0.1b98/submitr/tests/test_submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/tests/test_submit_ontology.py` & `smaht_submitr-0.7.0.1b98/submitr/tests/test_submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/tests/test_testing_helpers.py` & `smaht_submitr-0.7.0.1b98/submitr/tests/test_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/tests/test_upload_item_data.py` & `smaht_submitr-0.7.0.1b98/submitr/tests/test_upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/tests/test_utils.py` & `smaht_submitr-0.7.0.1b98/submitr/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/tests/testing_helpers.py` & `smaht_submitr-0.7.0.1b98/submitr/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/submitr/utils.py` & `smaht_submitr-0.7.0.1b98/submitr/utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b96/PKG-INFO` & `smaht_submitr-0.7.0.1b98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smaht-submitr
-Version: 0.7.0.1b96
+Version: 0.7.0.1b98
 Summary: Support for uploading file submissions to SMAHT.
 Home-page: https://github.com/smaht-dac/submitr
 License: MIT
 Keywords: submitr,smaht
 Author: SMaHT DAC
 Author-email: smhelp@hms-dbmi.atlassian.net 
 Requires-Python: >=3.8.0,<3.12
```

