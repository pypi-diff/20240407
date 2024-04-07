# Comparing `tmp/smaht_submitr-0.7.0.1b90.tar.gz` & `tmp/smaht_submitr-0.7.0.1b94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smaht_submitr-0.7.0.1b90.tar", max compression
+gzip compressed data, was "smaht_submitr-0.7.0.1b94.tar", max compression
```

## Comparing `smaht_submitr-0.7.0.1b90.tar` & `smaht_submitr-0.7.0.1b94.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1098 2024-04-06 21:04:35.837760 smaht_submitr-0.7.0.1b90/LICENSE.txt
--rw-r--r--   0        0        0     2602 2024-04-06 21:04:35.837760 smaht_submitr-0.7.0.1b90/README.rst
--rw-r--r--   0        0        0     3422 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/__init__.py
--rw-r--r--   0        0        0      731 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/base.py
--rw-r--r--   0        0        0      294 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/exceptions.py
--rw-r--r--   0        0        0     2628 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/output.py
--rw-r--r--   0        0        0    13407 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/progress_bar.py
--rw-r--r--   0        0        0    10819 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/s3_utils.py
--rw-r--r--   0        0        0        0 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/__init__.py
--rw-r--r--   0        0        0     3844 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/check_submission.py
--rw-r--r--   0        0        0     7601 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/cli_utils.py
--rw-r--r--   0        0        0     1835 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/list_submissions.py
--rw-r--r--   0        0        0      940 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/make_sample_fastq_file.py
--rw-r--r--   0        0        0     5718 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/resume_uploads.py
--rw-r--r--   0        0        0     1368 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/show_upload_info.py
--rw-r--r--   0        0        0     1572 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/submit_genelist.py
--rw-r--r--   0        0        0    19866 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/submit_metadata_bundle.py
--rw-r--r--   0        0        0     3437 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/submit_ontology.py
--rw-r--r--   0        0        0     1616 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/upload_item_data.py
--rw-r--r--   0        0        0    28731 2024-04-06 21:04:35.877760 smaht_submitr-0.7.0.1b90/submitr/scripts/view_portal_object.py
--rw-r--r--   0        0        0   149054 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/submission.py
--rw-r--r--   0        0        0        0 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/__init__.py
--rw-r--r--   0        0        0      355 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/conftest_settings.py
--rw-r--r--   0        0        0      163 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/f1_R1.fastq.gz
--rw-r--r--   0        0        0      165 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/f1_R2.fastq.gz
--rw-r--r--   0        0        0      167 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/f2_R1.fastq.gz
--rw-r--r--   0        0        0      164 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/f2_R2.fastq.gz
--rw-r--r--   0        0        0      272 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/simulated_bundle.json
--rw-r--r--   0        0        0    10870 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/submission_simple.xlsx
--rw-r--r--   0        0        0    10875 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/submission_simple2.xlsx
--rw-r--r--   0        0        0    13306 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/submission_test.xlsx
--rw-r--r--   0        0        0    13192 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/submission_test_with_errors.xlsx
--rw-r--r--   0        0        0      169 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/test1_R1.fastq.gz
--rw-r--r--   0        0        0      168 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/data/test1_R2.fastq.gz
--rw-r--r--   0        0        0     1333 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_base.py
--rw-r--r--   0        0        0     2629 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_check_submission.py
--rw-r--r--   0        0        0      551 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_exceptions.py
--rw-r--r--   0        0        0     1620 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_make_sample_fastq_file.py
--rw-r--r--   0        0        0     1421 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_misc.py
--rw-r--r--   0        0        0    11606 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_resume_uploads.py
--rw-r--r--   0        0        0     2478 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_show_upload_info.py
--rw-r--r--   0        0        0   157433 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_submission.py
--rw-r--r--   0        0        0     2836 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_submit_genelist.py
--rw-r--r--   0        0        0     6874 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_submit_metadata_bundle.py
--rw-r--r--   0        0        0     3013 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_submit_ontology.py
--rw-r--r--   0        0        0     1300 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_testing_helpers.py
--rw-r--r--   0        0        0     3661 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_upload_item_data.py
--rw-r--r--   0        0        0     4353 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/test_utils.py
--rw-r--r--   0        0        0     1351 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/tests/testing_helpers.py
--rw-r--r--   0        0        0    11074 2024-04-06 21:04:35.881760 smaht_submitr-0.7.0.1b90/submitr/utils.py
--rw-r--r--   0        0        0     3989 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.1b90/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-06 21:54:40.257927 smaht_submitr-0.7.0.1b94/LICENSE.txt
+-rw-r--r--   0        0        0     2602 2024-04-06 21:54:40.257927 smaht_submitr-0.7.0.1b94/README.rst
+-rw-r--r--   0        0        0     3422 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/base.py
+-rw-r--r--   0        0        0      294 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/exceptions.py
+-rw-r--r--   0        0        0     2628 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/output.py
+-rw-r--r--   0        0        0    12723 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/progress_bar.py
+-rw-r--r--   0        0        0    10819 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/s3_utils.py
+-rw-r--r--   0        0        0        0 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/__init__.py
+-rw-r--r--   0        0        0     3844 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/check_submission.py
+-rw-r--r--   0        0        0     7601 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/cli_utils.py
+-rw-r--r--   0        0        0     1835 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/list_submissions.py
+-rw-r--r--   0        0        0      940 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/make_sample_fastq_file.py
+-rw-r--r--   0        0        0     5718 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/resume_uploads.py
+-rw-r--r--   0        0        0     1368 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/show_upload_info.py
+-rw-r--r--   0        0        0     1572 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/submit_genelist.py
+-rw-r--r--   0        0        0    19866 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3437 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/submit_ontology.py
+-rw-r--r--   0        0        0     1616 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/upload_item_data.py
+-rw-r--r--   0        0        0    28731 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/scripts/view_portal_object.py
+-rw-r--r--   0        0        0   149229 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/submission.py
+-rw-r--r--   0        0        0        0 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/tests/__init__.py
+-rw-r--r--   0        0        0      355 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/tests/conftest_settings.py
+-rw-r--r--   0        0        0      163 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/tests/data/f1_R1.fastq.gz
+-rw-r--r--   0        0        0      165 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/tests/data/f1_R2.fastq.gz
+-rw-r--r--   0        0        0      167 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/tests/data/f2_R1.fastq.gz
+-rw-r--r--   0        0        0      164 2024-04-06 21:54:40.297927 smaht_submitr-0.7.0.1b94/submitr/tests/data/f2_R2.fastq.gz
+-rw-r--r--   0        0        0      272 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/data/simulated_bundle.json
+-rw-r--r--   0        0        0    10870 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/data/submission_simple.xlsx
+-rw-r--r--   0        0        0    10875 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/data/submission_simple2.xlsx
+-rw-r--r--   0        0        0    13306 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/data/submission_test.xlsx
+-rw-r--r--   0        0        0    13192 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/data/submission_test_with_errors.xlsx
+-rw-r--r--   0        0        0      169 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/data/test1_R1.fastq.gz
+-rw-r--r--   0        0        0      168 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/data/test1_R2.fastq.gz
+-rw-r--r--   0        0        0     1333 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_base.py
+-rw-r--r--   0        0        0     2629 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_check_submission.py
+-rw-r--r--   0        0        0      551 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1620 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_make_sample_fastq_file.py
+-rw-r--r--   0        0        0     1421 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_misc.py
+-rw-r--r--   0        0        0    11606 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_resume_uploads.py
+-rw-r--r--   0        0        0     2478 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_show_upload_info.py
+-rw-r--r--   0        0        0   157433 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_submission.py
+-rw-r--r--   0        0        0     2836 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_submit_genelist.py
+-rw-r--r--   0        0        0     6874 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3013 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_submit_ontology.py
+-rw-r--r--   0        0        0     1300 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_testing_helpers.py
+-rw-r--r--   0        0        0     3661 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_upload_item_data.py
+-rw-r--r--   0        0        0     4353 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/test_utils.py
+-rw-r--r--   0        0        0     1351 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/tests/testing_helpers.py
+-rw-r--r--   0        0        0    11074 2024-04-06 21:54:40.301927 smaht_submitr-0.7.0.1b94/submitr/utils.py
+-rw-r--r--   0        0        0     3989 1970-01-01 00:00:00.000000 smaht_submitr-0.7.0.1b94/PKG-INFO
```

### Comparing `smaht_submitr-0.7.0.1b90/LICENSE.txt` & `smaht_submitr-0.7.0.1b94/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/README.rst` & `smaht_submitr-0.7.0.1b94/README.rst`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/pyproject.toml` & `smaht_submitr-0.7.0.1b94/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smaht-submitr"
-version = "0.7.0.1b90"  # TODO: To become 0.8.0
+version = "0.7.0.1b94"  # TODO: To become 0.8.0
 description = "Support for uploading file submissions to SMAHT."
 # TODO: Update this email address when a more specific one is available for SMaHT.
 authors = ["SMaHT DAC <smhelp@hms-dbmi.atlassian.net >"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["submitr", "smaht"]
 homepage = "https://github.com/smaht-dac/submitr"
```

