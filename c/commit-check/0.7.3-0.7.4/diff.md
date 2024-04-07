# Comparing `tmp/commit_check-0.7.3-py3-none-any.whl.zip` & `tmp/commit_check-0.7.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 11346 bytes, number of entries: 13
--rw-r--r--  2.0 unx     2119 b- defN 24-Mar-11 07:57 commit_check/__init__.py
--rw-r--r--  2.0 unx     1115 b- defN 24-Mar-11 07:57 commit_check/author.py
--rw-r--r--  2.0 unx      926 b- defN 24-Mar-11 07:57 commit_check/branch.py
--rw-r--r--  2.0 unx     2614 b- defN 24-Mar-11 07:57 commit_check/commit.py
--rw-r--r--  2.0 unx     2675 b- defN 24-Mar-11 07:57 commit_check/error.py
--rw-r--r--  2.0 unx     2928 b- defN 24-Mar-11 07:57 commit_check/main.py
--rw-r--r--  2.0 unx     4040 b- defN 24-Mar-11 07:57 commit_check/util.py
--rw-r--r--  2.0 unx     1095 b- defN 24-Mar-11 07:57 commit_check-0.7.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     8478 b- defN 24-Mar-11 07:57 commit_check-0.7.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-11 07:57 commit_check-0.7.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       56 b- defN 24-Mar-11 07:57 commit_check-0.7.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 24-Mar-11 07:57 commit_check-0.7.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1060 b- defN 24-Mar-11 07:57 commit_check-0.7.3.dist-info/RECORD
-13 files, 27211 bytes uncompressed, 9576 bytes compressed:  64.8%
+Zip file size: 11452 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     2119 b- defN 24-Apr-07 06:44 commit_check/__init__.py
+-rw-r--r--  2.0 unx     1115 b- defN 24-Apr-07 06:44 commit_check/author.py
+-rw-r--r--  2.0 unx      926 b- defN 24-Apr-07 06:44 commit_check/branch.py
+-rw-r--r--  2.0 unx     2614 b- defN 24-Apr-07 06:44 commit_check/commit.py
+-rw-r--r--  2.0 unx     2675 b- defN 24-Apr-07 06:44 commit_check/error.py
+-rw-r--r--  2.0 unx     2928 b- defN 24-Apr-07 06:44 commit_check/main.py
+-rw-r--r--  2.0 unx     4040 b- defN 24-Apr-07 06:44 commit_check/util.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-Apr-07 06:44 commit_check-0.7.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8770 b- defN 24-Apr-07 06:44 commit_check-0.7.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-07 06:44 commit_check-0.7.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 24-Apr-07 06:44 commit_check-0.7.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-07 06:44 commit_check-0.7.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1060 b- defN 24-Apr-07 06:44 commit_check-0.7.4.dist-info/RECORD
+13 files, 27503 bytes uncompressed, 9682 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: commit_check/main.py
 Comment: 
 
 Filename: commit_check/util.py
 Comment: 
 
-Filename: commit_check-0.7.3.dist-info/LICENSE
+Filename: commit_check-0.7.4.dist-info/LICENSE
 Comment: 
 
-Filename: commit_check-0.7.3.dist-info/METADATA
+Filename: commit_check-0.7.4.dist-info/METADATA
 Comment: 
 
-Filename: commit_check-0.7.3.dist-info/WHEEL
+Filename: commit_check-0.7.4.dist-info/WHEEL
 Comment: 
 
-Filename: commit_check-0.7.3.dist-info/entry_points.txt
+Filename: commit_check-0.7.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: commit_check-0.7.3.dist-info/top_level.txt
+Filename: commit_check-0.7.4.dist-info/top_level.txt
 Comment: 
 
-Filename: commit_check-0.7.3.dist-info/RECORD
+Filename: commit_check-0.7.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `commit_check-0.7.3.dist-info/LICENSE` & `commit_check-0.7.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `commit_check-0.7.3.dist-info/METADATA` & `commit_check-0.7.4.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commit-check
-Version: 0.7.3
+Version: 0.7.4
 Summary: Check commit message formatting, branch naming, commit author, email, and more.
 Author-email: Peter Shen <xianpeng.shen@gmail.com>
 License: MIT License
 Project-URL: source, https://github.com/commit-check/commit-check
 Project-URL: tracker, https://github.com/commit-check/commit-check/issues
 Keywords: commit conventions,conventional commits,branch naming,commit-check,message,lint message
 Classifier: Development Status :: 4 - Beta
@@ -25,51 +25,53 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: pyyaml
 
 Commit Check
 ============
 
-.. image:: https://img.shields.io/pypi/v/commit-check?logo=python&logoColor=white
+.. |pypi-version| image:: https://img.shields.io/pypi/v/commit-check?logo=python&logoColor=white
     :target: https://pypi.org/project/commit-check/
     :alt: PyPI
 
-.. image:: https://github.com/commit-check/commit-check/actions/workflows/main.yml/badge.svg
+.. |ci-badge| image:: https://github.com/commit-check/commit-check/actions/workflows/main.yml/badge.svg
     :target: https://github.com/commit-check/commit-check/actions/workflows/main.yml
     :alt: CI
 