### Comparing `smaht_submitr-0.7.0.1b90/submitr/base.py` & `smaht_submitr-0.7.0.1b94/submitr/base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/output.py` & `smaht_submitr-0.7.0.1b94/submitr/output.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/progress_bar.py` & `smaht_submitr-0.7.0.1b94/submitr/progress_bar.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,49 +20,33 @@
       # This is a bit worrying but so far no other deleterious effects observed.
       # This looks maybe promising:
     return
     """
 
     # Nevermind the above; found a more pointed solution from here:
     # https://stackoverflow.com/questions/41707229/why-is-tqdm-printing-to-a-newline-instead-of-updating-the-same-line
+    # Why in the world would tqdm be maintaining state across instances?? Whatever, this fixes it.
     def __init__(self, *args, **kwargs):
-        self._instances.clear() if self._instances else None
+        super()._instances.clear() if super()._instances else None
         super().__init__(*args, **kwargs)
 
 
 # Wrapper around tqdm command-line progress bar.
 class ProgressBar:
 
     @staticmethod
     @contextmanager
-    def define(total: Optional[int] = None, description: Optional[str] = None,
-               catch_interrupt: bool = True,
-               interrupt: Optional[Callable] = None,
-               interrupt_continue: Optional[Callable] = None,
-               interrupt_stop: Optional[Callable] = None,
-               interrupt_exit: bool = None,
-               interrupt_message: Optional[str] = None,
-               printf: Optional[Callable] = None,
-               tidy_output_hack: bool = True) -> None:
-
-        progress_bar = ProgressBar(
-            total=total,
-            description=description,
-            catch_interrupt=catch_interrupt,
-            interrupt=interrupt,
-            interrupt_continue=interrupt_continue,
-            interrupt_stop=interrupt_stop,
-            interrupt_exit=interrupt_exit,
-            interrupt_message=interrupt_message,
-            printf=printf,
-            tidy_output_hack=tidy_output_hack)
+    def define(*args, **kwargs):
+        progress_bar = None
         try:
+            progress_bar = ProgressBar(*args, **kwargs)
             yield progress_bar
         finally:
-            progress_bar.done()
+            if progress_bar:
+                progress_bar.done()
 
     def __init__(self, total: Optional[int] = None,
                  description: Optional[str] = None,
                  catch_interrupt: bool = True,
                  interrupt: Optional[Callable] = None,
                  interrupt_continue: Optional[Callable] = None,
                  interrupt_stop: Optional[Callable] = None,
@@ -193,15 +177,15 @@
         return value
 
     def _define_interrupt_handler(self) -> None:
         def handle_interrupt(signum: int, frame: frame) -> None:  # noqa
             nonlocal self
             def handle_secondary_interrupt(signum: int, frame: frame) -> None:  # noqa
                 nonlocal self
-                self._printf("\nEnter 'yes' to 'no' or CTRL-\\ to completely abort ...")
+                self._printf("\nEnter 'yes' or 'no' or CTRL-\\ to completely abort ...")
             self.disable()
             self._interrupt(self) if self._interrupt else None
             set_interrupt_handler(handle_secondary_interrupt)
             if self._confirmation(f"\nALERT! You have interrupted this {self._interrupt_message or 'process'}."
                                   f" Do you want to stop{' (exit)' if self._interrupt_exit else ''}?"):
                 # Here there was an interrupt (CTRL-C) and the user confirmed (yes)
                 # that they want to stop the process; if the interrupt_stop handler
```

### Comparing `smaht_submitr-0.7.0.1b90/submitr/s3_utils.py` & `smaht_submitr-0.7.0.1b94/submitr/s3_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/scripts/check_submission.py` & `smaht_submitr-0.7.0.1b94/submitr/scripts/check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/scripts/cli_utils.py` & `smaht_submitr-0.7.0.1b94/submitr/scripts/cli_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/scripts/list_submissions.py` & `smaht_submitr-0.7.0.1b94/submitr/scripts/list_submissions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/scripts/make_sample_fastq_file.py` & `smaht_submitr-0.7.0.1b94/submitr/scripts/make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/scripts/resume_uploads.py` & `smaht_submitr-0.7.0.1b94/submitr/scripts/resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/scripts/show_upload_info.py` & `smaht_submitr-0.7.0.1b94/submitr/scripts/show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/scripts/submit_genelist.py` & `smaht_submitr-0.7.0.1b94/submitr/scripts/submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/scripts/submit_metadata_bundle.py` & `smaht_submitr-0.7.0.1b94/submitr/scripts/submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/scripts/submit_ontology.py` & `smaht_submitr-0.7.0.1b94/submitr/scripts/submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/scripts/upload_item_data.py` & `smaht_submitr-0.7.0.1b94/submitr/scripts/upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/scripts/view_portal_object.py` & `smaht_submitr-0.7.0.1b94/submitr/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/submission.py` & `smaht_submitr-0.7.0.1b94/submitr/submission.py`

 * *Files 0% similar despite different names*

```diff
@@ -507,15 +507,15 @@
         "post_only": post_only,
         "patch_only": patch_only,
         "ref_nocache": False,  # Do not do this server-side at all; only client-side for testing.
         "autoadd": json.dumps(autoadd),
         "ingestion_directory": os.path.dirname(ingestion_filename) if ingestion_filename else None,
         "datafile_size": datafile_size or get_file_size(ingestion_filename),
         "datafile_checksum": datafile_checksum or get_file_checksum(ingestion_filename),
-        "user": json.dumps(user)
+        "user": json.dumps(user) if user else None
     }
 
     if validation_ingestion_submission_uuid:
         submission_post_data["validation_uuid"] = validation_ingestion_submission_uuid
     if debug_sleep:
         submission_post_data["debug_sleep"] = debug_sleep
 
@@ -1242,28 +1242,33 @@
         # Get parameters for this submission from the validation IngestionSubmission object.
         consortia = None
         submission_centers = None
         if consortium := check_parameters.get("consortium"):
             consortia = [consortium]
         if submission_center := check_parameters.get("submission_center"):
             submission_centers = [submission_center]
+        if isinstance(user := check_parameters.get("user"), str):
+            try:
+                user = json.loads(user)
+            except Exception:
+                user = None
         if debug:
             PRINT("DEBUG: Continuing with submission process after a previous server validation timeout.")
         submission_uuid = _initiate_server_ingestion_process(
             portal=portal,
             ingestion_filename=None,
             is_server_validation=False,
             is_resume_submission=True,
             validation_ingestion_submission_object=check_response,
             consortia=consortia,
             submission_centers=submission_centers,
             autoadd=check_parameters.get("autoadd"),
             datafile_size=check_parameters.get("datafile_size"),
             datafile_checksum=check_parameters.get("datafile_checksum"),
-            user=check_parameters.get("user"),
+            user=user,
             debug=debug,
             debug_sleep=debug_sleep)
         SHOW(f"Submission tracking ID: {submission_uuid}")
         submission_done, submission_status, submission_response = _monitor_ingestion_process(
                 submission_uuid, portal.server, portal.env, app=portal.app, keys_file=portal.keys_file,
                 show_details=show_details, report=False, messages=True,
                 validation=False,
```

### Comparing `smaht_submitr-0.7.0.1b90/submitr/tests/data/submission_simple.xlsx` & `smaht_submitr-0.7.0.1b94/submitr/tests/data/submission_simple.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/tests/data/submission_simple2.xlsx` & `smaht_submitr-0.7.0.1b94/submitr/tests/data/submission_simple2.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/tests/data/submission_test.xlsx` & `smaht_submitr-0.7.0.1b94/submitr/tests/data/submission_test.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/tests/data/submission_test_with_errors.xlsx` & `smaht_submitr-0.7.0.1b94/submitr/tests/data/submission_test_with_errors.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/tests/test_base.py` & `smaht_submitr-0.7.0.1b94/submitr/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/tests/test_check_submission.py` & `smaht_submitr-0.7.0.1b94/submitr/tests/test_check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/tests/test_exceptions.py` & `smaht_submitr-0.7.0.1b94/submitr/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/tests/test_make_sample_fastq_file.py` & `smaht_submitr-0.7.0.1b94/submitr/tests/test_make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/tests/test_misc.py` & `smaht_submitr-0.7.0.1b94/submitr/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/tests/test_resume_uploads.py` & `smaht_submitr-0.7.0.1b94/submitr/tests/test_resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/tests/test_show_upload_info.py` & `smaht_submitr-0.7.0.1b94/submitr/tests/test_show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/tests/test_submission.py` & `smaht_submitr-0.7.0.1b94/submitr/tests/test_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/tests/test_submit_genelist.py` & `smaht_submitr-0.7.0.1b94/submitr/tests/test_submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/tests/test_submit_metadata_bundle.py` & `smaht_submitr-0.7.0.1b94/submitr/tests/test_submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/tests/test_submit_ontology.py` & `smaht_submitr-0.7.0.1b94/submitr/tests/test_submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/tests/test_testing_helpers.py` & `smaht_submitr-0.7.0.1b94/submitr/tests/test_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/tests/test_upload_item_data.py` & `smaht_submitr-0.7.0.1b94/submitr/tests/test_upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/tests/test_utils.py` & `smaht_submitr-0.7.0.1b94/submitr/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/tests/testing_helpers.py` & `smaht_submitr-0.7.0.1b94/submitr/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/submitr/utils.py` & `smaht_submitr-0.7.0.1b94/submitr/utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.7.0.1b90/PKG-INFO` & `smaht_submitr-0.7.0.1b94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smaht-submitr
-Version: 0.7.0.1b90
+Version: 0.7.0.1b94
 Summary: Support for uploading file submissions to SMAHT.
 Home-page: https://github.com/smaht-dac/submitr
 License: MIT
 Keywords: submitr,smaht
 Author: SMaHT DAC
 Author-email: smhelp@hms-dbmi.atlassian.net 
 Requires-Python: >=3.8.0,<3.12
```