-.. image:: https://sonarcloud.io/api/project_badges/measure?project=commit-check_commit-check&metric=alert_status
+.. |sonar-badge| image:: https://sonarcloud.io/api/project_badges/measure?project=commit-check_commit-check&metric=alert_status
     :target: https://sonarcloud.io/summary/new_code?id=commit-check_commit-check
     :alt: Quality Gate Status
 
-.. image:: https://codecov.io/gh/commit-check/commit-check/branch/main/graph/badge.svg?token=GC2U5V5ZRT
+.. |codecov-badge| image:: https://codecov.io/gh/commit-check/commit-check/branch/main/graph/badge.svg?token=GC2U5V5ZRT
     :target: https://codecov.io/gh/commit-check/commit-check
     :alt: CodeCov
 
-.. image:: https://img.shields.io/badge/commit--check-enabled-brightgreen?logo=Git&logoColor=white
+.. |commit-check-badge| image:: https://img.shields.io/badge/commit--check-enabled-brightgreen?logo=Git&logoColor=white
     :target: https://github.com/commit-check/commit-check
     :alt: commit-check
 
-.. image:: https://slsa.dev/images/gh-badge-level3.svg
+.. |slsa-badge| image:: https://slsa.dev/images/gh-badge-level3.svg
     :target: https://slsa.dev
     :alt: SLSA
 
+|pypi-version| |ci-badge| |sonar-badge| |codecov-badge| |commit-check-badge| |slsa-badge|
+
 Overview
 --------
 
 Commit Check supports checking commit messages, branch naming, committer name/email, commit signoff, customizing error messages, suggested commands and more.
 
 It is a powerful, free solution for individuals and teams aiming to standardize commit message formatting and branch naming, including
 
 - writing descriptive commit is easy to read
 - identify branch according to the branch type
 - triggering the specific types of commit/branch CI build
 - automatically generate changelogs
 
-If you're using Bitbucket, it's an open source alternative to Yet Another Commit Checker.
+If you're using Bitbucket, it's an open source alternative to `Yet Another Commit Checker <https://marketplace.atlassian.com/apps/1211854/yet-another-commit-checker?tab=overview&hosting=datacenter>`_.
 
 Configuration
 -------------
 
 Use Custom Configuration
 ~~~~~~~~~~~~~~~~~~~~~~~~
```

## Comparing `commit_check-0.7.3.dist-info/RECORD` & `commit_check-0.7.4.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 commit_check/__init__.py,sha256=O9VtMWp02Fw_TbTVguhACJ0jP0-cjQuTlVs18AjV9q0,2119
 commit_check/author.py,sha256=e5WNoYb5DbH2nbqoMeXsX64EXfR8W1x2HZRgCOFAr58,1115
 commit_check/branch.py,sha256=4Vt5qf3NniQdMA5x19kE3xLClyLDGFKRZhP_veXn7y0,926
 commit_check/commit.py,sha256=fxon9TTJkMxrZpcDFo0srXY6G6IUkhJnhBa9qkPR19M,2614
 commit_check/error.py,sha256=aLMLB1s591f9bMSoz9Bbn7gwOh1QLn6zEIeXX7KhhJ4,2675
 commit_check/main.py,sha256=q548-4KcjWqW5QfTysNtUC3sRBZaQp6EiTRwOC7VJRg,2928
 commit_check/util.py,sha256=RXBX2BBe_-lbXpYKzo_gcIb0sP-GdXgJm3h_-S_kRj8,4040
-commit_check-0.7.3.dist-info/LICENSE,sha256=VAJ9TE1ov8aUKmeoBRYqciMs0CXag1TeDCoLhwbeQmA,1095
-commit_check-0.7.3.dist-info/METADATA,sha256=rA-Js911AQ3I2KqVhJ-q1aK42EfoBHORQiOsdtmRZXM,8478
-commit_check-0.7.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-commit_check-0.7.3.dist-info/entry_points.txt,sha256=2IMogDXLAFnwmH_-_EFBwYixY9sTvcwxze59OFs8ybA,56
-commit_check-0.7.3.dist-info/top_level.txt,sha256=Wf46u-ooHBMJNHbhfrBNQw3wC5_m8wt-o_Lfbc4QpRg,13
-commit_check-0.7.3.dist-info/RECORD,,
+commit_check-0.7.4.dist-info/LICENSE,sha256=VAJ9TE1ov8aUKmeoBRYqciMs0CXag1TeDCoLhwbeQmA,1095
+commit_check-0.7.4.dist-info/METADATA,sha256=PRRTpK_MeAxzWL5IEv0nU-d_mVBp9q7omTeja1pJrrw,8770
+commit_check-0.7.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+commit_check-0.7.4.dist-info/entry_points.txt,sha256=2IMogDXLAFnwmH_-_EFBwYixY9sTvcwxze59OFs8ybA,56
+commit_check-0.7.4.dist-info/top_level.txt,sha256=Wf46u-ooHBMJNHbhfrBNQw3wC5_m8wt-o_Lfbc4QpRg,13
+commit_check-0.7.4.dist-info/RECORD,,
```

